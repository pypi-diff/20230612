# Comparing `tmp/pyneoncli-0.0.9a3.tar.gz` & `tmp/pyneoncli-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneoncli-0.0.9a3.tar", max compression
+gzip compressed data, was "pyneoncli-0.1.0a2.tar", max compression
```

## Comparing `pyneoncli-0.0.9a3.tar` & `pyneoncli-0.1.0a2.tar`

### file list

```diff
@@ -1,12 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.9a3/LICENSE
--rw-r--r--   0        0        0     1755 2023-06-06 10:11:40.711513 pyneoncli-0.0.9a3/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.9a3/pyneoncli/__init__.py
--rw-r--r--   0        0        0    10304 2023-06-06 10:03:39.539573 pyneoncli-0.0.9a3/pyneoncli/clicommands.py
--rw-r--r--   0        0        0     4213 2023-06-06 09:13:18.161210 pyneoncli-0.0.9a3/pyneoncli/climain.py
--rw-r--r--   0        0        0     1778 2023-06-02 20:28:14.388877 pyneoncli-0.0.9a3/pyneoncli/neon.py
--rw-r--r--   0        0        0    11366 2023-06-05 12:43:00.026285 pyneoncli-0.0.9a3/pyneoncli/neonapi.py
--rw-r--r--   0        0        0      190 2023-06-01 14:26:25.551090 pyneoncli-0.0.9a3/pyneoncli/neonfunction.py
--rw-r--r--   0        0        0     6264 2023-06-06 09:15:31.945372 pyneoncli-0.0.9a3/pyneoncli/printer.py
--rw-r--r--   0        0        0       23 2023-06-06 10:12:06.207284 pyneoncli-0.0.9a3/pyneoncli/version.py
--rw-r--r--   0        0        0      677 2023-06-06 10:12:06.209537 pyneoncli-0.0.9a3/pyproject.toml
--rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 pyneoncli-0.0.9a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     8278 2023-06-09 09:31:15.780474 pyneoncli-0.1.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.1.0a2/pyneoncli/__init__.py
+-rw-r--r--   0        0        0     6910 2023-06-10 11:23:53.263947 pyneoncli-0.1.0a2/pyneoncli/clicommands.py
+-rw-r--r--   0        0        0     3038 2023-06-11 18:26:54.787575 pyneoncli-0.1.0a2/pyneoncli/clidispatcher.py
+-rw-r--r--   0        0        0     3245 2023-06-09 18:11:47.236682 pyneoncli-0.1.0a2/pyneoncli/clilist.py
+-rw-r--r--   0        0        0     5677 2023-06-07 20:06:42.981654 pyneoncli-0.1.0a2/pyneoncli/climain.py
+-rw-r--r--   0        0        0     2886 2023-06-07 11:02:46.695750 pyneoncli-0.1.0a2/pyneoncli/colortext.py
+-rw-r--r--   0        0        0     1080 2023-06-07 20:07:20.413137 pyneoncli-0.1.0a2/pyneoncli/configfile.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:23:56.004114 pyneoncli-0.1.0a2/pyneoncli/endpoint_template.json
+-rw-r--r--   0        0        0        1 2023-06-11 16:34:26.267305 pyneoncli-0.1.0a2/pyneoncli/exceptions.py
+-rw-r--r--   0        0        0     1478 2023-06-07 12:01:09.344156 pyneoncli-0.1.0a2/pyneoncli/msg.py
+-rw-r--r--   0        0        0     2205 2023-06-10 10:34:02.048055 pyneoncli-0.1.0a2/pyneoncli/neon.py
+-rw-r--r--   0        0        0     4445 2023-06-11 18:25:19.573798 pyneoncli-0.1.0a2/pyneoncli/neonapi.py
+-rw-r--r--   0        0        0     1580 2023-06-11 16:34:26.268625 pyneoncli-0.1.0a2/pyneoncli/neonapiexceptions.py
+-rw-r--r--   0        0        0     1237 2023-06-10 11:20:45.709200 pyneoncli-0.1.0a2/pyneoncli/neonliterals.py
+-rw-r--r--   0        0        0     4558 2023-06-07 08:56:54.007032 pyneoncli-0.1.0a2/pyneoncli/printer.py
+-rw-r--r--   0        0        0     7496 2023-06-11 16:34:26.266017 pyneoncli-0.1.0a2/pyneoncli/rawneonapi.py
+-rw-r--r--   0        0        0     5235 2023-06-11 21:46:14.385802 pyneoncli-0.1.0a2/pyneoncli/requester.py
+-rw-r--r--   0        0        0     1335 2023-06-11 17:05:54.225765 pyneoncli-0.1.0a2/pyneoncli/threadedcreate.py
+-rw-r--r--   0        0        0     3557 2023-06-11 21:08:18.995480 pyneoncli-0.1.0a2/pyneoncli/threadedneonapi.py
+-rw-r--r--   0        0        0       23 2023-06-11 22:02:57.017160 pyneoncli-0.1.0a2/pyneoncli/version.py
+-rw-r--r--   0        0        0      703 2023-06-11 22:02:57.014809 pyneoncli-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     9092 1970-01-01 00:00:00.000000 pyneoncli-0.1.0a2/PKG-INFO
```

### Comparing `pyneoncli-0.0.9a3/LICENSE` & `pyneoncli-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.0.9a3/pyneoncli/climain.py` & `pyneoncli-0.1.0a2/pyneoncli/climain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 import argparse
 import os
 import sys
