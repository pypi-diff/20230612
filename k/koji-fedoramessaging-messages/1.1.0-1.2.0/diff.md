# Comparing `tmp/koji-fedoramessaging-messages-1.1.0.tar.gz` & `tmp/koji-fedoramessaging-messages-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koji-fedoramessaging-messages-1.1.0.tar", max compression
+gzip compressed data, was "koji-fedoramessaging-messages-1.2.0.tar", max compression
```

## Comparing `koji-fedoramessaging-messages-1.1.0.tar` & `koji-fedoramessaging-messages-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0    18092 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.1.0/LICENSE
--rw-r--r--   0        0        0      257 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.1.0/README.md
--rw-r--r--   0        0        0      676 2023-01-30 14:55:09.035636 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-03 08:49:37.133775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/base.py
--rw-r--r--   0        0        0     4377 2023-04-03 08:49:37.133775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/build.py
--rw-r--r--   0        0        0     3498 2023-04-03 08:53:46.826498 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/package.py
--rw-r--r--   0        0        0     2470 2023-04-03 09:01:28.592868 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/repo.py
--rw-r--r--   0        0        0     9699 2023-04-03 08:55:29.437796 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/rpm.py
--rw-r--r--   0        0        0     4710 2023-05-03 12:32:49.824172 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tag.py
--rw-r--r--   0        0        0     6121 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/task.py
--rw-r--r--   0        0        0        0 2023-01-24 15:38:49.841028 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/__init__.py
--rw-r--r--   0        0        0      895 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_base.py
--rw-r--r--   0        0        0     1310 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_build.py
--rw-r--r--   0        0        0     1541 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_package.py
--rw-r--r--   0        0        0     1036 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_repo.py
--rw-r--r--   0        0        0     3510 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_rpm.py
--rw-r--r--   0        0        0     2307 2023-05-03 12:32:49.825172 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_tag.py
--rw-r--r--   0        0        0     4301 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_task.py
--rw-r--r--   0        0        0     1648 2023-05-05 14:34:41.381139 koji-fedoramessaging-messages-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      746 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.1.0/tox.ini
--rw-r--r--   0        0        0     2204 2023-05-05 14:37:14.994838 koji-fedoramessaging-messages-1.1.0/setup.py
--rw-r--r--   0        0        0      999 2023-05-05 14:37:14.995073 koji-fedoramessaging-messages-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.2.0/LICENSE
+-rw-r--r--   0        0        0      257 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.2.0/README.md
+-rw-r--r--   0        0        0      676 2023-01-30 14:55:09.035636 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/__init__.py
+-rw-r--r--   0        0        0     4969 2023-06-12 09:08:17.321402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/base.py
+-rw-r--r--   0        0        0     6977 2023-06-12 09:21:47.340321 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/build.py
+-rw-r--r--   0        0        0     3468 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/package.py
+-rw-r--r--   0        0        0     2470 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/repo.py
+-rw-r--r--   0        0        0     9699 2023-06-12 09:08:17.321402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/rpm.py
+-rw-r--r--   0        0        0     4686 2023-06-12 09:07:06.617144 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/tag.py
+-rw-r--r--   0        0        0     4155 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/task.py
+-rw-r--r--   0        0        0     1534 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/utilities.py
+-rwxr-xr-x   0        0        0      333 2023-05-03 11:22:25.710843 koji-fedoramessaging-messages-1.2.0/make-spec.sh
+-rw-r--r--   0        0        0     2108 2023-06-12 10:28:52.708142 koji-fedoramessaging-messages-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1315 2023-05-05 14:55:46.956888 koji-fedoramessaging-messages-1.2.0/python-koji-fedoramessaging-messages.spec.in
+-rw-r--r--   0        0        0        0 2023-01-24 15:38:49.841028 koji-fedoramessaging-messages-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2023-06-12 08:59:04.745385 koji-fedoramessaging-messages-1.2.0/tests/test_base.py
+-rw-r--r--   0        0        0     4681 2023-06-12 09:22:34.937492 koji-fedoramessaging-messages-1.2.0/tests/test_build.py
+-rw-r--r--   0        0        0     1541 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.2.0/tests/test_package.py
+-rw-r--r--   0        0        0     1036 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.2.0/tests/test_repo.py
+-rw-r--r--   0        0        0     3510 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.2.0/tests/test_rpm.py
+-rw-r--r--   0        0        0     2283 2023-06-12 08:59:04.820385 koji-fedoramessaging-messages-1.2.0/tests/test_tag.py
+-rw-r--r--   0        0        0    14967 2023-06-12 09:17:58.576499 koji-fedoramessaging-messages-1.2.0/tests/test_task.py
+-rw-r--r--   0        0        0      322 2023-06-12 08:56:09.866746 koji-fedoramessaging-messages-1.2.0/tests/test_utilities.py
+-rw-r--r--   0        0        0      512 2023-06-12 09:23:28.867686 koji-fedoramessaging-messages-1.2.0/tox.ini
+-rw-r--r--   0        0        0     2165 2023-06-12 10:34:00.099405 koji-fedoramessaging-messages-1.2.0/setup.py
+-rw-r--r--   0        0        0      999 2023-06-12 10:34:00.099705 koji-fedoramessaging-messages-1.2.0/PKG-INFO
```

### Comparing `koji-fedoramessaging-messages-1.1.0/LICENSE` & `koji-fedoramessaging-messages-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/__init__.py` & `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/build.py` & `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/tag.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,143 +8,160 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Define schema for fedora messages sent by koji"""
-from enum import Enum
-from typing import List, Optional, Any
 
-from .base import KojiFedoraMessagingMessage, SCHEMA_URL
+import re
 
+from fedora_messaging.message import DEBUG
 
-# This enums is defined in
-# https://pagure.io/koji/blob/master/f/koji/__init__.py
-# But we need it here as the messages we get from the
-# koji plugin only gives us the ints -- so we need to decode
-# for summaries
-class BUILD_STATES(Enum):
-    BUILDING = 0
-    COMPLETE = 1
-    DELETED = 2
-    FAILED = 3
-    CANCELED = 4
+from .base import SCHEMA_URL, KojiFedoraMessagingMessage
 
+TAG = {
+    "type": "object",
+    "properties": {
+        "build_id": {"type": "integer", "description": "build id"},
+        "name": {"type": "string", "description": "package name"},
+        "tag_id": {
+            "type": "integer",
+            "description": "tag id",
+        },
+        "instance": {
+            "type": "string",
+            "description": "distinguish between messages from primary and secondary koji",
+        },
+        "tag": {
+            "type": "string",
+            "description": "name of the tag",
+        },
+        "user": {
+            "type": "string",
+            "description": "name of the user that trigger the build",
+        },
+        "version": {
+            "type": "string",
+            "description": "version of the build",
+        },
+        "owner": {
+            "type": "string",
+            "description": "name of the package owner",
+        },
+        "release": {
+            "type": "string",
+            "description": "release number of the package",
+        },
+    },
+}
 
-class BuildStateChangeV1(KojiFedoraMessagingMessage):
-    """This message is sent when a build state changes."""
+_MASS_REBUILD_RE = re.compile(r"^f\d+-rebuild$")
+_ELN_RE = re.compile(r"^eln(-.*)?$")
 
-    topic = "buildsys.build.state.change"
 
-    body_schema = {
-        "$id": f"{SCHEMA_URL}/v1/{topic}#",
-        "$schema": "https://json-schema.org/draft/2019-09/schema",
-        "description": "The state of the build changed.",
-        "type": "object",
-        "properties": {
-            "build_id": {"type": ["null", "integer"], "description": "build id"},
-            "old": {"type": ["null", "integer"], "description": "previous state"},
-            "name": {
-                "type": "string",
-                "description": "name of the package built",
-            },
-            "task_id": {
-                "type": ["null", "integer"],
-                "description": "task id",
-            },
-            "attribute": {
-                "type": "string",
-                "description": "attribute",
-            },
-            "request": {
-                "description": "build request details",
-            },
-            "instance": {
-                "type": "string",
-                "description": "distinguish between messages from primary and secondary koji",
-            },
-            "epoch": {
-                "type": ["null", "string", "integer"],
-                "description": "epoch",
-            },
-            "version": {
-                "type": "string",
-                "description": "version of the build",
-            },
-            "owner": {
-                "type": ["null", "integer", "string"],
-                "description": "the owner of the build",
-            },
-            "new": {
-                "type": "integer",
-                "description": "new state",
-            },
-            "release": {
-                "type": "string",
-                "description": "release number of the package",
-            },
-        },
-    }
+class TagMessage(KojiFedoraMessagingMessage):
+    severity = DEBUG
 
-    @property
-    def build_id(self) -> Optional[int]:
-        return self.body.get("build_id")
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.priority = self._choose_priority()
 
     @property
-    def old(self) -> int:
-        return self.body.get("old")
+    def build_id(self) -> int:
+        return self.body.get("build_id")
 
     @property
     def name(self) -> str:
         return self.body.get("name")
 
     @property
-    def task_id(self) -> Optional[int]:
-        return self.body.get("task_id")
+    def tag_id(self) -> int:
+        return self.body.get("tag_id")
 
     @property
-    def attribute(self) -> str:
-        return self.body.get("attribute")
+    def instance(self) -> str:
+        return self.body.get("instance")
 
     @property
-    def request(self) -> Optional[List]:
-        return self.body["request"]
+    def tag(self) -> str:
+        return self.body.get("tag")
 
     @property
-    def instance(self) -> str:
-        return self.body["instance"]
+    def user(self) -> str:
+        return self.body.get("user")
 
     @property
     def version(self) -> str:
-        return self.body["version"]
+        return self.body.get("version")
 
     @property
     def owner(self) -> str:
         return self.body.get("owner")
 
     @property
-    def new(self) -> int:
-        return self.body["new"]
+    def release(self) -> str:
+        return self.body.get("release")
 
     @property
-    def release(self) -> str:
-        return self.body["release"]
+    def summary(self) -> str:
+        return (
+            f"{self.name}-{self.version}-{self.release} was {self._summary_action}"
+            f" {self.tag} by {self.user}"
+        )
 
     @property
-    def epoch(self) -> Any:
-        return self.body["epoch"]
+    def packages(self) -> list[str]:
+        return [self.name] if self.name else []
 
     @property
     def agent_name(self) -> str:
-        return self.owner
+        # This looks like it's the action initiator, no? Seems more correct than the owner.
+        return self.user
 
     @property
-    def summary(self):
-        return (
-            f"Build {BUILD_STATES(self.new).name}: {self.owner}'s "
-            f"{self.name}-{self.version}-{self.release}"
-        )
+    def usernames(self) -> list[str]:
+        return [name for name in (self.agent_name, self.owner) if name is not None]
 
     @property
-    def packages(self) -> List[str]:
-        return [self.name] if self.name else []
+    def is_mass_rebuild(self) -> bool:
+        return self.tag and _MASS_REBUILD_RE.match(self.tag) is not None
+
+    @property
+    def is_eln(self) -> bool:
+        return self.tag and _ELN_RE.match(self.tag) is not None
+
+    def _choose_priority(self) -> int:
+        # https://pagure.io/fedora-infrastructure/issue/10899
+        if self.is_mass_rebuild:
+            return 0
+        if self.is_eln:
+            return 1
+        return 2
+
+
+class TagV1(TagMessage):
+    """This message is sent when a package is tagged."""
+
+    topic = "buildsys.tag"
+    _summary_action = "tagged into"
+    body_schema = {
+        "$id": f"{SCHEMA_URL}/v1/{topic}#",
+        "$schema": "https://json-schema.org/draft/2019-09/schema",
+        "description": "A package is tagged.",
+        "type": "object",
+        "properties": TAG,
+    }
+
+
+class UntagV1(TagMessage):
+    """This message is sent when a package is untagged."""
+
+    topic = "buildsys.untag"
+    _summary_action = "untagged from"
+    body_schema = {
+        "$id": f"{SCHEMA_URL}/v1/{topic}#",
+        "$schema": "https://json-schema.org/draft/2019-09/schema",
+        "description": "A package is untagged.",
+        "type": "object",
+        "properties": TAG,
+    }
```

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/package.py` & `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Define schema for fedora messages sent by koji"""
-from typing import Optional, List
+from typing import Optional
 
 from fedora_messaging.message import DEBUG
 
