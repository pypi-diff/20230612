# Comparing `tmp/xt_st_common-0.8.2.tar.gz` & `tmp/xt_st_common-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.8.2.tar", max compression
+gzip compressed data, was "xt_st_common-0.8.3.tar", max compression
```

## Comparing `xt_st_common-0.8.2.tar` & `xt_st_common-0.8.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-08 10:07:59.069908 xt_st_common-0.8.2/README.md
--rw-r--r--   0        0        0     2603 2023-06-08 10:07:59.069908 xt_st_common-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-08 10:07:22.081981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-08 10:07:22.081981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-08 10:07:59.065908 xt_st_common-0.8.2/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2750 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3177 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    39344 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6518 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6854 2023-06-08 10:07:22.161980 xt_st_common-0.8.2/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-08 10:07:22.161980 xt_st_common-0.8.2/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-12 10:12:11.156918 xt_st_common-0.8.3/README.md
+-rw-r--r--   0        0        0     2603 2023-06-12 10:12:11.156918 xt_st_common-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-12 10:11:31.073096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-12 10:11:31.073096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-12 10:11:31.097096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-12 10:11:31.097096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-12 10:12:11.156918 xt_st_common-0.8.3/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2750 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3327 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    41597 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6941 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6936 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.3/PKG-INFO
```

### Comparing `xt_st_common-0.8.2/README.md` & `xt_st_common-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.8.2
+# XT-STREAMLIT - 0.8.3
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.8.2/pyproject.toml` & `xt_st_common-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.8.2"
+version = "0.8.3"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
```

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.8.3/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/xt_st_common/components.py` & `xt_st_common-0.8.3/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/xt_st_common/config.py` & `xt_st_common-0.8.3/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/xt_st_common/database.py` & `xt_st_common-0.8.3/src/xt_st_common/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,23 +34,26 @@
 @st.cache_data(ttl=30)
 def get_project(project_id: str, cache_id=None) -> Optional[Project]:
     project_dict = get_collection().find_one({"_id": ObjectId(project_id)})
     return Project(**project_dict) if project_dict is not None else None
 
 
 @st.cache_data(ttl=30)
-def get_projects(include_public=False, cache_id=None) -> List[Project]:
+def get_projects(include_public=False, other_apps=False, cache_id=None) -> List[Project]:
     current_user = get_user_email()
-    or_query = [
-        {"users": {"$elemMatch": {"$regex": current_user, "$options": "i"}}},
-        {"owner": {"$regex": current_user, "$options": "i"}},
-    ]
+    or_query = {
+        "$or": [
+            {"users": {"$elemMatch": {"$regex": current_user, "$options": "i"}}},
+            {"owner": {"$regex": current_user, "$options": "i"}},
+        ]
+    }
     if include_public:
-        or_query.append({"public": True})
-    return [Project(**item) for item in get_collection().find({"$or": or_query})]
+        or_query["$or"].append({"public": True})
+    query = or_query if other_apps else {"$and": [{"application": f"{settings.APP_NAME}"}, or_query]}
+    return [Project(**item) for item in get_collection().find(query)]
 
 
 @st.cache_data(ttl=30)
 def project_exists(project_id: str, cache_id=None) -> bool:
     return get_collection().count_documents({"_id": ObjectId(project_id)}) > 0
```

### Comparing `xt_st_common-0.8.2/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.8.3/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/xt_st_common/project_components.py` & `xt_st_common-0.8.3/src/xt_st_common/project_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,16 +293,16 @@
     save_project(project)
     set_state(
         ProjectState.UPLOAD_SUCCESS_MESSAGE,
         f"{count} folders were added to **'{project.name}'**",
     )
 
 
-def rename_file(selected_file):
-    project = st.session_state["selected_project"]
+def rename_file(selected_file: FileRef):
+    project: Project = st.session_state["selected_project"]
     rename_string = st.session_state["rename_project_file_name"]
 
     if not rename_string:
         set_state(
             ProjectState.FILE_WARNING_MESSAGE,
             "Cannot rename file. New name was empty",
         )
@@ -313,25 +313,26 @@
             ProjectState.FILE_WARNING_MESSAGE,
             f"You don't have write access to project: {project.name}",
         )
         return
 
     new_path = f"{selected_file.get_prefix()}/{rename_string}"
 
-    storage_client.move_file(selected_file.path, new_path)
+    project.move_file_to_path(selected_file, new_path)
+
+    save_project(project)
 
-    # save_project(project)
     set_state(
         ProjectState.FILE_SUCCESS_MESSAGE,
-        f"File **'{selected_file}'** was renamed to **'{rename_string}'**",
+        f"File **'{selected_file.name}'** was succesfully renamed to **'{rename_string}'**",
     )
 
 
 @st.cache_data(ttl=300)
