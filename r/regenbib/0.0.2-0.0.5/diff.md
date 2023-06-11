# Comparing `tmp/regenbib-0.0.2.tar.gz` & `tmp/regenbib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regenbib-0.0.2.tar", max compression
+gzip compressed data, was "regenbib-0.0.5.tar", max compression
```

## Comparing `regenbib-0.0.2.tar` & `regenbib-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-05-02 01:39:23.906584 regenbib-0.0.2/LICENSE
--rw-r--r--   0        0        0       61 2023-05-02 01:39:23.906584 regenbib-0.0.2/README.md
--rw-r--r--   0        0        0      812 2023-05-02 02:40:15.020088 regenbib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 02:39:13.284829 regenbib-0.0.2/regenbib/__init__.py
--rw-r--r--   0        0        0     6911 2023-05-02 02:32:02.813995 regenbib-0.0.2/regenbib/cli_import.py
--rw-r--r--   0        0        0      971 2023-05-02 02:32:05.397964 regenbib-0.0.2/regenbib/cli_render.py
--rw-r--r--   0        0        0     4320 2023-05-02 02:32:09.121919 regenbib-0.0.2/regenbib/store.py
--rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 regenbib-0.0.2/setup.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 regenbib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-02 01:39:23.906584 regenbib-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4467 2023-05-02 19:58:01.560973 regenbib-0.0.5/README.md
+-rw-r--r--   0        0        0      812 2023-06-11 22:43:39.555580 regenbib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 02:39:13.284829 regenbib-0.0.5/regenbib/__init__.py
+-rw-r--r--   0        0        0     7677 2023-05-10 04:49:14.758026 regenbib-0.0.5/regenbib/cli_import.py
+-rw-r--r--   0        0        0     1282 2023-05-02 04:53:00.069837 regenbib-0.0.5/regenbib/cli_render.py
+-rw-r--r--   0        0        0     4320 2023-05-02 05:41:52.242372 regenbib-0.0.5/regenbib/store.py
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 regenbib-0.0.5/setup.py
+-rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 regenbib-0.0.5/PKG-INFO
```

### Comparing `regenbib-0.0.2/LICENSE` & `regenbib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `regenbib-0.0.2/pyproject.toml` & `regenbib-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "regenbib"
-version = "0.0.2"
+version = "0.0.5"
 description = "(Re-)generate tidy .bib files from online sources"
 authors = ["Joachim Neu <jneu@stanford.edu>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/joachimneu/regenbib"
 repository = "https://github.com/joachimneu/regenbib"
 documentation = "https://github.com/joachimneu/regenbib"
@@ -14,16 +14,16 @@
 [tool.poetry.scripts]
 regenbib = 'regenbib.cli_render:run'
 regenbib-import = 'regenbib.cli_import:run'
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-bibtex-dblp = "^0.5"
-marshmallow-dataclass = { version = "8.5.11", extras = ["enum", "union"] }
+bibtex-dblp = "^0.9"
+marshmallow-dataclass = { version = "8.5.14", extras = ["enum", "union"] }
 arxiv = "^1.4.7"
 beautifulsoup4 = "^4.12.2"
 requests = "^2.29.0"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `regenbib-0.0.2/regenbib/cli_import.py` & `regenbib-0.0.5/regenbib/cli_import.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #! /usr/bin/env python3
 
-from .store import Store
+import argparse
+import re
 import bibtex_dblp.dblp_data
 import bibtex_dblp.dblp_api
 import bibtex_dblp.io
 import bibtex_dblp.database
-import sys
-import re
+from .store import Store
 
 
 def format_dblp_publication(pub: bibtex_dblp.dblp_data.DblpPublication):
     authors = ", ".join([str(author) for author in pub.authors])
     book = ""
     if pub.venue:
         book += pub.venue + (" ({})".format(pub.volume) if pub.volume else "")
@@ -41,15 +41,15 @@
         return ("cancelled", None)
 
     publication = search_results.results[select - 1].publication
     return ("found", publication.key)
 
 
 def import_dblp_free_search(bibtexid):
-    from store import DblpEntry
+    from .store import DblpEntry
 
     while True:
         search_query = bibtex_dblp.io.get_user_input(
             "---> DBLP query [<empty>=abort]: ")
         if search_query == "":
             return None
         (status, key) = search_key_on_dblp(search_query)
@@ -61,29 +61,29 @@
         elif status == "found":
             return DblpEntry(bibtexid, key)
         else:
             raise NotImplementedError()
 
 
 def import_dblp_search_title(bibtexid, entry_old):
-    from store import DblpEntry
+    from .store import DblpEntry
 
     search_query = entry_old.fields['title']
     (status, key) = search_key_on_dblp(search_query)
 
     if status == "cancelled" or status == "not-found":
         return None
     elif status == "found":
         return DblpEntry(bibtexid, key)
     else:
         raise NotImplementedError()
 
 
 def import_dblp_search_authortitle(bibtexid, entry_old):
-    from store import DblpEntry
+    from .store import DblpEntry
 
     authors = ", ".join([str(author)
                         for author in entry_old.persons['author']])
     search_query = "{} {}".format(authors, entry_old.fields['title'])
     (status, key) = search_key_on_dblp(search_query)
 
     if status == "cancelled" or status == "not-found":