-from dotenv import load_dotenv
+from configparser import ConfigParser
 
-from pyneoncli.clicommands import CLIDispatcher
+from pyneoncli.clidispatcher import CLIDispatcher
+from pyneoncli.configfile import ConfigFileDefaults
+from pyneoncli.msg import Msg
 from pyneoncli.version import __VERSION__
 
 NEON_API_KEY = None
 
 epilog = f'''
 use neoncli list  -h for more information on the list command
 use neoncli branch  -h for more information on the branch command
 use neoncli project -h for more information on the project command
 
 Version : {__VERSION__}
-
 '''
 
+
 def main():
 
-    load_dotenv()
+    env_api_key = os.getenv("NEON_API_KEY")
+    cfg_files = ConfigFileDefaults()
+    cfg = ConfigParser()
+    cfg.read(cfg_files.config_file_list)
+    default_project_id = cfg['DEFAULT']['project_id'] if 'DEFAULT' in cfg and 'project_id' in cfg['DEFAULT'] else None
+    api_key = cfg['DEFAULT']['api_key'] if 'DEFAULT' in cfg and 'api_key' in cfg['DEFAULT'] else env_api_key
+    #print(f"project id: {default_project_id}, api_key: {api_key}")
+
     parser = argparse.ArgumentParser(description='neoncli -  neon command line client',
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
                                      epilog=epilog)
-    parser.add_argument('--apikey', type=str, help='Specify NEON API Key (env NEON_API_KEY)', default=os.getenv( "NEON_API_KEY"))
+    parser.add_argument('--apikey', type=str, default=api_key,
+                        help='Specify NEON API Key (env NEON_API_KEY)')
     parser.add_argument("--version", action="version", version=f"neoncli {__VERSION__}")
     parser.add_argument("--nocolor", action="store_true", default=False, help="Turn off Color output")
     parser.add_argument('--yes', action="store_true", default=False, help='Answer yes to all prompts')
 
     parser.add_argument( '-f', '--fieldfilter', action="append", type=str, help='Enter field values to filter results on')
     parser.set_defaults(func=CLIDispatcher.dispatch_main)
 
     subparsers = parser.add_subparsers(dest='command', description='Invoke a specific neon command',
                                        help='e.g. neoncli list will list all projects')
 
     # List
     list_parser = subparsers.add_parser('list', help='List Neon objects')
