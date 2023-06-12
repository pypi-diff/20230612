# Comparing `tmp/pytest-dynamodb-2.2.2.tar.gz` & `tmp/pytest-dynamodb-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-dynamodb-2.2.2.tar", last modified: Mon Mar 27 10:24:19 2023, max compression
+gzip compressed data, was "pytest-dynamodb-2.2.3.tar", last modified: Mon Jun 12 13:39:04 2023, max compression
```

## Comparing `pytest-dynamodb-2.2.2.tar` & `pytest-dynamodb-2.2.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:24:19.871533 pytest-dynamodb-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)    14770 2023-03-27 10:24:19.871533 pytest-dynamodb-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:24:19.871533 pytest-dynamodb-2.2.2/pytest_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/pytest_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/pytest_dynamodb/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/pytest_dynamodb/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/pytest_dynamodb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:24:19.871533 pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14770 2023-03-27 10:24:19.000000 pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-27 10:24:19.000000 pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:24:19.000000 pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-27 10:24:19.000000 pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-27 10:24:19.000000 pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 10:24:19.000000 pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:24:19.000000 pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-27 10:24:19.871533 pytest-dynamodb-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:24:19.871533 pytest-dynamodb-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-27 10:24:10.000000 pytest-dynamodb-2.2.2/tests/test_dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:39:04.503220 pytest-dynamodb-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-06-12 13:39:04.499220 pytest-dynamodb-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:39:04.499220 pytest-dynamodb-2.2.3/pytest_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/pytest_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/pytest_dynamodb/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/pytest_dynamodb/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/pytest_dynamodb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:39:04.499220 pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-06-12 13:39:04.000000 pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-12 13:39:04.000000 pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:39:04.000000 pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 13:39:04.000000 pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 13:39:04.000000 pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 13:39:04.000000 pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:39:04.000000 pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:39:04.503220 pytest-dynamodb-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:39:04.499220 pytest-dynamodb-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-12 13:38:51.000000 pytest-dynamodb-2.2.3/tests/test_dynamodb.py
```

### Comparing `pytest-dynamodb-2.2.2/COPYING.lesser` & `pytest-dynamodb-2.2.3/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-dynamodb-2.2.2/PKG-INFO` & `pytest-dynamodb-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dynamodb
-Version: 2.2.2
+Version: 2.2.3
 Summary: DynamoDB fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-dynamodb
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-dynamodb/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-dynamodb/blob/v2.2.2/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-dynamodb/blob/v2.2.3/CHANGES.rst
 Keywords: tests,pytest,fixture,dynamodb,aws,boto
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -186,14 +186,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: COPYING
+License-File: COPYING.lesser
 License-File: AUTHORS.rst
 
 .. image:: https://raw.githubusercontent.com/ClearcodeHQ/pytest-dynamodb/master/logo.png
     :width: 100px
     :height: 100px
     
 pytest-dynamodb
@@ -214,20 +216,20 @@
 .. image:: https://img.shields.io/pypi/l/pytest-dynamodb.svg
     :target: https://pypi.python.org/pypi/pytest-dynamodb/
     :alt: License
 
 Package status
 --------------
 
-.. image:: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb.svg?branch=v2.2.2
+.. image:: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb.svg?branch=v2.2.3
     :target: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb
     :alt: Tests
 
-.. image:: https://coveralls.io/repos/ClearcodeHQ/pytest-dynamodb/badge.png?branch=v2.2.2
-    :target: https://coveralls.io/r/ClearcodeHQ/pytest-dynamodb?branch=v2.2.2
+.. image:: https://coveralls.io/repos/ClearcodeHQ/pytest-dynamodb/badge.png?branch=v2.2.3
+    :target: https://coveralls.io/r/ClearcodeHQ/pytest-dynamodb?branch=v2.2.3
     :alt: Coverage Status
 
 What is this?
 =============
 
 This is a pytest plugin, that enables you to test your code that relies on a running DynamoDB Database.
 It allows you to specify fixtures for DynamoDB process and client (resource in AWS boto terms).
