# Comparing `tmp/dwiqc-0.4.1-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.4.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24428 bytes, number of entries: 22
+Zip file size: 24427 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-Jun-08 18:05 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 14:19 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 14:28 dwiqc/__version__.py
 -rw-r--r--  2.0 unx     1352 b- defN 23-Jun-08 18:05 dwiqc/browser/__init__.py
--rw-r--r--  2.0 unx       62 b- defN 23-Jun-08 18:05 dwiqc/cli/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-12 14:27 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-Jun-08 18:05 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5989 b- defN 23-Jun-08 18:05 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     3731 b- defN 23-Jun-08 18:05 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-08 18:05 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jun-08 18:05 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jun-08 18:05 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jun-08 18:05 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    10168 b- defN 23-Jun-08 18:05 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4415 b- defN 23-Jun-08 18:05 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6146 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13083 b- defN 23-Jun-08 18:05 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5781 b- defN 23-Jun-12 14:21 dwiqc-0.4.1.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-12 14:21 dwiqc-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      428 b- defN 23-Jun-12 14:21 dwiqc-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-12 14:21 dwiqc-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-12 14:21 dwiqc-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-12 14:21 dwiqc-0.4.1.dist-info/RECORD
-22 files, 67949 bytes uncompressed, 21676 bytes compressed:  68.1%
+-rwxr-xr-x  2.0 unx     5781 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      428 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/RECORD
+22 files, 67948 bytes uncompressed, 21675 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.4.1.data/scripts/dwiQC.py
+Filename: dwiqc-0.4.2.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.4.1.dist-info/LICENSE
+Filename: dwiqc-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.4.1.dist-info/METADATA
+Filename: dwiqc-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.4.1.dist-info/WHEEL
+Filename: dwiqc-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.4.1.dist-info/top_level.txt
+Filename: dwiqc-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.4.1.dist-info/RECORD
+Filename: dwiqc-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/cli/__init__.py

```diff
@@ -1,3 +1,3 @@
 from . import get
 from . import process
-#from . import tandem
+from . import tandem
```

## Comparing `dwiqc-0.4.1.data/scripts/dwiQC.py` & `dwiqc-0.4.2.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.4.1.dist-info/LICENSE` & `dwiqc-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.4.1.dist-info/RECORD` & `dwiqc-0.4.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=-kADW4UDYmZNachSLIvMP9VmEM8moVlBPdQ4i4GcXw0,247
+dwiqc/__version__.py,sha256=noxzUrjYFz5OSiFqcXq8EZygunPEV5GAByEnrmF8Qy4,247
 dwiqc/browser/__init__.py,sha256=4lK-1-VH4l6ppP_5Ju6MeYIctiQmFQfGA7gclqh8euE,1352
-dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
+dwiqc/cli/__init__.py,sha256=1Y4dYEbkHH-jZ3cwbFnlb6TthH_K0t4xT_-IphRBu6k,61
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=BNKCLSHtJSM--sslUHJhmjhL4bCVKnJ-oZ210DO9wns,5989
 dwiqc/cli/tandem.py,sha256=Ir_g60_WTHGbwv5dLPOs3MeTJO985vC5YcjScHdVFf0,3731
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=jQsq46tK9UdCtKW7iqh2VD9JsA3BKZ7Pp4pzCBCt0hM,10168
 dwiqc/tasks/prequal_EQ.py,sha256=vWtvf0BDuV70c7ibdFPwkoUPqr0I78599e8USO1F0jA,4415
 dwiqc/tasks/qsiprep.py,sha256=CWalSV29PeSXhPANLR6MQiH6eAAFaaN6PxDITnTZ3Pw,6146
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=HDjDNAQVSzr_e_ySPF_0vGHE5GjIWKXO7bv8ka4whm4,13083
-dwiqc-0.4.1.data/scripts/dwiQC.py,sha256=dnECv98OfKb6nj_kgS72vCge7VWaX6uhY0Ro0Qu2UZQ,5781
-dwiqc-0.4.1.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.4.1.dist-info/METADATA,sha256=1unBW9ptm3zsdznArUSf8YrGd-xsbAf2ouq3GmcZjEc,428
-dwiqc-0.4.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-dwiqc-0.4.1.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.4.1.dist-info/RECORD,,
+dwiqc-0.4.2.data/scripts/dwiQC.py,sha256=dnECv98OfKb6nj_kgS72vCge7VWaX6uhY0Ro0Qu2UZQ,5781
+dwiqc-0.4.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.4.2.dist-info/METADATA,sha256=mz0l7SvKTHI0gOy_sa0miFbdAvP01YnneuVANtPlzFw,428
+dwiqc-0.4.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.4.2.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.4.2.dist-info/RECORD,,
```