+    list_parser.add_argument('-k', '--getkey', action="store_true", default=False, help='list NEON API Key')
     list_parser.add_argument('-a', '--all', action="store_true", default=False, help='List all objects')
     list_parser.add_argument('-p', '--projects', action='store_true', default=False, help='list projects')
     list_parser.add_argument('-n', '--project_name', action='append', dest="project_names",
                              help='list all projects by project name')
     list_parser.add_argument('-b', '--branches', action="append", dest="project_ids",
                              help='List branches associated with project_id(s)')
     list_parser.add_argument('-pi', '--project_id', action="append", dest="project_ids",  type=str,
                              help='List projects specificed by project_id')
     list_parser.add_argument('-bi', '--branch_id', action="append", dest="branch_ids",  type=str,
                              help='List branches specified by project_id:branch_id')
     list_parser.add_argument('-o', '--operations', action="append", dest="op_project_ids",
                              help='List operations associated with project_id(s)')
     list_parser.add_argument('-d', '--operation_details', action="append", dest="op_ids",
                              help='Get operation details for project_id:operation_id')
+    list_parser.add_argument('-e', '--endpoints', type=str, dest="project_id",
+                             help='list endpoints for the specified project_id')
     list_parser.set_defaults(func=CLIDispatcher.dispatch_list)
 
     # Projects
     project_parser = subparsers.add_parser('project', help='Create and delete Neon projects')
     project_parser.add_argument('-c', '--create', action="append", dest="create_names", type=str,  help='create project')
     project_parser.add_argument('-d', '--delete', action="append", dest="delete_ids",  type=str, help='delete project')
     project_parser.add_argument('--delete_all', action="store_true", default=False,  help='delete all projects')
@@ -64,17 +77,30 @@
     branch_parser = subparsers.add_parser('branch', help='create and delete Neon branches')
     branch_parser.add_argument('-c', '--create', action="append",  dest="project_ids", type=str, help='create branch on the project specified by project id')
     branch_parser.add_argument('-d', '--delete', action="append", dest="delete_ids", type=str,  help='delete branches specified by project_id:branch_id')
     branch_parser.add_argument('--delete_all', action="store_true", default=False,  help='delete all branches')
 
     branch_parser.set_defaults(func=CLIDispatcher.dispatch_branch)
 
-    args = parser.parse_args()
-    args.func(args)
+    #endpoints
+    endpoint_parser = subparsers.add_parser('endpoint', help='create and delete Neon endpoints')
+    endpoint_parser.add_argument('-c', '--create',  dest="create_id", type=str,
+                                 help='create endpoint on the project specified by project_id:branch_id')
+    endpoint_parser.add_argument('-d', '--delete',  dest="delete_id", type=str,
+                                 help='delete endpoints specified by project_id:endpoint_id')
 
+    endpoint_parser.set_defaults(func=CLIDispatcher.dispatch_endpoint)
 
-if __name__ == '__main__':
+    msg = None
     try:
-        main()
+        args = parser.parse_args()
+        msg = Msg(args.nocolor)
+        args.func(args)
     except KeyboardInterrupt:
-        print("Exiting : Ctrl-C detected")
-        sys.exit(1)
+        print("")
+        msg.warning("Exiting...Ctrl-C detected")
+
+    except Exception as e:
+        msg.error(f"{e}")
+        sys.exit(1)
+if __name__ == '__main__':
+    main()
```

### Comparing `pyneoncli-0.0.9a3/pyneoncli/neonapi.py` & `pyneoncli-0.1.0a2/pyneoncli/rawneonapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,49 @@
-import json
-import pprint
-import sys
 import time
 from typing import Iterator
 
