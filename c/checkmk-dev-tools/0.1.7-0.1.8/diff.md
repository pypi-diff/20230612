# Comparing `tmp/checkmk_dev_tools-0.1.7.tar.gz` & `tmp/checkmk_dev_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmk_dev_tools-0.1.7.tar", max compression
+gzip compressed data, was "checkmk_dev_tools-0.1.8.tar", max compression
```

## Comparing `checkmk_dev_tools-0.1.7.tar` & `checkmk_dev_tools-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1475 2023-06-05 17:25:55.667846 checkmk_dev_tools-0.1.7/Readme.md
--rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.7/cmk_dev/__init__.py
--rwxr-xr-x   0        0        0    20158 2023-06-05 17:14:33.207269 checkmk_dev_tools-0.1.7/cmk_dev/ci_artifacts.py
--rwxr-xr-x   0        0        0     2184 2023-06-05 16:21:12.072374 checkmk_dev_tools-0.1.7/cmk_dev/cli.py
--rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.7/cmk_dev/listen_std.py
--rw-r--r--   0        0        0     2179 2023-06-05 17:20:06.805662 checkmk_dev_tools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1475 2023-06-12 09:05:06.347787 checkmk_dev_tools-0.1.8/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.8/cmk_dev/__init__.py
+-rwxr-xr-x   0        0        0    23922 2023-06-12 09:05:06.347787 checkmk_dev_tools-0.1.8/cmk_dev/ci_artifacts.py
+-rwxr-xr-x   0        0        0     2184 2023-06-05 16:21:12.072374 checkmk_dev_tools-0.1.8/cmk_dev/cli.py
+-rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.8/cmk_dev/listen_std.py
+-rw-r--r--   0        0        0     2179 2023-06-12 09:05:27.943828 checkmk_dev_tools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.8/PKG-INFO
```

### Comparing `checkmk_dev_tools-0.1.7/Readme.md` & `checkmk_dev_tools-0.1.8/Readme.md`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.7/cmk_dev/ci_artifacts.py` & `checkmk_dev_tools-0.1.8/cmk_dev/ci_artifacts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 
-"""Give information about and download named arguments from Nexus
-"""
+"""Give information about and download Jenkins job artifacts"""
 
 import hashlib
 import logging
 import os
 import sys
 import time
 from argparse import ArgumentParser
@@ -15,42 +14,57 @@
 from contextlib import contextmanager, suppress
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from subprocess import check_output
 from typing import TypeAlias, Union, cast
 
-import yaml
-from jenkins import Jenkins, JenkinsException
+from jenkins import Jenkins
 
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=fixme
 
 GenMapVal: TypeAlias = Union[None, bool, str, float, int, "GenMapArray", "GenMap"]
 GenMapArray: TypeAlias = Sequence[GenMapVal]
 GenMap: TypeAlias = Mapping[str, GenMapVal]
 
 PathHashes: TypeAlias = Mapping[str, str]
-JobParams: TypeAlias = Mapping[str, int | str]
+JobParamValue: TypeAlias = int | str
+JobParams: TypeAlias = Mapping[str, JobParamValue]
+
+QueueId: TypeAlias = int
+BuildId: TypeAlias = int
 
 
 class Fatal(RuntimeError):
     """Rien ne va plus"""
 
 
 def parse_args() -> Args:
     """Cool git like multi command argument parser"""
     parser = ArgumentParser("Provide CI artifacts locally")
     parser.add_argument(
         "--log-level",
         "-l",
-        choices=["DEBUG", "INFO", "WARN", "ERROR", "CRITICAL"],
+        choices=["ALL_DEBUG", "DEBUG", "INFO", "WARN", "ERROR", "CRITICAL"],
+        help="Sets the logging level - ALL_DEBUG sets all other loggers to DEBUG, too",
         type=str.upper,
         default="INFO",
     )
+    parser.add_argument(
+        "-c",
+        "--credentials",
+        type=split_params,
+        help=(
+            "Provide 'url', 'username' and 'password' "
+            "or 'username_env', 'url_env' and 'password_env' respectively."
+            " If no credentials are provided, the JJB config at "
+            " ~/.config/jenkins_jobs/jenkins_jobs.ini is being used."
+        ),
+    )
 
     parser.set_defaults(func=lambda *_: parser.print_usage())
     subparsers = parser.add_subparsers(help="available commands", metavar="CMD")
 
     parser_info = subparsers.add_parser("info")
     parser_info.set_defaults(func=_fn_info)
     parser_info.add_argument(
@@ -59,25 +73,14 @@
         type=lambda a: a.strip(" /"),
     )
 
     parser_fetch = subparsers.add_parser("fetch")
     parser_fetch.set_defaults(func=_fn_fetch)
     parser_fetch.add_argument("job", type=str)
     parser_fetch.add_argument(
-        "-c",
-        "--credentials",
-        type=split_params,
-        help=(
-            "Provide 'url', 'username' and 'password' "
-            "or 'username_env', 'url_env' and 'password_env' respectively."
-            " If no credentials are provided, the JJB config at "
-            " ~/.config/jenkins_jobs/jenkins_jobs.ini is being used."
-        ),
-    )
-    parser_fetch.add_argument(
         "-p",
         "--params",
         type=split_params,
         action="append",
     )
     parser_fetch.add_argument(
         "-d",
@@ -108,16 +111,22 @@
         "-o",
         "--out-dir",
         default="out",
         type=Path,
         help="Directory to put artifacts to - relative to --base-dir if relative",
     )
     parser_fetch.add_argument(
+        "-f",
+        "--force-new-build",
+        action="store_true",
+        help="Don't check for existing matching builds, but start a new build immediately instead",
+    )
+    parser_fetch.add_argument(
         "-n",
-        "--omit-new-builds",
+        "--omit-new-build",
         action="store_true",
         help="Don't issue new builds, even if no matching build could be found",
     )
 
     return parser.parse_args()
 
 
@@ -130,45 +139,47 @@
     """Splits a 'string packed map' into a dict
     >>> split_params("foo=23,bar=42")
     {'foo': '23', 'bar': '42'}
     """
     return {k: v for p in string.split(",") for k, v in (p.split("="),)}
 
 
+def compact_dict(mapping: GenMap) -> str:
+    """Splits a 'string packed map' into a dict
+    >>> compact_dict({'foo': '23', 'bar': '42'})
+    'foo=23, bar=42'
+    """
+
+    def short(string: str) -> str:
+        return string if len(string) <= 12 else f"{string[:10]}.."
+
+    return ", ".join(f"{k}={short_str}" for k, v in mapping.items() if (short_str := short(str(v))))
+
+
 @dataclass
 class Build:
     """Models a Jenkins job build"""
 
     url: str
     number: int
     timestamp: datetime
-    result: str
+    result: None | str
     building: str
     in_progress: bool
     parameters: GenMap
     path_hashes: Mapping[str, str]
     artifacts: list[str]
 
-    def __init__(self, raw_build_info: GenMap):
-        def params_from(build_info: GenMap, action_name: str, item_name: str) -> GenMap:
-            """Return job parameters of provided @build_info as dict"""
-            actions = cast(GenMapArray, build_info.get("actions") or [])
-            for action in map(lambda a: cast(GenMap, a), actions):
-                if cast(str, action.get("_class") or "").rsplit(".", 1)[-1] == action_name:
-                    if action_name == "ParametersAction":
-                        return {
-                            str(p["name"]): p["value"]
-                            for p in map(
-                                lambda a: cast(GenMap, a), cast(GenMapArray, action[item_name])
-                            )
-                        }
-                    if action_name == "CustomBuildPropertiesAction":
-                        return cast(GenMap, action[item_name])
-            return {}
+    def __str__(self) -> str:
+        return (
+            f"Build({self.result}, {self.timestamp}, params={{{compact_dict(self.parameters)}}}, "
+            f"hashes={{{compact_dict(self.path_hashes)}}})"
+        )
 
+    def __init__(self, raw_build_info: GenMap):
         self.url = cast(str, raw_build_info["url"])
         self.number = cast(int, raw_build_info["number"])
         self.timestamp = datetime.fromtimestamp(cast(int, raw_build_info["timestamp"]) // 1000)
         self.result = cast(str, raw_build_info["result"])
         self.building = cast(str, raw_build_info["building"])
         self.in_progress = cast(bool, raw_build_info["inProgress"])
         self.parameters = params_from(raw_build_info, "ParametersAction", "parameters")
@@ -188,18 +199,24 @@
 @dataclass
 class Job:
     """Models a Jenkins job"""
 
     name: str
     fullname: str
     builds: Mapping[int, Build]
+    url: str
+
+    def __str__(self) -> str:
+        return f"Job('{self.fullname}', {len(self.builds)} builds)"
 
     def __init__(self, raw_job_info: GenMap, raw_build_infos: GenMapArray):
+        assert not raw_job_info.get("queueItem") and not raw_job_info.get("inQueue")
         self.name = cast(str, raw_job_info["name"])
         self.fullname = cast(str, raw_job_info["fullName"])
+        self.url = cast(str, raw_job_info["url"])
         self.builds = {
             cast(int, bi["id"]): Build(bi) for bi in map(lambda a: cast(GenMap, a), raw_build_infos)
         }
 
 
 @dataclass
 class Folder:
@@ -263,22 +280,26 @@
     """Entry point for information about job artifacts"""
     credentials = extract_credentials(args.credentials)
     with jenkins_client(
         credentials["url"], credentials["username"], credentials["password"]
     ) as client:
         class_name = (job_info := client.get_job_info(args.job))["_class"]
         if class_name == "com.cloudbees.hudson.plugins.folder.Folder":
-            # print(yaml.dump(job_info))
             print(Folder(job_info))
         elif class_name == "org.jenkinsci.plugins.workflow.job.WorkflowJob":
-            build_infos = [
-                client.get_build_info(args.job, cast(int, cast(GenMap, b)["number"]))
-                for b in cast(GenMapArray, job_info["builds"])
-            ]
-            print(Job(job_info, build_infos))
+            job = Job(
+                job_info,
+                [
+                    client.get_build_info(args.job, cast(int, cast(GenMap, b)["number"]))
+                    for b in cast(GenMapArray, job_info["builds"])
+                ],
+            )
+            print(job)
+            for build_nr, build in job.builds.items():
+                print(f"  - {build_nr}: {build}")
         else:
             raise Fatal(f"Don't know class type {class_name}")
 
 
 def md5from(filepath: Path) -> str | None:
     """Returns an MD5 sum from contents of file provided"""
     with suppress(FileNotFoundError):
@@ -311,17 +332,35 @@
             # use the full hash - short hashes cannot be checked out and they are not
             # unique among machines
             ["git", "log", "--pretty=tformat:%H", "-n1"] + ([str(path)] if path else []),
             text=True,
         ).strip("\n")
 
 
-def download_artifacts(client: Jenkins, build_url: str, out_dir: Path) -> None:
+def params_from(build_info: GenMap, action_name: str, item_name: str) -> GenMap:
+    """Return job parameters of provided @build_info as dict"""
+    actions = cast(GenMapArray, build_info.get("actions") or [])
+    for action in map(lambda a: cast(GenMap, a), actions):
+        if cast(str, action.get("_class") or "").rsplit(".", 1)[-1] == action_name:
+            if action_name == "ParametersAction":
+                return {
+                    str(p["name"]): p["value"]
+                    for p in map(lambda a: cast(GenMap, a), cast(GenMapArray, action[item_name]))
+                }
+            if action_name == "CustomBuildPropertiesAction":
+                return cast(GenMap, action[item_name])
+    return {}
+
+
+def download_artifacts(client: Jenkins, build_url: str, out_dir: Path) -> tuple[int, int]:
     """Downloads all artifacts listed for given job/build to @out_dir"""
     # pylint: disable=protected-access
+
+    downloaded, skipped = 0, 0
+
     out_dir.mkdir(parents=True, exist_ok=True)
 
     # https://bugs.launchpad.net/python-jenkins/+bug/1973243
     # https://bugs.launchpad.net/python-jenkins/+bug/2018576
     fingerprints = client._session.get(
         f"{build_url}api/json?tree=fingerprint[fileName,hash]"
     ).json()["fingerprint"]
@@ -333,14 +372,15 @@
         fp_filename, fp_hash = fingerprint["fileName"], fingerprint["hash"]
         logger().debug("Handle artifact: %s (md5: %s)", fp_filename, fp_hash)
         artifact_filename = out_dir / fp_filename
         local_hash = md5from(artifact_filename)
 
         if local_hash == fp_hash:
             logger().debug("File is already available locally: %s (md5: %s)", fp_filename, fp_hash)
+            skipped += 1
             continue
 
         if local_hash and local_hash != fp_hash:
             logger().warning(
                 "File exists locally but hashes differ: %s %s != %s",
                 fp_filename,
                 local_hash,
@@ -349,80 +389,80 @@
 
         with client._session.get(f"{build_url}artifact/{fp_filename}", stream=True) as reply:
             logger().debug("Download: %s", fp_filename)
             reply.raise_for_status()
             with open(artifact_filename, "wb") as out_file:
                 for chunk in reply.iter_content(chunk_size=1 << 16):
                     out_file.write(chunk)
+            downloaded += 1
+    return downloaded, skipped
 
 
-def path_hashes_match(first: PathHashes, second: PathHashes) -> bool:
+def path_hashes_match(actual: PathHashes, required: PathHashes) -> bool:
     """Returns True if two given path hash mappings are semantically equal, i.e. at least one hash
     is prefix of the other (to handle short hashes, as returned with %h)
     >>> path_hashes_match({}, None)
     True
-    >>> path_hashes_match({"a": "abc"}, None)
+    >>> path_hashes_match(None, {"a": "abc"})
     False
     >>> path_hashes_match({"a": "abc"}, {"a": "abc"})
     True
     >>> path_hashes_match({"a": "abc"}, {"a": "abcde"})
     True
     """
-    if not first and not second:
+    if not required:
         return True
-    if bool(first) != bool(second):
+    if required and not actual:
         return False
-    if first.keys() != second.keys():
+    if required.keys() - actual.keys():
         return False
     return all(
-        hash1.startswith(hash2) or hash2.startswith(hash1)
-        for key, hash1 in first.items()
-        for hash2 in (second[key],)
+        hash_required.startswith(hash_actual) or hash_actual.startswith(hash_required)
+        for key, hash_required in required.items()
+        for hash_actual in (actual[key],)
     )
 
 
+def find_mismatching_parameters(
+    first: GenMap, second: GenMap
+) -> Sequence[tuple[str, JobParamValue, JobParamValue]]:
+    """Returns list of key and mismatching values in mapping @first which also occur in @second"""
+    # TODO: find solution for unprovided parameters and default/empty values
+    return [
+        (key, cast(JobParamValue, first.get(key, "")), cast(JobParamValue, second.get(key, "")))
+        for key in set(first.keys() | second.keys()) - {"DISABLE_CACHE"}
+        if first.get(key) and first.get(key, "") != second.get(key, "")
+    ]
+
+
 def meets_constraints(
     build: Build,
     params: None | JobParams,
     time_constraints: None | str,
-    path_hashes: PathHashes,
     now: datetime = datetime.now(),
 ) -> bool:
     """Checks if a set of requirements are met for a given build"""
 
-    result = True
-    used_params = params or {}
-    # TODO: find solution for unprovided parameters and default/empty values
-    mismatching_parameters = [
-        (key, build.parameters.get(key, ""), used_params.get(key, ""))
-        for key in set(build.parameters.keys() | used_params.keys()) - {"DISABLE_CACHE"}
-        if build.parameters.get(key, "") != used_params.get(key, "")
-    ]
+    # TODO: discuss: should only the last job be taken into account?
 
-    assert build.result in {"SUCCESS", "FAILURE"}
+    assert build.result in {None, "SUCCESS", "FAILURE"}
 
-    if build.result != "SUCCESS":
+    result = True
+
+    # Prune if the build already failed (might still be ongoing)
+    if build.result not in {"SUCCESS", None}:
         logger().debug("build #%d result was: %s", build.number, build.result)
         return False
 
-    if mismatching_parameters:
+    if mismatching_parameters := find_mismatching_parameters(params or {}, build.parameters):
         logger().debug(
             "build #%d has mismatching parameters: %s", build.number, mismatching_parameters
         )
         result = False
 
-    if not path_hashes_match(build.path_hashes, path_hashes):
-        logger().debug(
-            "build #%d has mismatching path hashes: %s != %s",
-            build.number,
-            build.path_hashes,
-            path_hashes,
-        )
-        result = False
-
     if time_constraints is None or time_constraints == "today":
         if build.timestamp.date() != datetime.now().date():
             logger().debug(
                 "build #%d does not meet time constraints: %s != %s",
                 build.number,
                 build.timestamp.date(),
                 now.date(),
@@ -436,133 +476,186 @@
     else:
         raise Fatal(f"Don't understand time constraint specifier {time_constraints!r}")
 
     return result
 
 
 def find_matching_build(
-    job: Job, params: None | JobParams, time_constraints: None | str, path_hashes: Mapping[str, str]
+    job: Job,
+    params: None | JobParams,
+    time_constraints: None | str,
 ) -> Build | None:
     """Goes through a job's build items and returns the first one to match certain criteria or None
     if none is found"""
     for build_id, build in job.builds.items():
-        if meets_constraints(build, params, time_constraints, path_hashes):
-            print(
-                f"Found matching build: {build_id}"
-                f" {build.timestamp} {build.result} {build.parameters}"
-            )
+        if meets_constraints(build, params, time_constraints):
+            print(f"Found matching build: {build_id} ({build.url})")
             for key, value in build.__dict__.items():
-                print(f"  {key}: {value}")
+                logger().debug("  %s: %s", key, value)
             return build
     return None
 
 
-def create_new(client: Jenkins, job_full_path: str, params: None | JobParams) -> Build:
-    """Starts a job specified by @job_full_path using @params and returns its build info object"""
-    queue_id = client.build_job(job_full_path, params)
+def build_id_from_queue_item(client: Jenkins, queue_id: QueueId) -> BuildId:
+    """Waits for queue item with given @queue_id to be scheduled and returns Build instance"""
     while True:
         queue_item = client.get_queue_item(queue_id)
-        print(yaml.dump(queue_item))
+        # print(yaml.dump(queue_item))
         if executable := queue_item.get("executable"):
-            print(yaml.dump(executable))
-            return Build(client.get_build_info(job_full_path, executable["number"]))
+            # print(yaml.dump(executable))
+            return executable["number"]
+        print(f"Waiting for queue item {queue_item['id']} to be scheduled ({queue_item['why']})")
         time.sleep(1)
 
 
+def find_matching_queue_item(client: Jenkins, job: Job, params: None | JobParams) -> BuildId | None:
+    """Looks for a queued build matching job and parameters and returns the QueueId"""
+    for queue_item in client.get_queue_info():
+
+        if not cast(str, queue_item.get("_class", "")).startswith("hudson.model.Queue"):
+            continue
+        if cast(str, cast(GenMap, queue_item.get("task", {})).get("url", "")) != job.url:
+            continue
+        mismatching_parameters = find_mismatching_parameters(
+            params or {},
+            params_from(queue_item, "ParametersAction", "parameters"),
+        )
+        if mismatching_parameters:
+            logger().debug(
+                "queue item %d has mismatching parameters: %s",
+                queue_item.get("id"),
+                mismatching_parameters,
+            )
+            continue
+        return build_id_from_queue_item(client, cast(int, queue_item.get("id")))
+    return None
+
+
 def _fn_fetch(args: Args) -> None:
     """Entry point for fetching artifacts"""
     # logger().debug("Parsed params: %s", params)
     fetch_job_artifacts(
         args.job,
         credentials=args.credentials,
-        params={k: v for p in (args.params or []) for k, v in p.items()},
-        dependency_paths=[path for paths in args.dependency_paths for path in paths.split(",")],
+        params=args.params and {k: v for p in (args.params) for k, v in p.items()},
+        dependency_paths=args.dependency_paths
+        and [path for paths in (args.dependency_paths) for path in paths.split(",")],
         base_dir=args.base_dir,
         time_constraints=args.time_constraints,
         out_dir=args.out_dir,
-        omit_new_build=args.omit_new_builds,
+        omit_new_build=args.omit_new_build,
+        force_new_build=args.force_new_build,
     )
 
 
 def fetch_job_artifacts(
     job_full_path: str,
     *,
     credentials: None | Mapping[str, str] = None,
     params: None | JobParams = None,
     dependency_paths: None | Sequence[str] = None,
-    base_dir: Path = Path("."),
+    base_dir: None | Path = None,
     time_constraints: None | str = None,
     out_dir: None | Path = None,
     omit_new_build: bool = False,
+    force_new_build: bool = False,
 ) -> None:
     """Returns artifacts of Jenkins job specified by @job_full_path matching @params and
     @time_constraints. If none of the existing builds match the conditions a new build will be
     issued. If the existing build has not finished yet it will be waited for."""
+    # pylint: disable=too-many-locals
+
+    used_base_dir = base_dir or Path(".")
     creds = extract_credentials(credentials)
     with jenkins_client(creds["url"], creds["username"], creds["password"]) as client:
         if not str((job_info := client.get_job_info(job_full_path))["_class"]).endswith(
             "WorkflowJob"
         ):
             raise Fatal(f"{job_full_path} is not a WorkflowJob")
-        job = Job(
-            job_info,
-            [
-                client.get_build_info(job_full_path, cast(int, cast(GenMap, b)["number"]))
-                for b in cast(GenMapArray, job_info["builds"])
-            ],
-        )
-        path_hashes = {path: git_commit_id(base_dir, path) for path in (dependency_paths or [])}
 
-        build_candidate = (
-            find_matching_build(job, params, time_constraints, path_hashes) or None
-            if omit_new_build
-            else create_new(client, job_full_path, params)
-        )
+        def elect_build_candidate() -> Build:
+            if not force_new_build:
+                job = Job(
+                    job_info,
+                    [
+                        client.get_build_info(job_full_path, cast(int, cast(GenMap, b)["number"]))
+                        for b in cast(GenMapArray, job_info["builds"])
+                    ],
+                )
+                if matching_queue_item := find_matching_queue_item(client, job, params):
+                    return Build(client.get_build_info(job_full_path, matching_queue_item))
 
-        if not build_candidate:
-            assert omit_new_build
-            raise Fatal(
-                f"No matching build could be found for job '{job.name}' and new builds are omitted."
+                if matching_build := find_matching_build(job, params, time_constraints):
+                    return matching_build
+                if omit_new_build:
+                    raise Fatal(
+                        f"No matching build found for job '{job.name}' but new builds are omitted."
+                    )
+            return Build(
+                client.get_build_info(
+                    job_full_path,
+                    build_id_from_queue_item(client, client.build_job(job_full_path, params)),
+                )
             )
 
+        path_hashes = {
+            path: git_commit_id(used_base_dir, path) for path in (dependency_paths or [])
+        }
+
+        build_candidate = elect_build_candidate()
+
         if build_candidate.in_progress or build_candidate.building:
             print(f"Waiting for job #{build_candidate.number} to finish..")
             while True:
                 build_candidate = Build(
                     client.get_build_info(job_full_path, build_candidate.number)
                 )
+                # TODO: what's the difference between .in_progress and .building?
                 if build_candidate.in_progress or build_candidate.building:
-                    logger().debug(
-                        "build.in_progress=%s build.building=%s",
-                        build_candidate.in_progress,
-                        build_candidate.building,
-                    )
-                    time.sleep(2)
+                    logger().info("build %d in progress", build_candidate.number)
+                    time.sleep(10)
                     continue
                 break
-            if not build_candidate.artifacts:
-                raise Fatal("Job has no artifacts!")
 
-        download_artifacts(client, build_candidate.url, base_dir / (out_dir or ""))
+            if build_candidate.result != "SUCCESS":
+                raise Fatal(
+                    "The build we started has "
+                    f"result={build_candidate.result} ({build_candidate.url})"
+                )
+            logger().info("build finished successfully")
+
+        if not path_hashes_match(build_candidate.path_hashes, path_hashes):
+            raise Fatal(
+                f"Most recent build #{build_candidate.number} has mismatching path hashes: "
+                f"{build_candidate.path_hashes} != {path_hashes}"
+            )
+
+        if not build_candidate.artifacts:
+            raise Fatal("Job has no artifacts!")
+
+        full_out_dir = used_base_dir / (out_dir or "")
+        downloaded, skipped = download_artifacts(client, build_candidate.url, full_out_dir)
+        print(f"{downloaded + skipped} artifacts available in {full_out_dir} ({skipped} skipped)")
 
 
 def main() -> None:
     """Entry point for everything else"""
     try:
         args = parse_args()
         logging.basicConfig(
             format="%(levelname)s %(asctime)s %(name)s: %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
-            level=getattr(logging, args.log_level),
+            level=logging.DEBUG if args.log_level == "ALL_DEBUG" else logging.WARNING,
         )
+        logger().setLevel(getattr(logging, args.log_level.split("_")[-1]))
         logger().debug("Parsed args: %s", args)
         args.func(args)
     except Fatal as exc:
         print(exc, file=sys.stderr)
         raise SystemExit(-1) from exc
-    except JenkinsException as exc:
-        logger().error("%r", exc)
-        sys.exit(1)
+    # except JenkinsException as exc:
+    #    logger().error("%r", exc)
+    #    sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `checkmk_dev_tools-0.1.7/cmk_dev/cli.py` & `checkmk_dev_tools-0.1.8/cmk_dev/cli.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.7/cmk_dev/listen_std.py` & `checkmk_dev_tools-0.1.8/cmk_dev/listen_std.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.7/pyproject.toml` & `checkmk_dev_tools-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkmk-dev-tools"
-version = "0.1.7"
+version = "0.1.8"
 description = "Checkmk DevOps tools"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/tribe29/checkmk"
 readme = "Readme.md"
 packages = [
   {include = "cmk_dev/**/*.py"}
 ]
```

### Comparing `checkmk_dev_tools-0.1.7/PKG-INFO` & `checkmk_dev_tools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkmk-dev-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Checkmk DevOps tools
 Home-page: https://github.com/tribe29/checkmk
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

