# Comparing `tmp/dwiqc-0.4.4-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.4.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24440 bytes, number of entries: 22
+Zip file size: 24431 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-Jun-08 18:05 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 19:02 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 20:46 dwiqc/__version__.py
 -rw-r--r--  2.0 unx     1352 b- defN 23-Jun-08 18:05 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       61 b- defN 23-Jun-12 14:27 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-Jun-08 18:05 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5989 b- defN 23-Jun-08 18:05 dwiqc/cli/process.py
--rw-r--r--  2.0 unx     3819 b- defN 23-Jun-12 19:02 dwiqc/cli/tandem.py
+-rw-r--r--  2.0 unx     3801 b- defN 23-Jun-12 20:46 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-08 18:05 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jun-08 18:05 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jun-08 18:05 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jun-08 18:05 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    10168 b- defN 23-Jun-08 18:05 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4415 b- defN 23-Jun-08 18:05 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6146 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13083 b- defN 23-Jun-08 18:05 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5781 b- defN 23-Jun-12 19:03 dwiqc-0.4.4.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-12 19:03 dwiqc-0.4.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      428 b- defN 23-Jun-12 19:03 dwiqc-0.4.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-12 19:03 dwiqc-0.4.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-12 19:03 dwiqc-0.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-12 19:03 dwiqc-0.4.4.dist-info/RECORD
-22 files, 68036 bytes uncompressed, 21688 bytes compressed:  68.1%
+-rwxr-xr-x  2.0 unx     5781 b- defN 23-Jun-12 20:48 dwiqc-0.4.5.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-12 20:48 dwiqc-0.4.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      428 b- defN 23-Jun-12 20:48 dwiqc-0.4.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-12 20:48 dwiqc-0.4.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-12 20:48 dwiqc-0.4.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-12 20:48 dwiqc-0.4.5.dist-info/RECORD
+22 files, 68018 bytes uncompressed, 21679 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.4.4.data/scripts/dwiQC.py
+Filename: dwiqc-0.4.5.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.4.4.dist-info/LICENSE
+Filename: dwiqc-0.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.4.4.dist-info/METADATA
+Filename: dwiqc-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.4.4.dist-info/WHEEL
+Filename: dwiqc-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.4.4.dist-info/top_level.txt
+Filename: dwiqc-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.4.4.dist-info/RECORD
+Filename: dwiqc-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.4.4'
+__version__ = '0.4.5'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/cli/tandem.py

```diff
@@ -90,16 +90,16 @@
             logger.info('getting anat run=%s, scan=%s', run, scansr['anat'])
             get.get_anat(args, auth, run, scansr['anat'], verbose=args.verbose)
 
     # populate the necessary arguments for process, then call process
         args.run = int(run)
         bids_ses_label = yaxil.bids.legal.sub('', args.label)
         bids_sub_label = yaxil.bids.legal.sub('', subject_label)
-        args.sub = 'sub-' + bids_sub_label
-        args.ses = 'ses-' + bids_ses_label
+        args.sub = bids_sub_label
+        args.ses = bids_ses_label
         logger.debug('sub=%s, ses=%s', args.sub, args.ses)
         process.do(args)
 
 
 def match(note, patterns):
     for pattern in patterns:
         m = re.match(pattern, note, flags=re.IGNORECASE)
```

## Comparing `dwiqc-0.4.4.data/scripts/dwiQC.py` & `dwiqc-0.4.5.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.4.4.dist-info/LICENSE` & `dwiqc-0.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.4.4.dist-info/RECORD` & `dwiqc-0.4.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=ImYXrkacGI9Pld5phwe6Rv_MCN5okJMyCTC5pIK5e-s,247
+dwiqc/__version__.py,sha256=Lac-wG0xy9NcC-qS8LOKHwHjlBwjBRzIqUQSuVQu-Q8,247
 dwiqc/browser/__init__.py,sha256=4lK-1-VH4l6ppP_5Ju6MeYIctiQmFQfGA7gclqh8euE,1352
 dwiqc/cli/__init__.py,sha256=1Y4dYEbkHH-jZ3cwbFnlb6TthH_K0t4xT_-IphRBu6k,61
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=BNKCLSHtJSM--sslUHJhmjhL4bCVKnJ-oZ210DO9wns,5989
-dwiqc/cli/tandem.py,sha256=a-XNeXkrA_2_K6rsRN4kBoH8J6jvipaThM7iuani1tA,3819
+dwiqc/cli/tandem.py,sha256=aB2uJN6X6aJWXT_JtL6U_Lj7ljItplFU8sVFnfpmrfA,3801
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=jQsq46tK9UdCtKW7iqh2VD9JsA3BKZ7Pp4pzCBCt0hM,10168
 dwiqc/tasks/prequal_EQ.py,sha256=vWtvf0BDuV70c7ibdFPwkoUPqr0I78599e8USO1F0jA,4415
 dwiqc/tasks/qsiprep.py,sha256=CWalSV29PeSXhPANLR6MQiH6eAAFaaN6PxDITnTZ3Pw,6146
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=HDjDNAQVSzr_e_ySPF_0vGHE5GjIWKXO7bv8ka4whm4,13083
-dwiqc-0.4.4.data/scripts/dwiQC.py,sha256=dnECv98OfKb6nj_kgS72vCge7VWaX6uhY0Ro0Qu2UZQ,5781
-dwiqc-0.4.4.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.4.4.dist-info/METADATA,sha256=xZe5_qRLXe-Y4DAWETGMM_YpNJgGaoBMrk8yeufql8U,428
-dwiqc-0.4.4.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.4.4.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.4.4.dist-info/RECORD,,
+dwiqc-0.4.5.data/scripts/dwiQC.py,sha256=dnECv98OfKb6nj_kgS72vCge7VWaX6uhY0Ro0Qu2UZQ,5781
+dwiqc-0.4.5.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.4.5.dist-info/METADATA,sha256=B8ujaQMT3A77JaakPEDJ09680uFT2RBz2yOvtoHPiPU,428
+dwiqc-0.4.5.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.4.5.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.4.5.dist-info/RECORD,,
```

