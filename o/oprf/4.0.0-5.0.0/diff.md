# Comparing `tmp/oprf-4.0.0.tar.gz` & `tmp/oprf-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oprf-4.0.0.tar", last modified: Sat Sep 24 23:17:36 2022, max compression
+gzip compressed data, was "oprf-5.0.0.tar", last modified: Sun Jun 11 22:21:18 2023, max compression
```

## Comparing `oprf-4.0.0.tar` & `oprf-5.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-09-24 23:17:36.672899 oprf-4.0.0/
--rw-rw-rw-   0        0        0     1093 2022-04-13 22:16:12.000000 oprf-4.0.0/LICENSE
--rw-rw-rw-   0        0        0     6971 2022-09-24 23:17:36.672899 oprf-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6401 2022-09-24 23:11:09.000000 oprf-4.0.0/README.rst
--rw-rw-rw-   0        0        0     1054 2022-09-24 22:55:50.000000 oprf-4.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-24 23:17:36.672899 oprf-4.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-24 23:17:36.646899 oprf-4.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-09-24 23:17:36.653899 oprf-4.0.0/src/oprf/
--rw-rw-rw-   0        0        0       79 2022-04-13 22:16:12.000000 oprf-4.0.0/src/oprf/__init__.py
--rw-rw-rw-   0        0        0     7629 2022-09-24 23:04:37.000000 oprf-4.0.0/src/oprf/oprf.py
-drwxrwxrwx   0        0        0        0 2022-09-24 23:17:36.672899 oprf-4.0.0/src/oprf.egg-info/
--rw-rw-rw-   0        0        0     6971 2022-09-24 23:17:36.000000 oprf-4.0.0/src/oprf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2022-09-24 23:17:36.000000 oprf-4.0.0/src/oprf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-24 23:17:36.000000 oprf-4.0.0/src/oprf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2022-09-24 23:17:36.000000 oprf-4.0.0/src/oprf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-09-24 23:17:36.000000 oprf-4.0.0/src/oprf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 22:21:18.256600 oprf-5.0.0/
+-rw-rw-rw-   0        0        0     1093 2022-10-06 21:12:53.000000 oprf-5.0.0/LICENSE
+-rw-rw-rw-   0        0        0     8427 2023-06-11 22:21:18.255601 oprf-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7857 2023-06-11 18:39:54.000000 oprf-5.0.0/README.rst
+-rw-rw-rw-   0        0        0     1053 2023-06-11 18:08:31.000000 oprf-5.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 22:21:18.256600 oprf-5.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 22:21:18.243732 oprf-5.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 22:21:18.246306 oprf-5.0.0/src/oprf/
+-rw-rw-rw-   0        0        0       79 2022-10-06 21:12:53.000000 oprf-5.0.0/src/oprf/__init__.py
+-rw-rw-rw-   0        0        0     7629 2023-06-11 16:13:01.000000 oprf-5.0.0/src/oprf/oprf.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:21:18.255601 oprf-5.0.0/src/oprf.egg-info/
+-rw-rw-rw-   0        0        0     8427 2023-06-11 22:21:18.000000 oprf-5.0.0/src/oprf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-11 22:21:18.000000 oprf-5.0.0/src/oprf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 22:21:18.000000 oprf-5.0.0/src/oprf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      203 2023-06-11 22:21:18.000000 oprf-5.0.0/src/oprf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-11 22:21:18.000000 oprf-5.0.0/src/oprf.egg-info/top_level.txt
```

### Comparing `oprf-4.0.0/LICENSE` & `oprf-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oprf-4.0.0/PKG-INFO` & `oprf-5.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: oprf
-Version: 4.0.0
-Summary: Oblivious pseudo-random function (OPRF) protocol functionality implementations based on Curve25519 and the Ristretto group.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/nthparty/oprf
-Project-URL: Documentation, https://oprf.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
 ====
 oprf
 ====
 
 Oblivious pseudo-random function (OPRF) protocol functionality implementations based on `Curve25519 <https://cr.yp.to/ecdh.html>`__ and the `Ristretto <https://ristretto.group>`__ group.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -38,125 +20,166 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/nthparty/oprf/badge.svg?branch=main
    :target: https://coveralls.io/github/nthparty/oprf?branch=main
    :alt: Coveralls test coverage summary.
 
 Purpose
 -------
