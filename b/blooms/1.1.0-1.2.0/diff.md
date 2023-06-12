# Comparing `tmp/blooms-1.1.0.tar.gz` & `tmp/blooms-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blooms-1.1.0.tar", last modified: Mon Aug  8 05:19:47 2022, max compression
+gzip compressed data, was "blooms-1.2.0.tar", last modified: Mon Jun 12 03:48:23 2023, max compression
```

## Comparing `blooms-1.1.0.tar` & `blooms-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-08-08 05:19:47.676010 blooms-1.1.0/
--rw-rw-rw-   0        0        0     1093 2022-03-17 07:44:36.000000 blooms-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    10445 2022-08-08 05:19:47.676183 blooms-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9911 2022-07-27 01:17:57.000000 blooms-1.1.0/README.rst
--rw-rw-rw-   0        0        0      937 2022-08-06 03:01:54.000000 blooms-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-08 05:19:47.676236 blooms-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-08 05:19:47.659044 blooms-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-08 05:19:47.664456 blooms-1.1.0/src/blooms/
--rw-rw-rw-   0        0        0       77 2022-06-23 05:46:23.000000 blooms-1.1.0/src/blooms/__init__.py
--rw-rw-rw-   0        0        0    14611 2022-08-06 02:56:33.000000 blooms-1.1.0/src/blooms/blooms.py
-drwxrwxrwx   0        0        0        0 2022-08-08 05:19:47.674939 blooms-1.1.0/src/blooms.egg-info/
--rw-rw-rw-   0        0        0    10445 2022-08-08 05:19:47.000000 blooms-1.1.0/src/blooms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2022-08-08 05:19:47.000000 blooms-1.1.0/src/blooms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-08 05:19:47.000000 blooms-1.1.0/src/blooms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2022-08-08 05:19:47.000000 blooms-1.1.0/src/blooms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-08 05:19:47.000000 blooms-1.1.0/src/blooms.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-08 05:19:47.675482 blooms-1.1.0/test/
--rw-rw-rw-   0        0        0     6168 2022-08-06 03:00:16.000000 blooms-1.1.0/test/test_blooms.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:48:23.996209 blooms-1.2.0/
+-rw-rw-rw-   0        0        0     1093 2022-03-17 07:44:36.000000 blooms-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10980 2023-06-12 03:48:23.996209 blooms-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10446 2023-06-12 03:41:57.000000 blooms-1.2.0/README.rst
+-rw-rw-rw-   0        0        0      938 2023-06-12 03:43:58.000000 blooms-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 03:48:23.996209 blooms-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 03:48:23.978338 blooms-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 03:48:23.983331 blooms-1.2.0/src/blooms/
+-rw-rw-rw-   0        0        0       77 2022-06-23 05:46:23.000000 blooms-1.2.0/src/blooms/__init__.py
+-rw-rw-rw-   0        0        0    14623 2023-06-12 03:36:01.000000 blooms-1.2.0/src/blooms/blooms.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:48:23.994209 blooms-1.2.0/src/blooms.egg-info/
+-rw-rw-rw-   0        0        0    10980 2023-06-12 03:48:23.000000 blooms-1.2.0/src/blooms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-12 03:48:23.000000 blooms-1.2.0/src/blooms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 03:48:23.000000 blooms-1.2.0/src/blooms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-06-12 03:48:23.000000 blooms-1.2.0/src/blooms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 03:48:23.000000 blooms-1.2.0/src/blooms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 03:48:23.995209 blooms-1.2.0/test/
+-rw-rw-rw-   0        0        0     6168 2022-08-06 03:00:16.000000 blooms-1.2.0/test/test_blooms.py
```

### Comparing `blooms-1.1.0/LICENSE` & `blooms-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blooms-1.1.0/PKG-INFO` & `blooms-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blooms
-Version: 1.1.0
+Version: 1.2.0
 Summary: Lightweight Bloom filter data structure derived from the built-in bytearray type.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/blooms
 Project-URL: Documentation, https://blooms.readthedocs.io
 Requires-Python: >=3.7
@@ -46,184 +46,228 @@
 .. |bytearray| replace:: ``bytearray``
 .. _bytearray: https://docs.python.org/3/library/stdtypes.html#bytearray
 
 This library provides a simple and lightweight data structure for representing `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__ that is derived from the built-in |bytearray|_ type. The data structure has methods for the insertion, membership, union, and subset operations. In addition, methods for estimating capacity and for converting to and from Base64 strings are available.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/blooms>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/blooms>`__:
