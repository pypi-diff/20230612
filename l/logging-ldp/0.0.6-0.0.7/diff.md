# Comparing `tmp/logging-ldp-0.0.6.tar.gz` & `tmp/logging-ldp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logging-ldp-0.0.6.tar", last modified: Thu Jun 13 14:25:55 2019, max compression
+gzip compressed data, was "dist/logging-ldp-0.0.7.tar", last modified: Mon Jun 12 09:28:05 2023, max compression
```

## Comparing `logging-ldp-0.0.6.tar` & `logging-ldp-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1934 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/README.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)      888 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1516 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      517 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/CONTRIBUTORS
--rw-rw-r--   0 travis    (2000) travis    (2000)     3242 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2762 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/VERSION
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/AUTHORS
--rw-rw-r--   0 travis    (2000) travis    (2000)     2844 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/CONTRIBUTING.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/logging_ldp.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/logging_ldp.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/logging_ldp.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/logging_ldp.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2762 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/logging_ldp.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/logging_ldp.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/logging_ldp.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-13 14:25:55.000000 logging-ldp-0.0.6/src/logging_ldp/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1241 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/src/logging_ldp/formatters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      213 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/src/logging_ldp/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      529 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/src/logging_ldp/handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2019-06-13 14:25:35.000000 logging-ldp-0.0.6/src/logging_ldp/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)      517 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/CONTRIBUTORS
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/README.rst
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/VERSION
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      888 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/logging_ldp/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/src/logging_ldp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/src/logging_ldp/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/src/logging_ldp/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-12 09:27:47.000000 logging-ldp-0.0.7/src/logging_ldp/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/logging_ldp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/logging_ldp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/logging_ldp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/logging_ldp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/logging_ldp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/logging_ldp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:28:05.000000 logging-ldp-0.0.7/src/logging_ldp.egg-info/zip-safe
```

### Comparing `logging-ldp-0.0.6/README.rst` & `logging-ldp-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `logging-ldp-0.0.6/setup.py` & `logging-ldp-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `logging-ldp-0.0.6/LICENSE` & `logging-ldp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `logging-ldp-0.0.6/CONTRIBUTORS` & `logging-ldp-0.0.7/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `logging-ldp-0.0.6/CODE_OF_CONDUCT.md` & `logging-ldp-0.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `logging-ldp-0.0.6/PKG-INFO` & `logging-ldp-0.0.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,78 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: logging-ldp
-Version: 0.0.6
+Version: 0.0.7
 Summary: OVH library bundle to send logs on Log Data Platform (LDP)
 Home-page: https://github.com/ovh/python-logging-ldp
 Author: OVH SAS
 Author-email: github@ovh.net
 License: BSD
-Description: **********************************
-        Logging for OVH Logs Data Platform
-        **********************************
-        
-        .. image:: https://img.shields.io/pypi/v/logging-ldp.svg
-           :target: https://pypi.python.org/pypi/logging-ldp/
-           :alt: Latest Version
-        
-        .. image:: https://travis-ci.org/ovh/python-logging-ldp.svg?branch=master
-           :target: https://travis-ci.org/ovh/python-logging-ldp
-           :alt: Latest version
-        
-        
-        .. image:: https://readthedocs.org/projects/logging-ldp/badge/?version=latest
-           :target: http://logging-ldp.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Status
-        
-        
-        A python logging bundle to send logs using GELF on the OVH Logs Data Platform.
-        
-        Quickstart
-        ==========
-        
-        First, install logging-ldp using `pip <https://pip.pypa.io/en/stable/>`_::
-        
-            pip install -U logging-ldp
-        
-        The following example shows how to send log in Graylog TCP input
-        
-        .. code-block:: python
-        
-            import logging
-            from logging_ldp.formatters import LDPGELFFormatter
-            from logging_ldp.handlers import LDPGELFTCPSocketHandler
-        
-            logger = logging.getLogger("ldp")
-            logger.setLevel(logging.DEBUG)
-        
-            handler = LDPGELFTCPSocketHandler(hostname="gra1.logs.ovh.com")
-            handler.setFormatter(LDPGELFFormatter(token="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"))
-            logger.addHandler(handler)
-            logger.debug("hello !")
-        
-        
-        Requirements
-        ============
-        
-        - Python >= 3.3
-        
-        Project Links
-        =============
-        
-        - Docs: http://logging-ldp.readthedocs.io/
-        - PyPI: https://pypi.python.org/pypi/logging-ldp
-        - Issues: https://github.com/ovh/python-logging-ldp/issues
-        - OVH Logs Data Platform
-            - Homepage (FR): https://logs.ovh.com
-            - Documentation: https://docs.ovh.com/fr/logs-data-platform/
-        - Graylog & GELF
-            - Documentation: http://docs.graylog.org/en/latest/pages/gelf.html
-            - Python logging-gelf: http://logging-gelf.readthedocs.io/
-        
-        License
-        =======
-        
-        Licensed under `BSD 3-Clause License <./LICENSE>`_ or https://opensource.org/licenses/BSD-3-Clause.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
+License-File: LICENSE
+License-File: AUTHORS
+
+**********************************
+Logging for OVH Logs Data Platform
+**********************************
+
+.. image:: https://img.shields.io/pypi/v/logging-ldp.svg
+   :target: https://pypi.python.org/pypi/logging-ldp/
+   :alt: Latest Version
+
+.. image:: https://travis-ci.org/ovh/python-logging-ldp.svg?branch=master
+   :target: https://travis-ci.org/ovh/python-logging-ldp
+   :alt: Latest version
+
+
+.. image:: https://readthedocs.org/projects/logging-ldp/badge/?version=latest
+   :target: http://logging-ldp.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+
+A python logging bundle to send logs using GELF on the OVH Logs Data Platform.
+
+Quickstart
+==========
+
+First, install logging-ldp using `pip <https://pip.pypa.io/en/stable/>`_::
+
+    pip install -U logging-ldp
+
+The following example shows how to send log in Graylog TCP input
+
+.. code-block:: python
+
+    import logging
+    from logging_ldp.formatters import LDPGELFFormatter
+    from logging_ldp.handlers import LDPGELFTCPSocketHandler
+
+    logger = logging.getLogger("ldp")
+    logger.setLevel(logging.DEBUG)
+
+    handler = LDPGELFTCPSocketHandler(hostname="gra1.logs.ovh.com")
+    handler.setFormatter(LDPGELFFormatter(token="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"))
+    logger.addHandler(handler)
+    logger.debug("hello !")
+
+
+Requirements
+============
+
+- Python >= 3.3
+
+Project Links
+=============
+
+- Docs: http://logging-ldp.readthedocs.io/
+- PyPI: https://pypi.python.org/pypi/logging-ldp
+- Issues: https://github.com/ovh/python-logging-ldp/issues
+- OVH Logs Data Platform
+    - Homepage (FR): https://logs.ovh.com
+    - Documentation: https://docs.ovh.com/fr/logs-data-platform/
+- Graylog & GELF
+    - Documentation: http://docs.graylog.org/en/latest/pages/gelf.html
+    - Python logging-gelf: http://logging-gelf.readthedocs.io/
+
+License
+=======
+
+Licensed under `BSD 3-Clause License <./LICENSE>`_ or https://opensource.org/licenses/BSD-3-Clause.
```

### Comparing `logging-ldp-0.0.6/CONTRIBUTING.md` & `logging-ldp-0.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `logging-ldp-0.0.6/src/logging_ldp.egg-info/PKG-INFO` & `logging-ldp-0.0.7/src/logging_ldp.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,78 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: logging-ldp
-Version: 0.0.6
+Version: 0.0.7
 Summary: OVH library bundle to send logs on Log Data Platform (LDP)
 Home-page: https://github.com/ovh/python-logging-ldp
 Author: OVH SAS
 Author-email: github@ovh.net
 License: BSD
-Description: **********************************
-        Logging for OVH Logs Data Platform
-        **********************************
-        
-        .. image:: https://img.shields.io/pypi/v/logging-ldp.svg
-           :target: https://pypi.python.org/pypi/logging-ldp/
-           :alt: Latest Version
-        
-        .. image:: https://travis-ci.org/ovh/python-logging-ldp.svg?branch=master
-           :target: https://travis-ci.org/ovh/python-logging-ldp
-           :alt: Latest version
-        
-        
-        .. image:: https://readthedocs.org/projects/logging-ldp/badge/?version=latest
-           :target: http://logging-ldp.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Status
-        
-        
-        A python logging bundle to send logs using GELF on the OVH Logs Data Platform.
-        
-        Quickstart
-        ==========
-        
-        First, install logging-ldp using `pip <https://pip.pypa.io/en/stable/>`_::
-        
-            pip install -U logging-ldp
-        
-        The following example shows how to send log in Graylog TCP input
-        
-        .. code-block:: python
-        
-            import logging
-            from logging_ldp.formatters import LDPGELFFormatter
-            from logging_ldp.handlers import LDPGELFTCPSocketHandler
-        
-            logger = logging.getLogger("ldp")
-            logger.setLevel(logging.DEBUG)
-        
-            handler = LDPGELFTCPSocketHandler(hostname="gra1.logs.ovh.com")
-            handler.setFormatter(LDPGELFFormatter(token="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"))
-            logger.addHandler(handler)
-            logger.debug("hello !")
-        
-        
-        Requirements
-        ============
-        
-        - Python >= 3.3
-        
-        Project Links
-        =============
-        
-        - Docs: http://logging-ldp.readthedocs.io/
-        - PyPI: https://pypi.python.org/pypi/logging-ldp
-        - Issues: https://github.com/ovh/python-logging-ldp/issues
-        - OVH Logs Data Platform
-            - Homepage (FR): https://logs.ovh.com
-            - Documentation: https://docs.ovh.com/fr/logs-data-platform/
-        - Graylog & GELF
-            - Documentation: http://docs.graylog.org/en/latest/pages/gelf.html
-            - Python logging-gelf: http://logging-gelf.readthedocs.io/
-        
-        License
-        =======
-        
-        Licensed under `BSD 3-Clause License <./LICENSE>`_ or https://opensource.org/licenses/BSD-3-Clause.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
+License-File: LICENSE
+License-File: AUTHORS
+
+**********************************
+Logging for OVH Logs Data Platform
+**********************************
+
+.. image:: https://img.shields.io/pypi/v/logging-ldp.svg
+   :target: https://pypi.python.org/pypi/logging-ldp/
+   :alt: Latest Version
+
+.. image:: https://travis-ci.org/ovh/python-logging-ldp.svg?branch=master
+   :target: https://travis-ci.org/ovh/python-logging-ldp
+   :alt: Latest version
+
+
+.. image:: https://readthedocs.org/projects/logging-ldp/badge/?version=latest
+   :target: http://logging-ldp.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+
+A python logging bundle to send logs using GELF on the OVH Logs Data Platform.
+
+Quickstart
+==========
+
+First, install logging-ldp using `pip <https://pip.pypa.io/en/stable/>`_::
+
+    pip install -U logging-ldp
+
+The following example shows how to send log in Graylog TCP input
+
+.. code-block:: python
+
+    import logging
+    from logging_ldp.formatters import LDPGELFFormatter
+    from logging_ldp.handlers import LDPGELFTCPSocketHandler
+
+    logger = logging.getLogger("ldp")
+    logger.setLevel(logging.DEBUG)
+
+    handler = LDPGELFTCPSocketHandler(hostname="gra1.logs.ovh.com")
+    handler.setFormatter(LDPGELFFormatter(token="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"))
+    logger.addHandler(handler)
+    logger.debug("hello !")
+
+
+Requirements
+============
+
+- Python >= 3.3
+
+Project Links
+=============
+
+- Docs: http://logging-ldp.readthedocs.io/
+- PyPI: https://pypi.python.org/pypi/logging-ldp
+- Issues: https://github.com/ovh/python-logging-ldp/issues
+- OVH Logs Data Platform
+    - Homepage (FR): https://logs.ovh.com
+    - Documentation: https://docs.ovh.com/fr/logs-data-platform/
+- Graylog & GELF
+    - Documentation: http://docs.graylog.org/en/latest/pages/gelf.html
+    - Python logging-gelf: http://logging-gelf.readthedocs.io/
+
+License
+=======
+
+Licensed under `BSD 3-Clause License <./LICENSE>`_ or https://opensource.org/licenses/BSD-3-Clause.
```

### Comparing `logging-ldp-0.0.6/src/logging_ldp/formatters.py` & `logging-ldp-0.0.7/src/logging_ldp/formatters.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,19 @@
     def __init__(self, token, schema=LDPSchema, null_character=True,
                  JSONEncoder=json.JSONEncoder, exclude_patterns=None):
         GELFFormatter.__init__(
             self, schema, null_character, JSONEncoder, exclude_patterns
         )
         self.token = token
 
-    def format(self, record):
-        """Format the specified record into json using the schema which MUST
-        inherit from :class:`logging_ldp.schemas.LDPSchema`.
+    def serialize_record(self, record):
+        """Serialize logging record into a dict
 
+        :param record:
         :param logging.LogRecord record: Contains all the information pertinent
         to the event being logged.
-        :return: A JSON dump of the record.
-        :rtype: str
+        :return: A dict dump of the record.
+        :rtype: dict
         """
-        data = self.filter_keys(self.schema().dump(record))
+        data = GELFFormatter.serialize_record(self, record)
         data['_X-OVH-TOKEN'] = self.token
-        out = json.dumps(data, cls=self._encoder_cls)
-        if self.null_character is True:
-            out += '\0'
-        return out
+        return data
```

### Comparing `logging-ldp-0.0.6/src/logging_ldp/handlers.py` & `logging-ldp-0.0.7/src/logging_ldp/handlers.py`

 * *Files identical despite different names*

### Comparing `logging-ldp-0.0.6/src/logging_ldp/schemas.py` & `logging-ldp-0.0.7/src/logging_ldp/schemas.py`

 * *Files identical despite different names*