-This library provides data structures and methods for a basic `oblivious pseudo-random function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__ protocol. Thanks to the underlying `oblivious <https://pypi.org/project/oblivious>`__ library, method implementations rely on cryptographic primitives found within the `libsodium <https://github.com/jedisct1/libsodium>`__ library.
+This library provides data structures and methods for a basic `oblivious pseudo-random function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__ protocol. Method implementations rely on cryptographic primitives involving the `Ristretto <https://ristretto.group>`__ group that are exported by the `oblivious <https://pypi.org/project/oblivious>`__ library. By default, these are wrappers for functions found in the subset of the `libsodium <https://github.com/jedisct1/libsodium>`__ library that is bundled with the `rbcl <https://pypi.org/project/rbcl>`__ library.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/oprf>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/oprf>`__:
+
+.. code-block:: bash
 
     python -m pip install oprf
 
-The library can be imported in the usual ways::
+By default, this library indirectly relies on `rbcl <https://pypi.org/project/rbcl>`__ (which bundles a subset of the `libsodium <https://github.com/jedisct1/libsodium>`__ library that is compiled for common architectures). However, it is possible to install a fully working pure-Python version of this library by installing only the pure-Python subset of the `oblivious <https://pypi.org/project/oblivious>`__ dependency (*i.e.*, within an environment where `rbcl <https://pypi.org/project/rbcl>`__ is not a required dependency of other installed packages). This approach makes it possible to use this library for rapid prototyping on exotic architectures (with the caveat that pure-Python implementations of primitives are much slower):
+
+.. code-block:: bash
+
+    python -m pip install oblivious~=7.0
+    python -m pip install oprf --no-dependencies
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import oprf
     from oprf import *
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely prepare binary or string data for masking::
+This library makes it possible to concisely prepare binary or string data for masking:
+
+.. code-block:: python
 
     >>> from oprf import data, mask
     >>> d = data.hash('abc')
 
-A random mask can be constructed and applied to the data. A number of distinct notations is supported for masking in order to minimize differences between the notation within a protocol definition and its implementation::
+A random mask can be constructed and applied to the data. A number of distinct notations is supported for masking in order to minimize differences between the notation within a protocol definition and its implementation:
+
+.. code-block:: python
 
     >>> m = mask() # Create random mask.
     >>> m.mask(d) == m(d) == m * d
     True
     >>> m(d) == d
     False
 
-Mask inversion and unmasking are also supported::
+Mask inversion and unmasking are also supported:
+
+.. code-block:: python
 
     >>> c = m(d)
     >>> m.unmask(c) == (~m)(c) == c / m == d
     True
 
-Masks can also be constructed deterministically from a bytes-like object or string::
+Masks can also be constructed deterministically from a bytes-like object or string:
+
+.. code-block:: python
 
     >>> m = mask.hash('123')
 
 .. |data| replace:: ``data``
-.. _data: https://oprf.readthedocs.io/en/4.0.0/_source/oprf.html#oprf.oprf.data
+.. _data: https://oprf.readthedocs.io/en/5.0.0/_source/oprf.html#oprf.oprf.data
 
 .. |mask| replace:: ``mask``
-.. _mask: https://oprf.readthedocs.io/en/4.0.0/_source/oprf.html#oprf.oprf.mask
+.. _mask: https://oprf.readthedocs.io/en/5.0.0/_source/oprf.html#oprf.oprf.mask
 
 .. |bytes| replace:: ``bytes``
 .. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
 
-Because the classes |data|_ and |mask|_ are derived from |bytes|_, `all methods and other operators <https://docs.python.org/3/library/stdtypes.html#bytes>`__ supported by |bytes|_ objects are supported by |data|_ and |mask|_ objects::
+Because the classes |data|_ and |mask|_ are derived from |bytes|_, `all methods and other operators <https://docs.python.org/3/library/stdtypes.html#bytes>`__ supported by |bytes|_ objects are supported by |data|_ and |mask|_ objects:
+
+.. code-block:: python
 
     >>> hex = 'a665a45920422f9d417e4867efdc4fb8a04a1f3fff1fa07e998e86f7f7a27a03'
     >>> m = mask.fromhex(hex)
     >>> m.hex()
     'a665a45920422f9d417e4867efdc4fb8a04a1f3fff1fa07e998e86f7f7a27a03'
 