+
+.. code-block:: bash
 
     python -m pip install blooms
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import blooms
     from blooms import blooms
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely create, populate, and query simple `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__. The example below constructs a Bloom filter that is 32 bits (*i.e.*, four bytes) in size::
+This library makes it possible to concisely create, populate, and query simple `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__. The example below constructs a Bloom filter that is 32 bits (*i.e.*, four bytes) in size:
+
+.. code-block:: python
 
     >>> from blooms import blooms
     >>> b = blooms(4)
 
 .. |insertion_operator| replace:: insertion operator ``@=``
-.. _insertion_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__imatmul__
+.. _insertion_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__imatmul__
 
-A bytes-like object can be inserted into an instance using the |insertion_operator|_. It is the responsibility of the user of the library to hash and truncate the bytes-like object being inserted. Only the bytes that remain after truncation contribute to the membership of the bytes-like object within the Bloom filter::
+A bytes-like object can be inserted into an instance using the |insertion_operator|_. It is the responsibility of the user of the library to hash and truncate the bytes-like object being inserted. Only the bytes that remain after truncation contribute to the membership of the bytes-like object within the Bloom filter:
+
+.. code-block:: python
 
     >>> from hashlib import sha256
     >>> x = 'abc' # Value to insert.
     >>> h = sha256(x.encode()).digest() # Hash of value.
     >>> t = h[:2] # Truncated hash.
     >>> b @= t # Insert the value into the Bloom filter.
     >>> b.hex()
     '00000004'
 
 .. |membership_operator| replace:: membership operator ``@``
-.. _membership_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__rmatmul__
+.. _membership_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__rmatmul__
+
+When testing whether a bytes-like object is a member using the |membership_operator|_ of an instance, the same hashing and truncation operations should be applied:
 
-When testing whether a bytes-like object is a member using the |membership_operator|_ of an instance, the same hashing and truncation operations should be applied::
+.. code-block:: python
 
     >>> sha256('abc'.encode()).digest()[:2] @ b
     True
     >>> sha256('xyz'.encode()).digest()[:2] @ b
     False
 
 
-The |insertion_operator|_ also accepts iterable containers::
+The |insertion_operator|_ also accepts iterable containers:
+
+.. code-block:: python
 
     >>> x = sha256('x'.encode()).digest()[:2]
     >>> y = sha256('y'.encode()).digest()[:2]
     >>> z = sha256('z'.encode()).digest()[:2]
     >>> b @= [x, y, z]
     >>> b.hex()
     '02200006'
 
 .. |union_operator| replace:: built-in ``|`` operator
-.. _union_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__or__
+.. _union_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__or__
 
-The union of two Bloom filters (both having the same size) can be computed via the |union_operator|_::
+The union of two Bloom filters (both having the same size) can be computed via the |union_operator|_:
+
+.. code-block:: python
 
     >>> c = blooms(4)
     >>> c @= sha256('xyz'.encode()).digest()[:2]
     >>> d = c | b
     >>> sha256('abc'.encode()).digest()[:2] @ d
     True
     >>> sha256('xyz'.encode()).digest()[:2] @ d
     True
 
-It is also possible to check whether the members of one Bloom filter `are a subset <https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.issubset>`__ of the members of another Bloom filter::
+It is also possible to check whether the members of one Bloom filter `are a subset <https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.issubset>`__ of the members of another Bloom filter:
+
+.. code-block:: python
 
     >>> b.issubset(c)
     False
     >>> b.issubset(d)
     True
 
 .. |saturation| replace:: ``saturation``
-.. _saturation: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.saturation
+.. _saturation: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.saturation
 
 .. |float| replace:: ``float``
 .. _float: https://docs.python.org/3/library/functions.html#float
 
