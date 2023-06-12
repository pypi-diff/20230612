# Comparing `tmp/blspy-2.0.0b1.tar.gz` & `tmp/blspy-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blspy-2.0.0b1.tar", last modified: Fri Jun  9 20:17:22 2023, max compression
+gzip compressed data, was "blspy-2.0.0b2.tar", last modified: Mon Jun 12 17:02:03 2023, max compression
```

## Comparing `blspy-2.0.0b1.tar` & `blspy-2.0.0b2.tar`

### file list

```diff
@@ -1,104 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.963346 blspy-2.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.951346 blspy-2.0.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.github/workflows/build-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.github/workflows/js-bindings.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-09 20:17:13.000000 blspy-2.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-09 20:17:13.000000 blspy-2.0.0b1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-09 20:17:13.000000 blspy-2.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-09 20:17:13.000000 blspy-2.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-09 20:17:22.963346 blspy-2.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-09 20:17:13.000000 blspy-2.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/blspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 20:17:22.000000 blspy-2.0.0b1/blspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/cmake_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-09 20:17:13.000000 blspy-2.0.0b1/cmake_modules/Findsodium.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.951346 blspy-2.0.0b1/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/contrib/gmp-patch-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-09 20:17:13.000000 blspy-2.0.0b1/contrib/gmp-patch-6.2.1/compat.c
--rw-r--r--   0 runner    (1001) docker     (123)    85426 2023-06-09 20:17:13.000000 blspy-2.0.0b1/contrib/gmp-patch-6.2.1/longlong.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-06-09 20:17:13.000000 blspy-2.0.0b1/emsdk_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.955346 blspy-2.0.0b1/js-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/blsjs.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/jsbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   126728 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.959346 blspy-2.0.0b1/js-bindings/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/PrivateKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/PublicKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/Signature.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/karma.test.js
--rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/typings.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/tests/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.959346 blspy-2.0.0b1/js-bindings/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/G1ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/G1ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/G2ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/G2ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/JSWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/PrivateKeyWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/PrivateKeyWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/SchemeMPLWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/SchemeMPLWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/UtilWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js-bindings/wrappers/UtilWrapper.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      219 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-09 20:17:13.000000 blspy-2.0.0b1/js_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-09 20:17:13.000000 blspy-2.0.0b1/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 20:17:13.000000 blspy-2.0.0b1/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-09 20:17:13.000000 blspy-2.0.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.959346 blspy-2.0.0b1/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    29858 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/pythonbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-bindings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.959346 blspy-2.0.0b1/python-impl/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/bls12381.py
--rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/hash_to_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/hd_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/impl-test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/op_swu_g2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-09 20:17:13.000000 blspy-2.0.0b1/python-impl/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:17:22.963346 blspy-2.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-09 20:17:13.000000 blspy-2.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:17:22.963346 blspy-2.0.0b1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/bls.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/bls.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   261840 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/blstasm.lib
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/elements.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/elements.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/hdkeys.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/hkdf.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/privatekey.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/privatekey.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/schemes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/schemes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/test-bench.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/test-utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    54259 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-09 20:17:13.000000 blspy-2.0.0b1/src/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.757443 blspy-2.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.745443 blspy-2.0.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.github/workflows/build-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.github/workflows/js-bindings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 17:01:54.000000 blspy-2.0.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-12 17:01:54.000000 blspy-2.0.0b2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-12 17:01:54.000000 blspy-2.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 17:01:54.000000 blspy-2.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-12 17:02:03.757443 blspy-2.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-12 17:01:54.000000 blspy-2.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/blspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 17:02:03.000000 blspy-2.0.0b2/blspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/cmake_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-12 17:01:54.000000 blspy-2.0.0b2/cmake_modules/Findsodium.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-06-12 17:01:54.000000 blspy-2.0.0b2/emsdk_build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/js-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/blsjs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/jsbindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   126728 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.749443 blspy-2.0.0b2/js-bindings/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/PrivateKey.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/PublicKey.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/Signature.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/karma.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/typings.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/tests/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.753443 blspy-2.0.0b2/js-bindings/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/G1ElementWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/G1ElementWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/G2ElementWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/G2ElementWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/JSWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/PrivateKeyWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/PrivateKeyWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/SchemeMPLWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/SchemeMPLWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/UtilWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js-bindings/wrappers/UtilWrapper.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      219 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-12 17:01:54.000000 blspy-2.0.0b2/js_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 17:01:54.000000 blspy-2.0.0b2/lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 17:01:54.000000 blspy-2.0.0b2/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 17:01:54.000000 blspy-2.0.0b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.753443 blspy-2.0.0b2/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29858 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/pythonbindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-bindings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.753443 blspy-2.0.0b2/python-impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/bls12381.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/hash_to_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/hd_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/impl-test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/op_swu_g2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 17:01:54.000000 blspy-2.0.0b2/python-impl/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:02:03.757443 blspy-2.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-12 17:01:54.000000 blspy-2.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:02:03.757443 blspy-2.0.0b2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/bls.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/bls.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   261840 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/blstasm.lib
+-rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/elements.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/elements.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/hdkeys.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/hkdf.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/privatekey.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/privatekey.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/schemes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/schemes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/test-bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/test-utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    55932 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-12 17:01:54.000000 blspy-2.0.0b2/src/util.hpp
```

### Comparing `blspy-2.0.0b1/.github/workflows/build-test.yaml` & `blspy-2.0.0b2/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/.github/workflows/build-wheels.yml` & `blspy-2.0.0b2/.github/workflows/build-wheels.yml`

 * *Files 3% similar despite different names*

```diff
@@ -138,26 +138,24 @@
         CIBW_MANYLINUX_X86_64_IMAGE: ${{ matrix.python.manylinux['intel'] }}
         CIBW_ENVIRONMENT_LINUX: "PATH=/project/cmake-3.17.3-Linux-`uname -m`/bin:$PATH"
         CIBW_BEFORE_ALL_LINUX: >
           yum -y install epel-release
           && echo "epel-release installed"
           && yum -y install lzip
           && echo "lzip installed"
