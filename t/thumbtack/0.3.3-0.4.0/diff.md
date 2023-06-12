# Comparing `tmp/thumbtack-0.3.3.tar.gz` & `tmp/thumbtack-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/thumbtack-0.3.3.tar", last modified: Wed Mar  3 20:51:19 2021, max compression
+gzip compressed data, was "thumbtack-0.4.0.tar", last modified: Mon Jun 12 18:57:48 2023, max compression
```

## Comparing `thumbtack-0.3.3.tar` & `thumbtack-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-03 20:51:19.000000 thumbtack-0.3.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11368 2021-03-03 20:50:22.000000 thumbtack-0.3.3/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2021-03-03 20:50:22.000000 thumbtack-0.3.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3391 2021-03-03 20:51:19.000000 thumbtack-0.3.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2022 2021-03-03 20:50:22.000000 thumbtack-0.3.3/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2021-03-03 20:51:19.000000 thumbtack-0.3.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2046 2021-03-03 20:50:22.000000 thumbtack-0.3.3/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-03 20:51:19.000000 thumbtack-0.3.3/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-03 20:51:19.000000 thumbtack-0.3.3/src/thumbtack/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4473 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      275 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/directory_monitoring.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      153 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3900 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/resources.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-03 20:51:19.000000 thumbtack-0.3.3/src/thumbtack/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-03 20:51:19.000000 thumbtack-0.3.3/src/thumbtack/static/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/static/css/thumbtack.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-03 20:51:19.000000 thumbtack-0.3.3/src/thumbtack/static/js/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1155 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/static/js/thumbtack.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-03 20:51:19.000000 thumbtack-0.3.3/src/thumbtack/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/templates/base.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      197 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/templates/form_complete.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3724 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/templates/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    16994 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3341 2021-03-03 20:50:22.000000 thumbtack-0.3.3/src/thumbtack/views.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-03 20:51:19.000000 thumbtack-0.3.3/src/thumbtack.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3391 2021-03-03 20:51:18.000000 thumbtack-0.3.3/src/thumbtack.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      686 2021-03-03 20:51:18.000000 thumbtack-0.3.3/src/thumbtack.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-03 20:51:18.000000 thumbtack-0.3.3/src/thumbtack.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2021-03-03 20:51:18.000000 thumbtack-0.3.3/src/thumbtack.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-03 20:50:39.000000 thumbtack-0.3.3/src/thumbtack.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2021-03-03 20:51:18.000000 thumbtack-0.3.3/src/thumbtack.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-03-03 20:51:18.000000 thumbtack-0.3.3/src/thumbtack.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:57:48.837235 thumbtack-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11368 2023-06-12 18:57:47.000000 thumbtack-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-12 18:57:47.000000 thumbtack-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3841 2023-06-12 18:57:48.837235 thumbtack-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-06-12 18:57:47.000000 thumbtack-0.4.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-12 18:57:48.837235 thumbtack-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-12 18:57:47.000000 thumbtack-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:57:48.833235 thumbtack-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:57:48.833235 thumbtack-0.4.0/src/thumbtack/
+-rw-r--r--   0 root         (0) root         (0)     5016 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/config.py
+-rw-r--r--   0 root         (0) root         (0)      353 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/directory_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6365 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:57:48.833235 thumbtack-0.4.0/src/thumbtack/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:57:48.833235 thumbtack-0.4.0/src/thumbtack/static/css/
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/static/css/thumbtack.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:57:48.833235 thumbtack-0.4.0/src/thumbtack/static/js/
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/static/js/thumbtack.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:57:48.833235 thumbtack-0.4.0/src/thumbtack/templates/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/templates/form_complete.html
+-rw-r--r--   0 root         (0) root         (0)     5006 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)    23246 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/utils.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-06-12 18:57:47.000000 thumbtack-0.4.0/src/thumbtack/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:57:48.833235 thumbtack-0.4.0/src/thumbtack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3841 2023-06-12 18:57:48.000000 thumbtack-0.4.0/src/thumbtack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-12 18:57:48.000000 thumbtack-0.4.0/src/thumbtack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 18:57:48.000000 thumbtack-0.4.0/src/thumbtack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-12 18:57:48.000000 thumbtack-0.4.0/src/thumbtack.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 18:57:48.000000 thumbtack-0.4.0/src/thumbtack.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-12 18:57:48.000000 thumbtack-0.4.0/src/thumbtack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 18:57:48.000000 thumbtack-0.4.0/src/thumbtack.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `thumbtack-0.3.3/LICENSE` & `thumbtack-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thumbtack-0.3.3/PKG-INFO` & `thumbtack-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbtack
-Version: 0.3.3
+Version: 0.4.0
 Summary: Service to manage disk image mounts.
 Home-page: https://github.com/mitre/thumbtack
 Author: The MITRE Corporation
 Author-email: thumbtack@mitre.org
 License: Apache 2.0
 Description: 
         .. image:: https://travis-ci.org/mitre/thumbtack.svg?branch=master
@@ -43,22 +43,26 @@
         
         .. code-block:: bash
         
             $ thumbtack --help
             Usage: thumbtack [OPTIONS]
         
             Options:
-              -d, --debug           Run the Thumbtack server in debug mode
-              -h, --host TEXT       Host to run Thumbtack server on  [default: 127.0.0.1]
-              -p, --port TEXT       Port to run Thumbtack server on  [default: 8208]
-              -i, --image-dir TEXT  Directory of disk images for Thumbtack server to
-                                    monitor  [default: $CWD]
-              --db TEXT             SQLite database to store mount state  [default:
-                                    database.db]
-              --help                Show this message and exit.
+              -d, --debug                   Run the Thumbtack server in debug mode
+              -h, --host TEXT               Host to run Thumbtack server on  [default: 127.0.0.1]
+              -p, --port TEXT               Port to run Thumbtack server on  [default: 8208]
+              -m, --mount-dir TEXT          Directory to mount disk images  [Default: /mnt/thumbtack]
+              -i, --image-dir TEXT          Directory of disk images for Thumbtack server to
+                                            monitor  [default: $CWD]
+              --db TEXT                     SQLite database to store mount state  [default:
+                                            database.db]
+              -b, --base-url TEXT           Base URL where Thumbtack is hosted on the server
+              --path-contains TEXT          Only select files containing specified string in the path
+              -s, --skip-subdirectory TEXT  Subdirectory to ignore when monitoring files
+              --help                        Show this message and exit.
         
         LICENSE
         -------
         
         Thumbtack is licensed under the `Apache License, Version 2.0
         <https://www.apache.org/licenses/LICENSE-2.0.html>`_. See the `LICENSE` file for
         more information.