-The |saturation|_ method calculates the saturation of a Bloom filter. The *saturation* is a |float|_ value (between ``0.0`` and ``1.0``) that represents an upper bound on the rate with which false positives will occur when testing bytes-like objects (of a specific length) for membership within the Bloom filter::
+The |saturation|_ method calculates the saturation of a Bloom filter. The *saturation* is a |float|_ value (between ``0.0`` and ``1.0``) that represents an upper bound on the rate with which false positives will occur when testing bytes-like objects (of a specific length) for membership within the Bloom filter:
+
+.. code-block:: python
 
     >>> b = blooms(32)
     >>> from secrets import token_bytes
     >>> for _ in range(8):
     ...     b @= token_bytes(4)
     >>> b.saturation(4)
     0.03125
 
 .. |capacity| replace:: ``capacity``
-.. _capacity: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.capacity
+.. _capacity: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.capacity
 
-It is also possible to determine the approximate maximum capacity of a Bloom filter for a given saturation limit using the |capacity|_ method. For example, the output below indicates that a saturation of ``0.05`` will likely be reached after more than ``28`` insertions of bytes-like objects of length ``8``::
+It is also possible to determine the approximate maximum capacity of a Bloom filter for a given saturation limit using the |capacity|_ method. For example, the output below indicates that a saturation of ``0.05`` will likely be reached after more than ``28`` insertions of bytes-like objects of length ``8``:
+
+.. code-block:: python
 
     >>> b = blooms(32)
     >>> b.capacity(8, 0.05)
     28
 
-In addition, conversion methods to and from Base64 strings are included to support concise encoding and decoding::
+In addition, conversion methods to and from Base64 strings are included to support concise encoding and decoding:
+
+.. code-block:: python
 
     >>> b.to_base64()
     'AiAABg=='
     >>> sha256('abc'.encode()).digest()[:2] @ blooms.from_base64('AiAABg==')
     True
 
 .. |specialize| replace:: ``specialize``
-.. _specialize: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.specialize
+.. _specialize: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.specialize
 
-If it is preferable to have a Bloom filter data structure that encapsulates a particular serialization, hashing, and truncation scheme, the recommended approach is to define a derived class. The |specialize|_ method makes it possible to do so in a concise way::
+If it is preferable to have a Bloom filter data structure that encapsulates a particular serialization, hashing, and truncation scheme, the recommended approach is to define a derived class. The |specialize|_ method makes it possible to do so in a concise way:
+
+.. code-block:: python
 
     >>> encode = lambda x: sha256(x).digest()[:2]
     >>> blooms_custom = blooms.specialize(name='blooms_custom', encode=encode)
     >>> b = blooms_custom(4)
     >>> b @= bytes([1, 2, 3])
     >>> bytes([1, 2, 3]) @ b
     True
 
 .. |from_base64| replace:: ``from_base64``
-.. _from_base64: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.from_base64
+.. _from_base64: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.from_base64
+
+The user of the library is responsible for ensuring that Base64-encoded Bloom filters are converted back into an an instance of the appropriate derived class by using the |from_base64|_ method that belongs to that derived class:
 
