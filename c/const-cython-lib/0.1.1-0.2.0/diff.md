# Comparing `tmp/const_cython_lib-0.1.1.tar.gz` & `tmp/const_cython_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "const_cython_lib-0.1.1.tar", last modified: Mon Jun 12 12:03:07 2023, max compression
+gzip compressed data, was "const_cython_lib-0.2.0.tar", last modified: Mon Jun 12 13:07:55 2023, max compression
```

## Comparing `const_cython_lib-0.1.1.tar` & `const_cython_lib-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 12:03:07.684636 const_cython_lib-0.1.1/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 12:03:07.684486 const_cython_lib-0.1.1/PKG-INFO
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 12:03:07.683521 const_cython_lib-0.1.1/const_cython_lib/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   119108 2023-06-12 12:03:07.000000 const_cython_lib-0.1.1/const_cython_lib/lsum.c
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      811 2023-06-12 12:03:07.000000 const_cython_lib-0.1.1/const_cython_lib/lsum.h
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       32 2023-06-12 12:02:49.000000 const_cython_lib-0.1.1/const_cython_lib/lsum.pxd
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       50 2023-06-12 12:02:55.000000 const_cython_lib-0.1.1/const_cython_lib/lsum.pyx
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 12:03:07.684266 const_cython_lib-0.1.1/const_cython_lib.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 12:03:07.000000 const_cython_lib-0.1.1/const_cython_lib.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      322 2023-06-12 12:03:07.000000 const_cython_lib-0.1.1/const_cython_lib.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 12:03:07.000000 const_cython_lib-0.1.1/const_cython_lib.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 11:52:57.000000 const_cython_lib-0.1.1/const_cython_lib.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 12:03:07.000000 const_cython_lib-0.1.1/const_cython_lib.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 12:03:00.000000 const_cython_lib-0.1.1/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 12:03:07.684679 const_cython_lib-0.1.1/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      364 2023-06-12 11:52:46.000000 const_cython_lib-0.1.1/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 13:07:55.873531 const_cython_lib-0.2.0/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 13:07:55.873400 const_cython_lib-0.2.0/PKG-INFO
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 13:07:55.872511 const_cython_lib-0.2.0/const_cython_lib/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 13:06:05.000000 const_cython_lib-0.2.0/const_cython_lib/__init__.py
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   119182 2023-06-12 13:07:55.000000 const_cython_lib-0.2.0/const_cython_lib/lsum.c
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      825 2023-06-12 13:07:55.000000 const_cython_lib-0.2.0/const_cython_lib/lsum.h
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       44 2023-06-12 13:06:21.000000 const_cython_lib-0.2.0/const_cython_lib/lsum.pxd
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       62 2023-06-12 12:53:28.000000 const_cython_lib-0.2.0/const_cython_lib/lsum.pyx
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 13:07:55.873201 const_cython_lib-0.2.0/const_cython_lib.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      133 2023-06-12 13:07:55.000000 const_cython_lib-0.2.0/const_cython_lib.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      351 2023-06-12 13:07:55.000000 const_cython_lib-0.2.0/const_cython_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 13:07:55.000000 const_cython_lib-0.2.0/const_cython_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 13:07:55.000000 const_cython_lib-0.2.0/const_cython_lib.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       17 2023-06-12 13:07:55.000000 const_cython_lib-0.2.0/const_cython_lib.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      229 2023-06-12 12:53:13.000000 const_cython_lib-0.2.0/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 13:07:55.873689 const_cython_lib-0.2.0/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      367 2023-06-12 13:07:46.000000 const_cython_lib-0.2.0/setup.py
```

### Comparing `const_cython_lib-0.1.1/const_cython_lib/lsum.c` & `const_cython_lib-0.2.0/const_cython_lib/lsum.c`

 * *Files 0% similar despite different names*

```diff
@@ -1176,15 +1176,15 @@
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'const_cython_lib' */
-__PYX_EXTERN_C PyObject *lsum(int, int, int __pyx_skip_dispatch); /*proto*/
+__PYX_EXTERN_C PyObject *lsum(int const , int const , int __pyx_skip_dispatch); /*proto*/
 #define __Pyx_MODULE_NAME "const_cython_lib"
 extern int __pyx_module_is_main_const_cython_lib;
 int __pyx_module_is_main_const_cython_lib = 0;
 
 /* Implementation of 'const_cython_lib' */
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
@@ -1198,41 +1198,41 @@
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_pf_16const_cython_lib_lsum(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b); /* proto */
 /* Late includes */
 
 /* "const_cython_lib/lsum.pyx":1
- * cpdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
+ * cpdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
 static PyObject *__pyx_pw_16const_cython_lib_1lsum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-PyObject *lsum(int __pyx_v_a, int __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
+PyObject *lsum(int const __pyx_v_a, int const __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lsum", 0);
 
   /* "const_cython_lib/lsum.pyx":2
- * cpdef public lsum(int a, int b):
+ * cpdef public lsum(const int a, const int b):
  *     return a + b             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_a + __pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "const_cython_lib/lsum.pyx":1
- * cpdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
+ * cpdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("const_cython_lib.lsum", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -1667,15 +1667,15 @@
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "const_cython_lib/lsum.pyx":1
- * cpdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
+ * cpdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `const_cython_lib-0.1.1/const_cython_lib/lsum.h` & `const_cython_lib-0.2.0/const_cython_lib/lsum.h`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   #endif
 #endif
 
 #ifndef DL_IMPORT
   #define DL_IMPORT(_T) _T
 #endif
 
-__PYX_EXTERN_C PyObject *lsum(int, int, int __pyx_skip_dispatch);
+__PYX_EXTERN_C PyObject *lsum(int const , int const , int __pyx_skip_dispatch);
 
 #endif /* !__PYX_HAVE_API__const_cython_lib */
 
 /* WARNING: the interface of the module init function changed in CPython 3.5. */
 /* It now returns a PyModuleDef instance instead of a PyModule instance. */
 
 #if PY_MAJOR_VERSION < 3
```