-def get_df_preview(path: str, ext: Optional[str], num_rows=10):
+def get_df_preview(path: str, ext: Optional[str], num_rows=25):
     # if filepath.suffix == ".zip":
     #     frame = get_gdf_from_file(filepath)
     #     return frame.iloc[:num_rows, :-1]
     if ext == ".csv":
         file = storage_client().get_file(path)
         encoding, dialect = get_encoding_and_dialect(file)
         return pd.read_csv(file, nrows=num_rows, sep=dialect.delimiter, encoding=encoding)
@@ -351,70 +352,85 @@
 
 
 def _state_name(project_id: str, folder: str) -> str:
     return f"{project_id}-{folder}_fs"
 
 
 @st.cache_data(ttl=15)
-def get_proj_options(include_public: bool, cache_id=None):
+def get_proj_options(include_public: bool, other_apps: bool = True, cache_id=None):
     selected_project = get_selected_project()
-    projects = get_projects(include_public, get_project_cache())
+    projects = get_projects(include_public, other_apps, get_project_cache())
     sel_idx = 0
     options = {}
     for idx, proj in enumerate(projects):
         if selected_project and proj.id == selected_project.id:
             sel_idx = idx
         options[idx] = proj.name
     return options, projects, sel_idx
 
 
 def on_project_select():
     proj_idx = get_state("project_select")
     include_public = bool(get_state("include_public_projects", False))
-    options, projects, _ = get_proj_options(include_public, get_project_cache())
+    include_other_apps = bool(get_state("include_other_apps", False))
+    options, projects, _ = get_proj_options(include_public, include_other_apps, cache_id=get_project_cache())
 
     if proj_idx is not None and proj_idx > -1:
         selected_project = projects[proj_idx] if proj_idx != -1 else None
         set_selected_project(selected_project)
     else:
         set_selected_project(None)
 
 
 def project_selector(
     header_text: Optional[str] = "Projects",
     select_box_label="Select Project",
     null_option="-- Select Project --",
     st_context=st.sidebar,
+    on_select_change=None,
+    enable_filters=True,
+    render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
 ) -> Tuple[Union["Project", None], List["Project"]]:
     """UI to select and create projects
     Args:
         root_path (Path): The root Path to where the project folders live
     """
     selected_project = None
 
+    if render_layout == "horizontal":
+        container1, container2 = st_context.columns(2)
+    else:
+        container1 = st_context.container()
+        container2 = st_context.container()
+
     if header_text is not None:
         st_context.subheader(header_text)
-    include_public = st_context.checkbox("Public projects", value=False, key="include_public_projects")
-    options, projects, sel_idx = get_proj_options(include_public, get_project_cache())
+    include_public = bool(get_state("include_public_projects", False))
+    include_other_apps = bool(get_state("include_other_apps", False))
+    if enable_filters:
+        with container2.expander("Project Filters"):
+            include_public = st.checkbox("Public projects", value=False, key="include_public_projects")
+            include_other_apps = st.checkbox("Other Apps", value=False, key="include_other_apps")
+    options, projects, sel_idx = get_proj_options(include_public, include_other_apps, get_project_cache())
     proj_options = {}
 
     # accomodate the null option if one is provided
     if null_option is not None:
         proj_options = {-1: null_option}
         sel_idx = sel_idx + 1
 
     if options is not None:
         proj_options = {**proj_options, **options}
 
     if len(proj_options) > 0:
-        proj_idx = st_context.selectbox(
+        proj_idx = container1.selectbox(
             select_box_label,
             key="project_select",
             index=sel_idx,
-            # on_change=on_project_select,
+            on_change=on_select_change,
             options=proj_options.keys(),
             format_func=lambda x: proj_options[x],
         )
 
         selected_project = None
         if proj_idx is not None:
             selected_project = projects[proj_idx] if proj_idx != -1 else None
@@ -707,15 +723,15 @@
             if selected_file is not None and selected_key is not None:
                 row = container2.expander("File Actions", expanded=expand_file_actions)
                 if len(selected_key) > 30:
                     row.caption(selected_key)
 
                 if render_layout == "compact":
                     file_container0 = row.container()
-                    file_container1, file_container2 = row.columns([1, 1])
+                    file_container1, file_container2 = row.columns([5, 3])
                     file_container3 = row.container()
                     file_container4 = row.container()
                     file_container5 = row.container()
 
                 else:
                     file_container0, file_container1, file_container2 = row.columns([1, 1, 1])
                     file_container3, file_container4, file_container5 = row.columns([2, 1, 1])
@@ -817,25 +833,26 @@
         proj_dict["users"] = ", ".join(proj.users)
         proj_dict["select"] = proj.name == (selected_project.name if selected_project is not None else None)
 
         proj_data.append(proj_dict)
     return proj_data
 
 
-def add_new_project(number=1):
+def add_new_project(number=1, name_value: Optional[str] = None):
     user_email = get_user_email()
-    default_proj_name = f"{user_email.split('@')[0]}_#{number}"
-    project = Project(name=default_proj_name, owner=get_user_email())
+    if name_value is None:
+        name_value = f"{user_email.split('@')[0]}_#{number}"
+    project = Project(name=name_value, owner=get_user_email())
 
     project = save_project(project)
     set_selected_project(project)
 
     set_state(
         ProjectState.PROJECT_SUCCESS_MESSAGE,
-        f"Project **'{default_proj_name}'** has been initialised.",
+        f"Project **'{name_value}'** has been initialised.",
     )
 
     st.experimental_rerun()
 
 
 def get_next_project_number(projects: list[Project]):
     highest_number = len(projects) + 1
@@ -850,14 +867,15 @@
     return highest_number
 
 
 def project_manager(
     st_context=st.sidebar,
     null_option=None,
     render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
+    on_project_select_change=None,
 ):
     delete_confirm = get_state(ProjectState.PROJECT_DELETE_CONFIRM)
     project_to_delete = get_state(ProjectState.PROJECT_TO_DELETE, None)
     success_message = get_state(ProjectState.PROJECT_SUCCESS_MESSAGE)
     warning_message = get_state(ProjectState.PROJECT_WARNING_MESSAGE)
     get_state(ProjectState.UPLOAD_DELETE_CONFIRM)
     get_state(ProjectState.FOLDER_TO_DELETE)
@@ -870,46 +888,41 @@
         st.success(success_message)
     if warning_message:
         st.warning(warning_message)
     if delete_confirm and project_to_delete:
         st.warning(delete_confirm)
         st.button("I'm Sure", on_click=action_delete, args=(project_to_delete,))
 
-    if render_layout == "vertical":
-        grid_container = st_context.container()
-
-        select_container = st_context.container()
-
-        container1, container2, container3 = st_context.columns([1, 1, 1])
-    elif render_layout == "horizontal":
+    if render_layout == "horizontal":
+        add_container, save_container, filter_container = st_context.columns([3, 1, 4])
         grid_container = st_context.container()
-        select_container, container1, container2, container3, _ = st_context.columns([6, 1, 1, 1, 3])
+        select_container, delete_container, _ = st_context.columns([3, 1, 2])
 
-        # do some spacing that is particular to this layout
-        container1.markdown("#")
-        container1.markdown("#")
-        container2.markdown("#")
-        container2.markdown("#")
-        container3.markdown("#")
-        container3.markdown("#")
+        # # do some spacing that is particular to this layout
+        delete_container.markdown("#")
     else:
+        filter_container = st_context.container()
         grid_container = st_context.container()
-
         select_container = st_context.container()
 
-        container1 = st_context.container()
-        container2 = st_context.container()
-        container3 = st_context.container()
+        add_container = st_context.container()
+        save_container, delete_container = st_context.columns([1, 1])
+
+    with filter_container.expander("Project Filters"):
+        st.checkbox("Public projects", value=False, key="include_public_projects")
+        st.checkbox("Other Apps", value=False, key="include_other_apps")
 
     with select_container:
         project, projects = project_selector(
             header_text=None,
             null_option=null_option,
             select_box_label="Select Project",
             st_context=select_container,  # type: ignore
+            on_select_change=on_project_select_change,
+            enable_filters=False,
         )
 
         if len(projects) < 1:
             add_new_project()
 
     with grid_container:
         if render_layout == "compact":
@@ -989,25 +1002,46 @@
                     help="The list of users with access to the project",
                     disabled=False,
                     width=set_col_width,
                 ),
             },
         )
 
-        with container1:
-            if st.button("Add New"):
+        with add_container:
+            name_col, btn_col = st.columns([3, 1])
+            name_value = name_col.text_input(
+                "Project Name",
+                placeholder="Project_Name",
+                help="Name to use for a new project",
+                label_visibility="collapsed",
+            )
+            if btn_col.button("Add New"):
+                if not name_value:
+                    set_state(
+                        ProjectState.PROJECT_WARNING_MESSAGE,
+                        "**ADD PROJECT ERROR**: No project name value was entered for the new project.",
+                    )
+                    st.experimental_rerun()
+                for proj in projects:
+                    if proj.name.lower() == name_value.lower() and proj.owner.lower() == get_user_email().lower():
+                        set_state(
+                            ProjectState.PROJECT_WARNING_MESSAGE,
+                            f"**ADD PROJECT ERROR**: Project with the name **{name_value}** already exists.",
+                        )
+                        st.experimental_rerun()
+
                 new_proj_number = get_next_project_number(projects)
