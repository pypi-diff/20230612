# Comparing `tmp/reddit2pdf-1.0.0.tar.gz` & `tmp/reddit2pdf-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit2pdf-1.0.0.tar", max compression
+gzip compressed data, was "reddit2pdf-1.1.0.tar", max compression
```

## Comparing `reddit2pdf-1.0.0.tar` & `reddit2pdf-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      395 2023-06-11 21:16:09.101631 reddit2pdf-1.0.0/README.md
--rw-r--r--   0        0        0      467 2023-06-11 21:16:09.101631 reddit2pdf-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-11 21:16:09.101631 reddit2pdf-1.0.0/reddit2pdf/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-11 21:16:09.101631 reddit2pdf-1.0.0/reddit2pdf/__main__.py
--rw-r--r--   0        0        0     2980 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/bdfrjsonhelper.py
--rw-r--r--   0        0        0     1814 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/configuration.py
--rw-r--r--   0        0        0     1106 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/html2pdf.py
--rw-r--r--   0        0        0     3420 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/htmlwriter.py
--rw-r--r--   0        0        0     1508 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/json2html.py
--rw-r--r--   0        0        0     3663 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/library.py
--rw-r--r--   0        0        0     3822 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/reddit2pdf.py
--rw-r--r--   0        0        0     2636 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/comments.html
--rw-r--r--   0        0        0       99 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/footer.html
--rw-r--r--   0        0        0      209 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/gallery.html
--rw-r--r--   0        0        0      884 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/header.html
--rw-r--r--   0        0        0      111 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/page.html
--rw-r--r--   0        0        0     1779 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/post.html
--rw-r--r--   0        0        0     6089 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/templates/style.css
--rw-r--r--   0        0        0     1699 2023-06-11 21:16:09.105631 reddit2pdf-1.0.0/reddit2pdf/url2bdfr.py
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 reddit2pdf-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      395 2023-06-12 01:37:48.364192 reddit2pdf-1.1.0/README.md
+-rw-r--r--   0        0        0      467 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0       70 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/__main__.py
+-rw-r--r--   0        0        0     2980 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/bdfrjsonhelper.py
+-rw-r--r--   0        0        0     1814 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/configuration.py
+-rw-r--r--   0        0        0     1106 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/html2pdf.py
+-rw-r--r--   0        0        0     4092 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/htmlwriter.py
+-rw-r--r--   0        0        0     1730 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/json2html.py
+-rw-r--r--   0        0        0     3663 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/library.py
+-rw-r--r--   0        0        0     4166 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/reddit2pdf.py
+-rw-r--r--   0        0        0     2636 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/templates/comments.html
+-rw-r--r--   0        0        0       99 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/templates/footer.html
+-rw-r--r--   0        0        0      209 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/templates/gallery.html
+-rw-r--r--   0        0        0      884 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/templates/header.html
+-rw-r--r--   0        0        0      111 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/templates/page.html
+-rw-r--r--   0        0        0     1779 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/templates/post.html
+-rw-r--r--   0        0        0     6089 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/templates/style.css
+-rw-r--r--   0        0        0     1699 2023-06-12 01:37:48.368192 reddit2pdf-1.1.0/reddit2pdf/url2bdfr.py
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 reddit2pdf-1.1.0/PKG-INFO
```

### Comparing `reddit2pdf-1.0.0/reddit2pdf/__main__.py` & `reddit2pdf-1.1.0/reddit2pdf/__main__.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/bdfrjsonhelper.py` & `reddit2pdf-1.1.0/reddit2pdf/bdfrjsonhelper.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/configuration.py` & `reddit2pdf-1.1.0/reddit2pdf/configuration.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/html2pdf.py` & `reddit2pdf-1.1.0/reddit2pdf/html2pdf.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/htmlwriter.py` & `reddit2pdf-1.1.0/reddit2pdf/htmlwriter.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import shutil
 import subprocess
 import time
 
 import jinja2
 import markdown
 
+import reddit2pdf.library as library
+
 logger = logging.getLogger(__name__)
 
 templateLoader = jinja2.ChoiceLoader(
     [
         jinja2.FileSystemLoader(searchpath="./reddit2pdf/templates"),
         jinja2.PackageLoader("reddit2pdf", "templates"),
     ]
@@ -98,7 +100,27 @@
     else:
         try:
             data = pkgutil.get_data(__name__, "templates/style.css")
             with open(css_output_path, "wb") as file:
                 file.write(data)
         except Exception as e:
             logger.error(e)
+
+
+def remove_css_file(output):
+    css_output_path = os.path.join(output, "style.css")
+    if os.path.exists(css_output_path):
+        os.remove(css_output_path)
+
+
+def combine_to_single_html(filepath):
+    # monolith https://teddit.net/r/ObsidianMD/comments/12gfs0k/my_new_look_using_callouts/ -o test.html
+    cmd = f"monolith {filepath} -o {filepath}"
+
+    # Run the command with logging
+    library.run_command(cmd)
+
+    # Check that the html file exists in the directory
+    assert os.path.exists(filepath), f"HTML file '{filepath}' does not exist"
+
+    logging.debug(f"Created HTML archive file: {filepath}")
+    return filepath
```

### Comparing `reddit2pdf-1.0.0/reddit2pdf/json2html.py` & `reddit2pdf-1.1.0/reddit2pdf/json2html.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,11 +32,17 @@
 
             # Move + log media
             post = htmlwriter.find_matching_media(post, bdfr_json_dir, bdfr_json_dir)
 
             # Create HTML collateral
             htmlwriter.write_post_to_file(post, bdfr_json_dir)
             htmlwriter.populate_css_file(bdfr_json_dir)
+
+            # Convert to single HTML
+            htmlwriter.combine_to_single_html(post["filepath"])
+            htmlwriter.remove_css_file(
+                bdfr_json_dir
+            )  # Remove now that we have archived
         except Exception as e:
             logging.error(f"Processing post {post['id']} has failed due to: {str(e)}")
 
     return bdfr_json_dir
```

### Comparing `reddit2pdf-1.0.0/reddit2pdf/library.py` & `reddit2pdf-1.1.0/reddit2pdf/library.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/reddit2pdf.py` & `reddit2pdf-1.1.0/reddit2pdf/reddit2pdf.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,34 +15,42 @@
     indir: str, outdir: str, include_media: bool = False, include_html: bool = False
 ):
     # Get a list of files in the input directory
     files = os.listdir(indir)
 
     # Loop through the files and move any pdfs to the output directory
     pdf_count = 0
