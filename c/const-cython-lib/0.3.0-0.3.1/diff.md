# Comparing `tmp/const_cython_lib-0.3.0.tar.gz` & `tmp/const_cython_lib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "const_cython_lib-0.3.0.tar", last modified: Mon Jun 12 14:10:01 2023, max compression
+gzip compressed data, was "const_cython_lib-0.3.1.tar", last modified: Mon Jun 12 14:10:33 2023, max compression
```

## Comparing `const_cython_lib-0.3.0.tar` & `const_cython_lib-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:10:01.719478 const_cython_lib-0.3.0/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 14:10:01.719342 const_cython_lib-0.3.0/PKG-INFO
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:10:01.718280 const_cython_lib-0.3.0/const_cython_lib/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:09:09.000000 const_cython_lib-0.3.0/const_cython_lib/__init__.py
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   109689 2023-06-12 14:10:01.000000 const_cython_lib-0.3.0/const_cython_lib/lsum.c
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      800 2023-06-12 14:10:01.000000 const_cython_lib-0.3.0/const_cython_lib/lsum.h
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       43 2023-06-12 14:09:57.000000 const_cython_lib-0.3.0/const_cython_lib/lsum.pxd
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       61 2023-06-12 14:09:57.000000 const_cython_lib-0.3.0/const_cython_lib/lsum.pyx
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:10:01.719148 const_cython_lib-0.3.0/const_cython_lib.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 14:10:01.000000 const_cython_lib-0.3.0/const_cython_lib.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      351 2023-06-12 14:10:01.000000 const_cython_lib-0.3.0/const_cython_lib.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:10:01.000000 const_cython_lib-0.3.0/const_cython_lib.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:10:01.000000 const_cython_lib-0.3.0/const_cython_lib.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 14:10:01.000000 const_cython_lib-0.3.0/const_cython_lib.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 14:09:46.000000 const_cython_lib-0.3.0/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 14:10:01.719519 const_cython_lib-0.3.0/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      376 2023-06-12 13:33:19.000000 const_cython_lib-0.3.0/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:10:33.031898 const_cython_lib-0.3.1/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 14:10:33.031721 const_cython_lib-0.3.1/PKG-INFO
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:10:33.030288 const_cython_lib-0.3.1/const_cython_lib/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:09:09.000000 const_cython_lib-0.3.1/const_cython_lib/__init__.py
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   109615 2023-06-12 14:10:32.000000 const_cython_lib-0.3.1/const_cython_lib/lsum.c
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      786 2023-06-12 14:10:32.000000 const_cython_lib-0.3.1/const_cython_lib/lsum.h
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       31 2023-06-12 14:10:28.000000 const_cython_lib-0.3.1/const_cython_lib/lsum.pxd
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       49 2023-06-12 14:10:28.000000 const_cython_lib-0.3.1/const_cython_lib/lsum.pyx
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 14:10:33.031429 const_cython_lib-0.3.1/const_cython_lib.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 14:10:33.000000 const_cython_lib-0.3.1/const_cython_lib.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      351 2023-06-12 14:10:33.000000 const_cython_lib-0.3.1/const_cython_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:10:33.000000 const_cython_lib-0.3.1/const_cython_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 14:10:32.000000 const_cython_lib-0.3.1/const_cython_lib.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 14:10:33.000000 const_cython_lib-0.3.1/const_cython_lib.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 14:10:21.000000 const_cython_lib-0.3.1/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 14:10:33.031947 const_cython_lib-0.3.1/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      376 2023-06-12 13:33:19.000000 const_cython_lib-0.3.1/setup.py
```

### Comparing `const_cython_lib-0.3.0/const_cython_lib/lsum.c` & `const_cython_lib-0.3.1/const_cython_lib/lsum.c`

 * *Files 1% similar despite different names*

```diff
@@ -1164,15 +1164,15 @@
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'const_cython_lib' */
-__PYX_EXTERN_C PyObject *lsum(int const , int const ); /*proto*/
+__PYX_EXTERN_C PyObject *lsum(int, int); /*proto*/
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
 
 /* "const_cython_lib/lsum.pyx":1
- * cdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
+ * cdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
-PyObject *lsum(int const __pyx_v_a, int const __pyx_v_b) {
+PyObject *lsum(int __pyx_v_a, int __pyx_v_b) {
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
   __Pyx_AddTraceback("const_cython_lib.lsum", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -1556,15 +1556,15 @@
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

### Comparing `const_cython_lib-0.3.0/const_cython_lib/lsum.h` & `const_cython_lib-0.3.1/const_cython_lib/lsum.h`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   #endif
 #endif
 
 #ifndef DL_IMPORT
   #define DL_IMPORT(_T) _T
 #endif
 
-__PYX_EXTERN_C PyObject *lsum(int const , int const );
+__PYX_EXTERN_C PyObject *lsum(int, int);
 
 #endif /* !__PYX_HAVE_API__const_cython_lib */
 
 /* WARNING: the interface of the module init function changed in CPython 3.5. */
 /* It now returns a PyModuleDef instance instead of a PyModule instance. */
 
 #if PY_MAJOR_VERSION < 3
```