-                add_new_project(new_proj_number)
+                add_new_project(new_proj_number, name_value)
 
-        with container2:
+        with delete_container:
             if st.button("Delete Selected"):
                 submit_delete_project(project)
                 st.experimental_rerun()
 
-        with container3:
+        with save_container:
             if st.button("Save Changes") and st.session_state.get("project_editor_key").get("edited_rows") is not None:
                 update_messages = []
                 project_table_data = st.session_state.get("project_editor_key")
                 for changed_id in project_table_data["edited_rows"]:
                     # Get latest DB copy of the project
                     db_project = get_project(
                         str(edited_project_data["id"][changed_id]),
@@ -1039,14 +1073,20 @@
                                 f"Cannot update project: A Project with the name: **'{db_project.name}'** "
                                 + "already exists",
                             )
                         else:
                             db_project = save_project(db_project)
                             update_messages.append(f"Project **'{db_project.name}'** updated successfully")
 
-                set_state(
-                    ProjectState.PROJECT_SUCCESS_MESSAGE,
-                    "".join([f"> 1. {msg} \n" for msg in update_messages]),
-                )
+                if len(update_messages) > 1:
+                    set_state(
+                        ProjectState.PROJECT_SUCCESS_MESSAGE,
+                        "".join([f"> 1. {msg} \n" for msg in update_messages]),
+                    )
+                else:
+                    set_state(
+                        ProjectState.PROJECT_SUCCESS_MESSAGE,
+                        "".join([f"{msg}" for msg in update_messages]),
+                    )
                 st.experimental_rerun()
 
     return project, projects
```

### Comparing `xt_st_common-0.8.2/src/xt_st_common/project_models.py` & `xt_st_common-0.8.3/src/xt_st_common/project_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,21 @@
         if child_dict := _dict[key]:
             for child_key in child_dict:
                 new_children = None
                 new_path = f"{path}/{child_key}"
                 if child_dict[child_key]:
                     new_children = []
                     self.populate_children(child_dict, child_key, new_children, new_path)
-                children.append({"label": child_key, "value": f"{path}/{child_key}", "children": new_children})
+                children.append(
+                    {
+                        "label": child_key,
+                        "value": f"{path}/{child_key}",
+                        "children": new_children,
+                    }
+                )
 
     def get_file_tree(self):
         main_dict = {}
         full_list = (
             [file.path.removeprefix(self.get_folder_path("")).strip("/") for file in self.files] if self.files else []
         )
         if self.folders:
@@ -141,14 +147,20 @@
                 replaced = True
                 break
         if not replaced:
             self.files.append(file_ref)
 
         return file_ref
 
+    def move_file_to_path(self, file: FileRef, new_path: str) -> FileRef:
+        new_file_ref = storage_client().move_file(file.path, new_path, file.content_type, file.size_bytes)
+        index = self.files.index(file)
+        self.files[index] = new_file_ref
+        return new_file_ref
+
     def delete_file(self, file: FileRef):
         storage_client().delete_file(file.path)
         try:
             self.files.remove(file)
         except ValueError:
             logging.warning(f"File {file.path} didn't exist and couldn't be deleted.")
```

### Comparing `xt_st_common-0.8.2/src/xt_st_common/session.py` & `xt_st_common-0.8.3/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/src/xt_st_common/storage.py` & `xt_st_common-0.8.3/src/xt_st_common/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,18 +138,18 @@
         # set MIME_TYPE for MSCL/GeoTek files
         if content_type is None and file_path.lower().endswith((".cal", ".out", ".raw", ".sbd", ".xrf")):
             content_type = "text/plain"
 
         obj = self.__client.put_object(self.__bucket, file_path, file_bytes, file_len, content_type=content_type)
         return self.object_to_file(obj, file_len, content_type)
 
-    def move_file(self, file_path: str, new_file_path: str) -> Optional[FileRef]:
+    def move_file(self, file_path: str, new_file_path: str, content_type, size_bytes: int) -> Optional[FileRef]:
         obj = self.__client.copy_object(self.__bucket, new_file_path, CopySource(self.__bucket, file_path))
         self.delete_file(file_path)
-        return self.object_to_file(obj)
+        return self.object_to_file(obj, file_length=size_bytes, content_type=content_type)
 
     def get_file(self, file_path: str):
         response_data = None
         try:
             response = self.__client.get_object(self.__bucket, file_path)
             # Read data from response.
             response_data = BytesIO(response.read())
```

### Comparing `xt_st_common-0.8.2/src/xt_st_common/utils.py` & `xt_st_common-0.8.3/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.2/PKG-INFO` & `xt_st_common-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.8.2
+Version: 0.8.3
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,15 @@
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
 Requires-Dist: streamlit (>=1.23.1)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.8.2
+# XT-STREAMLIT - 0.8.3
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