-          && curl -L https://gmplib.org/download/gmp/gmp-6.2.1.tar.lz | tar x --lzip
-          && cp contrib/gmp-patch-6.2.1/longlong.h gmp-6.2.1/
-          && cp contrib/gmp-patch-6.2.1/compat.c gmp-6.2.1/
-          && cd gmp-6.2.1 && ./configure --enable-fat
-          && make && make install && cd .. && rm -rf gmp-6.2.1
+          && curl -L https://github.com/Kitware/CMake/releases/download/v3.17.3/cmake-3.17.3-Linux-`uname -m`.sh > cmake.sh
+          && yes | sh cmake.sh | cat
+          && rm -f /usr/bin/cmake
           && cmake --version
           && uname -a
         CIBW_BEFORE_BUILD_LINUX: >
           python -m pip install --upgrade pip
         CIBW_ARCHS_MACOS: ${{ matrix.os.cibw-archs-macos[matrix.arch.matrix] }}
         CIBW_BEFORE_ALL_MACOS: >
-          brew install gmp boost cmake
+          brew install boost cmake
         CIBW_BEFORE_BUILD_MACOS: >
           python -m pip install --upgrade pip
         CIBW_ENVIRONMENT_MACOS: "MACOSX_DEPLOYMENT_TARGET=10.14"
         CIBW_BEFORE_ALL_WINDOWS: >
           curl -L https://download.libsodium.org/libsodium/releases/libsodium-1.0.18-stable-msvc.zip > libsodium-1.0.18-stable-msvc.zip
           && 7z x libsodium-1.0.18-stable-msvc.zip
           && git clone https://github.com/supranational/blst.git
