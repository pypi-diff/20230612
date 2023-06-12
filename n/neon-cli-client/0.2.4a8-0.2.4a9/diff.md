# Comparing `tmp/neon_cli_client-0.2.4a8-py3-none-any.whl.zip` & `tmp/neon_cli_client-0.2.4a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27177 bytes, number of entries: 12
--rw-r--r--  2.0 unx     2433 b- defN 23-Mar-14 00:20 neon_cli/__init__.py
--rw-r--r--  2.0 unx     3776 b- defN 23-Mar-14 00:20 neon_cli/__main__.py
--rw-r--r--  2.0 unx     2824 b- defN 23-Mar-14 00:20 neon_cli/cli.py
--rw-r--r--  2.0 unx     6243 b- defN 23-Mar-14 00:20 neon_cli/gui_server.py
--rw-r--r--  2.0 unx    48476 b- defN 23-Mar-14 00:20 neon_cli/text_client.py
--rw-r--r--  2.0 unx       94 b- defN 23-Mar-14 00:20 neon_cli/utils.py
--rw-r--r--  2.0 unx    11745 b- defN 23-Mar-14 00:20 neon_cli_client-0.2.4a8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1882 b- defN 23-Mar-14 00:20 neon_cli_client-0.2.4a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-14 00:20 neon_cli_client-0.2.4a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Mar-14 00:20 neon_cli_client-0.2.4a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-14 00:20 neon_cli_client-0.2.4a8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1002 b- defN 23-Mar-14 00:20 neon_cli_client-0.2.4a8.dist-info/RECORD
-12 files, 78627 bytes uncompressed, 25485 bytes compressed:  67.6%
+Zip file size: 27172 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     2433 b- defN 23-Jun-12 18:38 neon_cli/__init__.py
+-rw-r--r--  2.0 unx     3776 b- defN 23-Jun-12 18:38 neon_cli/__main__.py
+-rw-r--r--  2.0 unx     2824 b- defN 23-Jun-12 18:38 neon_cli/cli.py
+-rw-r--r--  2.0 unx     6242 b- defN 23-Jun-12 18:38 neon_cli/gui_server.py
+-rw-r--r--  2.0 unx    48473 b- defN 23-Jun-12 18:38 neon_cli/text_client.py
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-12 18:38 neon_cli/utils.py
+-rw-r--r--  2.0 unx    11745 b- defN 23-Jun-12 18:39 neon_cli_client-0.2.4a9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1866 b- defN 23-Jun-12 18:39 neon_cli_client-0.2.4a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 18:39 neon_cli_client-0.2.4a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-12 18:39 neon_cli_client-0.2.4a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-12 18:39 neon_cli_client-0.2.4a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1002 b- defN 23-Jun-12 18:39 neon_cli_client-0.2.4a9.dist-info/RECORD
+12 files, 78607 bytes uncompressed, 25480 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: neon_cli/text_client.py
 Comment: 
 
 Filename: neon_cli/utils.py
 Comment: 
 
-Filename: neon_cli_client-0.2.4a8.dist-info/LICENSE.md
+Filename: neon_cli_client-0.2.4a9.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_cli_client-0.2.4a8.dist-info/METADATA
+Filename: neon_cli_client-0.2.4a9.dist-info/METADATA
 Comment: 
 
-Filename: neon_cli_client-0.2.4a8.dist-info/WHEEL
+Filename: neon_cli_client-0.2.4a9.dist-info/WHEEL
 Comment: 
 
-Filename: neon_cli_client-0.2.4a8.dist-info/entry_points.txt
+Filename: neon_cli_client-0.2.4a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_cli_client-0.2.4a8.dist-info/top_level.txt
+Filename: neon_cli_client-0.2.4a9.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_cli_client-0.2.4a8.dist-info/RECORD
+Filename: neon_cli_client-0.2.4a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_cli/gui_server.py

```diff
@@ -36,16 +36,16 @@
 # limitations under the License.
 #
 
 from os import getpid
 from os.path import basename
 import json
 import websocket
-from threading import Thread, Lock
-from mycroft_bus_client import Message
+from threading import Thread
+from ovos_bus_client.message import Message
 
 
 bus = None
 buffer = None       # content will show on the CLI "GUI" representation
 msgs = []
 
 loaded = []
```

## neon_cli/text_client.py

```diff
@@ -46,15 +46,15 @@
 import os
 import os.path
 import time
 import curses
 import textwrap
 import json
 from threading import Thread, Lock
-from mycroft_bus_client import Message, MessageBusClient
+from ovos_bus_client import Message, MessageBusClient
 from ovos_config.config import Configuration
 from logging import getLogger
 
 
 import locale
 
 LOG = getLogger("NeonDebugCLI")
```

## Comparing `neon_cli_client-0.2.4a8.dist-info/LICENSE.md` & `neon_cli_client-0.2.4a9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_cli_client-0.2.4a8.dist-info/METADATA` & `neon_cli_client-0.2.4a9.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: neon-cli-client
-Version: 0.2.4a8
+Version: 0.2.4a9
 Summary: Packaged CLI Client from Neon, Mycroft, and OVOS cores
 Home-page: https://github.com/NeonGeckoCom/neon_cli
 Author: Neongecko
 Author-email: developers@neon.ai
 License: apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: mycroft-messagebus-client (>=0.9.4,~=0.9)
+Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: neon-utils (~=1.0)
 Requires-Dist: ovos-config (~=0.0)
 Requires-Dist: click (~=8.0)
 Requires-Dist: click-default-group (~=1.2)
 
 # Neon CLI Client
 This is a lightly modified client from [mycroft-core](https://github.com/MycroftAI/mycroft-core/tree/dev/mycroft/client/text).
```

