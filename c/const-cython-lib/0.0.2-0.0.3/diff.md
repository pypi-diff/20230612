# Comparing `tmp/const_cython_lib-0.0.2.tar.gz` & `tmp/const_cython_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "const_cython_lib-0.0.2.tar", last modified: Mon Jun 12 09:49:04 2023, max compression
+gzip compressed data, was "const_cython_lib-0.0.3.tar", last modified: Mon Jun 12 09:50:31 2023, max compression
```

## Comparing `const_cython_lib-0.0.2.tar` & `const_cython_lib-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 09:49:04.080404 const_cython_lib-0.0.2/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       29 2023-06-12 09:16:54.000000 const_cython_lib-0.0.2/MANIFEST.in
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 09:49:04.080270 const_cython_lib-0.0.2/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   109651 2023-06-12 09:49:03.000000 const_cython_lib-0.0.2/const_cython_lib.c
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 09:49:04.080106 const_cython_lib-0.0.2/const_cython_lib.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 09:49:04.000000 const_cython_lib-0.0.2/const_cython_lib.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      274 2023-06-12 09:49:04.000000 const_cython_lib-0.0.2/const_cython_lib.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 09:49:04.000000 const_cython_lib-0.0.2/const_cython_lib.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 09:49:03.000000 const_cython_lib-0.0.2/const_cython_lib.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 09:49:04.000000 const_cython_lib-0.0.2/const_cython_lib.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       60 2023-06-12 09:46:30.000000 const_cython_lib-0.0.2/const_cython_lib.pyx
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 09:48:29.000000 const_cython_lib-0.0.2/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 09:49:04.080445 const_cython_lib-0.0.2/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      265 2023-06-12 09:12:18.000000 const_cython_lib-0.0.2/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 09:50:31.036898 const_cython_lib-0.0.3/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       29 2023-06-12 09:16:54.000000 const_cython_lib-0.0.3/MANIFEST.in
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 09:50:31.036769 const_cython_lib-0.0.3/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   109577 2023-06-12 09:50:30.000000 const_cython_lib-0.0.3/const_cython_lib.c
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 09:50:31.036586 const_cython_lib-0.0.3/const_cython_lib.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 09:50:31.000000 const_cython_lib-0.0.3/const_cython_lib.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      274 2023-06-12 09:50:31.000000 const_cython_lib-0.0.3/const_cython_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 09:50:31.000000 const_cython_lib-0.0.3/const_cython_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 09:50:30.000000 const_cython_lib-0.0.3/const_cython_lib.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 09:50:31.000000 const_cython_lib-0.0.3/const_cython_lib.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       48 2023-06-12 09:49:42.000000 const_cython_lib-0.0.3/const_cython_lib.pyx
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 09:50:09.000000 const_cython_lib-0.0.3/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 09:50:31.036943 const_cython_lib-0.0.3/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      265 2023-06-12 09:12:18.000000 const_cython_lib-0.0.3/setup.py
```

### Comparing `const_cython_lib-0.0.2/const_cython_lib.c` & `const_cython_lib-0.0.3/const_cython_lib.c`

 * *Files 0% similar despite different names*

```diff
@@ -1164,15 +1164,15 @@
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'const_cython_lib' */
-__PYX_EXTERN_C PyObject *sum(int const , int const ); /*proto*/
+__PYX_EXTERN_C PyObject *sum(int, int); /*proto*/
 #define __Pyx_MODULE_NAME "const_cython_lib"
 extern int __pyx_module_is_main_const_cython_lib;
 int __pyx_module_is_main_const_cython_lib = 0;
 
 /* Implementation of 'const_cython_lib' */
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -1181,40 +1181,40 @@
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_test;
 /* Late includes */
 
 /* "const_cython_lib.pyx":1
- * cdef public sum(const int a, const int b):             # <<<<<<<<<<<<<<
+ * cdef public sum(int a, int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
-PyObject *sum(int const __pyx_v_a, int const __pyx_v_b) {
+PyObject *sum(int __pyx_v_a, int __pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sum", 0);
 
   /* "const_cython_lib.pyx":2
- * cdef public sum(const int a, const int b):
+ * cdef public sum(int a, int b):
  *     return a + b             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_a + __pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "const_cython_lib.pyx":1
- * cdef public sum(const int a, const int b):             # <<<<<<<<<<<<<<
+ * cdef public sum(int a, int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("const_cython_lib.sum", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -1556,15 +1556,15 @@
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "const_cython_lib.pyx":1
- * cdef public sum(const int a, const int b):             # <<<<<<<<<<<<<<
+ * cdef public sum(int a, int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