-import requests
-
-from pyneoncli.neon import NeonProject, NeonBranch, NeonOperations, NeonOperationsDetails
-from pyneoncli.neonfunction import NeonFunction as nf
-
-BASE_URL_V2 = "https://console.neon.tech/api/v2/"
-
-
-class NeonAPIException(requests.exceptions.HTTPError):
-
-    def __init__(self, *args, **kwargs):
-        self._path = kwargs.pop("path", None)
-        self._header = kwargs.pop("header", None)
-        self._method = kwargs.pop("method", None)
-        self._err = kwargs.pop("err", None)
-        self._text = kwargs.pop("text", None)
-        self._operation = kwargs.pop("operation", None)
-        super().__init__(*args, **kwargs)
-
-    @property
-    def operation(self):
-        return self._operation
-
-    @operation.setter
-    def operation(self, value):
-        self._operation = value
-
-    @property
-    def path(self):
-        return self._path
-
-    @property
-    def header(self):
-        return self._header
-
-    @property
-    def method(self):
-        return self._method
-
-    @property
-    def err(self):
-        return self._err
-
-    @property
-    def text(self):
-        return self._text
-
-    @staticmethod
-    def blank_if_none(label: str, value: str, end="\n") -> str:
-        if value is None:
-            return ""
-        else:
-            return f"{label}: {value}{end}"
-
-    def __str__(self):
-        if self._header is None:
-            h = ""
-        else:
-            h = f"header: {pprint.pformat(self._header)}"
-        m = self.blank_if_none("method", self._method)
-        o = self.blank_if_none("operation", self._operation)
-        p = self.blank_if_none("path", self._path)
-        msg = self.blank_if_none("message", self._text)
-
-        return f'{p}{h}{m}{o}{msg}'
-
-
-class NeonTimeoutException(Exception):
-    pass
-
-
-class Requester:
-
-    def __init__(self, base_url: str = BASE_URL_V2, key=None):
-        self._key = key
-        self._base_url = base_url
-        self._headers = {'Authorization': f"Bearer {self._key}",
-                         'Content-Type': "application/json"}
-
-    def request(self, method: str, operation: str, **kwargs):
-        try:
-            # print(self._headers)
-            # print(kwargs)
-            path = f"{self._base_url}{operation}"
-            r = requests.request(method, path, headers=self._headers, **kwargs)
-            r.raise_for_status()
-            return r.json()
-
-        except requests.exceptions.HTTPError as err:
-            raise NeonAPIException(path=path, method=method, err=err, text=r.text)
-
-    def GET(self, operation: str, **kwargs):
-        return self.request("GET", operation)
-
-    def POST(self, operation: str, data: dict = None) -> dict:
-        if data is None:
-            data = dict()
-        self._headers["Accept"] = "application/json"
-        return self.request("POST", operation, data=json.dumps(data))
-
-    def PUT(self, operation: str, **kwargs) -> dict:
-        return self.request("PUT", operation, **kwargs)
-
-    def DELETE(self, operation: str, **kwargs) -> dict:
-        return self.request("DELETE", operation, **kwargs)
-
-    def PATCH(self, operation: str, **kwargs) -> dict:
-        return self.request("PATCH", operation, **kwargs)
-
-    def HEAD(self, operation: str, **kwargs):
-        return self.request("HEAD", operation, **kwargs)
+from pyneoncli.neon import NeonOperation, NeonProject, NeonBranch, NeonEndPoint
+from pyneoncli.neonapiexceptions import NeonAPIException
+from pyneoncli.neonliterals import NeonAPIPaths as np, NeonFunction as nf
+from pyneoncli.requester import Requester
 
 
 class RawNeonAPI:
 
     def __init__(self, api_key: str = None) -> None:
         self._api_key = api_key
-        self._requester = Requester(key=self._api_key)
+        self._requester = Requester(api_key=self._api_key)
 
-    def get_first_operation(self, project_id: str) -> NeonOperations:
+    def get_first_operation(self, project_id: str) -> NeonOperation:
         try:
-            path = f"{nf.projects}/{project_id}/{nf.operations}"
-            for item in self._requester.GET(path)[str(nf.operations)]:
-                return NeonOperations(item)
+            path = np.GET_OPERATIONS(project_id=project_id)
+            for item in self._requester.paginate(path=path, selector=nf.operations()):
+                return NeonOperation(item)
         except NeonAPIException as err:
             err.operation = "get_first_operation"
             raise err
 
-    def get_list_of_operations(self, project_id: str) -> Iterator[NeonOperations]:
+    def get_operations(self, project_id: str) -> Iterator[NeonOperation]:
         try:
-            path = f"{nf.projects}/{project_id}/{nf.operations}"
-            for item in self._requester.GET(path)[str(nf.operations)]:
-                yield NeonOperations(item)
+            path = np.GET_OPERATIONS( project_id=project_id)
+            for item in self._requester.paginate(path=path, selector=nf.operations()):
+                yield NeonOperation(item)
         except NeonAPIException as err:
-            err.operation = "get_list_of_operations"
+            err.operation = "get_operations"
             raise err
 
-    def get_operation_details(self, project_id:str, operation_id:str) -> NeonOperationsDetails:
+    def get_operation(self, project_id: str, operation_id: str) -> NeonOperation:
         try:
-            path = f"{nf.projects}/{project_id}/{nf.operations}/{operation_id}"
-            return NeonOperationsDetails(self._requester.GET(path)["operation"])
+            path = np.GET_OPERATION(project_id=project_id, operation_id=operation_id)
+            return NeonOperation(self._requester.get_one(path=path, selector=nf.operation()))
         except NeonAPIException as err:
-            err.operation = "get_operation_details"
+            err.operation = "get_operation"
             raise err
 
-    def is_complete(self, project_id: str, sleep_time: float = 0.1, timeout: float = 30.0) -> bool:
+    def is_complete(self, project_id: str, sleep_time: float = 0.01, timeout: float = 30.0) -> bool:
         complete, _ = self.completion_time(project_id, sleep_time=sleep_time, timeout=timeout)
         return complete
 
     def completion_time(self, project_id: str, sleep_time: float = 0.1, timeout: float = 30.0) -> tuple[bool, float]:
         start = time.time()
         so_far = start
         while True:
@@ -166,137 +56,131 @@
                 so_far = time.time() - start
                 if so_far > timeout:
                     return False, so_far
 
     def create_project(self, project_name: str) -> NeonProject:
         payload = {"project": {"name": project_name}}
         try:
-            data = self._requester.POST(str(nf.projects), data=payload)
+            data = self._requester.create(path=np.GET_PROJECTS(), payload=payload, selector=nf.project())
+            return NeonProject(data=data)
         except NeonAPIException as err:
             err.operation = "create_project"
             raise err
-        return NeonProject(data=data["project"])
 
     def delete_project(self, project_id: str) -> NeonProject:
         try:
-            data = self._requester.DELETE(f"{nf.projects}/{project_id}")["project"]
+            data = self._requester.delete(np.GET_PROJECT(project_id=project_id), selector=nf.project())
             return NeonProject(data=data)
         except NeonAPIException as err:
             err.operation = "delete_projects"
             raise err
 
-    def get_projects(self) -> Iterator[NeonProject]:
+    def count_projects(self) -> int:
+        return len(list(self.get_projects()))
+
+    def get_projects(self, batch_size: int = 20) -> Iterator[NeonProject]:
         try:
-            return (NeonProject(item) for item in self._requester.GET(str(nf.projects))[str(nf.projects)])
+            for item in self._requester.paginate(np.GET_PROJECTS(), limit=batch_size, selector=nf.projects()):
+                yield NeonProject(item)
         except NeonAPIException as err:
             err.operation = "get_projects"
             raise err
 
-    def get_project_by_id(self, project_id: str) -> NeonProject:
+    def get_project(self, project_id: str) -> NeonProject:
         try:
