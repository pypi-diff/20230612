# Comparing `tmp/nerotest-0.0.0.1-py3-none-any.whl.zip` & `tmp/nerotest-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1643 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      106 b- defN 23-Jun-12 07:47 nerotest/test1.py
--rw-rw-rw-  2.0 fat      138 b- defN 23-Jun-12 07:48 nerotest/test2.py
--rw-rw-rw-  2.0 fat      242 b- defN 23-Jun-12 08:24 nerotest-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:24 nerotest-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-12 08:24 nerotest-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      455 b- defN 23-Jun-12 08:24 nerotest-0.0.0.1.dist-info/RECORD
-6 files, 1059 bytes uncompressed, 817 bytes compressed:  22.9%
+Zip file size: 1645 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jun-12 08:44 nerotest/test1.py
+-rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-12 08:44 nerotest/test2.py
+-rw-rw-rw-  2.0 fat      242 b- defN 23-Jun-12 08:45 nerotest-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:45 nerotest-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-12 08:45 nerotest-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      455 b- defN 23-Jun-12 08:45 nerotest-0.0.0.2.dist-info/RECORD
+6 files, 1061 bytes uncompressed, 819 bytes compressed:  22.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: nerotest/test1.py
 Comment: 
 
 Filename: nerotest/test2.py
 Comment: 
 
-Filename: nerotest-0.0.0.1.dist-info/METADATA
+Filename: nerotest-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: nerotest-0.0.0.1.dist-info/WHEEL
+Filename: nerotest-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: nerotest-0.0.0.1.dist-info/top_level.txt
+Filename: nerotest-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: nerotest-0.0.0.1.dist-info/RECORD
+Filename: nerotest-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nerotest/test1.py

```diff
@@ -1,3 +1,3 @@
 def print_test1():
     '''테스트 문장을 출력합니다'''
-    print("Hi, This is test1.py page!")
+    print("Hi, This is test1.py page!d")
```

## nerotest/test2.py

```diff
@@ -1,3 +1,3 @@
 def print_test2():
       '''테스트 문장을 출력합니다'''
-      print("안녕하세요, 이것은 test2.py 페이지입니다")
+      print("안녕하세요, 이것은 test2.py 페이지입니다d")
```