```

### Comparing `thumbtack-0.3.3/README.rst` & `thumbtack-0.4.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -34,22 +34,26 @@
 
 .. code-block:: bash
 
     $ thumbtack --help
     Usage: thumbtack [OPTIONS]
 
     Options:
-      -d, --debug           Run the Thumbtack server in debug mode
-      -h, --host TEXT       Host to run Thumbtack server on  [default: 127.0.0.1]
-      -p, --port TEXT       Port to run Thumbtack server on  [default: 8208]
-      -i, --image-dir TEXT  Directory of disk images for Thumbtack server to
-                            monitor  [default: $CWD]
-      --db TEXT             SQLite database to store mount state  [default:
-                            database.db]
-      --help                Show this message and exit.
+      -d, --debug                   Run the Thumbtack server in debug mode
+      -h, --host TEXT               Host to run Thumbtack server on  [default: 127.0.0.1]
+      -p, --port TEXT               Port to run Thumbtack server on  [default: 8208]
+      -m, --mount-dir TEXT          Directory to mount disk images  [Default: /mnt/thumbtack]
+      -i, --image-dir TEXT          Directory of disk images for Thumbtack server to
+                                    monitor  [default: $CWD]
+      --db TEXT                     SQLite database to store mount state  [default:
+                                    database.db]
+      -b, --base-url TEXT           Base URL where Thumbtack is hosted on the server
+      --path-contains TEXT          Only select files containing specified string in the path
+      -s, --skip-subdirectory TEXT  Subdirectory to ignore when monitoring files
+      --help                        Show this message and exit.
 
 LICENSE
 -------
 
 Thumbtack is licensed under the `Apache License, Version 2.0
 <https://www.apache.org/licenses/LICENSE-2.0.html>`_. See the `LICENSE` file for
 more information.
```

### Comparing `thumbtack-0.3.3/setup.py` & `thumbtack-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 NAME = "thumbtack"
 DESCRIPTION = "Service to manage disk image mounts."
 URL = "https://github.com/mitre/thumbtack"
 EMAIL = "thumbtack@mitre.org"
 AUTHOR = "The MITRE Corporation"
 LICENSE = "Apache 2.0"
 REQUIRES_PYTHON = ">=3.4.0"
-VERSION = "0.3.3"
+VERSION = "0.4.0"
 
 REQUIRED = [
     "Click",
-    "Flask",
+    "Flask==2.3.2",
     "Flask-RESTful",
     "gunicorn",
-    "imagemounter",
+    "imagemounter_mitre==2023.6.12",
     "requests",
 ]
 
 doc_requires = [
     "sphinx",
 ]
```

### Comparing `thumbtack-0.3.3/src/thumbtack/__init__.py` & `thumbtack-0.4.0/src/thumbtack/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 try:
     __version__ = get_distribution("thumbtack").version
 except DistributionNotFound:
     __version__ = "Could not find version"
 
 
-def create_app(mount_dir=None, image_dir=None, database=None, base_url=None):
+def create_app(mount_dir=None, image_dir=None, database=None, base_url=None, path_contains=None, skip_subdirectory=None):
 
     if base_url:
         static_url_path = f"{base_url}/static"
         app = Flask(__name__, static_url_path=static_url_path)
     else:
         app = Flask(__name__)
 