```

### Comparing `blspy-2.0.0b1/.github/workflows/js-bindings.yml` & `blspy-2.0.0b2/.github/workflows/js-bindings.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/.github/workflows/stale-issue.yml` & `blspy-2.0.0b2/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/CMakeLists.txt` & `blspy-2.0.0b2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/LICENSE` & `blspy-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/PKG-INFO` & `blspy-2.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,15 +21,15 @@
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:python)
 [![Language grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:cpp)
 
 NOTE: THIS LIBRARY IS NOT YET FORMALLY REVIEWED FOR SECURITY
 
 NOTE: THIS LIBRARY WAS SHIFTED TO THE IETF BLS SPECIFICATION ON 7/16/20
 
-Implements BLS signatures with aggregation using [relic toolkit](https://github.com/relic-toolkit/relic)
+Implements BLS signatures with aggregation using [blst library](https://github.com/supranational/blst.git)
 for cryptographic primitives (pairings, EC, hashing) according to the
 [IETF BLS RFC](https://datatracker.ietf.org/doc/draft-irtf-cfrg-bls-signature/)
 with [these curve parameters](https://datatracker.ietf.org/doc/draft-irtf-cfrg-pairing-friendly-curves/)
 for BLS12-381.
 
 Features:
 
@@ -211,22 +211,21 @@
 ```
 
 On a 3.5 GHz i7 Mac, verification takes about 1.1ms per signature, and signing takes 1.3ms.
 
 ### Link the library to use it
 
 ```bash
-g++ -Wl,-no_pie -std=c++11  -Ibls-signatures/build/_deps/relic-src/include -Ibls-signatures/build/_deps/relic-build/include -Ibls-signatures/src -L./bls-signatures/build/ -l bls yourapp.cpp
+g++ -Wl,-no_pie -std=c++11 -Ibls-signatures/src -L./bls-signatures/build/ -l bls yourapp.cpp
 ```
 
 ## Notes on dependencies
 
-We use Libsodium and have GMP as an optional dependency: libsodium gives secure memory
-allocation, and GMP speeds up the library by ~ 3x. MPIR is used on Windows via
-GitHub Actions instead. To install them, either download them from github and
+We use Libsodium which provides secure memory
+allocation. To install it, either download them from github and
 follow the instructions for each repo, or use a package manager like APT or
 brew. You can follow the recipe used to build python wheels for multiple
 platforms in `.github/workflows/`.
 
 ## Discussion
 
 Discussion about this library and other Chia related development is in the #dev
@@ -247,18 +246,18 @@
 
 The primary build process for this repository is to use GitHub Actions to
 build binary wheels for MacOS, Linux (x64 and aarch64), and Windows and publish
 them with a source wheel on PyPi. MacOS ARM64 is supported but not automated
 due to a lack of M1 CI runners. See `.github/workflows/build.yml`. CMake uses
 [FetchContent](https://cmake.org/cmake/help/latest/module/FetchContent.html)
 to download [pybind11](https://github.com/pybind/pybind11) for the Python
-bindings and relic from a chia relic forked repository for Windows. Building
+bindings. Building
 is then managed by [cibuildwheel](https://github.com/joerick/cibuildwheel).
 Further installation is then available via `pip install blspy` e.g. The ci
-builds include GMP and a statically linked libsodium.
+builds include a statically linked libsodium.
 
 ## Contributing and workflow
 
 Contributions are welcome and more details are available in chia-blockchain's
 [CONTRIBUTING.md](https://github.com/Chia-Network/chia-blockchain/blob/main/CONTRIBUTING.md).
 
 The main branch is usually the currently released latest version on PyPI.
@@ -295,16 +294,11 @@
 >WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 >MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 >ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 >WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 >ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 >OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-## GMP license
+## BLST license
 
-GMP is distributed under the
-[GNU LGPL v3 license](https://www.gnu.org/licenses/lgpl-3.0.html)
-
-## Relic license
-
-Relic is used with the
-[Apache 2.0 license](https://github.com/relic-toolkit/relic/blob/master/LICENSE.Apache-2.0)
+BLST is used with the
+[Apache 2.0 license](https://github.com/supranational/blst/blob/master/LICENSE)
```

### Comparing `blspy-2.0.0b1/README.md` & `blspy-2.0.0b2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:python)
 [![Language grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:cpp)
 
 NOTE: THIS LIBRARY IS NOT YET FORMALLY REVIEWED FOR SECURITY
 
 NOTE: THIS LIBRARY WAS SHIFTED TO THE IETF BLS SPECIFICATION ON 7/16/20
 
-Implements BLS signatures with aggregation using [relic toolkit](https://github.com/relic-toolkit/relic)
+Implements BLS signatures with aggregation using [blst library](https://github.com/supranational/blst.git)
 for cryptographic primitives (pairings, EC, hashing) according to the
 [IETF BLS RFC](https://datatracker.ietf.org/doc/draft-irtf-cfrg-bls-signature/)
 with [these curve parameters](https://datatracker.ietf.org/doc/draft-irtf-cfrg-pairing-friendly-curves/)
 for BLS12-381.
 
 Features:
 
@@ -200,22 +200,21 @@
 ```
 
 On a 3.5 GHz i7 Mac, verification takes about 1.1ms per signature, and signing takes 1.3ms.
 
 ### Link the library to use it
 
 ```bash
-g++ -Wl,-no_pie -std=c++11  -Ibls-signatures/build/_deps/relic-src/include -Ibls-signatures/build/_deps/relic-build/include -Ibls-signatures/src -L./bls-signatures/build/ -l bls yourapp.cpp
+g++ -Wl,-no_pie -std=c++11 -Ibls-signatures/src -L./bls-signatures/build/ -l bls yourapp.cpp
 ```
 
 ## Notes on dependencies
 
-We use Libsodium and have GMP as an optional dependency: libsodium gives secure memory
-allocation, and GMP speeds up the library by ~ 3x. MPIR is used on Windows via
-GitHub Actions instead. To install them, either download them from github and
+We use Libsodium which provides secure memory
+allocation. To install it, either download them from github and
 follow the instructions for each repo, or use a package manager like APT or
 brew. You can follow the recipe used to build python wheels for multiple
 platforms in `.github/workflows/`.
 
 ## Discussion
 
 Discussion about this library and other Chia related development is in the #dev
@@ -236,18 +235,18 @@
 
 The primary build process for this repository is to use GitHub Actions to
 build binary wheels for MacOS, Linux (x64 and aarch64), and Windows and publish
 them with a source wheel on PyPi. MacOS ARM64 is supported but not automated
 due to a lack of M1 CI runners. See `.github/workflows/build.yml`. CMake uses
 [FetchContent](https://cmake.org/cmake/help/latest/module/FetchContent.html)
 to download [pybind11](https://github.com/pybind/pybind11) for the Python
-bindings and relic from a chia relic forked repository for Windows. Building
+bindings. Building
 is then managed by [cibuildwheel](https://github.com/joerick/cibuildwheel).
 Further installation is then available via `pip install blspy` e.g. The ci
-builds include GMP and a statically linked libsodium.
+builds include a statically linked libsodium.
 
 ## Contributing and workflow
 
 Contributions are welcome and more details are available in chia-blockchain's
 [CONTRIBUTING.md](https://github.com/Chia-Network/chia-blockchain/blob/main/CONTRIBUTING.md).
 
 The main branch is usually the currently released latest version on PyPI.
@@ -284,16 +283,11 @@
 >WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 >MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 >ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 >WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 >ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 >OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-## GMP license
+## BLST license
 
-GMP is distributed under the
-[GNU LGPL v3 license](https://www.gnu.org/licenses/lgpl-3.0.html)
-
-## Relic license
-
-Relic is used with the
-[Apache 2.0 license](https://github.com/relic-toolkit/relic/blob/master/LICENSE.Apache-2.0)
+BLST is used with the
+[Apache 2.0 license](https://github.com/supranational/blst/blob/master/LICENSE)
```

### Comparing `blspy-2.0.0b1/blspy.egg-info/PKG-INFO` & `blspy-2.0.0b2/blspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,15 +21,15 @@
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:python)
 [![Language grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:cpp)
 
 NOTE: THIS LIBRARY IS NOT YET FORMALLY REVIEWED FOR SECURITY
 
 NOTE: THIS LIBRARY WAS SHIFTED TO THE IETF BLS SPECIFICATION ON 7/16/20
 
-Implements BLS signatures with aggregation using [relic toolkit](https://github.com/relic-toolkit/relic)
+Implements BLS signatures with aggregation using [blst library](https://github.com/supranational/blst.git)
 for cryptographic primitives (pairings, EC, hashing) according to the
 [IETF BLS RFC](https://datatracker.ietf.org/doc/draft-irtf-cfrg-bls-signature/)
 with [these curve parameters](https://datatracker.ietf.org/doc/draft-irtf-cfrg-pairing-friendly-curves/)
 for BLS12-381.
 
 Features:
 
@@ -211,22 +211,21 @@
 ```
 
 On a 3.5 GHz i7 Mac, verification takes about 1.1ms per signature, and signing takes 1.3ms.
 
 ### Link the library to use it
 
 ```bash
-g++ -Wl,-no_pie -std=c++11  -Ibls-signatures/build/_deps/relic-src/include -Ibls-signatures/build/_deps/relic-build/include -Ibls-signatures/src -L./bls-signatures/build/ -l bls yourapp.cpp
+g++ -Wl,-no_pie -std=c++11 -Ibls-signatures/src -L./bls-signatures/build/ -l bls yourapp.cpp
 ```
 
 ## Notes on dependencies
 
-We use Libsodium and have GMP as an optional dependency: libsodium gives secure memory
-allocation, and GMP speeds up the library by ~ 3x. MPIR is used on Windows via
-GitHub Actions instead. To install them, either download them from github and
+We use Libsodium which provides secure memory
+allocation. To install it, either download them from github and
 follow the instructions for each repo, or use a package manager like APT or
 brew. You can follow the recipe used to build python wheels for multiple
 platforms in `.github/workflows/`.
 
 ## Discussion
 
 Discussion about this library and other Chia related development is in the #dev
@@ -247,18 +246,18 @@
 
 The primary build process for this repository is to use GitHub Actions to
 build binary wheels for MacOS, Linux (x64 and aarch64), and Windows and publish
 them with a source wheel on PyPi. MacOS ARM64 is supported but not automated
 due to a lack of M1 CI runners. See `.github/workflows/build.yml`. CMake uses
 [FetchContent](https://cmake.org/cmake/help/latest/module/FetchContent.html)
 to download [pybind11](https://github.com/pybind/pybind11) for the Python
-bindings and relic from a chia relic forked repository for Windows. Building
+bindings. Building
 is then managed by [cibuildwheel](https://github.com/joerick/cibuildwheel).
 Further installation is then available via `pip install blspy` e.g. The ci
-builds include GMP and a statically linked libsodium.
+builds include a statically linked libsodium.
 
 ## Contributing and workflow
 
 Contributions are welcome and more details are available in chia-blockchain's
 [CONTRIBUTING.md](https://github.com/Chia-Network/chia-blockchain/blob/main/CONTRIBUTING.md).
 
 The main branch is usually the currently released latest version on PyPI.
@@ -295,16 +294,11 @@
 >WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 >MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 >ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 >WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 >ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 >OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-## GMP license
+## BLST license
 
-GMP is distributed under the
-[GNU LGPL v3 license](https://www.gnu.org/licenses/lgpl-3.0.html)
-
-## Relic license
-
-Relic is used with the
-[Apache 2.0 license](https://github.com/relic-toolkit/relic/blob/master/LICENSE.Apache-2.0)
+BLST is used with the
+[Apache 2.0 license](https://github.com/supranational/blst/blob/master/LICENSE)
```

### Comparing `blspy-2.0.0b1/blspy.egg-info/SOURCES.txt` & `blspy-2.0.0b2/blspy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 blspy.egg-info/PKG-INFO
 blspy.egg-info/SOURCES.txt
 blspy.egg-info/dependency_links.txt
 blspy.egg-info/not-zip-safe
 blspy.egg-info/requires.txt
 blspy.egg-info/top_level.txt
 cmake_modules/Findsodium.cmake
-contrib/gmp-patch-6.2.1/compat.c
-contrib/gmp-patch-6.2.1/longlong.h
 js-bindings/CMakeLists.txt
 js-bindings/README.md
 js-bindings/blsjs.d.ts
 js-bindings/helpers.cpp
 js-bindings/helpers.h
 js-bindings/jsbindings.cpp
 js-bindings/package-lock.json
```

### Comparing `blspy-2.0.0b1/cmake_modules/Findsodium.cmake` & `blspy-2.0.0b2/cmake_modules/Findsodium.cmake`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/CMakeLists.txt` & `blspy-2.0.0b2/js-bindings/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 CMAKE_MINIMUM_REQUIRED(VERSION 3.14.0 FATAL_ERROR)
 set(CMAKE_CXX_STANDARD 17)
 
 include_directories(
         ${INCLUDE_DIRECTORIES}
-	${CMAKE_BINARY_DIR}/_deps/relic-src/include
-        ${CMAKE_BINARY_DIR}/_deps/relic-build/include
         ${CMAKE_CURRENT_SOURCE_DIR}/../contrib/catch
 )
 
 file(GLOB_RECURSE WRAP_HEADERS ${CMAKE_CURRENT_SOURCE_DIR}/wrappers/*.h)
 file(GLOB_RECURSE WRAP_SRC ${CMAKE_CURRENT_SOURCE_DIR}/wrappers/*.cpp)
 
 add_executable(blsjs ${CMAKE_CURRENT_SOURCE_DIR}/jsbindings.cpp
```

### Comparing `blspy-2.0.0b1/js-bindings/README.md` & `blspy-2.0.0b2/js-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/blsjs.d.ts` & `blspy-2.0.0b2/js-bindings/blsjs.d.ts`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/helpers.cpp` & `blspy-2.0.0b2/js-bindings/helpers.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/helpers.h` & `blspy-2.0.0b2/js-bindings/helpers.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/jsbindings.cpp` & `blspy-2.0.0b2/js-bindings/jsbindings.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/package-lock.json` & `blspy-2.0.0b2/js-bindings/package-lock.json`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/package.json` & `blspy-2.0.0b2/js-bindings/package.json`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/tests/PrivateKey.spec.js` & `blspy-2.0.0b2/js-bindings/tests/PrivateKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/tests/PublicKey.spec.js` & `blspy-2.0.0b2/js-bindings/tests/PublicKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/tests/Signature.spec.js` & `blspy-2.0.0b2/js-bindings/tests/Signature.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/tests/karma.conf.js` & `blspy-2.0.0b2/js-bindings/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/tests/test.js` & `blspy-2.0.0b2/js-bindings/tests/test.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/tests/typings.spec.ts` & `blspy-2.0.0b2/js-bindings/tests/typings.spec.ts`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/tests/yarn.lock` & `blspy-2.0.0b2/js-bindings/tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/G1ElementWrapper.cpp` & `blspy-2.0.0b2/js-bindings/wrappers/G1ElementWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/G1ElementWrapper.h` & `blspy-2.0.0b2/js-bindings/wrappers/G1ElementWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/G2ElementWrapper.cpp` & `blspy-2.0.0b2/js-bindings/wrappers/G2ElementWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/G2ElementWrapper.h` & `blspy-2.0.0b2/js-bindings/wrappers/G2ElementWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/JSWrapper.h` & `blspy-2.0.0b2/js-bindings/wrappers/JSWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/PrivateKeyWrapper.cpp` & `blspy-2.0.0b2/js-bindings/wrappers/PrivateKeyWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/PrivateKeyWrapper.h` & `blspy-2.0.0b2/js-bindings/wrappers/PrivateKeyWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/SchemeMPLWrapper.cpp` & `blspy-2.0.0b2/js-bindings/wrappers/SchemeMPLWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/SchemeMPLWrapper.h` & `blspy-2.0.0b2/js-bindings/wrappers/SchemeMPLWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/UtilWrapper.cpp` & `blspy-2.0.0b2/js-bindings/wrappers/UtilWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/js-bindings/wrappers/UtilWrapper.h` & `blspy-2.0.0b2/js-bindings/wrappers/UtilWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-bindings/README.md` & `blspy-2.0.0b2/python-bindings/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 Alternatively, to install from source, run the following, in the project root directory:
 
 ```bash
 pip3 install .
 ```
 
 Cmake, a c++ compiler, and a recent version of pip3 (v18) are required for source install.
-GMP(speed) is an optional dependency.
 Public keys are G1Elements, and signatures are G2Elements.
 
 Then, to use:
 
 ## Import the library
 
 ```python
```

### Comparing `blspy-2.0.0b1/python-bindings/benchmark.py` & `blspy-2.0.0b2/python-bindings/benchmark.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-bindings/pythonbindings.cpp` & `blspy-2.0.0b2/python-bindings/pythonbindings.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-bindings/test.py` & `blspy-2.0.0b2/python-bindings/test.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/README.md` & `blspy-2.0.0b2/python-impl/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/bls12381.py` & `blspy-2.0.0b2/python-impl/bls12381.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/ec.py` & `blspy-2.0.0b2/python-impl/ec.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/fields.py` & `blspy-2.0.0b2/python-impl/fields.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/hash_to_field.py` & `blspy-2.0.0b2/python-impl/hash_to_field.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/hd_keys.py` & `blspy-2.0.0b2/python-impl/hd_keys.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/hkdf.py` & `blspy-2.0.0b2/python-impl/hkdf.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/impl-test.py` & `blspy-2.0.0b2/python-impl/impl-test.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/op_swu_g2.py` & `blspy-2.0.0b2/python-impl/op_swu_g2.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/pairing.py` & `blspy-2.0.0b2/python-impl/pairing.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/private_key.py` & `blspy-2.0.0b2/python-impl/private_key.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/schemes.py` & `blspy-2.0.0b2/python-impl/schemes.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/python-impl/util.py` & `blspy-2.0.0b2/python-impl/util.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/setup.py` & `blspy-2.0.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/CMakeLists.txt` & `blspy-2.0.0b2/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/bls.cpp` & `blspy-2.0.0b2/src/bls.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/bls.hpp` & `blspy-2.0.0b2/src/bls.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/blstasm.lib` & `blspy-2.0.0b2/src/blstasm.lib`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/elements.cpp` & `blspy-2.0.0b2/src/elements.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
 GTElement GTElement::FromBytesUnchecked(Bytes const bytes)
 {
     if (bytes.size() != SIZE) {
         throw std::invalid_argument("GTElement::FromBytes: Invalid size");
     }
     GTElement ele = GTElement();
-    // TO DO  blst_fp12_from_bendian(&(ele.r), bytes.begin());
+    memcpy(&(ele.r), bytes.begin(), SIZE);
     return ele;
 }
 
 GTElement GTElement::FromByteVector(const std::vector<uint8_t>& bytevec)
 {
     return GTElement::FromBytes(Bytes(bytevec));
 }
@@ -480,15 +480,15 @@
     GTElement ans;
     blst_fp12_mul(&(ans.r), &(a.r), &(b.r));
     return ans;
 }
 
 void GTElement::Serialize(uint8_t* buffer) const
 {
-    blst_bendian_from_fp12(buffer, &r);
+    memcpy(buffer, &r, GTElement::SIZE);
 }
 
 std::vector<uint8_t> GTElement::Serialize() const
 {
     std::vector<uint8_t> data(GTElement::SIZE);
     Serialize(data.data());
     return data;
```

### Comparing `blspy-2.0.0b1/src/elements.hpp` & `blspy-2.0.0b2/src/elements.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,18 @@
 
 #ifndef SRC_BLSELEMENTS_HPP_
 #define SRC_BLSELEMENTS_HPP_
 
 extern "C" {
 #include "bindings/blst.h"
 }
-#include "util.hpp"
-
-#if defined GMP && ARITH == GMP
-#include <gmp.h>
-#endif
-
 #include <utility>
 
+#include "util.hpp"
+
 namespace bls {
 class G1Element;
 class G2Element;
 class GTElement;
 
 class G1Element {
 public:
```

### Comparing `blspy-2.0.0b1/src/hdkeys.hpp` & `blspy-2.0.0b2/src/hdkeys.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/hkdf.hpp` & `blspy-2.0.0b2/src/hkdf.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/privatekey.cpp` & `blspy-2.0.0b2/src/privatekey.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/privatekey.hpp` & `blspy-2.0.0b2/src/privatekey.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/schemes.cpp` & `blspy-2.0.0b2/src/schemes.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/schemes.hpp` & `blspy-2.0.0b2/src/schemes.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/test-bench.cpp` & `blspy-2.0.0b2/src/test-bench.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/test-utils.hpp` & `blspy-2.0.0b2/src/test-utils.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b1/src/test.cpp` & `blspy-2.0.0b2/src/test.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 // limitations under the License.
 
 #include <catch2/catch_session.hpp>
 #include <catch2/catch_test_macros.hpp>
 #include <thread>
 
 #include "bls.hpp"
-extern "C" {
-// #include "relic.h"
-}
 #include "test-utils.hpp"
 using std::cout;
 using std::endl;
 using std::string;
 using std::vector;
 
 using namespace bls;
@@ -1365,12 +1362,68 @@
 
         auto badSer = point.Serialize();
 
         REQUIRE_THROWS(G2Element::FromByteVector(badSer));
     }
 }
 
+TEST_CASE("GTElement")
+{
+    SECTION("GTElement serialization")
+    {
+        vector<uint8_t> seed(32, 0x05);
+        blst_p1_affine p1_affine;
+
+        PrivateKey sk1 = BasicSchemeMPL().KeyGen(seed);
+        G1Element pk1 = BasicSchemeMPL().SkToG1(sk1);
+        pk1.CheckValid();
+        pk1.ToAffine(&p1_affine);
+        GTElement gt1 = GTElement::FromAffine(p1_affine);
+
+        auto outbuf = gt1.Serialize();
+
+        auto gt2 = GTElement::FromBytesUnchecked(outbuf);
+
+        REQUIRE(gt1 == gt2);
+    }
+
+    SECTION("GTElement pairing")
+    {
+        vector<uint8_t> seed(32, 0x05), seed2(32, 0x06);
+        vector<uint8_t> msg1 = {7, 8, 9};
+        vector<uint8_t> msg2 = {10, 11, 12};
+
+        auto sk1 = BasicSchemeMPL().KeyGen(seed);
+        auto sk2 = BasicSchemeMPL().KeyGen(seed2);
+
+        auto pk1 = sk1.GetG1Element();
+        auto pk2 = sk2.GetG1Element();
+
+        auto sig1 = BasicSchemeMPL().Sign(sk1, msg1);
+        auto sig2 = BasicSchemeMPL().Sign(sk2, msg2);
+
+        auto aggsig = BasicSchemeMPL().Aggregate({sig1, sig2});
+
+        REQUIRE(BasicSchemeMPL().AggregateVerify(
+            {pk1, pk2}, vector<vector<uint8_t>>{msg1, msg2}, aggsig));
+
+        auto pair1 = pk1.Pair(G2Element::FromMessage(
+            msg1,
+            (const uint8_t*)BasicSchemeMPL::CIPHERSUITE_ID.c_str(),
+            BasicSchemeMPL::CIPHERSUITE_ID.length()));
+        auto pair2 = pk2.Pair(G2Element::FromMessage(
+            msg2,
+            (const uint8_t*)BasicSchemeMPL::CIPHERSUITE_ID.c_str(),
+            BasicSchemeMPL::CIPHERSUITE_ID.length()));
+        auto pair = pair1 * pair2;
+
+        auto agg_sig_pair = G1Element::Generator().Pair(aggsig);
+
+        REQUIRE(pair == agg_sig_pair);
+    }
+}
+
 int main(int argc, char* argv[])
 {
     int result = Catch::Session().run(argc, argv);
     return result;
 }
```

### Comparing `blspy-2.0.0b1/src/util.hpp` & `blspy-2.0.0b2/src/util.hpp`

 * *Files identical despite different names*