-            data = self._requester.GET(f"{nf.projects}/{project_id}")["project"]
+            path = np.GET_PROJECT(project_id=project_id)
+            data = self._requester.get_one(path=path, selector=nf.project())
             return NeonProject(data=data)
         except NeonAPIException as err:
-            err.operation = "get_project_by_id"
+            err.operation = "get_project"
             raise err
 
     def get_projects_by_id(self, project_ids: list[str] = None) -> Iterator[NeonProject]:
         try:
             if project_ids is None:
                 yield from self.get_projects()
             elif not isinstance(project_ids, list):
                 raise TypeError("project_ids must be a list")
             elif len(project_ids) == 0:
                 yield from self.get_projects()
             else:
                 for _id in project_ids:
-                    yield self.get_project_by_id(_id)
+                    yield self.get_project(_id)
         except NeonAPIException as err:
             err.operation = "get_projects_by_id"
             raise err
 
     def create_branch(self, project_id: str) -> NeonBranch:
         try:
-            data = self._requester.POST(f"projects/{project_id}/{nf.branches}")["branch"]
+            data = self._requester.POST(np.GET_BRANCHES(project_id=project_id))
             return NeonBranch(data=data)
         except NeonAPIException as err:
             err.operation = "create_branch"
             raise err
 
     def delete_branch(self, project_id: str, branch_id: str) -> NeonBranch:
         try:
-            data = self._requester.DELETE(f"projects/{project_id}/{nf.branches}/{branch_id}")["branch"]
+            data = self._requester.DELETE(f"projects/{project_id}/{nf.branches}/{branch_id}")
             return NeonBranch(data=data)
         except NeonAPIException as err:
             err.operation = "delete_branch"
             raise err
 
     def get_branch_by_id(self, project_id: str, branch_id: str) -> NeonBranch:
         try:
-            data = self._requester.GET(f"{nf.projects}/{project_id}/{nf.branches}/{branch_id}")["branch"]
+            path = np.GET_BRANCH(project_id=project_id, branch_id=branch_id)
+            data = self._requester.get_one(path=path, selector=nf.branch())
             return NeonBranch(data=data)
         except NeonAPIException as err:
             err.operation = "get_branch_by_id"
             raise err
 
     def get_branches(self, project_id: str) -> Iterator[NeonBranch]:
         try:
+            path = np.GET_BRANCHES(project_id=project_id)
             return (NeonBranch(item) for item in
-                    self._requester.GET(f"{nf.projects}/{project_id}/{nf.branches}")[str(nf.branches)])
+                    self._requester.paginate(path=path, selector=nf.branches()))
         except NeonAPIException as err:
             err.operation = "get_branches"
             raise err
 
+    def get_endpoints(self, project_id: str) -> Iterator[NeonEndPoint]:
+        try:
+            path = np.ENDPOINTS( project_id=project_id)
+            return (NeonEndPoint(item) for item in self._requester.paginate(path=path, selector=nf.endpoints()))
+        except NeonAPIException as err:
+            err.operation = "get_endpoints"
+            raise err
 