@@ -91,36 +91,36 @@
     elif status == "found":
         return DblpEntry(bibtexid, key)
     else:
         raise NotImplementedError()
 
 
 def import_current_raw_entry(bibtexid, entry_old):
-    from store import RawBibtexEntry
+    from .store import RawBibtexEntry
 
     return RawBibtexEntry.from_pybtex_entry(bibtexid, entry_old)
 
 
 def import_arxiv_manualid(bibtexid):
-    from store import ArxivEntry
+    from .store import ArxivEntry
 
     while True:
         manual = bibtex_dblp.io.get_user_input(
             "---> arXiv ID [<empty>=abort]: ")
         if manual == "":
             return None
 
         try:
             return ArxivEntry.from_manual(bibtexid, manual)
         except AssertionError:
             print("---> Assertion on parsing manual input, retry!")
 
 
 def import_eprint_manualid(bibtexid):
-    from store import EprintEntry
+    from .store import EprintEntry
 
     while True:
         manual = bibtex_dblp.io.get_user_input(
             "---> IACR ePrint ID [<empty>=abort]: ")
         if manual == "":
             return None
 
@@ -144,46 +144,61 @@
             if ret != None:
                 return ret
             else:
                 continue
 
 
 def run():
+    parser = argparse.ArgumentParser(
+        description='Import bibliography entries from  DBLP.')
+    parser.add_argument('--bib', metavar='BIB_FILE', type=str,
+                        default='references.bib', help='File name of .bib file')
+    parser.add_argument('--aux', metavar='AUX_FILE', type=str,
+                        default='_build/main.aux', help='File name of .aux file')
+    parser.add_argument('--yaml', metavar='YAML_FILE', type=str,
+                        default='references.yaml', help='File name of .yaml file')
+    args = parser.parse_args()
+
     METHODS_WITHOUT_OLDENTRY = [
         ('dblp-free-search', import_dblp_free_search),
         ('arxiv-manual-id', import_arxiv_manualid),
         ('eprint-manual-id', import_eprint_manualid),
     ]
 
     METHODS_WITH_OLDENTRY = [
         ('current-entry', import_current_raw_entry),
         ('dblp-search-title', import_dblp_search_title),
         ('dblp-search-authorstitle', import_dblp_search_authortitle),
     ]
 
-    if len(sys.argv) != 4:
-        print(f"Usage: {sys.argv[0]} <BIB FILE> <AUX FILE> <YAML FILE>")
-        exit(1)
-
-    (BIB_FILE, AUX_FILE, YAML_FILE) = sys.argv[1:]
-
     bibtexids_included = []
-    with open(AUX_FILE, 'r') as infile:
+    with open(args.aux, 'r') as infile:
         for l in infile.readlines():
             l = l.strip()
+
+            # BibLaTeX
             matches = re.findall(r"\\abx@aux@cite\{0\}\{(.*?)\}", l)
             assert len(matches) <= 1
             if matches:
                 m = matches[0]
                 if not m in bibtexids_included:
                     bibtexids_included.append(m)
 
-    store = Store.load_or_empty(YAML_FILE)
+            # BibTeX
+            matches = re.findall(r"\\citation\{(.*?)\}", l)
+            assert len(matches) <= 1
+            if matches:
+                for m in matches[0].split(','):
+                    m = m.strip()
+                    if not m in bibtexids_included:
+                        bibtexids_included.append(m)
+
+    store = Store.load_or_empty(args.yaml)
 
-    bibtex_entries = bibtex_dblp.database.load_from_file(BIB_FILE)
+    bibtex_entries = bibtex_dblp.database.load_from_file(args.bib)
 
     for bibtexid in bibtexids_included:
         if bibtexid in store.bibtexids:
             continue
 
         print("Importing entry:", bibtexid)
 
@@ -191,29 +206,29 @@
             print("-> Not found in .bib file!")
 
             entry = attempt_import([(lambda name, fun: (name, lambda: fun(bibtexid)))(name, fun)
                                     for (name, fun) in METHODS_WITHOUT_OLDENTRY])
 
             if entry != None:
                 store.entries.append(entry)
-                store.dump(YAML_FILE)
+                store.dump(args.yaml)
 
-            store.dump(YAML_FILE)
+            store.dump(args.yaml)
 
         else:
             entry_old = bibtex_entries.entries[bibtexid]
             print("-> Current entry:", entry_old)
 
             entry = attempt_import([(lambda name, fun: (name, lambda: fun(bibtexid)))(name, fun)
                                     for (name, fun) in METHODS_WITHOUT_OLDENTRY]
                                    + [(lambda name, fun: (name, lambda: fun(bibtexid, entry_old)))(name, fun)
                                       for (name, fun) in METHODS_WITH_OLDENTRY])
 
             if entry != None:
                 store.entries.append(entry)
-                store.dump(YAML_FILE)
+                store.dump(args.yaml)
 
-            store.dump(YAML_FILE)
+            store.dump(args.yaml)
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `regenbib-0.0.2/regenbib/store.py` & `regenbib-0.0.5/regenbib/store.py`

 * *Files identical despite different names*

