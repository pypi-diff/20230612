# Comparing `tmp/const-cython-client-0.0.2.tar.gz` & `tmp/const-cython-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "const-cython-client-0.0.2.tar", last modified: Mon Jun 12 14:12:26 2023, max compression
+gzip compressed data, was "const-cython-client-0.1.0.tar", last modified: Mon Jun 12 14:19:12 2023, max compression
```

## Comparing `const-cython-client-0.0.2.tar` & `const-cython-client-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:12:26.052713 const-cython-client-0.0.2/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       63 2023-06-12 13:40:04.000000 const-cython-client-0.0.2/MANIFEST.in
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      135 2023-06-12 14:12:26.052571 const-cython-client-0.0.2/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   113932 2023-06-12 14:12:25.000000 const-cython-client-0.0.2/const_cython_client.c
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:12:26.052325 const-cython-client-0.0.2/const_cython_client.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      135 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      337 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:12:25.000000 const-cython-client-0.0.2/const_cython_client.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       24 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/requires.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       20 2023-06-12 14:12:26.000000 const-cython-client-0.0.2/const_cython_client.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       78 2023-06-12 13:37:49.000000 const-cython-client-0.0.2/const_cython_client.pyx
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      307 2023-06-12 14:11:17.000000 const-cython-client-0.0.2/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 14:12:26.052758 const-cython-client-0.0.2/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      270 2023-06-12 13:40:11.000000 const-cython-client-0.0.2/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:19:12.718185 const-cython-client-0.1.0/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      135 2023-06-12 14:19:12.718041 const-cython-client-0.1.0/PKG-INFO
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:19:12.716796 const-cython-client-0.1.0/const_cython_client/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:17:13.000000 const-cython-client-0.1.0/const_cython_client/__init__.py
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   114007 2023-06-12 14:19:12.000000 const-cython-client-0.1.0/const_cython_client/plus.c
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       78 2023-06-12 14:16:55.000000 const-cython-client-0.1.0/const_cython_client/plus.pyx
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:19:12.717815 const-cython-client-0.1.0/const_cython_client.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      135 2023-06-12 14:19:12.000000 const-cython-client-0.1.0/const_cython_client.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      367 2023-06-12 14:19:12.000000 const-cython-client-0.1.0/const_cython_client.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:19:12.000000 const-cython-client-0.1.0/const_cython_client.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:19:12.000000 const-cython-client-0.1.0/const_cython_client.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       24 2023-06-12 14:19:12.000000 const-cython-client-0.1.0/const_cython_client.egg-info/requires.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       20 2023-06-12 14:19:12.000000 const-cython-client-0.1.0/const_cython_client.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      307 2023-06-12 14:17:23.000000 const-cython-client-0.1.0/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 14:19:12.718230 const-cython-client-0.1.0/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      361 2023-06-12 14:18:46.000000 const-cython-client-0.1.0/setup.py
```

### Comparing `const-cython-client-0.0.2/const_cython_client.c` & `const-cython-client-0.1.0/const_cython_client/plus.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "const_cython_client",
         "sources": [
-            "const_cython_client.pyx"
+            "const_cython_client/plus.pyx"
         ]
     },
     "module_name": "const_cython_client"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -962,15 +962,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "const_cython_client.pyx",
+  "const_cython_client/plus.pyx",
 };
 
 /*--- Type declarations ---*/
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
@@ -1179,29 +1179,29 @@
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_plus_1[] = "plus_1";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_const_cython_client[] = "const_cython_client";
-static const char __pyx_k_const_cython_client_pyx[] = "const_cython_client.pyx";
+static const char __pyx_k_const_cython_client_plus_pyx[] = "const_cython_client/plus.pyx";
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_const_cython_client;
-static PyObject *__pyx_kp_s_const_cython_client_pyx;
+static PyObject *__pyx_kp_s_const_cython_client_plus_pyx;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_plus_1;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_pf_19const_cython_client_plus_1(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a); /* proto */
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_codeobj__2;
 /* Late includes */
 
-/* "const_cython_client.pyx":3
+/* "const_cython_client/plus.pyx":3
  * from const_cython_lib.lsum cimport lsum
  * 
  * def plus_1(a):             # <<<<<<<<<<<<<<
  *     return lsum(a, 1)
  */
 
 /* Python wrapper */
@@ -1224,28 +1224,28 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("plus_1", 0);
 
-  /* "const_cython_client.pyx":4
+  /* "const_cython_client/plus.pyx":4
  * 
  * def plus_1(a):
  *     return lsum(a, 1)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_a); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 4, __pyx_L1_error)
   __pyx_t_2 = __pyx_f_16const_cython_lib_4lsum_lsum(__pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "const_cython_client.pyx":3
+  /* "const_cython_client/plus.pyx":3
  * from const_cython_lib.lsum cimport lsum
  * 
  * def plus_1(a):             # <<<<<<<<<<<<<<
  *     return lsum(a, 1)
  */
 
   /* function exit code */
@@ -1304,39 +1304,39 @@
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_const_cython_client, __pyx_k_const_cython_client, sizeof(__pyx_k_const_cython_client), 0, 0, 1, 1},
-  {&__pyx_kp_s_const_cython_client_pyx, __pyx_k_const_cython_client_pyx, sizeof(__pyx_k_const_cython_client_pyx), 0, 0, 1, 0},
+  {&__pyx_kp_s_const_cython_client_plus_pyx, __pyx_k_const_cython_client_plus_pyx, sizeof(__pyx_k_const_cython_client_plus_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_plus_1, __pyx_k_plus_1, sizeof(__pyx_k_plus_1), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "const_cython_client.pyx":3
+  /* "const_cython_client/plus.pyx":3
  * from const_cython_lib.lsum cimport lsum
  * 
  * def plus_1(a):             # <<<<<<<<<<<<<<
  *     return lsum(a, 1)
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_n_s_a); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_const_cython_client_pyx, __pyx_n_s_plus_1, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_const_cython_client_plus_pyx, __pyx_n_s_plus_1, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -1619,26 +1619,26 @@
   (void)__Pyx_modinit_variable_import_code();
   if (unlikely(__Pyx_modinit_function_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "const_cython_client.pyx":3
+  /* "const_cython_client/plus.pyx":3
  * from const_cython_lib.lsum cimport lsum
  * 
  * def plus_1(a):             # <<<<<<<<<<<<<<
  *     return lsum(a, 1)
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_19const_cython_client_1plus_1, NULL, __pyx_n_s_const_cython_client); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_plus_1, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "const_cython_client.pyx":1
+  /* "const_cython_client/plus.pyx":1
  * from const_cython_lib.lsum cimport lsum             # <<<<<<<<<<<<<<
  * 
  * def plus_1(a):
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
```