@@ -296,20 +298,20 @@
      - --dynamodb-port
      - dynamodb_port
      - random
    * - AWS Access Key
      - access_key
      - --dynamodb-aws_access_key
      - dynamodb_aws_access_key
-     - access_key
+     - fakeMyKeyId
    * - AWS Secret Key
      - secret_key
      - --dynamodb-aws_secret_key
      - dynamodb_aws_secret_key
-     - secret_key
+     - fakeSecretAccessKey
    * - AWS Region
      - region
      - --dynamodb-aws_region
      - dynamodb_aws_region
      - us-west-1
    * - `Introduce delays <https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.UsageNotes.html#:~:text=%2DdelayTransientStatuses>`_
      - delay
```

### Comparing `pytest-dynamodb-2.2.2/README.rst` & `pytest-dynamodb-2.2.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 .. image:: https://img.shields.io/pypi/l/pytest-dynamodb.svg
     :target: https://pypi.python.org/pypi/pytest-dynamodb/
     :alt: License
 
 Package status
 --------------
 
-.. image:: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb.svg?branch=v2.2.2
+.. image:: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb.svg?branch=v2.2.3
     :target: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb
     :alt: Tests
 
-.. image:: https://coveralls.io/repos/ClearcodeHQ/pytest-dynamodb/badge.png?branch=v2.2.2
-    :target: https://coveralls.io/r/ClearcodeHQ/pytest-dynamodb?branch=v2.2.2
+.. image:: https://coveralls.io/repos/ClearcodeHQ/pytest-dynamodb/badge.png?branch=v2.2.3
+    :target: https://coveralls.io/r/ClearcodeHQ/pytest-dynamodb?branch=v2.2.3
     :alt: Coverage Status
 
 What is this?
 =============
 
 This is a pytest plugin, that enables you to test your code that relies on a running DynamoDB Database.
 It allows you to specify fixtures for DynamoDB process and client (resource in AWS boto terms).
@@ -102,20 +102,20 @@
      - --dynamodb-port
      - dynamodb_port
      - random
    * - AWS Access Key
      - access_key
      - --dynamodb-aws_access_key
      - dynamodb_aws_access_key
-     - access_key
+     - fakeMyKeyId
    * - AWS Secret Key
      - secret_key
      - --dynamodb-aws_secret_key
      - dynamodb_aws_secret_key
-     - secret_key
+     - fakeSecretAccessKey
    * - AWS Region
      - region
      - --dynamodb-aws_region
      - dynamodb_aws_region
      - us-west-1
    * - `Introduce delays <https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.UsageNotes.html#:~:text=%2DdelayTransientStatuses>`_
      - delay
```

### Comparing `pytest-dynamodb-2.2.2/pyproject.toml` & `pytest-dynamodb-2.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-dynamodb"
-version = "2.2.2"
+version = "2.2.3"
 description = "DynamoDB fixtures for pytest"
 readme = "README.rst"
 keywords = ["tests", "pytest", "fixture", "dynamodb", "aws", "boto"]
 license = {file = "COPYING.lesser"}
 authors = [
     {name = "Grzegorz Śliwiński", email = "fizyk+pypi@fizyk.dev"}
 ]
@@ -34,15 +34,15 @@
     "boto3-stubs[dynamodb]",
 ]
 requires-python = ">= 3.8"
 
 [project.urls]
 "Source" = "https://github.com/ClearcodeHQ/pytest-dynamodb"
 "Bug Tracker" = "https://github.com/ClearcodeHQ/pytest-dynamodb/issues"