-class NeonAPI(RawNeonAPI):
-    TIMEOUT_DEFAULT = 30.0  # 30 seconds
-
-    def __init__(self, api_key: str = None, sleep_time: float = 0.1, timeout: float = TIMEOUT_DEFAULT) -> None:
-        self._api_key = api_key
-        self._timeout = timeout
-        self._sleep_time = sleep_time
-        super().__init__(api_key=self._api_key)
-
-    def create_project(self, project_name: str) -> NeonProject:
-        p = super().create_project(project_name)
-        if self.is_complete(project_id=p.id, sleep_time=self._sleep_time, timeout=self._timeout):
-            return p
-        else:
-            raise NeonTimeoutException(f"Project creation for {project_name} timed out after {self._timeout} seconds")
-
-    def delete_project(self, project_id: str) -> NeonProject:
-        return super().delete_project(project_id)
-
-    def get_project_by_id(self, project_id: str) -> NeonProject:
-        p = super().get_project_by_id(project_id)
-        if self.is_complete(project_id=p.id, sleep_time=self._sleep_time, timeout=self._timeout):
-            return p
-        else:
-            raise NeonTimeoutException(f"get_project_by_id timed out after {self._timeout} seconds for {p.id}")
-
-    def get_projects_by_id(self, project_ids: list[str] = None) -> Iterator[NeonProject]:
-        for p in super().get_projects_by_id(project_ids=project_ids):
-            if self.is_complete(project_id=p.id, sleep_time=self._sleep_time, timeout=self._timeout):
-                yield p
-            else:
-                raise NeonTimeoutException(f"get_project_by_id timed out after {self._timeout} seconds for {p.id}")
-
-    def create_branch(self, project_id: str) -> NeonBranch:
-        b = super().create_branch(project_id)
-        if self.is_complete(project_id=project_id, sleep_time=self._sleep_time, timeout=self._timeout):
-            return b
-        else:
-            raise NeonTimeoutException(f"Branch creation for {project_id} timed out after {self._timeout} seconds")
+    def create_endpoint(self, project_id: str, branch_id: str) -> NeonEndPoint:
+        payload = {
+            "endpoint": {
+                "type": "read_write",
+                "pooler_mode": "transaction",
+                "branch_id": branch_id
+            }
+        }
+        try:
+            path = np.ENDPOINTS(project_id=project_id)
+            data = self._requester.POST(path, data=payload)
+            return NeonEndPoint(data=data)
+        except NeonAPIException as err:
+            err.operation = "create_endpoint"
+            raise err
 
-    def get_branch_by_id(self, project_id: str, branch_id: str) -> NeonBranch:
-        b = super().get_branch_by_id(project_id, branch_id)
-        if self.is_complete(project_id=project_id, sleep_time=self._sleep_time, timeout=self._timeout):
-            return b
-        else:
-            raise NeonTimeoutException(f"get_branch_by_id timed out after {self._timeout} seconds for {b.id}")
+    def delete_endpoint(self, project_id, endpoint_id) -> NeonEndPoint:
+        try:
+            path =np.ENDPOINTS(project_id=project_id, endpoint_id=endpoint_id)
+            data = self._requester.DELETE(path)
+            return NeonEndPoint(data=data)
+        except NeonAPIException as err:
+            err.operation = "delete_endpoint"
+            raise err
 
-    def get_branches(self, project_id: str) -> Iterator[NeonBranch]:
-        for b in super().get_branches(project_id):
-            if self.is_complete(project_id=project_id, sleep_time=self._sleep_time, timeout=self._timeout):
-                yield b
-            else:
-                raise NeonTimeoutException(f"get_branches timed out after {self._timeout} seconds for {b.id}")
+    def get_branch(self, project_id, branch_id):
+        try:
+            path = np.GET_BRANCH(project_id=project_id, branch_id=branch_id)
+            data = self._requester.get_one(path)
+            return NeonBranch(data=data)
+        except NeonAPIException as err:
+            err.operation = "get_branch"
+            raise err
```

### Comparing `pyneoncli-0.0.9a3/pyproject.toml` & `pyneoncli-0.1.0a2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 
 [tool.poetry]
 name = "pyneoncli"
-version = "0.0.9a3"
+version = "0.1.0a2"
 description = "A Python CLI for the Neon API"
 authors = ["Joe Drumgoole <Joe.Drumgoole@neon.tech>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "^2.31.0"
 pygments = "^2.15.1"
 poetry = "^1.5.1"
 colorama = "^0.4.6"
 python-dotenv = "^1.0.0"
+configargparse = "^1.5.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 neoncli = "pyneoncli.climain:main"
```

