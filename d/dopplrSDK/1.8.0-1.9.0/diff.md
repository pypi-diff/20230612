# Comparing `tmp/dopplrSDK-1.8.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 3788 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     4924 b- defN 23-May-22 10:45 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-May-22 10:46 dopplrSDK-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      457 b- defN 23-May-22 10:46 dopplrSDK-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 10:46 dopplrSDK-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-22 10:46 dopplrSDK-1.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      477 b- defN 23-May-22 10:46 dopplrSDK-1.8.0.dist-info/RECORD
+-rw-rw-rw-  2.0 fat     4924 b- defN 23-Jun-12 13:28 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      457 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      477 b- defN 23-Jun-12 13:30 dopplrSDK-1.9.0.dist-info/RECORD
 6 files, 7037 bytes uncompressed, 2922 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-1.8.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-1.8.0.dist-info/METADATA
+Filename: dopplrSDK-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-1.8.0.dist-info/WHEEL
+Filename: dopplrSDK-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-1.8.0.dist-info/top_level.txt
+Filename: dopplrSDK-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-1.8.0.dist-info/RECORD
+Filename: dopplrSDK-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -7,15 +7,15 @@
 
 
 
 def putFileTomywrkspace(filePath,file_type,loginName):
     try:
         query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
         #print(query)
-        cnxn = psycopg2.connect(host='adf25b06d0e0d4d5aa6541ae233b7cc8-1562418356.ap-south-1.elb.amazonaws.com',database='Dopplr',user='postgres',password='SystechIndia@123',port='5432')
+        cnxn = psycopg2.connect(host='adb63cdf19ef14e14b3e7ffd2c4bd4e3-1623479541.ap-south-1.elb.amazonaws.com',database='Dopplr',user='postgres',password='SystechIndia@123',port='5432')
 
         cur=cnxn.cursor()
         cur.execute(query)
         results = cur.fetchone()
         
 
         ContainerName=results[2]
@@ -78,15 +78,15 @@
     #type = 2 then get file* (file pattern)
 
 
     #destination = "/data"
     folder_prefix = 'Systech/'+loginName.upper()+'/'
     query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
 
-    cnxn = psycopg2.connect(host='adf25b06d0e0d4d5aa6541ae233b7cc8-1562418356.ap-south-1.elb.amazonaws.com',database='Dopplr',user='postgres',password='SystechIndia@123',port='5432')
+    cnxn = psycopg2.connect(host='adb63cdf19ef14e14b3e7ffd2c4bd4e3-1623479541.ap-south-1.elb.amazonaws.com',database='Dopplr',user='postgres',password='SystechIndia@123',port='5432')
 
     cur=cnxn.cursor()
     cur.execute(query)
     results = cur.fetchone()
         
 
     ContainerName=results[2]
```

## Comparing `dopplrSDK-1.8.0.dist-info/LICENSE.txt` & `dopplrSDK-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

