# Comparing `tmp/FAIRSave-0.0.6-py3-none-any.whl.zip` & `tmp/FAIRSave-0.0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 38920 bytes, number of entries: 23
+Zip file size: 38890 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-01 12:17 FAIRSave/__init__.py
 -rw-rw-rw-  2.0 fat     9303 b- defN 23-Mar-01 12:17 FAIRSave/configuration.py
 -rw-rw-rw-  2.0 fat     2872 b- defN 23-Mar-01 12:17 FAIRSave/eln_manager.py
 -rw-rw-rw-  2.0 fat     4454 b- defN 23-Jun-11 18:32 FAIRSave/kadi_download.py
 -rw-rw-rw-  2.0 fat     4081 b- defN 23-Mar-01 12:17 FAIRSave/kadi_identifier.py
 -rw-rw-rw-  2.0 fat     3613 b- defN 23-Mar-01 12:17 FAIRSave/kadi_instances.py
 -rw-rw-rw-  2.0 fat     8198 b- defN 23-May-16 11:02 FAIRSave/kadi_json_writer.py
 -rw-rw-rw-  2.0 fat    18172 b- defN 23-Jun-12 13:18 FAIRSave/kadi_record.py
--rw-rw-rw-  2.0 fat    14016 b- defN 23-Jun-11 20:48 FAIRSave/kadi_search.py
+-rw-rw-rw-  2.0 fat    12066 b- defN 23-Jun-12 15:20 FAIRSave/kadi_search.py
 -rw-rw-rw-  2.0 fat     1351 b- defN 23-Mar-01 12:17 FAIRSave/kadi_template.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-01 12:17 FAIRSave/tools/__init__.py
 -rw-rw-rw-  2.0 fat     9443 b- defN 23-Mar-01 12:17 FAIRSave/tools/comparison.py
 -rw-rw-rw-  2.0 fat    16743 b- defN 23-Mar-01 12:17 FAIRSave/tools/difference.py
 -rw-rw-rw-  2.0 fat     6976 b- defN 23-Mar-01 12:17 FAIRSave/tools/json_reader.py
 -rw-rw-rw-  2.0 fat    10754 b- defN 23-Mar-01 12:17 FAIRSave/tools/key.py
 -rw-rw-rw-  2.0 fat     9861 b- defN 23-Mar-01 12:17 FAIRSave/tools/metadata.py
 -rw-rw-rw-  2.0 fat     2536 b- defN 23-Mar-01 12:17 FAIRSave/tools/surftheowl_json.py
 -rw-rw-rw-  2.0 fat     4495 b- defN 23-Mar-01 12:17 FAIRSave/tools/validation.py
--rw-rw-rw-  2.0 fat    11734 b- defN 23-Jun-12 14:16 FAIRSave-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3825 b- defN 23-Jun-12 14:16 FAIRSave-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 14:16 FAIRSave-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-12 14:16 FAIRSave-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1879 b- defN 23-Jun-12 14:16 FAIRSave-0.0.6.dist-info/RECORD
-23 files, 144407 bytes uncompressed, 35894 bytes compressed:  75.1%
+-rw-rw-rw-  2.0 fat    11734 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3827 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1889 b- defN 23-Jun-12 15:22 FAIRSave-0.0.6.1.dist-info/RECORD
+23 files, 142469 bytes uncompressed, 35844 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: FAIRSave/tools/surftheowl_json.py
 Comment: 
 
 Filename: FAIRSave/tools/validation.py
 Comment: 
 
-Filename: FAIRSave-0.0.6.dist-info/LICENSE
+Filename: FAIRSave-0.0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: FAIRSave-0.0.6.dist-info/METADATA
+Filename: FAIRSave-0.0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: FAIRSave-0.0.6.dist-info/WHEEL
+Filename: FAIRSave-0.0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: FAIRSave-0.0.6.dist-info/top_level.txt
+Filename: FAIRSave-0.0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: FAIRSave-0.0.6.dist-info/RECORD
+Filename: FAIRSave-0.0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## FAIRSave/kadi_search.py