-The user of the library is responsible for ensuring that Base64-encoded Bloom filters are converted back into an an instance of the appropriate derived class by using the |from_base64|_ method that belongs to that derived class::
+.. code-block:: python
 
     >>> isinstance(blooms_custom.from_base64(b.to_base64()), blooms_custom)
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
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-The subset of the unit tests included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+The subset of the unit tests included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/blooms/blooms.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/blooms test/test_blooms.py
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/blooms>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/blooms>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/blooms>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `blooms-1.1.0/README.rst` & `blooms-1.2.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -28,184 +28,228 @@
 .. |bytearray| replace:: ``bytearray``
 .. _bytearray: https://docs.python.org/3/library/stdtypes.html#bytearray
 
 This library provides a simple and lightweight data structure for representing `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__ that is derived from the built-in |bytearray|_ type. The data structure has methods for the insertion, membership, union, and subset operations. In addition, methods for estimating capacity and for converting to and from Base64 strings are available.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/blooms>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/blooms>`__:
+
+.. code-block:: bash
 
     python -m pip install blooms
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import blooms
     from blooms import blooms
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely create, populate, and query simple `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__. The example below constructs a Bloom filter that is 32 bits (*i.e.*, four bytes) in size::
+This library makes it possible to concisely create, populate, and query simple `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__. The example below constructs a Bloom filter that is 32 bits (*i.e.*, four bytes) in size:
+
+.. code-block:: python
 
     >>> from blooms import blooms
     >>> b = blooms(4)
 
 .. |insertion_operator| replace:: insertion operator ``@=``
-.. _insertion_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__imatmul__
+.. _insertion_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__imatmul__
 
-A bytes-like object can be inserted into an instance using the |insertion_operator|_. It is the responsibility of the user of the library to hash and truncate the bytes-like object being inserted. Only the bytes that remain after truncation contribute to the membership of the bytes-like object within the Bloom filter::
+A bytes-like object can be inserted into an instance using the |insertion_operator|_. It is the responsibility of the user of the library to hash and truncate the bytes-like object being inserted. Only the bytes that remain after truncation contribute to the membership of the bytes-like object within the Bloom filter:
+
+.. code-block:: python
 
     >>> from hashlib import sha256
     >>> x = 'abc' # Value to insert.
     >>> h = sha256(x.encode()).digest() # Hash of value.
     >>> t = h[:2] # Truncated hash.
     >>> b @= t # Insert the value into the Bloom filter.
     >>> b.hex()
     '00000004'
 
 .. |membership_operator| replace:: membership operator ``@``
-.. _membership_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__rmatmul__
+.. _membership_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__rmatmul__
+
+When testing whether a bytes-like object is a member using the |membership_operator|_ of an instance, the same hashing and truncation operations should be applied:
 
-When testing whether a bytes-like object is a member using the |membership_operator|_ of an instance, the same hashing and truncation operations should be applied::
+.. code-block:: python
 
     >>> sha256('abc'.encode()).digest()[:2] @ b
     True
     >>> sha256('xyz'.encode()).digest()[:2] @ b
     False
 
 
-The |insertion_operator|_ also accepts iterable containers::
+The |insertion_operator|_ also accepts iterable containers:
+
+.. code-block:: python
 
     >>> x = sha256('x'.encode()).digest()[:2]
     >>> y = sha256('y'.encode()).digest()[:2]
     >>> z = sha256('z'.encode()).digest()[:2]
     >>> b @= [x, y, z]
     >>> b.hex()
     '02200006'
 
 .. |union_operator| replace:: built-in ``|`` operator
-.. _union_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__or__
+.. _union_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__or__
 
-The union of two Bloom filters (both having the same size) can be computed via the |union_operator|_::
+The union of two Bloom filters (both having the same size) can be computed via the |union_operator|_:
+
+.. code-block:: python
 
     >>> c = blooms(4)
     >>> c @= sha256('xyz'.encode()).digest()[:2]
     >>> d = c | b
     >>> sha256('abc'.encode()).digest()[:2] @ d
     True
     >>> sha256('xyz'.encode()).digest()[:2] @ d
     True
 
-It is also possible to check whether the members of one Bloom filter `are a subset <https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.issubset>`__ of the members of another Bloom filter::
+It is also possible to check whether the members of one Bloom filter `are a subset <https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.issubset>`__ of the members of another Bloom filter:
+
+.. code-block:: python
 
     >>> b.issubset(c)
     False
     >>> b.issubset(d)
     True
 
 .. |saturation| replace:: ``saturation``
-.. _saturation: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.saturation
+.. _saturation: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.saturation
 
 .. |float| replace:: ``float``
 .. _float: https://docs.python.org/3/library/functions.html#float
 
-The |saturation|_ method calculates the saturation of a Bloom filter. The *saturation* is a |float|_ value (between ``0.0`` and ``1.0``) that represents an upper bound on the rate with which false positives will occur when testing bytes-like objects (of a specific length) for membership within the Bloom filter::
+The |saturation|_ method calculates the saturation of a Bloom filter. The *saturation* is a |float|_ value (between ``0.0`` and ``1.0``) that represents an upper bound on the rate with which false positives will occur when testing bytes-like objects (of a specific length) for membership within the Bloom filter:
+
+.. code-block:: python
 
     >>> b = blooms(32)
     >>> from secrets import token_bytes
     >>> for _ in range(8):
     ...     b @= token_bytes(4)
     >>> b.saturation(4)
     0.03125
 
 .. |capacity| replace:: ``capacity``
-.. _capacity: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.capacity
+.. _capacity: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.capacity
 
-It is also possible to determine the approximate maximum capacity of a Bloom filter for a given saturation limit using the |capacity|_ method. For example, the output below indicates that a saturation of ``0.05`` will likely be reached after more than ``28`` insertions of bytes-like objects of length ``8``::
+It is also possible to determine the approximate maximum capacity of a Bloom filter for a given saturation limit using the |capacity|_ method. For example, the output below indicates that a saturation of ``0.05`` will likely be reached after more than ``28`` insertions of bytes-like objects of length ``8``:
+
+.. code-block:: python
 
     >>> b = blooms(32)
     >>> b.capacity(8, 0.05)
     28
 
-In addition, conversion methods to and from Base64 strings are included to support concise encoding and decoding::
+In addition, conversion methods to and from Base64 strings are included to support concise encoding and decoding:
+
+.. code-block:: python
 
     >>> b.to_base64()
     'AiAABg=='
     >>> sha256('abc'.encode()).digest()[:2] @ blooms.from_base64('AiAABg==')
     True
 
 .. |specialize| replace:: ``specialize``
-.. _specialize: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.specialize
+.. _specialize: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.specialize
 
-If it is preferable to have a Bloom filter data structure that encapsulates a particular serialization, hashing, and truncation scheme, the recommended approach is to define a derived class. The |specialize|_ method makes it possible to do so in a concise way::
+If it is preferable to have a Bloom filter data structure that encapsulates a particular serialization, hashing, and truncation scheme, the recommended approach is to define a derived class. The |specialize|_ method makes it possible to do so in a concise way:
+
+.. code-block:: python
 
     >>> encode = lambda x: sha256(x).digest()[:2]
     >>> blooms_custom = blooms.specialize(name='blooms_custom', encode=encode)
     >>> b = blooms_custom(4)
     >>> b @= bytes([1, 2, 3])
     >>> bytes([1, 2, 3]) @ b
     True
 
 .. |from_base64| replace:: ``from_base64``
-.. _from_base64: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.from_base64
+.. _from_base64: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.from_base64
+
+The user of the library is responsible for ensuring that Base64-encoded Bloom filters are converted back into an an instance of the appropriate derived class by using the |from_base64|_ method that belongs to that derived class:
 
-The user of the library is responsible for ensuring that Base64-encoded Bloom filters are converted back into an an instance of the appropriate derived class by using the |from_base64|_ method that belongs to that derived class::
+.. code-block:: python
 
     >>> isinstance(blooms_custom.from_base64(b.to_base64()), blooms_custom)
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
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-The subset of the unit tests included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+The subset of the unit tests included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/blooms/blooms.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/blooms test/test_blooms.py
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/blooms>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/blooms>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/blooms>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `blooms-1.1.0/pyproject.toml` & `blooms-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "blooms"
-version = "1.1.0"
+version = "1.2.0"
 description = "Lightweight Bloom filter data structure derived from the built-in bytearray type."
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
@@ -17,29 +17,29 @@
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
 addopts = "--doctest-modules --ignore=docs --cov=blooms --cov-report term-missing"