-"Changelog" = "https://github.com/ClearcodeHQ/pytest-dynamodb/blob/v2.2.2/CHANGES.rst"
+"Changelog" = "https://github.com/ClearcodeHQ/pytest-dynamodb/blob/v2.2.3/CHANGES.rst"
 
 [project.entry-points."pytest11"]
 pytest_dynamodb = "pytest_dynamodb.plugin"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -60,14 +60,24 @@
 testpaths = "tests"
 
 [tool.black]
 line-length = 80
 target-version = ['py38']
 include = '.*\.pyi?$'
 
+[tool.ruff]
+# Decrease the maximum line length to 79 characters.
+line-length = 100
+select = [
+    "E",   # pycodestyle
+    "F",   # pyflakes
+    "I",   # isort
+    "D",   # pydocstyle
+]
+
 [tool.towncrier]
 directory = "newsfragments"
 single_file=true
 filename="CHANGES.rst"
 issue_format="`#{issue} <https://https://github.com/ClearcodeHQ/pytest-dynamodb/issues/{issue}>`_"
 
 [tool.towncrier.fragment.feature]
@@ -82,23 +92,20 @@
 name = "Breaking changes"
 showcontent = true
 
 [tool.towncrier.fragment.misc]
 name = "Miscellaneus"
 showcontent = true
 
-[tool.pydocstyle]
-ignore = "D203,D212"
-
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/ClearcodeHQ/pytest-dynamodb/"
 
 [tool.tbump.version]
-current = "2.2.2"
+current = "2.2.3"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pytest-dynamodb-2.2.2/pytest_dynamodb/__init__.py` & `pytest-dynamodb-2.2.3/pytest_dynamodb/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-dynamodb. If not, see <http://www.gnu.org/licenses/>.
 """Main module for pytest-dynamodb."""
-__version__ = "2.2.2"
+__version__ = "2.2.3"
```

### Comparing `pytest-dynamodb-2.2.2/pytest_dynamodb/factories.py` & `pytest-dynamodb-2.2.3/pytest_dynamodb/factories.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-dynamodb. If not, see <http://www.gnu.org/licenses/>.
 """Module containing factories for pytest-dynamodb."""
 import os
 from pathlib import Path
-from typing import TypedDict, Optional, Any, Callable, Generator
+from typing import Any, Callable, Generator, Optional, TypedDict
 
-import pytest
 import boto3
+import pytest
+from mirakuru import ProcessExitedWithError, TCPExecutor
 from mypy_boto3_dynamodb import DynamoDBServiceResource
-from pytest import FixtureRequest
-from mirakuru import TCPExecutor, ProcessExitedWithError
 from port_for import get_port
+from pytest import FixtureRequest
 
 
 class PytestDynamoDBConfigType(TypedDict):
     """Configuration type dict."""
 
     dir: Path
     host: str
@@ -37,16 +37,15 @@
     delay: str
     aws_access_key: str
     aws_secret_key: str
     aws_region: str
 
 
 class JarPathException(Exception):
-    """
-    Exception thrown, i ncase we can't locate dynamodb's dir to run dynamodb.
+    """Exception thrown, i ncase we can't locate dynamodb's dir to run dynamodb.
 
     We do not know where user has dynamodb jar file.
     So, we want to tell him that he has to provide a path to dynamodb dir.
     """
 
 
 def get_config(request: FixtureRequest) -> PytestDynamoDBConfigType:
@@ -72,16 +71,15 @@
 
 def dynamodb_proc(
     dynamodb_dir: Optional[str] = None,
     host: str = "localhost",
     port: Optional[int] = None,
     delay: bool = False,
 ) -> Callable[[FixtureRequest], Any]:
-    """
-    Process fixture factory for DynamoDB.
+    """Process fixture factory for DynamoDB.
 
     :param str dynamodb_dir: a path to dynamodb dir (without spaces)
     :param str host: hostname
     :param int port: port
     :param bool delay: causes DynamoDB to introduce delays for certain
         operations
 
@@ -92,16 +90,15 @@
     :return: function which makes a DynamoDB process
     """
 
     @pytest.fixture(scope="session")
     def dynamodb_proc_fixture(
         request: FixtureRequest,
     ) -> Generator[TCPExecutor, None, None]:
-        """
-        Process fixture for DynamoDB.
+        """Process fixture for DynamoDB.
 
         It starts DynamoDB when first used and stops it at the end
         of the tests. Works on ``DynamoDBLocal.jar``.
 
         :param FixtureRequest request: fixture request object
         :rtype: pytest_dbfixtures.executors.TCPExecutor
         :returns: tcp executor
@@ -143,31 +140,29 @@
 
 def dynamodb(
     process_fixture_name: str,
     access_key: Optional[str] = None,
     secret_key: Optional[str] = None,
     region: Optional[str] = None,
 ) -> Callable[[FixtureRequest], Any]:
-    """
-    Fixture factory for DynamoDB resource.
+    """Fixture factory for DynamoDB resource.
 
     :param str process_fixture_name: name of the process fixture
     :param str access_key: AWS acccess key
     :param str secret_key: AWS secret key
     :param str region: AWS region name
     :rtype: func
     :returns: function which makes a connection to DynamoDB
     """
 
     @pytest.fixture
     def dynamodb_factory(
         request: FixtureRequest,
     ) -> Generator[DynamoDBServiceResource, None, None]:
-        """
-        Fixture for DynamoDB resource.
+        """Fixture for DynamoDB resource.
 
         :param FixtureRequest request: fixture request object
         :rtype: Subclass of :py:class:`~boto3.resources.base.ServiceResource`
             https://boto3.readthedocs.io/en/latest/reference/services/dynamodb.html#DynamoDB.Client
         :returns: connection to DynamoDB database
         """
         proc_fixture = request.getfixturevalue(process_fixture_name)
```

### Comparing `pytest-dynamodb-2.2.2/pytest_dynamodb/plugin.py` & `pytest-dynamodb-2.2.3/pytest_dynamodb/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-dynamodb.  If not, see <http://www.gnu.org/licenses/>.
 """Plugin module of pytest-dynamodb."""
 from pytest import Parser
 
 from pytest_dynamodb import factories
 
-
 # pylint:disable=invalid-name
 _help_dir = "Path to DynamoDB installation path"
 _help_host = "Host at which DynamoDB will accept connections"
 _help_port = "Port at which DynamoDB will accept connections"
 _help_delay = "causes DynamoDB to introduce delays for certain operations"
 _help_aws_secret_key = "AWS secret key."
 _help_aws_access_key = "AWS access key."