```diff
@@ -1,10 +1,13 @@
 from kadi_apy import KadiManager
+from kadi_apy.globals import CONFIG_PATH
 import re
 from typing import Optional, List
+import  requests
+import configparser
 
 
 def Search_Item_Titles(*args, **kwargs):
     import warnings
     warnings.simplefilter('always', DeprecationWarning)
     warnings.warn('Warning! "Search_Item_Titles" will be renamed to '
                   '"search_item_titles_kadi" in a future release!',
@@ -151,14 +154,42 @@
 
     title_id_tuple = [(x['title'], x['id'])
                       for x in records
                       if x['title'] == title][0]
 
     return title_id_tuple[1]
 
+def search_record_from_file_kadi(instance: str,
+                                 file_id: str):
+    """Search for ID of record which contains a specific file.
+    
+    Args:
+        instance: The name of the instance to use in combination with a config file.
+        file_id: ID of the file whose recrd is searched.
+        
+    Returns:
+        int: ID of the record.
+    """
+    
+    # Get Kadi4Mat access token for API call
+    config = configparser.ConfigParser()
+    config.read(CONFIG_PATH)
+    token = config[instance]['pat']
+    
+    # Get file response from API call
+    endpoint = "https://kadi4mat.iam-cms.kit.edu/api/records/files/" + file_id
+    bearer_token = "Bearer " + token
+    headers = {"Authorization": bearer_token}
+    file = requests.get(endpoint, headers=headers)
+    
+    # Read record id where file is stored from metadata
+    record_id = int(file.json().get('_links').get('record').replace("https://kadi4mat.iam-cms.kit.edu/api/records/",""))
+    
+    return record_id
+
 
 def Search_Item_Identifier(*args, **kwargs):
     import warnings
     warnings.simplefilter('always', DeprecationWarning)
     warnings.warn('Warning! "Search_Item_Identifier" will be renamed to '
                   '"search_item_identifier_kadi" in a future release!',
                   DeprecationWarning)
@@ -242,97 +273,17 @@
     if record is None and record_id is None:
         raise ValueError('Choose a record to get files from.')
 
     if record is not None:
         record_id = search_item_id_kadi(instance=instance,
                                         title=record,
                                         item='record')
-    # TODO: test!!
     record = KadiManager(instance=instance).record(id=record_id)
     pages = record.get_filelist().json()['_pagination'].get('total_pages')
     filelist = []
     for n in range(1, pages+1):
         files_in_page = (record.get_filelist(per_page=100, page=n)
                          .json()
                          .get('items'))
         filelist += [x['name'] for x in files_in_page]
 
     return filelist
-
-
-def Latest_Title(*args, **kwargs):
-    import warnings
-    warnings.simplefilter('always', DeprecationWarning)
-    warnings.warn('Warning! "Latest_Title" will be renamed to '
-                  '"latest_title_kadi" in a future release!',
-                  DeprecationWarning)
-    return latest_title_kadi(*args, **kwargs)
-
-
-def latest_title_kadi(instance: str,
-                      record_type: str,
-                      collection: Optional[str] = None,
-                      collection_id: Optional[int] = None,
-                      keywords: Optional[str] = None) -> str:
-    # Suggests a title based on the latest title before
-    if collection is not None:
-        collection_id = search_item_id_kadi(instance=instance,
-                                            title=collection,
-                                            item='collection')
-
-    record_list = search_item_titles_kadi(instance=instance,
-                                          item='record',
-                                          collection_id=collection_id,
-                                          record_type=record_type,
-                                          keywords=keywords)
-    record_numbers = []
-
-    for record in record_list:
-        try:
-            number = int(re
-                     .findall('#[0-9]{4}', record)[0]
-                     .replace('#', '')
-                     .lstrip('0'))
-        except:
-            print("")
-        record_numbers.append(number)
-
-    if record_numbers != []:
-        record_max_number = str(max(record_numbers))
-        for record in record_list:
-            if record[-4:] == record_max_number.zfill(4):
-                record_name = record
-
-        return record_name
-
-
-def Suggest_Title(*args, **kwargs):
-    import warnings
-    warnings.simplefilter('always', DeprecationWarning)
-    warnings.warn('Warning! "Suggest_Title" will be renamed to '
-                  '"suggest_title_kadi" in a future release!',
-                  DeprecationWarning)
-    return suggest_title_kadi(*args, **kwargs)
-
-
-def suggest_title_kadi(instance: str,
-                       record_type: str,
-                       collection: Optional[str] = None,
-                       collection_id: Optional[int] = None,
-                       keywords: Optional[str] = None) -> str:
-
-    if collection is not None:
-        collection_id = search_item_id_kadi(instance=instance,
-                                            title=collection,
-                                            item='collection')
-
-    latest_title = latest_title_kadi(instance=instance,
-                                     collection_id=collection_id,
-                                     record_type=record_type,
-                                     keywords=keywords)
-
-    if latest_title != "":
-        record_number = str(int(latest_title[-4:].strip('0'))+1).zfill(4)
-        suggested_title = latest_title[:-4] + record_number
-
-        return suggested_title
-
```

