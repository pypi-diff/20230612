# Comparing `tmp/streamlit-deckgl-0.4.1.tar.gz` & `tmp/streamlit-deckgl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deckgl-0.4.1.tar", last modified: Tue May 23 22:40:56 2023, max compression
+gzip compressed data, was "streamlit-deckgl-0.5.0.tar", last modified: Mon Jun 12 07:27:44 2023, max compression
```

## Comparing `streamlit-deckgl-0.4.1.tar` & `streamlit-deckgl-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 22:40:56.206532 streamlit-deckgl-0.4.1/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.4.1/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.4.1/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-23 22:40:56.206532 streamlit-deckgl-0.4.1/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     2435 2023-05-08 19:47:36.000000 streamlit-deckgl-0.4.1/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-23 22:40:56.206532 streamlit-deckgl-0.4.1/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-23 22:40:00.000000 streamlit-deckgl-0.4.1/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 22:40:56.202532 streamlit-deckgl-0.4.1/src/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 22:40:56.202532 streamlit-deckgl-0.4.1/src/streamlit_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2672 2023-05-15 20:40:20.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 22:40:56.206532 streamlit-deckgl-0.4.1/src/streamlit_deckgl/frontend/
--rw-rw-r--   0 dave      (1000) dave      (1000)      816 2023-05-15 23:58:43.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl/frontend/index.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     3374 2023-05-23 22:40:39.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl/frontend/main.js
--rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl/frontend/style.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 22:40:56.202532 streamlit-deckgl-0.4.1/src/streamlit_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-23 22:40:55.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-23 22:40:56.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-23 22:40:55.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-23 22:40:55.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-23 22:40:55.000000 streamlit-deckgl-0.4.1/src/streamlit_deckgl.egg-info/top_level.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-12 07:27:44.788686 streamlit-deckgl-0.5.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.5.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.5.0/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-06-12 07:27:44.788686 streamlit-deckgl-0.5.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2435 2023-05-08 19:47:36.000000 streamlit-deckgl-0.5.0/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-12 07:27:44.788686 streamlit-deckgl-0.5.0/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-06-12 05:41:28.000000 streamlit-deckgl-0.5.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-12 07:27:44.764686 streamlit-deckgl-0.5.0/src/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-12 07:27:44.768686 streamlit-deckgl-0.5.0/src/streamlit_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2672 2023-05-15 20:40:20.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-12 07:27:44.788686 streamlit-deckgl-0.5.0/src/streamlit_deckgl/frontend/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      816 2023-05-15 23:58:43.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl/frontend/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3471 2023-06-12 05:41:15.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl/frontend/main.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl/frontend/style.css
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-12 07:27:44.776686 streamlit-deckgl-0.5.0/src/streamlit_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-06-12 07:27:43.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-06-12 07:27:44.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-12 07:27:43.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-06-12 07:27:43.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-06-12 07:27:43.000000 streamlit-deckgl-0.5.0/src/streamlit_deckgl.egg-info/top_level.txt
```

### Comparing `streamlit-deckgl-0.4.1/LICENSE` & `streamlit-deckgl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.4.1/PKG-INFO` & `streamlit-deckgl-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.4.1
+Version: 0.5.0
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-deckgl-0.4.1/README.md` & `streamlit-deckgl-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.4.1/setup.py` & `streamlit-deckgl-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-deckgl",
-    version="0.4.1",
+    version="0.5.0",
     author="Oceanum",
     author_email="developers@oceanum.science",
     description="Streamlit component for deck.gl visualisation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["streamlit_deckgl"],
     package_dir={"": "src"},
```

### Comparing `streamlit-deckgl-0.4.1/src/streamlit_deckgl/__init__.py` & `streamlit-deckgl-0.5.0/src/streamlit_deckgl/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.4.1/src/streamlit_deckgl/frontend/index.html` & `streamlit-deckgl-0.5.0/src/streamlit_deckgl/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.4.1/src/streamlit_deckgl/frontend/main.js` & `streamlit-deckgl-0.5.0/src/streamlit_deckgl/frontend/main.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -6,67 +6,67 @@
 
 /**
  * The component's render function. This will be called immediately after
  * the component is initially loaded, and then again every time the
  * component gets new data from Python.
  */
 
