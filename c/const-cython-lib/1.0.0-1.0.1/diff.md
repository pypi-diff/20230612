# Comparing `tmp/const_cython_lib-1.0.0.tar.gz` & `tmp/const_cython_lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "const_cython_lib-1.0.0.tar", last modified: Mon Jun 12 16:04:15 2023, max compression
+gzip compressed data, was "const_cython_lib-1.0.1.tar", last modified: Mon Jun 12 16:06:01 2023, max compression
```

## Comparing `const_cython_lib-1.0.0.tar` & `const_cython_lib-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 16:04:15.579235 const_cython_lib-1.0.0/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 16:04:15.579087 const_cython_lib-1.0.0/PKG-INFO
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 16:04:15.577910 const_cython_lib-1.0.0/const_cython_lib/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:09:09.000000 const_cython_lib-1.0.0/const_cython_lib/__init__.py
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   111066 2023-06-12 16:04:15.000000 const_cython_lib-1.0.0/const_cython_lib/lsum.c
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      839 2023-06-12 16:04:15.000000 const_cython_lib-1.0.0/const_cython_lib/lsum.h
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       43 2023-06-12 16:04:11.000000 const_cython_lib-1.0.0/const_cython_lib/lsum.pxd
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       61 2023-06-12 16:04:11.000000 const_cython_lib-1.0.0/const_cython_lib/lsum.pyx
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 16:04:15.578796 const_cython_lib-1.0.0/const_cython_lib.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 16:04:15.000000 const_cython_lib-1.0.0/const_cython_lib.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      351 2023-06-12 16:04:15.000000 const_cython_lib-1.0.0/const_cython_lib.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 16:04:15.000000 const_cython_lib-1.0.0/const_cython_lib.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 16:03:45.000000 const_cython_lib-1.0.0/const_cython_lib.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 16:04:15.000000 const_cython_lib-1.0.0/const_cython_lib.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 16:03:23.000000 const_cython_lib-1.0.0/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 16:04:15.579284 const_cython_lib-1.0.0/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      381 2023-06-12 16:04:09.000000 const_cython_lib-1.0.0/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 16:06:01.320014 const_cython_lib-1.0.1/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 16:06:01.319875 const_cython_lib-1.0.1/PKG-INFO
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 16:06:01.318934 const_cython_lib-1.0.1/const_cython_lib/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:09:09.000000 const_cython_lib-1.0.1/const_cython_lib/__init__.py
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   110978 2023-06-12 16:06:01.000000 const_cython_lib-1.0.1/const_cython_lib/lsum.c
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      825 2023-06-12 16:06:01.000000 const_cython_lib-1.0.1/const_cython_lib/lsum.h
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       31 2023-06-12 16:05:57.000000 const_cython_lib-1.0.1/const_cython_lib/lsum.pxd
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       49 2023-06-12 16:05:57.000000 const_cython_lib-1.0.1/const_cython_lib/lsum.pyx
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 16:06:01.319670 const_cython_lib-1.0.1/const_cython_lib.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 16:06:01.000000 const_cython_lib-1.0.1/const_cython_lib.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      351 2023-06-12 16:06:01.000000 const_cython_lib-1.0.1/const_cython_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 16:06:01.000000 const_cython_lib-1.0.1/const_cython_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 16:06:01.000000 const_cython_lib-1.0.1/const_cython_lib.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 16:06:01.000000 const_cython_lib-1.0.1/const_cython_lib.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 16:05:30.000000 const_cython_lib-1.0.1/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 16:06:01.320068 const_cython_lib-1.0.1/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      381 2023-06-12 16:04:09.000000 const_cython_lib-1.0.1/setup.py
```

### Comparing `const_cython_lib-1.0.0/const_cython_lib/lsum.c` & `const_cython_lib-1.0.1/const_cython_lib/lsum.c`

 * *Files 1% similar despite different names*

```diff
@@ -1167,15 +1167,15 @@
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'const_cython_lib.lsum' */
-__PYX_EXTERN_C PyObject *__pyx_f_16const_cython_lib_4lsum_lsum(int const , int const ); /*proto*/
+__PYX_EXTERN_C PyObject *__pyx_f_16const_cython_lib_4lsum_lsum(int, int); /*proto*/
 #define __Pyx_MODULE_NAME "const_cython_lib.lsum"
 extern int __pyx_module_is_main_const_cython_lib__lsum;
 int __pyx_module_is_main_const_cython_lib__lsum = 0;
 
 /* Implementation of 'const_cython_lib.lsum' */
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -1184,40 +1184,40 @@
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_test;
 /* Late includes */
 
 /* "const_cython_lib/lsum.pyx":1
- * cdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
+ * cdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
-PyObject *__pyx_f_16const_cython_lib_4lsum_lsum(int const __pyx_v_a, int const __pyx_v_b) {
+PyObject *__pyx_f_16const_cython_lib_4lsum_lsum(int __pyx_v_a, int __pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lsum", 0);
 
   /* "const_cython_lib/lsum.pyx":2
- * cdef public lsum(const int a, const int b):
+ * cdef public lsum(int a, int b):
  *     return a + b             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_a + __pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "const_cython_lib/lsum.pyx":1
- * cdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
+ * cdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("const_cython_lib.lsum.lsum", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -1325,15 +1325,15 @@
 static int __Pyx_modinit_function_export_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
-  if (__Pyx_ExportFunction("lsum", (void (*)(void))__pyx_f_16const_cython_lib_4lsum_lsum, "PyObject *(int const , int const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("lsum", (void (*)(void))__pyx_f_16const_cython_lib_4lsum_lsum, "PyObject *(int, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
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
 
   /* "const_cython_lib/lsum.pyx":1
- * cdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
+ * cdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `const_cython_lib-1.0.0/const_cython_lib/lsum.h` & `const_cython_lib-1.0.1/const_cython_lib/lsum.h`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   #endif
 #endif
 
 #ifndef DL_IMPORT
   #define DL_IMPORT(_T) _T
 #endif
 
-__PYX_EXTERN_C PyObject *__pyx_f_16const_cython_lib_4lsum_lsum(int const , int const );
+__PYX_EXTERN_C PyObject *__pyx_f_16const_cython_lib_4lsum_lsum(int, int);
 
 #endif /* !__PYX_HAVE_API__const_cython_lib__lsum */
 
 /* WARNING: the interface of the module init function changed in CPython 3.5. */
 /* It now returns a PyModuleDef instance instead of a PyModule instance. */
 
 #if PY_MAJOR_VERSION < 3
```