## Comparing `FAIRSave-0.0.6.dist-info/LICENSE` & `FAIRSave-0.0.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `FAIRSave-0.0.6.dist-info/METADATA` & `FAIRSave-0.0.6.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FAIRSave
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Package to run the FAIR-Save toolbox
 Home-page: UNKNOWN
 Author: Malte Flachmann, Floriane Bresser, Ilia Bagov (Karlsruhe Institute of Technology)
 Author-email: malte.flachmann@student.kit.edu
 License: Apache-2.0
 Project-URL: GitLab, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save_Utilities
 Project-URL: Changelog, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save-Utilities/-/blob/main/Changelog.md
```

## Comparing `FAIRSave-0.0.6.dist-info/RECORD` & `FAIRSave-0.0.6.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 FAIRSave/configuration.py,sha256=0ehQ_OkseYMsgKhRsdVUclBOXvt4NH1aiobHvN5ziW8,9303
 FAIRSave/eln_manager.py,sha256=dpo3PAS55a_wXGvemiE0eoNr4FsPmCvspezAio-HcX4,2872
 FAIRSave/kadi_download.py,sha256=PWFSppaWx7PjCW1d5W5G4vnisojNoUnZ0qYxp--l9hw,4454
 FAIRSave/kadi_identifier.py,sha256=3OiylNuqzwY3EQgw0Nfov196DOBt495aCEAZUhYdYfY,4081
 FAIRSave/kadi_instances.py,sha256=Xx0dMqouFFHBp9Yo8W4b5dDeX8iss_faGm9fufkVKyQ,3613
 FAIRSave/kadi_json_writer.py,sha256=2ke4ywZNqFYlLrlX30mPkdqnw5QfM0Bs3DjXqYjNh-w,8198
 FAIRSave/kadi_record.py,sha256=-_b38AQcNPPCU4FM_sRVbmK7d9W4fEfTG6tgYMIUNCc,18172
-FAIRSave/kadi_search.py,sha256=1MyPD85ud0pZGhUXJwfHO43gDMdGFOG0gGAlil3noSs,14016
+FAIRSave/kadi_search.py,sha256=P47wmL8B47qrq5IPwszxzKl1lNMLkZkKTtqlMFOlK-k,12066
 FAIRSave/kadi_template.py,sha256=m0vC4gxy_-liaAe40xlX3VRjxQJXw6pq4s6FDFDzgyk,1351
 FAIRSave/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 FAIRSave/tools/comparison.py,sha256=gQ76mS9glUf9bcS7kWB0mtSx7lZ7WySTz4zCMmdF6zI,9443
 FAIRSave/tools/difference.py,sha256=Drc0LwvT29WUhzyjUgphfM_nuGIi0Oab0138q1PUFKs,16743
 FAIRSave/tools/json_reader.py,sha256=YnE9_3lToaJxU0aVoYOchBcbQh0RoYvuRgtkuwuXRj0,6976
 FAIRSave/tools/key.py,sha256=kspBVidTf54F_GmUdhh6fPT5G7bLHQpjfI2CoUEc-jk,10754
 FAIRSave/tools/metadata.py,sha256=MBtDeQrfrl_uRUSamR7q1JFPoE8JkPN7_UNSi5qdIGs,9861
 FAIRSave/tools/surftheowl_json.py,sha256=Ie9MGa1mXrxaQxynb9daDhR2LFa4kkf4tZ0Hrdb8AgU,2536
 FAIRSave/tools/validation.py,sha256=pQDKRIaoEylU5hPuI_loncMEYAgzgYbZgpm7u7Doat8,4495
-FAIRSave-0.0.6.dist-info/LICENSE,sha256=itGSoY4BUSDO1X36lIFXCBlN8XsDnZRP-qdcfnmKazw,11734
-FAIRSave-0.0.6.dist-info/METADATA,sha256=GrAjAWV1Yo26OK4_CU3gfyQEOXWAIbPUVgbPj1krPuk,3825
-FAIRSave-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-FAIRSave-0.0.6.dist-info/top_level.txt,sha256=BemltgO7SU5GOPMbfMCBkSpXowdROrlrsN46O3nTt6A,9
-FAIRSave-0.0.6.dist-info/RECORD,,
+FAIRSave-0.0.6.1.dist-info/LICENSE,sha256=itGSoY4BUSDO1X36lIFXCBlN8XsDnZRP-qdcfnmKazw,11734
+FAIRSave-0.0.6.1.dist-info/METADATA,sha256=w4yQH-55R1gzPFcSm5TkeTCKtKQnCDQsg0HAJ2Anmnw,3827
+FAIRSave-0.0.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+FAIRSave-0.0.6.1.dist-info/top_level.txt,sha256=BemltgO7SU5GOPMbfMCBkSpXowdROrlrsN46O3nTt6A,9
+FAIRSave-0.0.6.1.dist-info/RECORD,,
```