+let deckEventList = [];
+let deckInstance = null;
+let overlayInstance = null;
+
+const mapEventHandler = (eventType, info) => {
+    if (eventType === "deck-view-state-change-event") {
+        currentViewState = info;
+
+        if (overlayInstance) {
+            overlayInstance.setProps({
+                viewState: currentViewState
+            });
+        }
+    }
+
+    if (deckEventList.includes(eventType)) {
+        Streamlit.setComponentValue({
+            ...info.object,
+            coordinate: info.coordinate,
+            eventType,
+        });
+    }
+};
+
 function onRender(event) {
     // Only run the render code the first time the component is loaded.
-    if (!window.rendered) {
-        const {
-            spec,
-            tooltip,
-            height,
-            customLibraries,
-            configuration,
-            events,
-            description,
-            overlay,
-            mapbox_key,
-            google_maps_key,
-        } = event.detail.args;
-
-        const eventlist = events && events.map((event) => `deck-${event}-event`);
+    const container = document.getElementById("deckgl-primary");
+    const {
+        spec,
+        tooltip,
+        height,
+        customLibraries,
+        configuration,
+        events,
+        description,
+        overlay,
+        mapbox_key,
+        google_maps_key,
+    } = event.detail.args;
 
-        const container = document.getElementById("deckgl-primary");
+    if (!window.rendered) {
+        if (events) deckEventList = events.map((event) => `deck-${event}-event`);
         container.style.width = window.innerWidth - 10 + "px";
         container.style.height = height - 10 + "px";
         container.style.position = "absolute";
         const ocontainer = document.getElementById("deckgl-overlay");
         ocontainer.style.width = window.innerWidth - 10 + "px";
         ocontainer.style.height = height - 10 + "px";
         ocontainer.style.position = "absolute";
         ocontainer.style["pointer-events"] = "none";
 
         const mapSpec = JSON.parse(spec);
 
-        let deckInstance = null;
-        let overlayInstance = null;
-
-        const mapEventHandler = (eventType, info) => {
-            if (eventType === "deck-view-state-change-event") {
-                currentViewState = info;
-
-                if (overlayInstance) {
-                    overlayInstance.setProps({
-                        viewState: currentViewState
-                    });
-                }
-            }
-
-            if (events && eventlist.includes(eventType)) {
-                Streamlit.setComponentValue({
-                    ...info.object,
-                    coordinate: info.coordinate,
-                    eventType,
-                });
-            }
-        };
-
         deckInstance = createDeck({
             mapboxApiKey: mapbox_key,
             googleMapsApiKey: google_maps_key,
             container,
             jsonInput: mapSpec,
             tooltip,
             customLibraries,
@@ -96,25 +96,28 @@
 
         if (description) {
             for (const key in description) {
                 if (
                     ["top-right", "top-left", "bottom-right", "bottom-left"].includes(key)
                 ) {
                     const pos = key.split("-");
-                    const style = `z-index:10; position: absolute; ${pos[0]}:10px; ${pos[1]}:10px;`;
+                    const style = `z-index:10; position: absolute; ${pos[0]}:10px; ${pos[1]}:10px;background-color:none;`;
                     const div = document.createElement("div");
                     div.innerHTML = description[key];
                     div.style = style;
                     container.appendChild(div);
                 }
             }
         }
 
         Streamlit.setFrameHeight(height);
         window.rendered = true;
+    } else {
+        if (deckInstance) updateDeck(JSON.parse(spec), deckInstance);
+        if (overlayInstance) updateDeck(JSON.parse(overlay), overlayInstance);
     }
 }
 
 // Render the component whenever python send a "render event"
 Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRender);
 // Tell Streamlit that the component is ready to receive events
 Streamlit.setComponentReady();
```

### Comparing `streamlit-deckgl-0.4.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js` & `streamlit-deckgl-0.5.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.4.1/src/streamlit_deckgl.egg-info/PKG-INFO` & `streamlit-deckgl-0.5.0/src/streamlit_deckgl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.4.1
+Version: 0.5.0
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

