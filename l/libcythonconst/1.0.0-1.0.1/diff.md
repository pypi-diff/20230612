# Comparing `tmp/libcythonconst-1.0.0.tar.gz` & `tmp/libcythonconst-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcythonconst-1.0.0.tar", last modified: Mon Jun 12 17:02:53 2023, max compression
+gzip compressed data, was "libcythonconst-1.0.1.tar", last modified: Mon Jun 12 17:03:57 2023, max compression
```

## Comparing `libcythonconst-1.0.0.tar` & `libcythonconst-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:02:53.529199 libcythonconst-1.0.0/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      131 2023-06-12 17:02:53.529075 libcythonconst-1.0.0/PKG-INFO
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:02:53.528209 libcythonconst-1.0.0/libcythonconst/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 16:42:30.000000 libcythonconst-1.0.0/libcythonconst/__init__.py
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   110930 2023-06-12 17:02:53.000000 libcythonconst-1.0.0/libcythonconst/lsum.c
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      813 2023-06-12 17:02:53.000000 libcythonconst-1.0.0/libcythonconst/lsum.h
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       31 2023-06-12 17:02:49.000000 libcythonconst-1.0.0/libcythonconst/lsum.pxd
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       49 2023-06-12 17:02:49.000000 libcythonconst-1.0.0/libcythonconst/lsum.pyx
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:02:53.528889 libcythonconst-1.0.0/libcythonconst.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      131 2023-06-12 17:02:53.000000 libcythonconst-1.0.0/libcythonconst.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      331 2023-06-12 17:02:53.000000 libcythonconst-1.0.0/libcythonconst.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 17:02:53.000000 libcythonconst-1.0.0/libcythonconst.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 17:02:53.000000 libcythonconst-1.0.0/libcythonconst.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       15 2023-06-12 17:02:53.000000 libcythonconst-1.0.0/libcythonconst.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      227 2023-06-12 17:01:56.000000 libcythonconst-1.0.0/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 17:02:53.529240 libcythonconst-1.0.0/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      375 2023-06-12 17:01:44.000000 libcythonconst-1.0.0/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:03:57.774759 libcythonconst-1.0.1/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      131 2023-06-12 17:03:57.774624 libcythonconst-1.0.1/PKG-INFO
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:03:57.773791 libcythonconst-1.0.1/libcythonconst/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 16:42:30.000000 libcythonconst-1.0.1/libcythonconst/__init__.py
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   111018 2023-06-12 17:03:57.000000 libcythonconst-1.0.1/libcythonconst/lsum.c
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      827 2023-06-12 17:03:57.000000 libcythonconst-1.0.1/libcythonconst/lsum.h
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       43 2023-06-12 17:03:53.000000 libcythonconst-1.0.1/libcythonconst/lsum.pxd
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       61 2023-06-12 17:03:53.000000 libcythonconst-1.0.1/libcythonconst/lsum.pyx
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:03:57.774440 libcythonconst-1.0.1/libcythonconst.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      131 2023-06-12 17:03:57.000000 libcythonconst-1.0.1/libcythonconst.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      331 2023-06-12 17:03:57.000000 libcythonconst-1.0.1/libcythonconst.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 17:03:57.000000 libcythonconst-1.0.1/libcythonconst.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 17:02:53.000000 libcythonconst-1.0.1/libcythonconst.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       15 2023-06-12 17:03:57.000000 libcythonconst-1.0.1/libcythonconst.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      227 2023-06-12 17:03:53.000000 libcythonconst-1.0.1/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 17:03:57.774801 libcythonconst-1.0.1/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      375 2023-06-12 17:01:44.000000 libcythonconst-1.0.1/setup.py
```

### Comparing `libcythonconst-1.0.0/libcythonconst/lsum.c` & `libcythonconst-1.0.1/libcythonconst/lsum.c`

 * *Files 0% similar despite different names*

```diff
@@ -1167,15 +1167,15 @@
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'libcythonconst.lsum' */
-__PYX_EXTERN_C PyObject *__pyx_f_14libcythonconst_4lsum_lsum(int, int); /*proto*/
+__PYX_EXTERN_C PyObject *__pyx_f_14libcythonconst_4lsum_lsum(int const , int const ); /*proto*/
 #define __Pyx_MODULE_NAME "libcythonconst.lsum"
 extern int __pyx_module_is_main_libcythonconst__lsum;
 int __pyx_module_is_main_libcythonconst__lsum = 0;
 
 /* Implementation of 'libcythonconst.lsum' */
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -1184,40 +1184,40 @@
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_test;
 /* Late includes */
 
 /* "libcythonconst/lsum.pyx":1
- * cdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
+ * cdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
-PyObject *__pyx_f_14libcythonconst_4lsum_lsum(int __pyx_v_a, int __pyx_v_b) {
+PyObject *__pyx_f_14libcythonconst_4lsum_lsum(int const __pyx_v_a, int const __pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lsum", 0);
 
   /* "libcythonconst/lsum.pyx":2
- * cdef public lsum(int a, int b):
+ * cdef public lsum(const int a, const int b):
  *     return a + b             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_a + __pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "libcythonconst/lsum.pyx":1
- * cdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
+ * cdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("libcythonconst.lsum.lsum", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -1325,15 +1325,15 @@
 static int __Pyx_modinit_function_export_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
-  if (__Pyx_ExportFunction("lsum", (void (*)(void))__pyx_f_14libcythonconst_4lsum_lsum, "PyObject *(int, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("lsum", (void (*)(void))__pyx_f_14libcythonconst_4lsum_lsum, "PyObject *(int const , int const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
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
 
   /* "libcythonconst/lsum.pyx":1
- * cdef public lsum(int a, int b):             # <<<<<<<<<<<<<<
+ * cdef public lsum(const int a, const int b):             # <<<<<<<<<<<<<<
  *     return a + b
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `libcythonconst-1.0.0/libcythonconst/lsum.h` & `libcythonconst-1.0.1/libcythonconst/lsum.h`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   #endif
 #endif
 
 #ifndef DL_IMPORT
   #define DL_IMPORT(_T) _T
 #endif
 
-__PYX_EXTERN_C PyObject *__pyx_f_14libcythonconst_4lsum_lsum(int, int);
+__PYX_EXTERN_C PyObject *__pyx_f_14libcythonconst_4lsum_lsum(int const , int const );
 
 #endif /* !__PYX_HAVE_API__libcythonconst__lsum */
 
 /* WARNING: the interface of the module init function changed in CPython 3.5. */
 /* It now returns a PyModuleDef instance instead of a PyModule instance. */
 
 #if PY_MAJOR_VERSION < 3
```