@@ -49,19 +49,25 @@
         app.config.update(DATABASE=os.environ.get("THUMBTACK_DATABASE"))
 
     if base_url:
         app.config.update(APPLICATION_ROOT=base_url)
     elif os.environ.get("THUMBTACK_APPLICATION_ROOT"):
         app.config.update(APPLICATION_ROOT=os.environ.get("THUMBTACK_APPLICATION_ROOT"))
 
+    if path_contains:
+        app.config.update(PATH_CONTAINS=path_contains)
+
+    if skip_subdirectory:
+        app.config.update(SKIP_SUBDIRECTORY=skip_subdirectory)
+
     app.mnt_mutex = threading.Lock()
 
     # configure the rest
     configure(app, base_url)
-    app.before_first_request(before_first_request)
+    configure_logging(app)
     return app
 
 
 def configure(app, base_url=None):
 
     app.logger.info("configuring extensions")
 
@@ -89,18 +95,14 @@
             db_file.unlink()
 
         if not db_file.is_file():
             init_db()
     app.logger.info("configured")
 
 
-def before_first_request():
-    configure_logging(current_app)
-
-
 def configure_logging(app):
     formatter = logging.Formatter(
         "[%(asctime)s] %(levelname)s in %(name)s.%(module)s: %(message)s"
     )
 
     if app.debug:
         app.logger.setLevel(logging.DEBUG)
@@ -150,14 +152,28 @@
 @click.option(
     "-b",
     "--base-url",
     default="/",
     show_default=True,
     help="Base URL where Thumbtack is hosted on the server",
 )
-def start_app(debug, host, port, mount_dir, image_dir, database, base_url):
+@click.option(
+    "--path-contains",
+    default=None,
+    show_default=True,
+    help="Only select files containing specified string in the path",
+)
+@click.option(
+    '-s',
+    "--skip-subdirectory",
+    multiple=True,
+    default=[],
+    show_default=True,
+    help="Subdirectory to ignore when monitoring files",
+)
+def start_app(debug, host, port, mount_dir, image_dir, database, base_url, path_contains, skip_subdirectory):
     app = create_app(
-        mount_dir=mount_dir, image_dir=image_dir, database=database, base_url=base_url
+        mount_dir=mount_dir, image_dir=image_dir, database=database, base_url=base_url, path_contains=path_contains, skip_subdirectory=skip_subdirectory
     )
     directory_monitoring_thread = DirectoryMonitoring(app)
     directory_monitoring_thread.start()
     app.run(debug=debug, host=host, port=port)
```

### Comparing `thumbtack-0.3.3/src/thumbtack/static/css/thumbtack.css` & `thumbtack-0.4.0/src/thumbtack/static/css/thumbtack.css`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
   border-collapse: collapse;
   width: 100%;
 }
 
 th, td {
   text-align: left;
   padding: 8px;
+  white-space: nowrap;
 }
 
 tr:nth-child(even) {
   background-color: #cecece;
 }
 
 /**** Other stuff (tree view for mounted disks) ****/
@@ -55,14 +56,15 @@
 .active {
   display: block;
 }
 
 .tooltip {
   position: relative;
   display: inline-block;
+  white-space: normal;
 }
 
 .tooltip .tooltiptext {
   visibility: hidden;
   width: 140px;
   background-color: #555;
   color: #fff;
```

### Comparing `thumbtack-0.3.3/src/thumbtack/static/js/thumbtack.js` & `thumbtack-0.4.0/src/thumbtack/static/js/thumbtack.js`

 * *Files identical despite different names*

### Comparing `thumbtack-0.3.3/src/thumbtack/templates/index.html` & `thumbtack-0.4.0/src/thumbtack/templates/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -30,21 +30,22 @@
 
   <table style="width:70%">
     <tr>
       <th>Filename</th>
       <th>Status</th>
       <th>Mount</th>
       <th>Unmount</th>
-      <th>Mountpoint</th>
+      <th>Mountpoints</th>
+      <th>Add existing mountpoint <div class="tooltip">&#9432;<span class="tooltiptext">If you manually mounted the image, add the path to the mounted image to the thumbtack database.</span></div></th>
     </tr>
     {% for image in images %}
       <tr>
         <!-- Filename -->
         <td>
-          {% if image.status == 'Mounted' %}
+          {% if image.status == 'Mounted' or image.status == 'Manual mount'%}
             <a href="{{ url_for('.mount', image_path=image.rel_path) }}" >{{ image.rel_path }}</a>
           {% else %}
             {{ image.rel_path }}
           {% endif %}
         </td>
 
         <!-- Status -->
@@ -59,30 +60,38 @@
             <button>Mount</button>
           </form>
           {% endif %}
         </td>
 
         <!-- Unount Button -->
         <td>
