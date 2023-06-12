# Comparing `tmp/const-cython-client-0.0.1.tar.gz` & `tmp/const-cython-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "const-cython-client-0.0.1.tar", last modified: Mon Jun 12 13:40:17 2023, max compression
+gzip compressed data, was "const-cython-client-0.0.2.tar", last modified: Mon Jun 12 14:12:26 2023, max compression
```

## Comparing `const-cython-client-0.0.1.tar` & `const-cython-client-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 13:40:17.432126 const-cython-client-0.0.1/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       63 2023-06-12 13:40:04.000000 const-cython-client-0.0.1/MANIFEST.in
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      135 2023-06-12 13:40:17.432005 const-cython-client-0.0.1/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   113985 2023-06-12 13:40:17.000000 const-cython-client-0.0.1/const_cython_client.c
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 13:40:17.431807 const-cython-client-0.0.1/const_cython_client.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      135 2023-06-12 13:40:17.000000 const-cython-client-0.0.1/const_cython_client.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      337 2023-06-12 13:40:17.000000 const-cython-client-0.0.1/const_cython_client.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 13:40:17.000000 const-cython-client-0.0.1/const_cython_client.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 13:38:01.000000 const-cython-client-0.0.1/const_cython_client.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       24 2023-06-12 13:40:17.000000 const-cython-client-0.0.1/const_cython_client.egg-info/requires.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       20 2023-06-12 13:40:17.000000 const-cython-client-0.0.1/const_cython_client.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       78 2023-06-12 13:37:49.000000 const-cython-client-0.0.1/const_cython_client.pyx
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      307 2023-06-12 13:33:19.000000 const-cython-client-0.0.1/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 13:40:17.432162 const-cython-client-0.0.1/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      270 2023-06-12 13:40:11.000000 const-cython-client-0.0.1/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:12:26.052713 const-cython-client-0.0.2/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       63 2023-06-12 13:40:04.000000 const-cython-client-0.0.2/MANIFEST.in
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      135 2023-06-12 14:12:26.052571 const-cython-client-0.0.2/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   113932 2023-06-12 14:12:25.000000 const-cython-client-0.0.2/const_cython_client.c
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:12:26.052325 const-cython-client-0.0.2/const_cython_client.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      135 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      337 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:12:25.000000 const-cython-client-0.0.2/const_cython_client.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       24 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/requires.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       20 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       78 2023-06-12 13:37:49.000000 const-cython-client-0.0.2/const_cython_client.pyx
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      307 2023-06-12 14:11:17.000000 const-cython-client-0.0.2/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 14:12:26.052758 const-cython-client-0.0.2/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      270 2023-06-12 13:40:11.000000 const-cython-client-0.0.2/setup.py
```

### Comparing `const-cython-client-0.0.1/const_cython_client.c` & `const-cython-client-0.0.2/const_cython_client.c`

 * *Files 0% similar despite different names*

```diff
@@ -1164,15 +1164,15 @@
 static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'const_cython_lib.lsum' */
-static PyObject *(*__pyx_f_16const_cython_lib_4lsum_lsum)(int const , int const , int __pyx_skip_dispatch); /*proto*/
+static PyObject *(*__pyx_f_16const_cython_lib_4lsum_lsum)(int const , int const ); /*proto*/
 
 /* Module declarations from 'const_cython_client' */
 #define __Pyx_MODULE_NAME "const_cython_client"
 extern int __pyx_module_is_main_const_cython_client;
 int __pyx_module_is_main_const_cython_client = 0;
 
 /* Implementation of 'const_cython_client' */
@@ -1231,15 +1231,15 @@
   /* "const_cython_client.pyx":4
  * 
  * def plus_1(a):
  *     return lsum(a, 1)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_a); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 4, __pyx_L1_error)
-  __pyx_t_2 = __pyx_f_16const_cython_lib_4lsum_lsum(__pyx_t_1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_16const_cython_lib_4lsum_lsum(__pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "const_cython_client.pyx":3
  * from const_cython_lib.lsum cimport lsum
@@ -1409,15 +1409,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("const_cython_lib.lsum"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "lsum", (void (**)(void))&__pyx_f_16const_cython_lib_4lsum_lsum, "PyObject *(int const , int const , int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "lsum", (void (**)(void))&__pyx_f_16const_cython_lib_4lsum_lsum, "PyObject *(int const , int const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