@@ -44,28 +43,28 @@
     )
 
     parser.addini(name="dynamodb_delay", help=_help_delay, default=False)
 
     parser.addini(
         name="dynamodb_aws_secret_key",
         help=_help_aws_secret_key,
-        default="secret_key",
+        default="fakeSecretAccessKey",
     )
 
     parser.addoption(
         "--dynamodb-aws_secret_key",
         action="store",
         dest="dynamodb_aws_secret_key",
         help=_help_aws_secret_key,
     )
 
     parser.addini(
         name="dynamodb_aws_access_key",
         help=_help_aws_access_key,
-        default="access_key",
+        default="fakeMyKeyId",
     )
 
     parser.addoption(
         "--dynamodb-aws_access_key",
         action="store",
         dest="dynamodb_aws_access_key",
         help=_help_aws_access_key,
```

### Comparing `pytest-dynamodb-2.2.2/pytest_dynamodb.egg-info/PKG-INFO` & `pytest-dynamodb-2.2.3/pytest_dynamodb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dynamodb
-Version: 2.2.2
+Version: 2.2.3
 Summary: DynamoDB fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-dynamodb
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-dynamodb/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-dynamodb/blob/v2.2.2/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-dynamodb/blob/v2.2.3/CHANGES.rst
 Keywords: tests,pytest,fixture,dynamodb,aws,boto
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -186,14 +186,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: COPYING
+License-File: COPYING.lesser
 License-File: AUTHORS.rst
 
 .. image:: https://raw.githubusercontent.com/ClearcodeHQ/pytest-dynamodb/master/logo.png
     :width: 100px
     :height: 100px
     
 pytest-dynamodb
@@ -214,20 +216,20 @@
 .. image:: https://img.shields.io/pypi/l/pytest-dynamodb.svg
     :target: https://pypi.python.org/pypi/pytest-dynamodb/
     :alt: License
 
 Package status
 --------------
 
-.. image:: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb.svg?branch=v2.2.2
+.. image:: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb.svg?branch=v2.2.3
     :target: https://travis-ci.org/ClearcodeHQ/pytest-dynamodb
     :alt: Tests
 
-.. image:: https://coveralls.io/repos/ClearcodeHQ/pytest-dynamodb/badge.png?branch=v2.2.2
-    :target: https://coveralls.io/r/ClearcodeHQ/pytest-dynamodb?branch=v2.2.2
+.. image:: https://coveralls.io/repos/ClearcodeHQ/pytest-dynamodb/badge.png?branch=v2.2.3
+    :target: https://coveralls.io/r/ClearcodeHQ/pytest-dynamodb?branch=v2.2.3
     :alt: Coverage Status
 
 What is this?
 =============
 
 This is a pytest plugin, that enables you to test your code that relies on a running DynamoDB Database.
 It allows you to specify fixtures for DynamoDB process and client (resource in AWS boto terms).
@@ -296,20 +298,20 @@
      - --dynamodb-port
      - dynamodb_port
      - random
    * - AWS Access Key
      - access_key
      - --dynamodb-aws_access_key
      - dynamodb_aws_access_key
-     - access_key
+     - fakeMyKeyId
    * - AWS Secret Key
      - secret_key
      - --dynamodb-aws_secret_key
      - dynamodb_aws_secret_key
-     - secret_key
+     - fakeSecretAccessKey
    * - AWS Region
      - region
      - --dynamodb-aws_region
      - dynamodb_aws_region
      - us-west-1
    * - `Introduce delays <https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.UsageNotes.html#:~:text=%2DdelayTransientStatuses>`_
      - delay
```

### Comparing `pytest-dynamodb-2.2.2/tests/test_dynamodb.py` & `pytest-dynamodb-2.2.3/tests/test_dynamodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 import pytest
 from botocore.exceptions import ClientError
 from mypy_boto3_dynamodb import DynamoDBServiceResource
 
 
 def test_dynamodb(dynamodb: DynamoDBServiceResource) -> None:
-    """
-    Simple test for DynamoDB.
+    """Simple test for DynamoDB.
 
     # Create a table
     # Put an item
     # Get the item and check the content of this item
     """
     # create a table
     table = dynamodb.create_table(
@@ -40,31 +39,29 @@
     )
 
     # check the content of the item
     assert item["Item"]["test_key"] == "test_value"
 
 
 def test_if_tables_does_not_exist(dynamodb: DynamoDBServiceResource) -> None:
-    """
-    We should clear this fixture (remove all tables).
+    """We should clear this fixture (remove all tables).
 
     .. note::
         `all` method on tables object creates an iterable of all
         Table resources in the collection.
     """
     assert not list(dynamodb.tables.all())
 
 
 def test_different_credentials(
     dynamodb_diff: DynamoDBServiceResource,
     dynamodb_same: DynamoDBServiceResource,
     dynamodb: DynamoDBServiceResource,
 ) -> None:
-    """
-    Check error when accessing table with different credentials.
+    """Check error when accessing table with different credentials.
 
     scan on dynamodb_diff should result in an error,
     while scans on dynamodb and dynamodb_same should pass.
     """
     dynamodb.create_table(
         AttributeDefinitions=[
             {"AttributeName": "string", "AttributeType": "S"},
```

