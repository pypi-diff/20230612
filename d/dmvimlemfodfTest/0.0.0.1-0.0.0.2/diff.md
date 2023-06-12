# Comparing `tmp/dmvimlemfodfTest-0.0.0.1-py3-none-any.whl.zip` & `tmp/dmvimlemfodfTest-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 1735 bytes, number of entries: 6
+Zip file size: 2169 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      446 b- defN 23-Jun-12 08:45 dmvimlemfodfTest/BMI_test.py
 -rw-rw-rw-  2.0 fat      105 b- defN 23-Jun-12 07:44 dmvimlemfodfTest/test1.py
--rw-rw-rw-  2.0 fat      134 b- defN 23-Jun-12 07:45 dmvimlemfodfTest/test2.py
--rw-rw-rw-  2.0 fat      223 b- defN 23-Jun-12 08:02 dmvimlemfodfTest-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:02 dmvimlemfodfTest-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       29 b- defN 23-Jun-12 08:02 dmvimlemfodfTest-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      503 b- defN 23-Jun-12 08:02 dmvimlemfodfTest-0.0.0.1.dist-info/RECORD
-6 files, 1091 bytes uncompressed, 813 bytes compressed:  25.5%
+-rw-rw-rw-  2.0 fat      158 b- defN 23-Jun-12 08:36 dmvimlemfodfTest/test2.py
+-rw-rw-rw-  2.0 fat      223 b- defN 23-Jun-12 08:49 dmvimlemfodfTest-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:49 dmvimlemfodfTest-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       32 b- defN 23-Jun-12 08:49 dmvimlemfodfTest-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      587 b- defN 23-Jun-12 08:49 dmvimlemfodfTest-0.0.0.2.dist-info/RECORD
+7 files, 1648 bytes uncompressed, 1115 bytes compressed:  32.3%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
+Filename: dmvimlemfodfTest/BMI_test.py
+Comment: 
+
 Filename: dmvimlemfodfTest/test1.py
 Comment: 
 
 Filename: dmvimlemfodfTest/test2.py
 Comment: 
 
-Filename: dmvimlemfodfTest-0.0.0.1.dist-info/METADATA
+Filename: dmvimlemfodfTest-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: dmvimlemfodfTest-0.0.0.1.dist-info/WHEEL
+Filename: dmvimlemfodfTest-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: dmvimlemfodfTest-0.0.0.1.dist-info/top_level.txt
+Filename: dmvimlemfodfTest-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dmvimlemfodfTest-0.0.0.1.dist-info/RECORD
+Filename: dmvimlemfodfTest-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dmvimlemfodfTest/test2.py

```diff
@@ -1,3 +1,5 @@
 def print_test2():
     '''테스트 문장을 출력합니다'''
-    print('안녕하세요, 이것은 test2.py 페이지입니다')
+    print('안녕하세요, 이것은 test2.py 페이지입니다')
+
+print(print_test2())
```

