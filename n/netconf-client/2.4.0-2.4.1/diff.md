# Comparing `tmp/netconf_client-2.4.0.tar.gz` & `tmp/netconf_client-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netconf_client-2.4.0.tar", max compression
+gzip compressed data, was "netconf_client-2.4.1.tar", max compression
```

## Comparing `netconf_client-2.4.0.tar` & `netconf_client-2.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1528 2023-06-12 17:11:16.937588 netconf_client-2.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 17:11:16.937588 netconf_client-2.4.0/netconf_client/__init__.py
--rw-r--r--   0        0        0     7590 2023-06-12 17:11:16.937588 netconf_client-2.4.0/netconf_client/connect.py
--rw-r--r--   0        0        0      511 2023-06-12 17:11:16.937588 netconf_client-2.4.0/netconf_client/constants.py
--rw-r--r--   0        0        0     1911 2023-06-12 17:11:16.937588 netconf_client-2.4.0/netconf_client/error.py
--rw-r--r--   0        0        0       61 2023-06-12 17:11:16.937588 netconf_client-2.4.0/netconf_client/log.py
--rw-r--r--   0        0        0    18737 2023-06-12 17:11:16.941589 netconf_client-2.4.0/netconf_client/ncclient.py
--rw-r--r--   0        0        0     4401 2023-06-12 17:11:16.941589 netconf_client-2.4.0/netconf_client/parser.py
--rw-r--r--   0        0        0     5621 2023-06-12 17:11:16.941589 netconf_client-2.4.0/netconf_client/rpc.py
--rw-r--r--   0        0        0     4795 2023-06-12 17:11:16.941589 netconf_client-2.4.0/netconf_client/session.py
--rw-r--r--   0        0        0      961 2023-06-12 17:11:16.941589 netconf_client-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 netconf_client-2.4.0/setup.py
--rw-r--r--   0        0        0     2537 1970-01-01 00:00:00.000000 netconf_client-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1360 2023-06-12 19:59:17.884200 netconf_client-2.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/__init__.py
+-rw-r--r--   0        0        0     7517 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/connect.py
+-rw-r--r--   0        0        0      511 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/constants.py
+-rw-r--r--   0        0        0     1911 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/error.py
+-rw-r--r--   0        0        0       61 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/log.py
+-rw-r--r--   0        0        0    18737 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/ncclient.py
+-rw-r--r--   0        0        0     4401 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/parser.py
+-rw-r--r--   0        0        0     5621 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/rpc.py
+-rw-r--r--   0        0        0     4795 2023-06-12 19:59:17.884200 netconf_client-2.4.1/netconf_client/session.py
+-rw-r--r--   0        0        0      959 2023-06-12 19:59:17.884200 netconf_client-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 netconf_client-2.4.1/setup.py
+-rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 netconf_client-2.4.1/PKG-INFO
```

### Comparing `netconf_client-2.4.0/README.md` & `netconf_client-2.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 ![Build Status](https://github.com/ADTRAN/netconf_client/workflows/CI%20Checks/badge.svg)
 [![PyPI version](https://badge.fury.io/py/netconf-client.svg)](https://badge.fury.io/py/netconf-client)
-[![Documentation Status](https://readthedocs.org/projects/netconf-client/badge/?version=latest)](https://netconf-client.readthedocs.io/en/latest/?badge=latest)
 
 # netconf_client
 
 A NETCONF client for Python 3.6+.
 
 ## Basic Usage
 
@@ -36,8 +35,8 @@
  - Support for non-RFC-compliant devices isn't really included in
    `netconf_client`
  - `netconf_client` does a lot less error checking and assumes you're
    sending valid messages to the server (however this can be useful
    for testing edge-case behavior of a server)
 
 
-[User Guide]: https://netconf-client.readthedocs.io/en/latest/
+[User Guide]: https://adtran.github.io/netconf_client/
```

### Comparing `netconf_client-2.4.0/netconf_client/connect.py` & `netconf_client-2.4.1/netconf_client/connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,21 +43,18 @@
     :param int initial_timeout: Seconds to wait when first connecting the socket.
 
     :param int general_timeout: Seconds to wait for a response from the server after connecting.
 
     :param int timeout: (Deprecated) Seconds to wait when connecting the socket if initial_timeout is None.  This will
                         be ignored if initial_timeout is not None, and will be removed in the next major release.
 
-    :param str hostkey_b64: (Deprecated) Base64-encoded SSH host key.  This will
-    be ignored if hostkey_b64 is not None.
+    :param str hostkey_b64: base64 encoded hostkey.
 
     :return: :class:`Session` object
 
-    :param str hostkey_b64: base64 encoded hostkey.
-
     :rtype: :class:`netconf_client.session.Session`
 
     """
     if not sock:
         sock = socket.socket()
         sock.settimeout(initial_timeout or timeout)
         sock.connect((host, port))
@@ -76,14 +73,16 @@
     host=None,
     port=6513,
     keyfile=None,
     certfile=None,
     ca_certs=None,
     sock=None,
     timeout=120,
+    initial_timeout=None,
+    general_timeout=None,
 ):
     """Connect to a NETCONF server over TLS.
 
     :param str host: Hostname or IP address; unused if an already-open
                      socket is provided
 
     :param int port: TCP port to initiate the connection; unused if an
```

### Comparing `netconf_client-2.4.0/netconf_client/error.py` & `netconf_client-2.4.1/netconf_client/error.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.4.0/netconf_client/ncclient.py` & `netconf_client-2.4.1/netconf_client/ncclient.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.4.0/netconf_client/parser.py` & `netconf_client-2.4.1/netconf_client/parser.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.4.0/netconf_client/rpc.py` & `netconf_client-2.4.1/netconf_client/rpc.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.4.0/netconf_client/session.py` & `netconf_client-2.4.1/netconf_client/session.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.4.0/pyproject.toml` & `netconf_client-2.4.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netconf_client"
-version = "2.4.0"
+version = "2.4.1"
 description = "A Python NETCONF client"
 authors = ["ADTRAN, Inc."]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ADTRAN/netconf_client"
 repository = "https://github.com/ADTRAN/netconf_client"
 documentation = "https://netconf-client.readthedocs.io"
@@ -21,16 +21,16 @@
 paramiko = "^2.7.2 || ^3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 pylama = "^7.7"
 pylint = "^2.9"
 pytest-cov = "^2.12"
-black = "21.7b0"
-sphinx = "^3.5"
+black = "22.8.0"
+sphinx = "^5"
 
 [tool.pytest.ini_options]
 addopts = "-vvl --cov=netconf_client --cov-branch --cov-report term-missing"
 testpaths = ["test"]
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
```

### Comparing `netconf_client-2.4.0/setup.py` & `netconf_client-2.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['lxml>=4.6.3,<5.0.0', 'paramiko>=2.7.2,<4']
 
 setup_kwargs = {
     'name': 'netconf-client',
-    'version': '2.4.0',
+    'version': '2.4.1',
     'description': 'A Python NETCONF client',
-    'long_description': '![Build Status](https://github.com/ADTRAN/netconf_client/workflows/CI%20Checks/badge.svg)\n[![PyPI version](https://badge.fury.io/py/netconf-client.svg)](https://badge.fury.io/py/netconf-client)\n[![Documentation Status](https://readthedocs.org/projects/netconf-client/badge/?version=latest)](https://netconf-client.readthedocs.io/en/latest/?badge=latest)\n\n# netconf_client\n\nA NETCONF client for Python 3.6+.\n\n## Basic Usage\n\n```python\nfrom netconf_client.connect import connect_ssh\nfrom netconf_client.ncclient import Manager\n\nsession = connect_ssh(host="localhost", port=830, username="admin", password="password")\nmgr = Manager(session, timeout=120)\n\nmgr.edit_config(config="""<config> ... </config>""")\nprint(mgr.get(filter="""<filter> ... </filter>""").data_xml)\n```\n\nMore complete documentation can be found in the [User Guide]\n\n## Comparison with `ncclient`\n\nCompared to [ncclient](https://github.com/ncclient/ncclient),\n`netconf_client` has several advantages:\n\n - It\'s simpler (at the time of writing: 789 LoC vs 2889 LoC)\n - lxml can be bypassed, which can work around issues where lxml\n   breaks namespaces of e.g. identityrefs\n - Support for TLS sessions\n\nAnd a few disadvantages:\n\n - Support for non-RFC-compliant devices isn\'t really included in\n   `netconf_client`\n - `netconf_client` does a lot less error checking and assumes you\'re\n   sending valid messages to the server (however this can be useful\n   for testing edge-case behavior of a server)\n\n\n[User Guide]: https://netconf-client.readthedocs.io/en/latest/\n',
+    'long_description': '![Build Status](https://github.com/ADTRAN/netconf_client/workflows/CI%20Checks/badge.svg)\n[![PyPI version](https://badge.fury.io/py/netconf-client.svg)](https://badge.fury.io/py/netconf-client)\n\n# netconf_client\n\nA NETCONF client for Python 3.6+.\n\n## Basic Usage\n\n```python\nfrom netconf_client.connect import connect_ssh\nfrom netconf_client.ncclient import Manager\n\nsession = connect_ssh(host="localhost", port=830, username="admin", password="password")\nmgr = Manager(session, timeout=120)\n\nmgr.edit_config(config="""<config> ... </config>""")\nprint(mgr.get(filter="""<filter> ... </filter>""").data_xml)\n```\n\nMore complete documentation can be found in the [User Guide]\n\n## Comparison with `ncclient`\n\nCompared to [ncclient](https://github.com/ncclient/ncclient),\n`netconf_client` has several advantages:\n\n - It\'s simpler (at the time of writing: 789 LoC vs 2889 LoC)\n - lxml can be bypassed, which can work around issues where lxml\n   breaks namespaces of e.g. identityrefs\n - Support for TLS sessions\n\nAnd a few disadvantages:\n\n - Support for non-RFC-compliant devices isn\'t really included in\n   `netconf_client`\n - `netconf_client` does a lot less error checking and assumes you\'re\n   sending valid messages to the server (however this can be useful\n   for testing edge-case behavior of a server)\n\n\n[User Guide]: https://adtran.github.io/netconf_client/\n',
     'author': 'ADTRAN, Inc.',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ADTRAN/netconf_client',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `netconf_client-2.4.0/PKG-INFO` & `netconf_client-2.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netconf-client
-Version: 2.4.0
+Version: 2.4.1
 Summary: A Python NETCONF client
 Home-page: https://github.com/ADTRAN/netconf_client
 License: Apache-2.0
 Keywords: netconf
 Author: ADTRAN, Inc.
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,14 @@
 Requires-Dist: paramiko (>=2.7.2,<4)
 Project-URL: Documentation, https://netconf-client.readthedocs.io
 Project-URL: Repository, https://github.com/ADTRAN/netconf_client
 Description-Content-Type: text/markdown
 
 ![Build Status](https://github.com/ADTRAN/netconf_client/workflows/CI%20Checks/badge.svg)
 [![PyPI version](https://badge.fury.io/py/netconf-client.svg)](https://badge.fury.io/py/netconf-client)
-[![Documentation Status](https://readthedocs.org/projects/netconf-client/badge/?version=latest)](https://netconf-client.readthedocs.io/en/latest/?badge=latest)
 
 # netconf_client
 
 A NETCONF client for Python 3.6+.
 
 ## Basic Usage
 
@@ -61,9 +60,9 @@
  - Support for non-RFC-compliant devices isn't really included in
    `netconf_client`
  - `netconf_client` does a lot less error checking and assumes you're
    sending valid messages to the server (however this can be useful
    for testing edge-case behavior of a server)
 
 
-[User Guide]: https://netconf-client.readthedocs.io/en/latest/
+[User Guide]: https://adtran.github.io/netconf_client/
```

