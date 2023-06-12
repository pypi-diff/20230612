# Comparing `tmp/epub2txt-0.1.4.tar.gz` & `tmp/epub2txt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epub2txt-0.1.4.tar", max compression
+gzip compressed data, was "epub2txt-0.1.5.tar", max compression
```

## Comparing `epub2txt-0.1.4.tar` & `epub2txt-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       95 2023-06-11 09:07:45.248748 epub2txt-0.1.4/epub2txt/__init__.py
--rw-r--r--   0        0        0     4911 2023-06-11 07:08:44.299392 epub2txt-0.1.4/epub2txt/__main__.py
--rw-r--r--   0        0        0      821 2023-06-11 07:07:56.005713 epub2txt-0.1.4/epub2txt/browse_filename.py
--rw-r--r--   0        0        0     5093 2023-06-11 09:06:34.713343 epub2txt-0.1.4/epub2txt/epub2txt.py
--rw-r--r--   0        0        0     1357 2023-06-11 07:07:56.045712 epub2txt-0.1.4/epub2txt/gen_filename.py
--rw-r--r--   0        0        0     1091 2021-02-07 07:51:04.577682 epub2txt-0.1.4/LICENSE
--rw-r--r--   0        0        0      614 2023-06-11 09:07:37.594793 epub2txt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1835 2023-06-11 09:18:38.643579 epub2txt-0.1.4/README.md
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 epub2txt-0.1.4/setup.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 epub2txt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       95 2023-06-12 05:26:19.373424 epub2txt-0.1.5/epub2txt/__init__.py
+-rw-r--r--   0        0        0     4911 2023-06-11 07:08:44.299392 epub2txt-0.1.5/epub2txt/__main__.py
+-rw-r--r--   0        0        0      821 2023-06-12 05:23:52.104528 epub2txt-0.1.5/epub2txt/browse_filename.py
+-rw-r--r--   0        0        0     5158 2023-06-12 05:19:30.110277 epub2txt-0.1.5/epub2txt/epub2txt.py
+-rw-r--r--   0        0        0     1357 2023-06-11 07:07:56.045712 epub2txt-0.1.5/epub2txt/gen_filename.py
+-rw-r--r--   0        0        0     1091 2021-02-07 07:51:04.577682 epub2txt-0.1.5/LICENSE
+-rw-r--r--   0        0        0      633 2023-06-12 05:25:55.878750 epub2txt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1835 2023-06-11 09:18:38.643579 epub2txt-0.1.5/README.md
+-rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 epub2txt-0.1.5/setup.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 epub2txt-0.1.5/PKG-INFO
```

### Comparing `epub2txt-0.1.4/epub2txt/__main__.py` & `epub2txt-0.1.5/epub2txt/__main__.py`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.4/epub2txt/browse_filename.py` & `epub2txt-0.1.5/epub2txt/browse_filename.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         title="Select a file",
         filetypes=(
             ("epub files", "*.epub"),
             ("all files", "*.*"),
         )
 ):
     # fmt: on
-    '''Browse for a filename.'''
+    """Browse for a filename."""
     root = Tkinter.Tk()
     root.withdraw()
     filename = tkFileDialog.askopenfilename(
         parent=root,
         initialdir=initialdir,
         title=title,
         filetypes=filetypes,
```

### Comparing `epub2txt-0.1.4/epub2txt/epub2txt.py` & `epub2txt-0.1.5/epub2txt/epub2txt.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,16 @@
 
     names = [elm.get_name() for elm in book.get_items_of_type(ebooklib.ITEM_DOCUMENT)]
 
     epub2txt.names = names
 
     # content/chapter titles
     # remove bookmark #: most toc_hrefs correspond to names
-    _ = [Path(elm).with_suffix('.xhtml').as_posix() for elm in epub2txt.toc_hrefs]
+    # _ = [Path(elm).with_suffix('.xhtml').as_posix() for elm in epub2txt.toc_hrefs]
+    _ = [elm.rsplit("#", 1)[0] for elm in epub2txt.toc_hrefs]
     name2title = dict(zip(_, epub2txt.toc_titles))
 
     epub2txt.content_titles = [name2title.get(name, "NA") for name in names]
 
     # texts = [pq(content).text() for content in contents]
 
     # Using XPath to find text
```

### Comparing `epub2txt-0.1.4/epub2txt/gen_filename.py` & `epub2txt-0.1.5/epub2txt/gen_filename.py`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.4/LICENSE` & `epub2txt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.4/pyproject.toml` & `epub2txt-0.1.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epub2txt"
-version = "0.1.4"
+version = "0.1.5"
 description = "Convert epub to txt with additonal utils"
 authors = ["freemt"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ffreemt/epub2txt"
 
 [tool.poetry.dependencies]
@@ -20,11 +20,12 @@
 pytest = "^5.2"
 
 [tool.poetry.scripts]
 epub2txt = "epub2txt.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
+ipython = "8.12.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `epub2txt-0.1.4/README.md` & `epub2txt-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.4/setup.py` & `epub2txt-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'tqdm>=4.56.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['epub2txt = epub2txt.__main__:main']}
 
 setup_kwargs = {
     'name': 'epub2txt',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Convert epub to txt with additonal utils',
     'long_description': '# epub2txt [![Codacy Badge](https://app.codacy.com/project/badge/Grade/05c422da73a14c23b87b0657af9c8df7)](https://www.codacy.com/gh/ffreemt/epub2txt/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ffreemt/epub2txt&amp;utm_campaign=Badge_Grade)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/epub2txt.svg)](https://badge.fury.io/py/epub2txt)\n\nConvert epub to txt with additonal utils\n\n<!--- Refer to dualtext-epub\\der_fanger_de_en.py\n\t\t__main__.py refer to tmx2epub.__main__\n--->\n\n## Installation\n\n```bash\npip install epub2txt\n# pip install epub2txt -U  # to upgrade\n```\n## Fixes\n* More resilent to mismatched tags\n* Added `epub2txt.content_titles`, useful for creating metada when needed\n\n## Usage\n\n### From command line\n\n```bash\n# convert test.epub to test.txt\nepub2txt -f test.epub\n\n# browse for epub file, txt file will be in the same directory as the epub file\nepub2txt\n\n# show epub book info: title and toc\nepub2txt -i\n\n# show more epub book info: title, toc, metadata, spine (list of stuff packed into the epub)\nepub2txt -m\n\n# show epub2txt version\nepub2txt -V\n\n```\n\n### `python` code\n\n```python\nfrom epub2txt import epub2txt\n# from a url to epub\nurl = "https://github.com/ffreemt/tmx2epub/raw/master/tests/1.tmx.epub"\nres = epub2txt(url)\n\n# from a local epub file\nfilepath = r"tests\\test.epub"\nres = epub2txt(filepath)\n\n# output as a list of chapters\nch_list = epub2txt(filepath, outputlist=True)\n# chapter titles will be available as epub2txt.content_titles if available\n\n```\n\n## TODO\n*   Batch conversion of several epub files\n\n',
     'author': 'freemt',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ffreemt/epub2txt',
```

### Comparing `epub2txt-0.1.4/PKG-INFO` & `epub2txt-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epub2txt
-Version: 0.1.4
+Version: 0.1.5
 Summary: Convert epub to txt with additonal utils
 Home-page: https://github.com/ffreemt/epub2txt
 License: MIT
 Author: freemt
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