-In addition, Base64 conversion methods are included to support concise encoding and decoding of |data|_ and |mask|_ objects::
+In addition, Base64 conversion methods are included to support concise encoding and decoding of |data|_ and |mask|_ objects:
+
+.. code-block:: python
 
     >>> d.from_base64(d.to_base64()) == d
     True
     >>> m.from_base64(m.to_base64()) == m
     True
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
-    sphinx-apidoc -f -e -E --templatedir=_templates -o _source .. && make html
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/oprf/oprf.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/oprf
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/oprf>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/oprf>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/oprf>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `oprf-4.0.0/pyproject.toml` & `oprf-5.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 [project]
 name = "oprf"
-version = "4.0.0"
+version = "5.0.0"
 description = """\
     Oblivious pseudo-random function (OPRF) protocol \
     functionality implementations based on Curve25519 \
     and the Ristretto group.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
-    "oblivious[rbcl]~=6.0"
+    "oblivious[rbcl]~=7.0"
 ]
 
-
 [project.urls]
 Repository = "https://github.com/nthparty/oprf"
 Documentation = "https://oprf.readthedocs.io"
 
 [project.optional-dependencies]
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0"
 ]
 test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
 ]
 lint = [
-    "pylint~=2.14.0"
+    "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
 publish = [
-    "build~=0.8",
+    "build~=0.10",
     "twine~=4.0"
 ]
 
 [build-system]
 requires = [
-    "setuptools~=62.0"
+    "setuptools~=67.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=docs --cov=oprf --cov-report term-missing"
```

### Comparing `oprf-4.0.0/src/oprf/oprf.py` & `oprf-5.0.0/src/oprf/oprf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Oblivious pseudo-random function (OPRF) protocol functionality implementations
 based on `Curve25519 <https://cr.yp.to/ecdh.html>`__ and the
 `Ristretto <https://ristretto.group>`__ group.
 """
 from __future__ import annotations
-from typing import Optional, Union
+from typing import Union, Optional
 import doctest
 import oblivious
 
 class data(oblivious.ristretto.point):
     """
     Wrapper class for a bytes-like object that corresponds to a piece of data
     that can be masked.
```

### Comparing `oprf-4.0.0/src/oprf.egg-info/PKG-INFO` & `oprf-5.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oprf
-Version: 4.0.0
+Version: 5.0.0
 Summary: Oblivious pseudo-random function (OPRF) protocol functionality implementations based on Curve25519 and the Ristretto group.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/oprf
 Project-URL: Documentation, https://oprf.readthedocs.io
 Requires-Python: >=3.7
@@ -38,125 +38,166 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/nthparty/oprf/badge.svg?branch=main
    :target: https://coveralls.io/github/nthparty/oprf?branch=main
    :alt: Coveralls test coverage summary.
 
 Purpose
 -------