-          {% if image.status == 'Mounted' %}
+          {% if image.status == 'Mounted' or image.status == 'Manual mount'%}
           <form class="myForm" method="post" action="{{ url_for('.mount_form') }}">
             <input type="hidden" name="img_to_mount" value="{{ image.rel_path }}">
             <input type="hidden" name="operation" value="unmount">
             <button>Unmount</button>
           </form>
           {% endif %}
         </td>
 
         <!-- Mountpoint info -->
         <td>
-          {% if image.status == 'Mounted' %}
+          {% if image.status == 'Mounted' or image.status == 'Manual mount'%}
           <ul class="myUL">
             <li>
-              <span class="caret">{{ image.disk_mountpoint }}</span>
-              <ul class="nested">
+	      <span>Disk mountpoint: <span id="{{ image.disk_mountpoint }}">{{ image.disk_mountpoint }}</span></span>
+	      <div class="tooltip">
+                <button onclick="copyByID('{{ image.disk_mountpoint }}')" onmouseout="outFunc('{{ image.disk_mountpoint }}Tooltip')">
+                  <span class="tooltiptext" id="{{ image.disk_mountpoint }}Tooltip">Copy to clipboard</span>
+                  Copy
+                </button>
+              </div>
+	      <br>
+	      <span>Volume mountpoints:</span>
+              <ul>
                 {% for volume in image.volume_info %}
                   <li>
                     [{{ volume.index }}] <span id="{{ volume.uid }}">{{ volume.mountpoint }}</span>
                     {% if volume.mountpoint %}
                     <div class="tooltip">
                       <button onclick="copyByID('{{ volume.uid }}')" onmouseout="outFunc('{{ volume.uid }}Tooltip')">
                         <span class="tooltiptext" id="{{ volume.uid }}Tooltip">Copy to clipboard</span>
@@ -93,12 +102,26 @@
                   </li>
                 {% endfor %}
               </ul>
             </li>
           </ul>
           {% endif %}
         </td>
