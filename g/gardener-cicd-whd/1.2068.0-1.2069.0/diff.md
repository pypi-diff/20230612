# Comparing `tmp/gardener-cicd-whd-1.2068.0.tar.gz` & `tmp/gardener-cicd-whd-1.2069.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-whd-1.2068.0.tar", last modified: Fri Jun  9 15:16:15 2023, max compression
+gzip compressed data, was "gardener-cicd-whd-1.2069.0.tar", last modified: Mon Jun 12 15:29:11 2023, max compression
```

## Comparing `gardener-cicd-whd-1.2068.0.tar` & `gardener-cicd-whd-1.2069.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:16:15.892964 gardener-cicd-whd-1.2068.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-09 15:16:15.892964 gardener-cicd-whd-1.2068.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:16:15.888964 gardener-cicd-whd-1.2068.0/gardener_cicd_whd.egg-info/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-09 15:16:15.000000 gardener-cicd-whd-1.2068.0/gardener_cicd_whd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      405 2023-06-09 15:16:15.000000 gardener-cicd-whd-1.2068.0/gardener_cicd_whd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:16:15.000000 gardener-cicd-whd-1.2068.0/gardener_cicd_whd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-09 15:16:15.000000 gardener-cicd-whd-1.2068.0/gardener_cicd_whd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-09 15:16:15.000000 gardener-cicd-whd-1.2068.0/gardener_cicd_whd.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-09 15:16:15.892964 gardener-cicd-whd-1.2068.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2096 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/setup.whd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:16:15.888964 gardener-cicd-whd-1.2068.0/whd/
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17025 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/metric.py
--rw-r--r--   0 root         (0) root         (0)     6297 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/model.py
--rw-r--r--   0 root         (0) root         (0)     3875 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/pipelines.py
--rw-r--r--   0 root         (0) root         (0)    18333 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/pull_request.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/server.py
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/util.py
--rw-r--r--   0 root         (0) root         (0)     3704 2023-06-09 15:15:21.000000 gardener-cicd-whd-1.2068.0/whd/webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:29:11.652516 gardener-cicd-whd-1.2069.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-12 15:29:11.652516 gardener-cicd-whd-1.2069.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:29:11.652516 gardener-cicd-whd-1.2069.0/gardener_cicd_whd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-12 15:29:11.000000 gardener-cicd-whd-1.2069.0/gardener_cicd_whd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      405 2023-06-12 15:29:11.000000 gardener-cicd-whd-1.2069.0/gardener_cicd_whd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 15:29:11.000000 gardener-cicd-whd-1.2069.0/gardener_cicd_whd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-12 15:29:11.000000 gardener-cicd-whd-1.2069.0/gardener_cicd_whd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-12 15:29:11.000000 gardener-cicd-whd-1.2069.0/gardener_cicd_whd.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-12 15:29:11.652516 gardener-cicd-whd-1.2069.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/setup.whd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:29:11.652516 gardener-cicd-whd-1.2069.0/whd/
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16972 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/metric.py
+-rw-r--r--   0 root         (0) root         (0)     6297 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/model.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    18333 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/pull_request.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/server.py
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/util.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2023-06-12 15:25:57.000000 gardener-cicd-whd-1.2069.0/whd/webhook.py
```

### Comparing `gardener-cicd-whd-1.2068.0/LICENSE.md` & `gardener-cicd-whd-1.2069.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/README.md` & `gardener-cicd-whd-1.2069.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/setup.py` & `gardener-cicd-whd-1.2069.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/setup.whd.py` & `gardener-cicd-whd-1.2069.0/setup.whd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/whd/__init__.py` & `gardener-cicd-whd-1.2069.0/whd/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/whd/dispatcher.py` & `gardener-cicd-whd-1.2069.0/whd/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,16 @@
         dispatch_start_time: datetime.datetime,
     ):
         ref_type = create_event.ref_type()
         if not ref_type == RefType.BRANCH:
             logger.info(f'ignored create event with type {ref_type}')
             return
 
-        # todo: rename parameter
         self._update_pipeline_definition(
-            push_event=create_event,
+            event=create_event,
             delivery_id=delivery_id,
             repository=repository,
             hostname=hostname,
             es_client=es_client,
             dispatch_start_time=dispatch_start_time,
         )
 
@@ -118,15 +117,15 @@
         hostname: str,
         es_client: ccc.elasticsearch.ElasticSearchClient,
         dispatch_start_time: datetime.datetime,
     ):
         if self._pipeline_definition_changed(push_event):
             try:
                 self._update_pipeline_definition(
-                    push_event=push_event,
+                    event=push_event,
                     delivery_id=delivery_id,
                     repository=repository,
                     hostname=hostname,
                     es_client=es_client,
                     dispatch_start_time=dispatch_start_time,
                 )
             except ValueError as e:
@@ -176,30 +175,30 @@
                 'dispatch_start_time': dispatch_start_time,
             }
         )
         thread.start()
 
     def _update_pipeline_definition(
         self,
-        push_event,
+        event,
         delivery_id: str,
         repository: str,
         hostname: str,
         es_client: ccc.elasticsearch.ElasticSearchClient,
         dispatch_start_time: datetime.datetime,
     ):
         def _do_update(
             delivery_id: str,
             event_type: str,
             repository: str,
             hostname: str,
             dispatch_start_time: datetime.datetime,
             es_client: ccc.elasticsearch.ElasticSearchClient,
         ):
-            repo_url = push_event.repository().repository_url()
+            repo_url = event.repository().repository_url()
             job_mapping_set = self.cfg_set.job_mapping()
             job_mapping = job_mapping_set.job_mapping_for_repo_url(repo_url, self.cfg_set)
 
             replicate_repository_pipelines(
                 repo_url=repo_url,
                 cfg_set=self.cfg_factory.cfg_set(job_mapping.replication_ctx_cfg_set()),
                 whd_cfg=self.whd_cfg,
```

### Comparing `gardener-cicd-whd-1.2068.0/whd/metric.py` & `gardener-cicd-whd-1.2069.0/whd/metric.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/whd/model.py` & `gardener-cicd-whd-1.2069.0/whd/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/whd/pipelines.py` & `gardener-cicd-whd-1.2069.0/whd/pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/whd/pull_request.py` & `gardener-cicd-whd-1.2069.0/whd/pull_request.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/whd/server.py` & `gardener-cicd-whd-1.2069.0/whd/server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/whd/util.py` & `gardener-cicd-whd-1.2069.0/whd/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2068.0/whd/webhook.py` & `gardener-cicd-whd-1.2069.0/whd/webhook.py`

 * *Files identical despite different names*

