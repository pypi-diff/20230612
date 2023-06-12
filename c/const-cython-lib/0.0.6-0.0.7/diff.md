# Comparing `tmp/const_cython_lib-0.0.6.tar.gz` & `tmp/const_cython_lib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "const_cython_lib-0.0.6.tar", last modified: Mon Jun 12 10:46:09 2023, max compression
+gzip compressed data, was "const_cython_lib-0.0.7.tar", last modified: Mon Jun 12 10:47:57 2023, max compression
```

## Comparing `const_cython_lib-0.0.6.tar` & `const_cython_lib-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 10:46:09.764912 const_cython_lib-0.0.6/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      113 2023-06-12 10:38:59.000000 const_cython_lib-0.0.6/MANIFEST.in
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 10:46:09.764778 const_cython_lib-0.0.6/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   111060 2023-06-12 10:43:54.000000 const_cython_lib-0.0.6/const_cython_lib.c
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 10:46:09.764583 const_cython_lib-0.0.6/const_cython_lib.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 10:46:09.000000 const_cython_lib-0.0.6/const_cython_lib.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      314 2023-06-12 10:46:09.000000 const_cython_lib-0.0.6/const_cython_lib.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 10:46:09.000000 const_cython_lib-0.0.6/const_cython_lib.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 10:43:37.000000 const_cython_lib-0.0.6/const_cython_lib.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 10:46:09.000000 const_cython_lib-0.0.6/const_cython_lib.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      826 2023-06-12 10:43:54.000000 const_cython_lib-0.0.6/const_cython_lib.h
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       42 2023-06-12 10:31:00.000000 const_cython_lib-0.0.6/const_cython_lib.pxd
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       60 2023-06-12 10:31:05.000000 const_cython_lib-0.0.6/const_cython_lib.pyx
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 10:31:17.000000 const_cython_lib-0.0.6/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 10:46:09.764955 const_cython_lib-0.0.6/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      331 2023-06-12 10:45:22.000000 const_cython_lib-0.0.6/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 10:47:57.862991 const_cython_lib-0.0.7/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      113 2023-06-12 10:38:59.000000 const_cython_lib-0.0.7/MANIFEST.in
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 10:47:57.862846 const_cython_lib-0.0.7/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   110972 2023-06-12 10:47:57.000000 const_cython_lib-0.0.7/const_cython_lib.c
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 10:47:57.862635 const_cython_lib-0.0.7/const_cython_lib.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 10:47:57.000000 const_cython_lib-0.0.7/const_cython_lib.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      314 2023-06-12 10:47:57.000000 const_cython_lib-0.0.7/const_cython_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 10:47:57.000000 const_cython_lib-0.0.7/const_cython_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 10:47:57.000000 const_cython_lib-0.0.7/const_cython_lib.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 10:47:57.000000 const_cython_lib-0.0.7/const_cython_lib.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      812 2023-06-12 10:47:57.000000 const_cython_lib-0.0.7/const_cython_lib.h
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       30 2023-06-12 10:46:58.000000 const_cython_lib-0.0.7/const_cython_lib.pxd
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       48 2023-06-12 10:47:05.000000 const_cython_lib-0.0.7/const_cython_lib.pyx
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 10:46:45.000000 const_cython_lib-0.0.7/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 10:47:57.863034 const_cython_lib-0.0.7/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      331 2023-06-12 10:45:22.000000 const_cython_lib-0.0.7/setup.py
```

### Comparing `const_cython_lib-0.0.6/const_cython_lib.c` & `const_cython_lib-0.0.7/const_cython_lib.c`

 * *Files 0% similar despite different names*

```diff
@@ -1167,15 +1167,15 @@
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'const_cython_lib' */
-__PYX_EXTERN_C PyObject *__pyx_f_16const_cython_lib_sum(int const , int const ); /*proto*/
+__PYX_EXTERN_C PyObject *__pyx_f_16const_cython_lib_sum(int, int); /*proto*/
 #define __Pyx_MODULE_NAME "const_cython_lib"
 extern int __pyx_module_is_main_const_cython_lib;
 int __pyx_module_is_main_const_cython_lib = 0;
 
 /* Implementation of 'const_cython_lib' */
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -1184,40 +1184,40 @@
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
 
-PyObject *__pyx_f_16const_cython_lib_sum(int const __pyx_v_a, int const __pyx_v_b) {
+PyObject *__pyx_f_16const_cython_lib_sum(int __pyx_v_a, int __pyx_v_b) {
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
@@ -1325,15 +1325,15 @@
 static int __Pyx_modinit_function_export_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
-  if (__Pyx_ExportFunction("sum", (void (*)(void))__pyx_f_16const_cython_lib_sum, "PyObject *(int const , int const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("sum", (void (*)(void))__pyx_f_16const_cython_lib_sum, "PyObject *(int, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -1566,15 +1566,15 @@
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

### Comparing `const_cython_lib-0.0.6/const_cython_lib.h` & `const_cython_lib-0.0.7/const_cython_lib.h`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   #endif
 #endif
 
 #ifndef DL_IMPORT
   #define DL_IMPORT(_T) _T
 #endif
 
-__PYX_EXTERN_C PyObject *__pyx_f_16const_cython_lib_sum(int const , int const );
+__PYX_EXTERN_C PyObject *__pyx_f_16const_cython_lib_sum(int, int);
 
 #endif /* !__PYX_HAVE_API__const_cython_lib */
 
 /* WARNING: the interface of the module init function changed in CPython 3.5. */
 /* It now returns a PyModuleDef instance instead of a PyModule instance. */
 
 #if PY_MAJOR_VERSION < 3
```