-This library provides data structures and methods for a basic `oblivious pseudo-random function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__ protocol. Thanks to the underlying `oblivious <https://pypi.org/project/oblivious>`__ library, method implementations rely on cryptographic primitives found within the `libsodium <https://github.com/jedisct1/libsodium>`__ library.
+This library provides data structures and methods for a basic `oblivious pseudo-random function (OPRF) <https://en.wikipedia.org/wiki/Pseudorandom_function_family>`__ protocol. Method implementations rely on cryptographic primitives involving the `Ristretto <https://ristretto.group>`__ group that are exported by the `oblivious <https://pypi.org/project/oblivious>`__ library. By default, these are wrappers for functions found in the subset of the `libsodium <https://github.com/jedisct1/libsodium>`__ library that is bundled with the `rbcl <https://pypi.org/project/rbcl>`__ library.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/oprf>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/oprf>`__:
+
+.. code-block:: bash
 
     python -m pip install oprf
 
-The library can be imported in the usual ways::
+By default, this library indirectly relies on `rbcl <https://pypi.org/project/rbcl>`__ (which bundles a subset of the `libsodium <https://github.com/jedisct1/libsodium>`__ library that is compiled for common architectures). However, it is possible to install a fully working pure-Python version of this library by installing only the pure-Python subset of the `oblivious <https://pypi.org/project/oblivious>`__ dependency (*i.e.*, within an environment where `rbcl <https://pypi.org/project/rbcl>`__ is not a required dependency of other installed packages). This approach makes it possible to use this library for rapid prototyping on exotic architectures (with the caveat that pure-Python implementations of primitives are much slower):
+
+.. code-block:: bash
+
+    python -m pip install oblivious~=7.0
+    python -m pip install oprf --no-dependencies
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import oprf
     from oprf import *
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely prepare binary or string data for masking::
+This library makes it possible to concisely prepare binary or string data for masking:
+
+.. code-block:: python
 
     >>> from oprf import data, mask
     >>> d = data.hash('abc')
 
-A random mask can be constructed and applied to the data. A number of distinct notations is supported for masking in order to minimize differences between the notation within a protocol definition and its implementation::
+A random mask can be constructed and applied to the data. A number of distinct notations is supported for masking in order to minimize differences between the notation within a protocol definition and its implementation:
+
+.. code-block:: python
 
     >>> m = mask() # Create random mask.
     >>> m.mask(d) == m(d) == m * d
     True
     >>> m(d) == d
     False
 
-Mask inversion and unmasking are also supported::
+Mask inversion and unmasking are also supported:
+
+.. code-block:: python
 
     >>> c = m(d)
     >>> m.unmask(c) == (~m)(c) == c / m == d
     True
 
-Masks can also be constructed deterministically from a bytes-like object or string::
+Masks can also be constructed deterministically from a bytes-like object or string:
+
+.. code-block:: python
 
     >>> m = mask.hash('123')
 
 .. |data| replace:: ``data``
-.. _data: https://oprf.readthedocs.io/en/4.0.0/_source/oprf.html#oprf.oprf.data
+.. _data: https://oprf.readthedocs.io/en/5.0.0/_source/oprf.html#oprf.oprf.data
 
 .. |mask| replace:: ``mask``
-.. _mask: https://oprf.readthedocs.io/en/4.0.0/_source/oprf.html#oprf.oprf.mask
+.. _mask: https://oprf.readthedocs.io/en/5.0.0/_source/oprf.html#oprf.oprf.mask
 
 .. |bytes| replace:: ``bytes``
 .. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
 
-Because the classes |data|_ and |mask|_ are derived from |bytes|_, `all methods and other operators <https://docs.python.org/3/library/stdtypes.html#bytes>`__ supported by |bytes|_ objects are supported by |data|_ and |mask|_ objects::
+Because the classes |data|_ and |mask|_ are derived from |bytes|_, `all methods and other operators <https://docs.python.org/3/library/stdtypes.html#bytes>`__ supported by |bytes|_ objects are supported by |data|_ and |mask|_ objects:
+
+.. code-block:: python
 
     >>> hex = 'a665a45920422f9d417e4867efdc4fb8a04a1f3fff1fa07e998e86f7f7a27a03'
     >>> m = mask.fromhex(hex)
     >>> m.hex()
     'a665a45920422f9d417e4867efdc4fb8a04a1f3fff1fa07e998e86f7f7a27a03'
 
-In addition, Base64 conversion methods are included to support concise encoding and decoding of |data|_ and |mask|_ objects::
+In addition, Base64 conversion methods are included to support concise encoding and decoding of |data|_ and |mask|_ objects:
+
+.. code-block:: python
 
     >>> d.from_base64(d.to_base64()) == d
     True
     >>> m.from_base64(m.to_base64()) == m
     True
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
-    sphinx-apidoc -f -e -E --templatedir=_templates -o _source .. && make html
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/oprf/oprf.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/oprf
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/oprf>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/oprf>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/oprf>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

