# Comparing `tmp/hcv_api-0.0.3-py3-none-any.whl.zip` & `tmp/hcv_api-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3593 bytes, number of entries: 8
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-11 18:47 vapi/__init__.py
--rw-r--r--  2.0 unx      367 b- defN 23-Jun-11 18:47 vapi/exceptions.py
--rw-r--r--  2.0 unx     4745 b- defN 23-Jun-11 18:47 vapi/vapi.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-11 18:48 hcv_api-0.0.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      192 b- defN 23-Jun-11 18:48 hcv_api-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 18:48 hcv_api-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-11 18:48 hcv_api-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      601 b- defN 23-Jun-11 18:48 hcv_api-0.0.3.dist-info/RECORD
-8 files, 7112 bytes uncompressed, 2547 bytes compressed:  64.2%
+Zip file size: 3592 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-12 01:38 vapi/__init__.py
+-rw-r--r--  2.0 unx      367 b- defN 23-Jun-12 01:38 vapi/exceptions.py
+-rw-r--r--  2.0 unx     4760 b- defN 23-Jun-12 01:38 vapi/vapi.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-12 01:39 hcv_api-0.0.4.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      192 b- defN 23-Jun-12 01:39 hcv_api-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 01:39 hcv_api-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-12 01:39 hcv_api-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      601 b- defN 23-Jun-12 01:39 hcv_api-0.0.4.dist-info/RECORD
+8 files, 7127 bytes uncompressed, 2546 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vapi/exceptions.py
 Comment: 
 
 Filename: vapi/vapi.py
 Comment: 
 
-Filename: hcv_api-0.0.3.dist-info/LICENSE.md
+Filename: hcv_api-0.0.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: hcv_api-0.0.3.dist-info/METADATA
+Filename: hcv_api-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: hcv_api-0.0.3.dist-info/WHEEL
+Filename: hcv_api-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: hcv_api-0.0.3.dist-info/top_level.txt
+Filename: hcv_api-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hcv_api-0.0.3.dist-info/RECORD
+Filename: hcv_api-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vapi/vapi.py

```diff
@@ -101,35 +101,35 @@
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
 
     def list(self, path, raw=False, accepted_status_codes=[204, 200]):
-        headers = _set_headers()
+        headers = self._set_headers()
         url = self._format_url(path)
         response = requests.get(url, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
 
     def post(self, path, data={}, raw=False, accepted_status_codes=[204, 200]):
-        headers = _set_headers()
+        headers = self._set_headers()
         url = self._format_url(path)
         response = requests.post(url, json=data, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
 
     def delete(self, path, raw=False, accepted_status_codes=[204, 200]):
-        headers = _set_headers()
+        headers = self._set_headers()
         url = self._format_url(path)
         response = requests.delete(url, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
```

## Comparing `hcv_api-0.0.3.dist-info/LICENSE.md` & `hcv_api-0.0.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `hcv_api-0.0.3.dist-info/RECORD` & `hcv_api-0.0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 vapi/__init__.py,sha256=1X3SDUjKbFmf8wgwfVDgHy1HiwSUqn3iFwLekAIJwME,49
 vapi/exceptions.py,sha256=i571A55U4_fQwU5dWjtFithl1ONntg91L_SmMRkyKU0,367
-vapi/vapi.py,sha256=Gss91zEnCDEjltZrRC2B5f9_lOldT1xisY3ON5Uq3pw,4745
-hcv_api-0.0.3.dist-info/LICENSE.md,sha256=S1pJL407BwTTXzZK0BQPNM7ZZs57uj1pTSfVZ8Whx30,1061
-hcv_api-0.0.3.dist-info/METADATA,sha256=YqN1jrX3KN5pbzKzafws4VXVGaRdS0vDmGRf-N8UyoY,192
-hcv_api-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hcv_api-0.0.3.dist-info/top_level.txt,sha256=WtIjxGq4gkdnp4MLZf6yEo-HMdTp5sRLDYmbTyoPhyE,5
-hcv_api-0.0.3.dist-info/RECORD,,
+vapi/vapi.py,sha256=hnmZEQLFHjf0gWH_y8bONL2j5fh_A_O5W7wKx-0LBZI,4760
+hcv_api-0.0.4.dist-info/LICENSE.md,sha256=S1pJL407BwTTXzZK0BQPNM7ZZs57uj1pTSfVZ8Whx30,1061
+hcv_api-0.0.4.dist-info/METADATA,sha256=E3aUhk9OdqfuiiP8I8xZC5ihlWGC8bDOgh3c8kpBmsk,192
+hcv_api-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hcv_api-0.0.4.dist-info/top_level.txt,sha256=WtIjxGq4gkdnp4MLZf6yEo-HMdTp5sRLDYmbTyoPhyE,5
+hcv_api-0.0.4.dist-info/RECORD,,
```