+
+	<!-- Add mountpoint -->
+        <td>
+          {% if image.status == 'Unmounted' %}
+          <form class="myForm" method="post" action="{{ url_for('.add_mountpoint_form') }}">
+	    <label for="mountpoint_path">Mountpoint: </label>
+	    <input type="text" id="mountpoint_path" name="mountpoint_path">
+            <input type="hidden" name="img_to_mount" value="{{ image.rel_path }}">
+            <input type="hidden" name="operation" value="add_mountpoint">
+
+            <button>Add mountpoint</button>
+          </form>
+          {% endif %}
+        </td>
       </tr>
     {% endfor %}
   </table>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -11,28 +11,34 @@
 documentation for that type in the imagemounter_documentation.
 Supported: {% for mount_type in supported_mount_types %} {{ mount_type }} {{ "-
 " if not loop.last }} {% endfor %}
 Unsupported: {% for mount_type in unsupported_mount_types %} {{ mount_type }} {
 { "-" if not loop.last }} {% endfor %}
 More_info
 ***** Path to disk images: {{_image_dir_}} *****
-Filename       Status       Mount        Unmount      Mountpoint
+                                                                                    Add existing mountpoint
+Filename       Status       Mount        Unmount      Mountpoints                   ⓘIf you manually mounted the image, add the path to the mounted image to
+                                                                                    the thumbtack database.
                                                       {% if image.status ==
-                                                      'Mounted' %}
-                                                          * {
+                                                      'Mounted' or image.status ==
+                                                      'Manual mount'%}
+                                                          * Disk mountpoint: {
                                                             { image.disk_mountpoint
 {% if                                                       }}
-image.status                                                    o {% for volume in
-== 'Mounted'                {% if                                 image.volume_info
-%} {                        image.status {% if                    %}
-{              {            ==           image.status           o [{{ volume.index
-image.rel_path {            'Unmounted'  == 'Mounted'             }}] {
-}} {% else %}  image.status %}           %}                       {
-{              }}             Mount        Unmount                volume.mountpoint
-{                           {% endif %}  {% endif %}              }} {% if
+image.status                                                 Copy to clipboard Copy
+== 'Mounted'                             {% if
+or                          {% if        image.status       Volume mountpoints:
+image.status                image.status == 'Mounted'           o {% for volume in
+== 'Manual     {            ==           or                       image.volume_info {% if image.status == 'Unmounted' %}
+mount'%} {     {            'Unmounted'  image.status             %}                Mountpoint:  [mountpoint_path     ]   Add mountpoint
+{              image.status %}           == 'Manual             o [{{ volume.index  {% endif %}
+image.rel_path }}             Mount      mount'%}                 }}] {
+}} {% else %}               {% endif %}    Unmount                {
+{                                        {% endif %}              volume.mountpoint
+{                                                                 }} {% if
 image.rel_path                                                    volume.mountpoint
 }} {% endif %}                                                    %}
                                                                    Copy to
                                                                   clipboard Copy
                                                                   {% endif %}
                                                                 o {% endfor %}
                                                       {% endif %}
```

### Comparing `thumbtack-0.3.3/src/thumbtack/utils.py` & `thumbtack-0.4.0/src/thumbtack/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
+import json
 import pickle
 import re
 import sqlite3
 import subprocess
 import sys
 
 from pathlib import Path
 
-from flask import current_app, g, abort
+from flask import current_app, g
 
-import imagemounter
+import imagemounter_mitre
 
 from .exceptions import (
     NoMountableVolumesError,
     UnexpectedDiskError,
     ImageNotInDatabaseError,
+    DuplicateMountAttemptError,
 )
 
-
 def get_supported_libraries():
     virtualenv_bin_directory = Path(sys.argv[0]).parent
     imount_cmd = str(virtualenv_bin_directory / "imount")
 
     run_args = [imount_cmd, "--check"]
 
     current_app.logger.info(run_args)
@@ -53,21 +54,22 @@
             ref_count = get_ref_count(rel_path)
             parser = image_info["parser"]
 
             response.append({"disk_info": parser.disks[0], "ref_count": ref_count})
         return response
 
     image_info = get_image_info(image_path)
+
     if not image_info:
         return None
     parser = image_info["parser"]
 
     disk_info = None
     if not parser:
-        abort(404, message=f"Image path {image_path} is not mounted")
+        return None
     else:
         disk_info = parser.disks[0]
 
     ref_count = get_ref_count(image_path)
 
     response = {"disk_info": disk_info, "ref_count": ref_count}
 
@@ -98,15 +100,66 @@
     update_or_insert_db(sql, [rel_path])
     new_ref_count = get_ref_count(rel_path)
     current_app.logger.info(
         f"* Increased ref count for {rel_path}. Now: {new_ref_count}"
     )
 
 
-def mount_image(relative_image_path):
+
+def process_image_parser(image_parser, relative_image_path):
+    # Volumes won't be mounted unless this generator is iterated
+    try:
+        for _ in image_parser.init():
+            pass
+    except Exception:
+        current_app.logger.info(f"* Error mounting volume in {relative_image_path}")
+        pass
+
+    # thumbtack can only handle images that have one disk
+    num_disks = len(image_parser.disks)
+    if num_disks != 1:
+        current_app.logger.error(
+            f"Error: Unexpected number of disks (expected 1, got {num_disks:d})"
+        )
+        image_parser.clean(allow_lazy=True)
+        raise UnexpectedDiskError(
+            f"Unexpected number of disks (expected 1, got {num_disks:d})"
+        )
+
+    """
+    Mountpoints for LVM volumes are not stored in the main mountpoint variable that we check and display in thumbtack.
+    This loop identifies the LVM volumes and add them to the main volumes list.
+    """
+    num_volumes = len(image_parser.disks[0].volumes.volumes)
+    for v in image_parser.disks[0].volumes:
+        if hasattr(v, 'volumes') and v.mountpoint is None:
+            current_app.logger.info(f"Volume: {str(v)}")
+            for vol in v.volumes:
+                current_app.logger.info(f"Mountpoint: {str(vol.mountpoint)}")
+                if vol.mountpoint is not None:
+                    vol.index = str(num_volumes)
+                    num_volumes += 1
+                    image_parser.disks[0].volumes.volumes.append(vol)
+                if hasattr(vol, 'volumes'):
+                    for sub_vol in vol.volumes:
+                        current_app.logger.info(f"Mountpoint: {str(sub_vol.mountpoint)}")
+                        if sub_vol.mountpoint is not None:
+                            sub_vol.index = str(num_volumes)
+                            num_volumes += 1
+                            image_parser.disks[0].volumes.volumes.append(sub_vol)
+
+    # Fail if we couldn't mount any of the volumes
+    if not [v for v in image_parser.disks[0].volumes if v.mountpoint]:
+        image_parser.clean(allow_lazy=True)
+        msg = f"* No mountable volumes in image {relative_image_path}"
+        current_app.logger.error(msg)
+        raise NoMountableVolumesError(msg)
+    return image_parser
+
+def mount_image(relative_image_path, creds=None):
     mount_dir = current_app.config["MOUNT_DIR"]
     if not mount_dir:
         msg = "Mount directory is not properly set by thumbtack server"
         current_app.logger.error(msg)
         raise NotADirectoryError(msg)
 
     full_image_path = f"{current_app.config['IMAGE_DIR']}/{relative_image_path}"
@@ -118,46 +171,60 @@
 
     # Verify we have a valid file path
     if not os.access(full_image_path, os.R_OK):
         msg = f"* {relative_image_path} is not a valid file or is not accessible for reading"
         current_app.logger.error(msg)
         raise PermissionError(msg)
 
+    # Check if the image is currently mounted
+    if image_info["status"] == "Mounted" or image_info["status"] == "Manual mount":
+        increment_ref_count(relative_image_path)
+        current_app.logger.info(f"* {relative_image_path} is already mounted")
+        return image_info["parser"].disks[0]
+    elif get_ref_count(relative_image_path) == 1:
+        msg = f"* Mount attempt in progress for {relative_image_path}"
+        current_app.logger.info(f"{msg}")
+        raise DuplicateMountAttemptError(msg)
+
     # Mount it
     current_app.logger.info(f'* Mounting image_path "{relative_image_path}"')
-    image_parser = imagemounter.ImageParser(
-        [full_image_path], pretty=True, mountdir=mount_dir
-    )
-
-    # Volumes won't be mounted unless this generator is iterated
-    for _ in image_parser.init():
-        pass
 
-    if image_info["status"] == "Mounted":
-        increment_ref_count(relative_image_path)
-        current_app.logger.info(f"* {relative_image_path} is already mounted")
-        return image_parser.disks[0]
+    # Set reference count to 1 to indicate we currently attempting to mount the image.
+    sql = """UPDATE disk_images
+                 SET ref_count = 1
+                 WHERE rel_path = ?
+          """
+    update_or_insert_db(sql, [relative_image_path])
 
-    # thumbtack can only handle images that have one disk
-    num_disks = len(image_parser.disks)
-    if num_disks != 1:
-        current_app.logger.error(
-            f"Error: Unexpected number of disks (expected 1, got {num_disks:d})"
+    no_mountable_volumes = False
+    try:
+        image_parser = imagemounter_mitre.ImageParser(
+            [full_image_path], pretty=True, mountdir=mount_dir, keys=creds
         )
-        image_parser.clean(allow_lazy=True)
-        raise UnexpectedDiskError(
-            f"Unexpected number of disks (expected 1, got {num_disks:d})"
-        )
-
-    # Fail if we couldn't mount any of the volumes
-    if not [v for v in image_parser.disks[0].volumes if v.mountpoint]:
-        image_parser.clean(allow_lazy=True)
-        msg = f"* No mountable volumes in image {relative_image_path}"
-        current_app.logger.error(msg)
-        raise NoMountableVolumesError(msg)
+        image_parser = process_image_parser(image_parser, relative_image_path)
+    except NoMountableVolumesError as e:
+        no_mountable_volumes = True
+        current_app.logger.error(f"* No mountable volumes in image {relative_image_path}. Attempting to mount with qemu-nbd")
+    if no_mountable_volumes:
+        try:
+            image_parser = imagemounter_mitre.ImageParser(
+                [full_image_path], pretty=True, mountdir=mount_dir, disk_mounter='qemu-nbd', keys=creds
+            )
+            image_parser = process_image_parser(image_parser, relative_image_path)
+        except NoMountableVolumesError as e:
+            no_mountable_volumes = True
+            msg = f"* No mountable volumes in image {relative_image_path}"
+
+            # Set ref count to 0 to indicate the mount attempt failed and is no longer in progress
+            sql = """UPDATE disk_images
+                         SET ref_count = 0
+                         WHERE rel_path = ?
+                  """
+            update_or_insert_db(sql, [relative_image_path])
+            raise NoMountableVolumesError(msg)
 
     mount_codes = get_mount_codes()
     disk_mount_status_id = (
         mount_codes["Mounted"]
         if image_parser.disks[0].mountpoint
         else mount_codes["Unable to mount"]
     )
@@ -203,42 +270,103 @@
             sql = "INSERT INTO volumes (disk_id, mount_status_id, partition_index, mountpoint) VALUES (?, ?, ?, ?)"
             update_or_insert_db(
                 sql, [disk_image_id, mount_status_id, v_index, v_mountpoint]
             )
 
     return image_parser.disks[0]
 
+def add_mountpoint(relative_image_path, mountpoint_path):
+    # Get image information and mount codes
+    image_info = get_image_info(relative_image_path)
+    mount_codes = get_mount_codes()
+    disk_mount_status_id = (mount_codes["Manual mount"])
+
+    full_image_path = f"{current_app.config['IMAGE_DIR']}/{relative_image_path}"
+    mount_dir = mountpoint_path
+
+    # Update disk_images table
+    sql = """UPDATE disk_images
+                 SET ref_count = 1, mountpoint = ?, mount_status_id = ?, parser = ?
+                 WHERE rel_path = ?
+          """
+
+    image_parser = imagemounter_mitre.ImageParser(
+        [full_image_path], pretty=True, mountdir=mount_dir
+    )
+
+
+
+    disk = image_parser.disks[0]
+
+    volume = imagemounter_mitre.volume.Volume(disk)
+    filesystem = imagemounter_mitre.filesystems.UnknownFileSystem(volume)
+    filesystem.mountpoint = mountpoint_path
+    volume.filesystem = filesystem
+
+    disk.volumes = [volume]
+    image_parser.disks[0].volumes = volume
+
+    #image_parser.disks.append(disk)
+
+    img_parser_pickle = pickle.dumps(image_parser)
+
+    update_or_insert_db(
+        sql,
+        [
+            mountpoint_path,
+            disk_mount_status_id,
+            sqlite3.Binary(img_parser_pickle),
+            relative_image_path,
+        ],
+    )
+
+    # Update volumes
+    disk_image_id = image_info["id"]
+    mount_status_id = (mount_codes["Manual mount"])
+    v_index = 0
+    sql = "INSERT INTO volumes (disk_id, mount_status_id, partition_index, mountpoint) VALUES (?, ?, ?, ?)"
+    update_or_insert_db(sql, [disk_image_id, mount_status_id, v_index, mountpoint_path])
+    return mountpoint_path
+
 
 def unmount_image(relative_image_path, force=False):
     image_info = get_image_info(relative_image_path)
     mount_codes = get_mount_codes()
     ref_count = image_info["ref_count"]
 
     if ref_count == 1 or force:
         current_app.logger.info(f"* Unmounting {relative_image_path}")
-        image_parser = image_info["parser"]
+        if image_info["status"] == "Mounted":
+            image_parser = image_info["parser"]
 
-        image_parser.clean(allow_lazy=True)
-        current_app.logger.info(f"* Unmounted {relative_image_path} successfully")
+            image_parser.clean(allow_lazy=True)
+            current_app.logger.info(f"* Unmounted {relative_image_path} successfully")
 
         sql = """UPDATE disk_images
                      SET ref_count = 0, mountpoint = NULL, mount_status_id = ?, parser = NULL
                      WHERE rel_path = ?
                  """
         update_or_insert_db(sql, [mount_codes["Unmounted"], relative_image_path])
 
-        sql = """UPDATE volumes
+        if image_info["status"] == "Mounted":
+            sql = """UPDATE volumes
                      SET mountpoint = NULL, mount_status_id = ?
                      WHERE disk_id = ?
                  """
-        update_or_insert_db(sql, [mount_codes["Unmounted"], image_info["id"]])
+            update_or_insert_db(sql, [mount_codes["Unmounted"], image_info["id"]])
+        elif image_info["status"] == "Manual mount":
+            sql = """DELETE FROM volumes
+                     WHERE disk_id = ?
+                 """
+            update_or_insert_db(sql, [image_info["id"]])
         return True
     # ref_count should only ever be 0 or greater, but anything less than 1 means it is not mounted
     elif ref_count < 1:
-        abort(404, message=f"Image path {relative_image_path} is not mounted")
+        current_app.logger.info(f"Image path {relative_image_path} is not mounted")
+        return True
     elif ref_count > 1:
         decrement_ref_count(relative_image_path)
         return False
 
 
 def unmount_all(force=False):
     current_app.logger.info("Unmounting all mounted images")
@@ -285,15 +413,15 @@
     filename = disk_image["filename"]
 
     status = get_mount_status_by_id(disk_image["mount_status_id"])
 
     disk_mountpoint = disk_image["mountpoint"]
 
     volume_info = []
-    if status == "Mounted":
+    if status == "Mounted" or status == "Manual mount":
         for volume in query_db(
             "SELECT * FROM volumes WHERE disk_id = ? ORDER BY partition_index",
             [disk_image["id"]],
         ):
             idx = volume["partition_index"]
 
             # uid is utilized by index.html as an HTML id, so no invalid characters accepted here
@@ -364,15 +492,24 @@
         sql = "INSERT INTO disk_images (full_path, rel_path, filename, mount_status_id) VALUES (?, ?, ?, ?)"
         update_or_insert_db(sql, [full_path_str, rel_path_str, filename, mount_status])
     # else:
     #     current_app.logger.debug(f"({disk_image['id']}) already in DB: {full_path}")
 
 
 def insert_images():
+    skip_subdirs = None
+    try:
+        skip_subdirs = list(current_app.config["SKIP_SUBDIRECTORY"])
+    except (KeyError, TypeError):
+        pass
+
     for root, dirs, files in os.walk(current_app.config["IMAGE_DIR"]):
+        if skip_subdirs:
+            dirs[:] = [d for d in dirs if d not in skip_subdirs]
+
         for filename in files:
 
             full_path = Path(root, filename)
 
             if check_ignored(full_path):
                 continue
 
@@ -394,15 +531,24 @@
         current_app.logger.debug(f"({disk_image['id']}) is on disk: {full_path}")
 
 
 def remove_images():
     images_in_db = get_images()
     full_path_filenames = []
 
+    skip_subdirs = None
+    try:
+        skip_subdirs = list(current_app.config["SKIP_SUBDIRECTORY"])
+    except (KeyError, TypeError):
+        pass
+
     for root, dirs, files in os.walk(current_app.config["IMAGE_DIR"]):
+        if skip_subdirs:
+            dirs[:] = [d for d in dirs if d not in skip_subdirs]
+
         for filename in files:
             full_path = Path(root, filename)
             full_path_filenames.append(full_path)
 
     # If image in DB is not on disk, remove it from DB
     [
         remove_image(image["full_path"])
@@ -411,15 +557,24 @@
     ]
 
 
 # More efficent than calling insert_images then remove_images which will scan all files twice _and_ hit disk
 def monitor_image_dir():
     full_path_filenames = []
 
+    skip_subdirs = None
+    try:
+        skip_subdirs = list(current_app.config["SKIP_SUBDIRECTORY"])
+    except (KeyError, TypeError):
+        pass
+
     for root, dirs, files in os.walk(current_app.config["IMAGE_DIR"]):
+        if skip_subdirs:
+            dirs[:] = [d for d in dirs if d not in skip_subdirs]
+
         for filename in files:
 
             full_path = Path(root, filename)
             full_path_filenames.append(full_path)
 
             if check_ignored(full_path):
                 continue
@@ -483,15 +638,15 @@
             FOREIGN KEY(mount_status_id) REFERENCES mount_status_codes(id)
             )"""
         db.cursor().execute(sql)
         db.commit()
 
         # insert status codes
         sql = "INSERT INTO mount_status_codes (status) VALUES (?)"
-        status_codes = ["Mounted", "Unable to mount", "Unmounted"]
+        status_codes = ["Mounted", "Unable to mount", "Unmounted", "Manual mount"]
         for code in status_codes:
             update_or_insert_db(sql, [code])
 
         insert_images()
 
 
 def query_db(query, args=(), one=False):
@@ -535,13 +690,24 @@
         return True
 
     # Ignore *-sXXX.vmdk, but not *.vmdk
     if re.match(r".*\-s\w\w\w\.vmdk$", full_path_str, flags=re.I):
         return True
 
     # Ignore  *-1.vhd, *-2.vhd, ...,  *-N.vhd, but not *-0.vhd
-    if re.match(r".*\-\w+\.vhd$", full_path_str, flags=re.I) and not re.match(
+    if re.match(r".*\-\d+\.vhd$", full_path_str, flags=re.I) and not re.match(
         r".*\-0\.vhd$", full_path_str, flags=re.I
     ):
         return True
 
+    # Ignore file not matching path_contains if specified
+    path_contains = None
+    try:
+        path_contains = current_app.config["PATH_CONTAINS"]
+    except KeyError:
+        pass
+
+    # Ignore file paths not containing specified string if applicable
+    if path_contains is not None and path_contains not in full_path_str:
+        return True
+
     return False
```

### Comparing `thumbtack-0.3.3/src/thumbtack.egg-info/PKG-INFO` & `thumbtack-0.4.0/src/thumbtack.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbtack
-Version: 0.3.3
+Version: 0.4.0
 Summary: Service to manage disk image mounts.
 Home-page: https://github.com/mitre/thumbtack
 Author: The MITRE Corporation
 Author-email: thumbtack@mitre.org
 License: Apache 2.0
 Description: 
         .. image:: https://travis-ci.org/mitre/thumbtack.svg?branch=master
@@ -43,22 +43,26 @@
         
         .. code-block:: bash
         
             $ thumbtack --help
             Usage: thumbtack [OPTIONS]
         
             Options:
-              -d, --debug           Run the Thumbtack server in debug mode
-              -h, --host TEXT       Host to run Thumbtack server on  [default: 127.0.0.1]
-              -p, --port TEXT       Port to run Thumbtack server on  [default: 8208]
-              -i, --image-dir TEXT  Directory of disk images for Thumbtack server to
-                                    monitor  [default: $CWD]
-              --db TEXT             SQLite database to store mount state  [default:
-                                    database.db]
-              --help                Show this message and exit.
+              -d, --debug                   Run the Thumbtack server in debug mode
+              -h, --host TEXT               Host to run Thumbtack server on  [default: 127.0.0.1]
+              -p, --port TEXT               Port to run Thumbtack server on  [default: 8208]
+              -m, --mount-dir TEXT          Directory to mount disk images  [Default: /mnt/thumbtack]
+              -i, --image-dir TEXT          Directory of disk images for Thumbtack server to
+                                            monitor  [default: $CWD]
+              --db TEXT                     SQLite database to store mount state  [default:
+                                            database.db]
+              -b, --base-url TEXT           Base URL where Thumbtack is hosted on the server
+              --path-contains TEXT          Only select files containing specified string in the path
+              -s, --skip-subdirectory TEXT  Subdirectory to ignore when monitoring files
+              --help                        Show this message and exit.
         
         LICENSE
         -------
         
         Thumbtack is licensed under the `Apache License, Version 2.0
         <https://www.apache.org/licenses/LICENSE-2.0.html>`_. See the `LICENSE` file for
         more information.
```

### Comparing `thumbtack-0.3.3/src/thumbtack.egg-info/SOURCES.txt` & `thumbtack-0.4.0/src/thumbtack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

