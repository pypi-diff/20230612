# Comparing `tmp/vios-0.0.0-py3-none-win_amd64.whl.zip` & `tmp/vios-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,28 @@
-Zip file size: 1789 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1272 b- defN 21-Nov-19 00:27 vios-0.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 21-Nov-19 00:27 vios-0.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       95 b- defN 21-Nov-19 00:27 vios-0.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 21-Nov-19 00:27 vios-0.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      377 b- defN 21-Nov-19 00:27 vios-0.0.0.dist-info/RECORD
-5 files, 1843 bytes uncompressed, 1081 bytes compressed:  41.3%
+Zip file size: 42893 bytes, number of entries: 26
+-rw-rw-rw-  2.0 fat     3944 b- defN 23-May-29 01:06 vios/__init__.py
+-rw-rw-rw-  2.0 fat     4867 b- defN 23-Jun-08 02:11 vios/collection/__init__.py
+-rw-rw-rw-  2.0 fat     1913 b- defN 23-Jun-08 02:06 vios/collection/analyzer.py
+-rw-rw-rw-  2.0 fat    11254 b- defN 23-Jun-08 02:06 vios/collection/experiment.py
+-rw-rw-rw-  2.0 fat    11189 b- defN 23-Jun-12 00:16 vios/collection/qcloud.py
+-rw-rw-rw-  2.0 fat     3527 b- defN 23-Jun-08 02:06 vios/collection/support.py
+-rw-rw-rw-  2.0 fat    10232 b- defN 23-Jun-08 02:06 vios/collection/uapi.py
+-rw-rw-rw-  2.0 fat     4756 b- defN 23-Jun-12 00:16 vios/driver/VirtualDevice.py
+-rw-rw-rw-  2.0 fat     2962 b- defN 23-Jun-08 02:11 vios/driver/__init__.py
+-rw-rw-rw-  2.0 fat      238 b- defN 23-Jun-08 02:11 vios/driver/common/__init__.py
+-rw-rw-rw-  2.0 fat     4199 b- defN 23-Jun-08 02:11 vios/driver/common/basedriver.py
+-rw-rw-rw-  2.0 fat     4666 b- defN 23-Jun-08 02:11 vios/driver/common/quantity.py
+-rw-rw-rw-  2.0 fat    17014 b- defN 23-Jun-08 02:11 vios/driver/common/tek_seq_builder.py
+-rw-rw-rw-  2.0 fat     1752 b- defN 23-Jun-08 02:11 vios/driver/common/utils.py
+-rw-rw-rw-  2.0 fat     5546 b- defN 23-Jun-08 02:11 vios/driver/common/visadriver.py
+-rw-rw-rw-  2.0 fat     1639 b- defN 23-Jun-08 02:11 vios/envelope/__init__.py
+-rw-rw-rw-  2.0 fat    10536 b- defN 23-Jun-12 00:16 vios/envelope/calculator.py
+-rw-rw-rw-  2.0 fat     2530 b- defN 23-Jun-12 00:16 vios/envelope/compiler.py
+-rw-rw-rw-  2.0 fat     4066 b- defN 23-Jun-12 00:16 vios/envelope/demodulator.py
+-rw-rw-rw-  2.0 fat     1047 b- defN 23-Mar-08 06:14 vios/envelope/device.py
+-rw-rw-rw-  2.0 fat     4093 b- defN 23-Jun-08 02:11 vios/envelope/rule.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-12 02:21 vios-1.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      879 b- defN 23-Jun-12 02:21 vios-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 02:21 vios-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jun-12 02:21 vios-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2131 b- defN 23-Jun-12 02:21 vios-1.0.0.dist-info/RECORD
+26 files, 116166 bytes uncompressed, 39485 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,16 +1,79 @@
-Filename: vios-0.0.0.dist-info/METADATA
+Filename: vios/__init__.py
 Comment: 
 
-Filename: vios-0.0.0.dist-info/WHEEL
+Filename: vios/collection/__init__.py
 Comment: 
 
-Filename: vios-0.0.0.dist-info/entry_points.txt
+Filename: vios/collection/analyzer.py
 Comment: 
 
-Filename: vios-0.0.0.dist-info/top_level.txt
+Filename: vios/collection/experiment.py
 Comment: 
 
-Filename: vios-0.0.0.dist-info/RECORD
+Filename: vios/collection/qcloud.py
+Comment: 
+
+Filename: vios/collection/support.py
+Comment: 
+
+Filename: vios/collection/uapi.py
+Comment: 
+
+Filename: vios/driver/VirtualDevice.py
+Comment: 
+
+Filename: vios/driver/__init__.py
+Comment: 
+
+Filename: vios/driver/common/__init__.py
+Comment: 
+
+Filename: vios/driver/common/basedriver.py
+Comment: 
+
+Filename: vios/driver/common/quantity.py
+Comment: 
+
+Filename: vios/driver/common/tek_seq_builder.py
+Comment: 
+
+Filename: vios/driver/common/utils.py
+Comment: 
+
+Filename: vios/driver/common/visadriver.py
+Comment: 
+
+Filename: vios/envelope/__init__.py
+Comment: 
+
+Filename: vios/envelope/calculator.py
+Comment: 
+
+Filename: vios/envelope/compiler.py
+Comment: 
+
+Filename: vios/envelope/demodulator.py
+Comment: 
+
+Filename: vios/envelope/device.py
+Comment: 
+
+Filename: vios/envelope/rule.py
+Comment: 
+
+Filename: vios-1.0.0.dist-info/LICENSE
+Comment: 
+
+Filename: vios-1.0.0.dist-info/METADATA
+Comment: 
+
+Filename: vios-1.0.0.dist-info/WHEEL
+Comment: 
+
+Filename: vios-1.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: vios-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