-from .base import KojiFedoraMessagingMessage, SCHEMA_URL
+from .base import SCHEMA_URL, KojiFedoraMessagingMessage
 
 
 class ListChangeV1(KojiFedoraMessagingMessage):
     """This message is sent when a package list changes."""
 
     topic = "buildsys.package.list.change"
     severity = DEBUG
@@ -83,17 +83,15 @@
 
     @property
     def owner(self) -> Optional[str]:
         return self.body.get("owner")
 
     @property
     def agent_name(self) -> Optional[str]:
-        return (
-            self.owner
-        )  # is this action always done by the package owner? This seems incorrect.
+        return self.owner  # is this action always done by the package owner? This seems incorrect.
 
     @property
     def tag(self) -> str:
         return self.body.get("tag")
 
     @property
     def action(self) -> str:
@@ -104,9 +102,9 @@
         return self.body.get("block")
 
     @property
     def summary(self):
         return f"Package list change for {self.package}:  {self.tag}"
 
     @property
-    def packages(self) -> List[str]:
+    def packages(self) -> list[str]:
         return [self.package] if self.package else []
```

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/repo.py` & `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Define schema for fedora messages sent by koji"""
 
 from fedora_messaging.message import DEBUG
 
-from .base import KojiFedoraMessagingMessage, SCHEMA_URL
+from .base import SCHEMA_URL, KojiFedoraMessagingMessage
 
 REPO = {
     "type": "object",
     "properties": {
         "instance": {
             "type": "string",
             "description": "distinguish between messages from primary and secondary koji",
```

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/rpm.py` & `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/rpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Define schema for fedora messages sent by koji"""
 
 from fedora_messaging.message import DEBUG
 
-from .base import KojiFedoraMessagingMessage, SCHEMA_URL
+from .base import SCHEMA_URL, KojiFedoraMessagingMessage
 
 
 class SignV1(KojiFedoraMessagingMessage):
     """This message is sent when a rpm is signed."""
 
     topic = "buildsys.rpm.sign"
     severity = DEBUG
```

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/task.py` & `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,183 +1,182 @@
-# Copyright © 2020 Red Hat, Inc.
+# Copyright (C) 2023  Red Hat, Inc.
 #
-# This program is free software: you can redistribute it and/or modify
+# This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3 of the License.
+# the Free Software Foundation; either version 2 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""Define schema for fedora messages sent by koji"""
-
-
-from .base import KojiFedoraMessagingMessage, SCHEMA_URL
-
-
-class TaskStateChangeV1(KojiFedoraMessagingMessage):
-    """This message is sent when a task state changes."""
-
-    topic = "buildsys.task.state.change"
-
-    body_schema = {
-        "$id": f"{SCHEMA_URL}/v1/{topic}#",
-        "$schema": "https://json-schema.org/draft/2019-09/schema",
-        "description": "A koji task state changed.",
-        "type": "object",
-        "properties": {
-            "info": {
-                "type": "object",
-                "description": "task info",
-                "properties": {
-                    "parent": {
-                        "type": ["null", "array"],
-                        "description": "parent tasks",
-                    },
-                    "completion_time": {
-                        "type": ["number", "null"],
-                        "description": "completion time",
-                    },
-                    "start_time": {
-                        "type": "number",
-                        "description": "start time",
-                    },
-                    "request": {
-                        "description": "task request details",
-                    },
-                    "waiting": {
-                        "type": ["boolean", "null"],
-                        "description": "Is the task waiting or not",
-                    },
-                    "awaited": {
-                        "type": "null",
-                        "description": "awaited",
-                    },
-                    "id": {
-                        "type": "integer",
-                        "description": "id",
-                    },
-                    "priority": {
-                        "type": "integer",
-                        "description": "priority",
-                    },
-                    "channel_id": {
-                        "type": "integer",
-                        "description": "channel_id",
-                    },
-                    "state": {
-                        "type": "integer",
-                        "description": "task state",
-                    },
-                    "create_time": {
-                        "type": "number",
-                        "description": "create time",
-                    },
-                    "result": {
-                        "type": ["null", "string"],
-                        "description": "result",
-                    },
-                    "owner": {
-                        "type": ["null", "string", "integer"],
-                        "description": "owner name or id",
-                    },
-                    "host_id": {
-                        "type": ["null", "integer"],
-                        "description": "host id",
-                    },
-                    "method": {
-                        "type": "string",
-                        "description": "task method",
-                    },
-                    "label": {
-                        "type": "null",
-                        "description": "label",
-                    },
-                    "arch": {
-                        "type": "string",
-                        "description": "task specific architecture",
-                    },
-                    "children": {
-                        "type": ["null", "array"],
-                        "description": "task childrens",
-                    },
-                },
-            },
-            "old": {
-                "type": ["string", "null"],
-                "description": "previous task state",
-            },
-            "attribute": {"type": "string", "description": "attribute"},
-            "id": {
-                "type": "integer",
-                "description": "task id",
-            },
-            "instance": {
+# You should have received a copy of the GNU General Public License along
+# with this program; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+
+
+from fedora_messaging import message
+
+SCHEMA_URL = "http://fedoraproject.org/message-schema/"
+
+
+TASK_RESULT = {
+    "type": ["null", "object"],
+    "description": "the results of a task (files)",
+    "properties": {
+        "srpm": {
+            "type": "string",
+        },
+        "rpms": {
+            "type": "array",
+            "items": {
                 "type": "string",
-                "description": "distinguish between messages from primary and secondary koji",
             },
-            "owner": {
+        },
+        "srpms": {
+            "type": "array",
+            "items": {
                 "type": "string",
-                "description": "name of the package owner",
             },
-            "new": {
+        },
+        "logs": {
+            "type": "array",
+            "items": {
                 "type": "string",
-                "description": "name of the new task state",
             },
-            "srpm": {
-                "type": "string",
-                "description": "name of the source rpm",
+        },
+        "brootid": {
+            "type": "number",
+        },
+        "source": {
+            "type": "object",
+            "properties": {
+                "source": {"type": "string"},
+                "url": {"type": "string"},
             },
-            "method": {"type": "string", "description": "name of the task method"},
         },
-    }
-
-    @property
-    def info(self) -> dict:
-        return self.body.get("info")
+    },
+}
 
-    @property
-    def old(self) -> str:
-        return self.body.get("old")
-
-    @property
-    def attribute(self) -> str:
-        return self.body.get("attribute")
-
-    @property
-    def task_id(self) -> int:
-        return self.body.get("id")
+TASK_INFO = {
+    "$anchor": "task_info",
+    "type": "object",
+    "description": "Information about a task",
+    "properties": {
+        "id": {
+            "type": "integer",
+            "description": "task id",
+        },
+        "url": {
+            "type": "string",
+            "description": "Task URL in koji-web",
+        },
+        "priority": {
+            "type": "integer",
+            "description": "priority",
+        },
+        "method": {
+            "type": "string",
+            "description": "task method",
+        },
+        "label": {
+            "type": ["null", "string"],
+            "description": "label",
+        },
+        "arch": {
+            "type": "string",
+            "description": "task specific architecture",
+        },
+        "channel_id": {
+            "type": "integer",
+            "description": "channel_id",
+        },
+        "request": {
+            "description": "task request details",
+            "type": ["array"],
+        },
+        "result": TASK_RESULT,
+        # Timestamps
+        "completion_time": {
+            "type": ["number", "null"],
+            "description": "completion time",
+        },
+        "start_time": {
+            "type": "number",
+            "description": "start time",
+        },
+        "create_time": {
+            "type": "number",
+            "description": "create time",
+        },
+        # State
+        "waiting": {
+            "type": ["boolean", "null"],
+            "description": "Is the task waiting or not",
+        },
+        "awaited": {
+            "type": ["boolean", "null"],
+            "description": "awaited",
+        },
+        "state": {
+            "type": "integer",
+            "description": "task state",
+        },
+        # Builder
+        "host_id": {
+            "type": ["null", "integer"],
+            "description": "builder host id",
+        },
+        "host_name": {
+            "type": ["null", "string"],
+            "description": "builder hostname",
+        },
+        # Hierarchy
+        "parent": {
+            "type": ["null", "number"],
+            "description": "parent task, if any",
+        },
+        "children": {
+            "type": "array",
+            "description": "sub-tasks",
+            "items": {"$ref": "#task_info"},
+        },
+    },
+    "required": ["id", "method", "host_id", "arch", "result"],
+}
 
-    @property
-    def instance(self) -> str:
-        return self.body.get("instance")
 
-    @property
-    def owner(self) -> str:
-        return self.body.get("owner")
+class KojiFedoraMessagingMessage(message.Message):
+    """
+    A sub-class of a Fedora message that defines a message schema for messages
+    published by the koji fedora-messaging plugin.
+    """
 
     @property
-    def agent_name(self) -> str:
-        return None  # Do we know who initiated the action?
+    def app_name(self):
+        return "Koji"
 
     @property
-    def new(self) -> str:
-        return self.body.get("new")
+    def app_icon(self):
+        return "https://apps.fedoraproject.org/img/icons/koji.png"
 
     @property
-    def srpm(self) -> str:
-        return self.body.get("srpm")
+    def owner(self):
+        return None
 
     @property
-    def arch(self) -> str:
-        return self.info.get("arch")
+    def agent_name(self):
+        # This seems wrong: actions on a package aren't always triggered by the package owner, no?
+        # If we're not sure who initiated the action, it's better to have agent_name be None.
+        # In any case, this seems like a dangerous default here.
+        return self.owner
 
     @property
-    def method(self) -> str:
-        return self.body.get("method")
+    def usernames(self):
+        if self.agent_name:
+            return [self.agent_name]
+        else:
+            return []
 
-    @property
-    def summary(self):
-        return f"Task {self.new} -- {self.method or ''} ({self.srpm or ''} {self.arch or ''})"
+    def __str__(self):
+        return self.summary
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_build.py` & `koji-fedoramessaging-messages-1.2.0/tests/test_tag.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,82 @@
-from koji_fedoramessaging_messages.build import BuildStateChangeV1
+import pytest
 
+from koji_fedoramessaging_messages.tag import TagV1, UntagV1
 
-def test_build_state_change_message():
+
+def test_tag_message():
     body = {
-        "build_id": 1478312,
-        "old": 0,
-        "name": "chromium",
-        "task_id": 42561864,
-        "attribute": "state",
-        "request": [
-            (
-                "git+https://src.fedoraproject.org/rpms/chromium.git#"
-                "5f8f367e482fe8e30711aea49bf2ecfd163d278f"
-            ),
-            "rawhide",
-            {},
-        ],
+        "build_id": 1457909,
+        "name": "http-parser",
+        "tag_id": 6446,
         "instance": "primary",
-        "epoch": None,
-        "version": "80.0.3987.132",
-        "owner": "spot",
-        "new": 1,
-        "release": "1.fc33",
+        "tag": "f31-updates-pending",
+        "user": "bodhi",
+        "version": "2.9.3",
+        "owner": "sgallagh",
+        "release": "1.fc31",
     }
 
-    msg = BuildStateChangeV1(body=body)
+    msg = TagV1(body=body)
     msg.validate()
-    assert msg.build_id == 1478312
-    assert msg.name == "chromium"
-    assert msg.owner == "spot"
-    assert msg.version == "80.0.3987.132"
-    assert msg.release == "1.fc33"
-    assert msg.old == 0
-    assert msg.new == 1
-    assert msg.task_id == 42561864
-    assert msg.attribute == "state"
-    assert msg.request == body["request"]
+    assert msg.build_id == 1457909
+    assert msg.name == "http-parser"
+    assert msg.tag == "f31-updates-pending"
+    assert msg.tag_id == 6446
     assert msg.instance == "primary"
-    assert msg.epoch is None
+    assert msg.user == "bodhi"
+    assert msg.owner == "sgallagh"
+    assert msg.version == "2.9.3"
+    assert msg.release == "1.fc31"
 
-    assert msg.agent_name == "spot"
-    assert msg.summary == "Build COMPLETE: spot's chromium-80.0.3987.132-1.fc33"
+    assert msg.agent_name == "bodhi"
+    assert msg.agent_avatar == (
+        "https://seccdn.libravatar.org/avatar/"
+        "6f26f2d69404c1b45b3cacc63054bdd0d8270c262335cdda5930c29a8ebc35f1?s=64&d=retro"
+    )
+    assert msg.summary == "http-parser-2.9.3-1.fc31 was tagged into f31-updates-pending by bodhi"
     assert str(msg) == msg.summary
-    assert msg.packages == ["chromium"]
+
+
+def test_untag_message():
+    body = {
+        "build_id": 1478431,
+        "name": "python-twisted",
+        "tag_id": 10321,
+        "instance": "primary",
+        "tag": "epel8-signing-pending",
+        "user": "autopen",
+        "version": "19.10.0",
+        "owner": "eclipseo",
+        "release": "2.el8",
+    }
+
+    msg = UntagV1(body=body)
+    msg.validate()
+    assert msg.build_id == 1478431
+    assert msg.name == "python-twisted"
+    assert msg.tag == "epel8-signing-pending"
+    assert msg.tag_id == 10321
+    assert msg.instance == "primary"
+    assert msg.user == "autopen"
+    assert msg.owner == "eclipseo"
+    assert msg.version == "19.10.0"
+    assert msg.release == "2.el8"
+    assert (
+        msg.summary
+        == "python-twisted-19.10.0-2.el8 was untagged from epel8-signing-pending by autopen"
+    )
+    assert str(msg) == msg.summary
+    assert msg.packages == ["python-twisted"]
+
+
+@pytest.mark.parametrize(
+    "tag,prio",
+    [("f42", 2), ("f42-rebuild", 0), ("eln", 1), ("eln-rebuild", 1), (None, 2)],
+)
+def test_tag_priority(tag, prio):
+    body = {
+        "tag": tag,
+    }
+    msg = TagV1(body=body)
+    msg.validate()
+    assert msg.priority == prio
```

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_package.py` & `koji-fedoramessaging-messages-1.2.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_repo.py` & `koji-fedoramessaging-messages-1.2.0/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_rpm.py` & `koji-fedoramessaging-messages-1.2.0/tests/test_rpm.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.1.0/setup.py` & `koji-fedoramessaging-messages-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['koji_fedoramessaging_messages', 'koji_fedoramessaging_messages.tests']
+['koji_fedoramessaging_messages']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['fedora-messaging>=3.0.1']
 
@@ -26,15 +26,15 @@
                      'koji_fedoramessaging.tag.UntagV1 = '
                      'koji_fedoramessaging_messages.tag:UntagV1',
                      'koji_fedoramessaging.task.TaskStateChangeV1 = '
                      'koji_fedoramessaging_messages.task:TaskStateChangeV1']}
 
 setup_kwargs = {
     'name': 'koji-fedoramessaging-messages',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': 'A schema package for messages sent by the koji-fedoramessaging plugin',
     'long_description': '# koji-fedoramessaging messages\n\nA schema package for [koji-fedoramessaging](http://github.com/fedora-infra/koji-fedoramessaging).\n\nSee the [detailed documentation](https://fedora-messaging.readthedocs.io/en/latest/messages.html) on packaging your schemas.\n',
     'author': 'Fedora Infrastructure Team',
     'author_email': 'infrastructure@lists.fedoraproject.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fedora-infra/koji-fedoramessaging-messages',
```

### Comparing `koji-fedoramessaging-messages-1.1.0/PKG-INFO` & `koji-fedoramessaging-messages-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji-fedoramessaging-messages
-Version: 1.1.0
+Version: 1.2.0
 Summary: A schema package for messages sent by the koji-fedoramessaging plugin
 Home-page: https://github.com/fedora-infra/koji-fedoramessaging-messages
 License: GPL-3.0-or-later
 Keywords: fedora
 Author: Fedora Infrastructure Team
 Author-email: infrastructure@lists.fedoraproject.org
 Requires-Python: >=3.10,<4.0
```

