# Comparing `tmp/const_cython_lib-0.0.4.tar.gz` & `tmp/const_cython_lib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "const_cython_lib-0.0.4.tar", last modified: Mon Jun 12 10:13:30 2023, max compression
+gzip compressed data, was "const_cython_lib-0.0.5.tar", last modified: Mon Jun 12 10:16:40 2023, max compression
```

## Comparing `const_cython_lib-0.0.4.tar` & `const_cython_lib-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 10:13:30.559345 const_cython_lib-0.0.4/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       58 2023-06-12 10:13:23.000000 const_cython_lib-0.0.4/MANIFEST.in
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 10:13:30.559219 const_cython_lib-0.0.4/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   111060 2023-06-12 10:13:30.000000 const_cython_lib-0.0.4/const_cython_lib.c
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 10:13:30.559047 const_cython_lib-0.0.4/const_cython_lib.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 10:13:30.000000 const_cython_lib-0.0.4/const_cython_lib.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      295 2023-06-12 10:13:30.000000 const_cython_lib-0.0.4/const_cython_lib.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 10:13:30.000000 const_cython_lib-0.0.4/const_cython_lib.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 10:13:30.000000 const_cython_lib-0.0.4/const_cython_lib.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 10:13:30.000000 const_cython_lib-0.0.4/const_cython_lib.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       42 2023-06-12 10:08:35.000000 const_cython_lib-0.0.4/const_cython_lib.pxd
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       60 2023-06-12 10:09:17.000000 const_cython_lib-0.0.4/const_cython_lib.pyx
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 10:11:02.000000 const_cython_lib-0.0.4/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 10:13:30.559385 const_cython_lib-0.0.4/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      265 2023-06-12 09:12:18.000000 const_cython_lib-0.0.4/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 10:16:40.849649 const_cython_lib-0.0.5/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       58 2023-06-12 10:13:23.000000 const_cython_lib-0.0.5/MANIFEST.in
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 10:16:40.849512 const_cython_lib-0.0.5/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   110972 2023-06-12 10:16:40.000000 const_cython_lib-0.0.5/const_cython_lib.c
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 10:16:40.849297 const_cython_lib-0.0.5/const_cython_lib.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 10:16:40.000000 const_cython_lib-0.0.5/const_cython_lib.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      295 2023-06-12 10:16:40.000000 const_cython_lib-0.0.5/const_cython_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 10:16:40.000000 const_cython_lib-0.0.5/const_cython_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 10:16:40.000000 const_cython_lib-0.0.5/const_cython_lib.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 10:16:40.000000 const_cython_lib-0.0.5/const_cython_lib.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       30 2023-06-12 10:15:05.000000 const_cython_lib-0.0.5/const_cython_lib.pxd
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       48 2023-06-12 10:15:12.000000 const_cython_lib-0.0.5/const_cython_lib.pyx
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 10:16:08.000000 const_cython_lib-0.0.5/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 10:16:40.849691 const_cython_lib-0.0.5/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      265 2023-06-12 09:12:18.000000 const_cython_lib-0.0.5/setup.py
```

### Comparing `const_cython_lib-0.0.4/const_cython_lib.c` & `const_cython_lib-0.0.5/const_cython_lib.c`

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