```

### Comparing `blooms-1.1.0/src/blooms/blooms.py` & `blooms-1.2.0/src/blooms/blooms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Lightweight Bloom filter data structure derived from the built-in
 :obj:`bytearray` type.
 """
 from __future__ import annotations
-from typing import Union, Callable
+from typing import Union, Callable, Iterable
 import doctest
-from collections.abc import Iterable
+import collections.abc
 import base64
 
 class blooms(bytearray):
     """
     Bloom filter data structure with support for common operations such as
     insertion (using :obj:`~blooms.__imatmul__`), membership (using
     :obj:`~blooms.__rmatmul__`), union (using :obj:`~blooms.__or__`), and
@@ -129,15 +129,15 @@
 
         The bytes-like object of length zero is a member of every :obj:`blooms` instance.
 
         >>> b = blooms(1)
         >>> bytes() @ b
         True
         """
-        if not isinstance(argument, (bytes, bytearray, Iterable)):
+        if not isinstance(argument, (bytes, bytearray, collections.abc.Iterable)):
             raise TypeError(
                 'supplied argument is not a bytes-like object and not iterable'
             )
 
         bss = [argument] if isinstance(argument, (bytes, bytearray)) else iter(argument)
         for bs in bss:
             bs = getattr(type(self), '_encode')(bs) if hasattr(self, '_encode') else bs
```

### Comparing `blooms-1.1.0/src/blooms.egg-info/PKG-INFO` & `blooms-1.2.0/src/blooms.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blooms
-Version: 1.1.0
+Version: 1.2.0
 Summary: Lightweight Bloom filter data structure derived from the built-in bytearray type.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/blooms
 Project-URL: Documentation, https://blooms.readthedocs.io
 Requires-Python: >=3.7
@@ -46,184 +46,228 @@
 .. |bytearray| replace:: ``bytearray``
 .. _bytearray: https://docs.python.org/3/library/stdtypes.html#bytearray
 
 This library provides a simple and lightweight data structure for representing `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__ that is derived from the built-in |bytearray|_ type. The data structure has methods for the insertion, membership, union, and subset operations. In addition, methods for estimating capacity and for converting to and from Base64 strings are available.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/blooms>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/blooms>`__:
+
+.. code-block:: bash
 
     python -m pip install blooms
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import blooms
     from blooms import blooms
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely create, populate, and query simple `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__. The example below constructs a Bloom filter that is 32 bits (*i.e.*, four bytes) in size::
+This library makes it possible to concisely create, populate, and query simple `Bloom filters <https://en.wikipedia.org/wiki/Bloom_filter>`__. The example below constructs a Bloom filter that is 32 bits (*i.e.*, four bytes) in size:
+
+.. code-block:: python
 
     >>> from blooms import blooms
     >>> b = blooms(4)
 
 .. |insertion_operator| replace:: insertion operator ``@=``
-.. _insertion_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__imatmul__
+.. _insertion_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__imatmul__
 
-A bytes-like object can be inserted into an instance using the |insertion_operator|_. It is the responsibility of the user of the library to hash and truncate the bytes-like object being inserted. Only the bytes that remain after truncation contribute to the membership of the bytes-like object within the Bloom filter::
+A bytes-like object can be inserted into an instance using the |insertion_operator|_. It is the responsibility of the user of the library to hash and truncate the bytes-like object being inserted. Only the bytes that remain after truncation contribute to the membership of the bytes-like object within the Bloom filter:
+
+.. code-block:: python
 
     >>> from hashlib import sha256
     >>> x = 'abc' # Value to insert.
     >>> h = sha256(x.encode()).digest() # Hash of value.
     >>> t = h[:2] # Truncated hash.
     >>> b @= t # Insert the value into the Bloom filter.
     >>> b.hex()
     '00000004'
 
 .. |membership_operator| replace:: membership operator ``@``
-.. _membership_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__rmatmul__
+.. _membership_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__rmatmul__
+
+When testing whether a bytes-like object is a member using the |membership_operator|_ of an instance, the same hashing and truncation operations should be applied:
 
-When testing whether a bytes-like object is a member using the |membership_operator|_ of an instance, the same hashing and truncation operations should be applied::
+.. code-block:: python
 
     >>> sha256('abc'.encode()).digest()[:2] @ b
     True
     >>> sha256('xyz'.encode()).digest()[:2] @ b
     False
 
 
-The |insertion_operator|_ also accepts iterable containers::
+The |insertion_operator|_ also accepts iterable containers:
+
+.. code-block:: python
 
     >>> x = sha256('x'.encode()).digest()[:2]
     >>> y = sha256('y'.encode()).digest()[:2]
     >>> z = sha256('z'.encode()).digest()[:2]
     >>> b @= [x, y, z]
     >>> b.hex()
     '02200006'
 
 .. |union_operator| replace:: built-in ``|`` operator
-.. _union_operator: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.__or__
+.. _union_operator: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.__or__
 
-The union of two Bloom filters (both having the same size) can be computed via the |union_operator|_::
+The union of two Bloom filters (both having the same size) can be computed via the |union_operator|_:
+
+.. code-block:: python
 
     >>> c = blooms(4)
     >>> c @= sha256('xyz'.encode()).digest()[:2]
     >>> d = c | b
     >>> sha256('abc'.encode()).digest()[:2] @ d
     True
     >>> sha256('xyz'.encode()).digest()[:2] @ d
     True
 
-It is also possible to check whether the members of one Bloom filter `are a subset <https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.issubset>`__ of the members of another Bloom filter::
+It is also possible to check whether the members of one Bloom filter `are a subset <https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.issubset>`__ of the members of another Bloom filter:
+
+.. code-block:: python
 
     >>> b.issubset(c)
     False
     >>> b.issubset(d)
     True
 
 .. |saturation| replace:: ``saturation``
-.. _saturation: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.saturation
+.. _saturation: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.saturation
 
 .. |float| replace:: ``float``
 .. _float: https://docs.python.org/3/library/functions.html#float
 
-The |saturation|_ method calculates the saturation of a Bloom filter. The *saturation* is a |float|_ value (between ``0.0`` and ``1.0``) that represents an upper bound on the rate with which false positives will occur when testing bytes-like objects (of a specific length) for membership within the Bloom filter::
+The |saturation|_ method calculates the saturation of a Bloom filter. The *saturation* is a |float|_ value (between ``0.0`` and ``1.0``) that represents an upper bound on the rate with which false positives will occur when testing bytes-like objects (of a specific length) for membership within the Bloom filter:
+
+.. code-block:: python
 
     >>> b = blooms(32)
     >>> from secrets import token_bytes
     >>> for _ in range(8):
     ...     b @= token_bytes(4)
     >>> b.saturation(4)
     0.03125
 
 .. |capacity| replace:: ``capacity``
-.. _capacity: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.capacity
+.. _capacity: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.capacity
 
-It is also possible to determine the approximate maximum capacity of a Bloom filter for a given saturation limit using the |capacity|_ method. For example, the output below indicates that a saturation of ``0.05`` will likely be reached after more than ``28`` insertions of bytes-like objects of length ``8``::
+It is also possible to determine the approximate maximum capacity of a Bloom filter for a given saturation limit using the |capacity|_ method. For example, the output below indicates that a saturation of ``0.05`` will likely be reached after more than ``28`` insertions of bytes-like objects of length ``8``:
+
+.. code-block:: python
 
     >>> b = blooms(32)
     >>> b.capacity(8, 0.05)
     28
 
-In addition, conversion methods to and from Base64 strings are included to support concise encoding and decoding::
+In addition, conversion methods to and from Base64 strings are included to support concise encoding and decoding:
+
+.. code-block:: python
 
     >>> b.to_base64()
     'AiAABg=='
     >>> sha256('abc'.encode()).digest()[:2] @ blooms.from_base64('AiAABg==')
     True
 
 .. |specialize| replace:: ``specialize``
-.. _specialize: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.specialize
+.. _specialize: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.specialize
 
-If it is preferable to have a Bloom filter data structure that encapsulates a particular serialization, hashing, and truncation scheme, the recommended approach is to define a derived class. The |specialize|_ method makes it possible to do so in a concise way::
+If it is preferable to have a Bloom filter data structure that encapsulates a particular serialization, hashing, and truncation scheme, the recommended approach is to define a derived class. The |specialize|_ method makes it possible to do so in a concise way:
+
+.. code-block:: python
 
     >>> encode = lambda x: sha256(x).digest()[:2]
     >>> blooms_custom = blooms.specialize(name='blooms_custom', encode=encode)
     >>> b = blooms_custom(4)
     >>> b @= bytes([1, 2, 3])
     >>> bytes([1, 2, 3]) @ b
     True
 
 .. |from_base64| replace:: ``from_base64``
-.. _from_base64: https://blooms.readthedocs.io/en/1.1.0/_source/blooms.html#blooms.blooms.blooms.from_base64
+.. _from_base64: https://blooms.readthedocs.io/en/1.2.0/_source/blooms.html#blooms.blooms.blooms.from_base64
+
+The user of the library is responsible for ensuring that Base64-encoded Bloom filters are converted back into an an instance of the appropriate derived class by using the |from_base64|_ method that belongs to that derived class:
 
-The user of the library is responsible for ensuring that Base64-encoded Bloom filters are converted back into an an instance of the appropriate derived class by using the |from_base64|_ method that belongs to that derived class::
+.. code-block:: python
 
     >>> isinstance(blooms_custom.from_base64(b.to_base64()), blooms_custom)
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
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-The subset of the unit tests included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+The subset of the unit tests included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/blooms/blooms.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/blooms test/test_blooms.py
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/blooms>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/blooms>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/blooms>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `blooms-1.1.0/test/test_blooms.py` & `blooms-1.2.0/test/test_blooms.py`

 * *Files identical despite different names*