+    output_files = {"pdf": None, "media": [], "html": None}
     for file in files:
         if file.endswith(".pdf"):
             if os.path.exists(os.path.join(outdir, file)):
                 logging.warning(
                     f"PDF file already existed in outdir: {outdir}. Replacing..."
                 )
                 os.remove(os.path.join(outdir, file))
 
+            if output_files["pdf"]:
+                raise ValueError(
+                    f"{pdf_count} PDF files were moved. Please ensure that exactly one PDF file is present in {indir}."
+                )
+
             shutil.move(os.path.join(indir, file), os.path.join(outdir, file))
-            pdf_count += 1
+            output_files["pdf"] = os.path.join(outdir, file)
             logging.info(f"Moved PDF file {file} from {indir} to {outdir}")
-        elif (file.endswith(".html") or file.endswith(".css")) and include_html:
+
+        elif file.endswith(".html") and include_html:
             if os.path.exists(os.path.join(outdir, file)):
                 logging.warning(
                     f"HTML file already existed in outdir: {outdir}. Replacing..."
                 )
                 os.remove(os.path.join(outdir, file))
 
             shutil.move(os.path.join(indir, file), os.path.join(outdir, file))
-            logging.info(f"Moved HTL file {file} from {indir} to {outdir}")
+            output_files["html"] = os.path.join(outdir, file)
+            logging.info(f"Moved HTML file {file} from {indir} to {outdir}")
         elif include_media:
             # If include_media is True, move any files with media extensions to the output directory
             media_extensions = [
                 ".jpg",
                 ".jpeg",
                 ".png",
                 ".gif",
@@ -63,20 +71,16 @@
                 if os.path.exists(os.path.join(outdir, file)):
                     logging.debug(
                         f"Media file already existed in output. Skipping {file}"
                     )
                 else:
                     shutil.move(file_path, os.path.join(outdir, file))
                     logging.info(f"Moved media file {file} from {indir} to {outdir}")
-
-    # Check that exactly one PDF file was moved
-    if pdf_count != 1:
-        raise ValueError(
-            f"{pdf_count} PDF files were moved. Please ensure that exactly one PDF file is present in {indir}."
-        )
+                output_files["media"].append(os.path.join(outdir, file))
+    return output_files
 
 
 def reddit2pdf(conf: Configuration):
     # Generate temporary directory to store all bdfr + html intermediaries
     tempdir = tempfile.mkdtemp(suffix="reddit2pdf", dir="/tmp")
     # Use BDFR to download the reddit URL to the temp directory
     bdfr_dir = url2bdfr.download_reddit_url(conf.link, tempdir)
@@ -87,12 +91,17 @@
     logging.info(f"Generated PDF: {pdf_path}")
 
     if not os.path.exists(conf.outdir):
         logging.info(f"Outdir {conf.outdir} did not exist. Creating...")
         os.makedirs(conf.outdir, exist_ok=True)
 
     # Move desired collateral to output directory
-    _move_collateral(tempdir, conf.outdir, conf.move_media, conf.move_html)
+    output_collateral = _move_collateral(
+        tempdir, conf.outdir, conf.move_media, conf.move_html
+    )
 
     # Destroy temp directory
     if not conf.unclean:
         os.remove(tempdir)
+
+    logging.info(f"Generated collateral: {output_collateral}")
+    return output_collateral
```

### Comparing `reddit2pdf-1.0.0/reddit2pdf/templates/comments.html` & `reddit2pdf-1.1.0/reddit2pdf/templates/comments.html`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/templates/header.html` & `reddit2pdf-1.1.0/reddit2pdf/templates/header.html`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/templates/post.html` & `reddit2pdf-1.1.0/reddit2pdf/templates/post.html`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/templates/style.css` & `reddit2pdf-1.1.0/reddit2pdf/templates/style.css`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/reddit2pdf/url2bdfr.py` & `reddit2pdf-1.1.0/reddit2pdf/url2bdfr.py`

 * *Files identical despite different names*

### Comparing `reddit2pdf-1.0.0/PKG-INFO` & `reddit2pdf-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit2pdf
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 License: MIT
 Author: David Cabinian
 Author-email: dhcabinian@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

