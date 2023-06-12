# Comparing `tmp/avro.py-2023.4.3.tar.gz` & `tmp/avro.py-2023.6.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro.py-2023.4.3.tar", last modified: Mon Apr  3 06:07:59 2023, max compression
+gzip compressed data, was "avro.py-2023.6.12.tar", last modified: Mon Jun 12 06:52:14 2023, max compression
```

## Comparing `avro.py-2023.4.3.tar` & `avro.py-2023.6.12.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.498247 avro.py-2023.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-03 06:07:47.000000 avro.py-2023.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-03 06:07:47.000000 avro.py-2023.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-03 06:07:59.498247 avro.py-2023.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-03 06:07:47.000000 avro.py-2023.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.494247 avro.py-2023.4.3/avro/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11711 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.498247 avro.py-2023.4.3/avro/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58945 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/resources/avrodict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.498247 avro.py-2023.4.3/avro/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1637 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/utils/count.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2792 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.494247 avro.py-2023.4.3/avro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-03 06:07:59.000000 avro.py-2023.4.3/avro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-03 06:07:59.000000 avro.py-2023.4.3/avro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 06:07:59.000000 avro.py-2023.4.3/avro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-03 06:07:59.000000 avro.py-2023.4.3/avro.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-03 06:07:47.000000 avro.py-2023.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 06:07:59.498247 avro.py-2023.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-04-03 06:07:47.000000 avro.py-2023.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.498247 avro.py-2023.4.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5735 2023-04-03 06:07:47.000000 avro.py-2023.4.3/tests/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-04-03 06:07:47.000000 avro.py-2023.4.3/tests/test_utils_count.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3742 2023-04-03 06:07:47.000000 avro.py-2023.4.3/tests/test_utils_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 06:51:49.000000 avro.py-2023.6.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 06:51:49.000000 avro.py-2023.6.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-12 06:52:14.635330 avro.py-2023.6.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-12 06:51:49.000000 avro.py-2023.6.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.631330 avro.py-2023.6.12/avro/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11695 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/avro/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59054 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/resources/avrodict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/avro/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/utils/count.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2814 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/avro.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-12 06:52:14.000000 avro.py-2023.6.12/avro.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-12 06:52:14.000000 avro.py-2023.6.12/avro.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 06:52:14.000000 avro.py-2023.6.12/avro.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 06:52:14.000000 avro.py-2023.6.12/avro.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 06:51:49.000000 avro.py-2023.6.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 06:52:14.635330 avro.py-2023.6.12/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-06-12 06:51:49.000000 avro.py-2023.6.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5744 2023-06-12 06:51:49.000000 avro.py-2023.6.12/tests/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-06-12 06:51:49.000000 avro.py-2023.6.12/tests/test_utils_count.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3750 2023-06-12 06:51:49.000000 avro.py-2023.6.12/tests/test_utils_validate.py
```

### Comparing `avro.py-2023.4.3/LICENSE` & `avro.py-2023.6.12/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 MIT License
 
 Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.3/PKG-INFO` & `avro.py-2023.6.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2023.4.3
+Version: 2023.6.12
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,avro,avro phonetic,bangla,bangla phonetics,bengali,bengali phonetics
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div align="center">
 
-# <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="35px"/> avro.py
+# <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
 
 A modern Pythonic implementation of the popular Bengali phonetic-typing software **Avro Phonetic.**
 
 [![Downloads](https://static.pepy.tech/personalized-badge/avro-py?period=total&units=international_system&left_color=grey&right_color=black&left_text=Downloads)](https://pepy.tech/project/avro-py)
 ![Python Version](https://img.shields.io/pypi/pyversions/avro.py.svg?color=black&label=Python)
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
@@ -42,21 +42,19 @@
 
 </div>
 
 ## Overview
 
 **avro.py**, being a Python package, provides a text parser that converts English text written in Roman script to its phonetic equivalent of Bengali. It implements the **Avro Phonetic Dictionary Search Library** by [Mehdi Hasan Khan](https://github.com/mugli).
 
-The original project ([pyAvroPhonetic](https://github.com/kaustavdm/pyAvroPhonetic)) can only be used on versions up to **Python 2.7** and doesn't contain proper support for Python's third major version AKA Python 3. It is noteworthy that Python 2 has officially been deprecated by the original maintainers and its usage is being discouraged overall.
-
-<br>
+The original project ([pyAvroPhonetic](https://github.com/kaustavdm/pyAvroPhonetic)) can only be used on versions up to **Python 2.7** and doesn't contain proper support for Python's third major version AKA Python 3. It is noteworthy that Python 2 has officially been deprecated by the original maintainers and its usage is being discouraged overall. <br>
 
 ## Inspirations
 
-This package is inspired from Rifat Nabi's jsAvroPhonetic library and derives from Kaustav Das Modak's pyAvroPhonetic.
+This package is inspired from Rifat Nabi's jsAvroPhonetic library and derives from Kaustav Das Modak's pyAvroPhonetic. 
 
 <br>
 
 ## Installation
 
 This package requires **Python 3.8 or higher** to be used inside your development environment.
 
@@ -89,25 +87,24 @@
 
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 print(reversed_text)
 
 # amar sonar bangla.
 ```
 
-Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally!
+Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally! 
 
 <br>
 
 ## Contributing
 
 :octocat: *Fork -> Do your changes -> Send a Pull Request, it's that easy!* <br>
 
 ---
 
-
 **Additional Developer Notes**
 
 In short, avro.py doesn't depend on any third-party libraries. However, if you'd like to contribute to the project, you'll need a handful of such useful tools. <br>
 
 - [flake8](https://flake8.pycqa.org/en/latest/) - linter
 - [pytest](https://pypi.python.org/pypi/pytest) - testing framework
 - [black](https://github.com/psf/black) - formatting
@@ -119,17 +116,15 @@
 # Running pytest.
 $ python3 -m pytest --verbose
 
 # The results should appear onwards.
 # The --verbose / -v flag is used to show all the test results in detail.
 ```
 
-<br>
-
-### We're looking for bug hunters!
+### We're looking for bug hunters, by the way!
 
 If you come across any kind of bug or wanna request a feature, please let us know by opening an issue [here](https://github.com/hitblast/avro.py/issues). We do need more ideas to keep the project alive and running, don't we? :P
 
 ---
 
 <br>
```

### Comparing `avro.py-2023.4.3/README.md` & `avro.py-2023.6.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
 
-# <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="35px"/> avro.py
+# <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
 
 A modern Pythonic implementation of the popular Bengali phonetic-typing software **Avro Phonetic.**
 
 [![Downloads](https://static.pepy.tech/personalized-badge/avro-py?period=total&units=international_system&left_color=grey&right_color=black&left_text=Downloads)](https://pepy.tech/project/avro-py)
 ![Python Version](https://img.shields.io/pypi/pyversions/avro.py.svg?color=black&label=Python)
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
@@ -20,21 +20,19 @@
 
 </div>
 
 ## Overview
 
 **avro.py**, being a Python package, provides a text parser that converts English text written in Roman script to its phonetic equivalent of Bengali. It implements the **Avro Phonetic Dictionary Search Library** by [Mehdi Hasan Khan](https://github.com/mugli).
 
-The original project ([pyAvroPhonetic](https://github.com/kaustavdm/pyAvroPhonetic)) can only be used on versions up to **Python 2.7** and doesn't contain proper support for Python's third major version AKA Python 3. It is noteworthy that Python 2 has officially been deprecated by the original maintainers and its usage is being discouraged overall.
-
-<br>
+The original project ([pyAvroPhonetic](https://github.com/kaustavdm/pyAvroPhonetic)) can only be used on versions up to **Python 2.7** and doesn't contain proper support for Python's third major version AKA Python 3. It is noteworthy that Python 2 has officially been deprecated by the original maintainers and its usage is being discouraged overall. <br>
 
 ## Inspirations
 
-This package is inspired from Rifat Nabi's jsAvroPhonetic library and derives from Kaustav Das Modak's pyAvroPhonetic.
+This package is inspired from Rifat Nabi's jsAvroPhonetic library and derives from Kaustav Das Modak's pyAvroPhonetic. 
 
 <br>
 
 ## Installation
 
 This package requires **Python 3.8 or higher** to be used inside your development environment.
 
@@ -67,25 +65,24 @@
 
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 print(reversed_text)
 
 # amar sonar bangla.
 ```
 
-Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally!
+Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally! 
 
 <br>
 
 ## Contributing
 
 :octocat: *Fork -> Do your changes -> Send a Pull Request, it's that easy!* <br>
 
 ---
 
-
 **Additional Developer Notes**
 
 In short, avro.py doesn't depend on any third-party libraries. However, if you'd like to contribute to the project, you'll need a handful of such useful tools. <br>
 
 - [flake8](https://flake8.pycqa.org/en/latest/) - linter
 - [pytest](https://pypi.python.org/pypi/pytest) - testing framework
 - [black](https://github.com/psf/black) - formatting
@@ -97,17 +94,15 @@
 # Running pytest.
 $ python3 -m pytest --verbose
 
 # The results should appear onwards.
 # The --verbose / -v flag is used to show all the test results in detail.
 ```
 
-<br>
-
-### We're looking for bug hunters!
+### We're looking for bug hunters, by the way!
 
 If you come across any kind of bug or wanna request a feature, please let us know by opening an issue [here](https://github.com/hitblast/avro.py/issues). We do need more ideas to keep the project alive and running, don't we? :P
 
 ---
 
 <br>
```

### Comparing `avro.py-2023.4.3/avro/__init__.py` & `avro.py-2023.6.12/avro/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## A modern Pythonic implementation of Avro Phonetic.
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
@@ -26,13 +26,13 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
 
 # Set version information.
-__version_info__ = ('2023', '4', '3')  # YYYY / MM / DD
+__version_info__ = ('2023', '6', '12')  # YYYY / MM / DD
 __version__ = '.'.join(__version_info__)
 
 
 # Import local modules.
 from .main import *
```

### Comparing `avro.py-2023.4.3/avro/config.py` & `avro.py-2023.6.12/avro/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## A modern Pythonic implementation of Avro Phonetic.
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
@@ -25,24 +25,17 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
 
-# Import built-in libraries.
-import os
-
 # Import local modules.
 from .resources import AVRO_DICT
 
-
-# Path to current directory.
-BASE_PATH = os.path.dirname(__file__)
-
 # Shortcuts to vowels, constants, case-sensitives and numbers.
 AVRO_VOWELS = set(AVRO_DICT['data']['vowel'])
 AVRO_CONSONANTS = set(AVRO_DICT['data']['consonant'])
 AVRO_CASESENSITIVES = set(AVRO_DICT['data']['casesensitive'])
 AVRO_NUMBERS = set(AVRO_DICT['data']['number'])
 
 # Shortcuts to Bengali Svaravarna, Kar(s)
```

### Comparing `avro.py-2023.4.3/avro/main.py` & `avro.py-2023.6.12/avro/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## A modern Pythonic implementation of Avro Phonetic.
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
@@ -24,23 +24,21 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
-
 # Import third-party modules.
-from typing import Any, List, Dict, Union
+import re
+from typing import Any, Dict, List, Optional, Union
 
 # Import local modules.
 from . import config
 from .utils import validate
-import re
-
 
 # Constants.
 PATTERNS: Any = config.AVRO_DICT['data']['patterns']
 NON_RULE_PATTERNS: list = [p for p in PATTERNS if 'rules' not in p]
 RULE_PATTERNS: list = [p for p in PATTERNS if 'rules' in p]
 
 
@@ -122,17 +120,15 @@
                     output.append(i)
 
         return ''.join(output)
 
     output = []
     for text in texts:  # Applies to non-keyword arguments.
         output.append(
-            subparse(text)
-            if not in_ascii
-            else str(subparse(text).encode('ascii', errors='backslashreplace'))
+            subparse(text) if not in_ascii else str(subparse(text).encode('ascii', errors='backslashreplace'))
         )
 
     return output[0] if len(output) == 1 else output
 
 
 def reverse(*texts: str) -> Union[str, List[str]]:
     '''
@@ -172,15 +168,15 @@
             if not uni_pass:
                 output.append(i)
 
             elif uni_pass:
                 match = match_patterns(text, cur, rule=False, reversed=True)
 
                 if match['matched']:
-                    if not match['reversed'] is None:
+                    if match['reversed']:
                         output.append(match['reversed'])
                     else:
                         output.append(match['found'])
 
                 if not match['matched']:
                     output.append(i)
 
@@ -192,15 +188,15 @@
     # Split using regex to remove noise.
     regex_pattern = "(\\s|\\.|,|\\?|\\।|\\-|;|')"
     compiled_regex = re.compile(regex_pattern, re.UNICODE)
 
     for text in texts:  # Applies to non-keyword arguments.
         exceptions = config.EXCEPTIONS.get(text, None)
 
-        if exceptions is None:
+        if not exceptions:
             separated_texts = compiled_regex.split(text)
 
             for separated_text in separated_texts:
                 text_segments.append(subparse(separated_text))
 
             output.append(''.join(text_segments))
             text_segments = []
@@ -247,15 +243,15 @@
             return {"matched": False, "found": None, "replaced": fixed_text[cur]}
         else:
             return {"matched": False, "found": None, "replaced": fixed_text[cur], "rules": None}
 
 
 def exact_find_in_pattern(
     fixed_text: str, reversed: bool, cur: int = 0, patterns: Any = PATTERNS
-) -> list:
+) -> List[Dict[str, Any]]:
     '''
     ### Returns pattern items that match given text, cursor position and pattern.
     '''
 
     if reversed:
         return [
             x
@@ -263,21 +259,21 @@
             if (cur + len(x['replace']) <= len(fixed_text))
             and x['replace'] == fixed_text[cur : (cur + len(x['replace']))]
         ]
 
     return [
         x
         for x in patterns
-        if (not x.get('find', None) is None)
+        if x.get('find', None)
         and (cur + len(x['find']) <= len(fixed_text))
         and x['find'] == fixed_text[cur : (cur + len(x['find']))]
     ]
 
 
-def reverse_with_rules(cursor: int, fixed_text: str, text_reversed) -> bool:
+def reverse_with_rules(cursor: int, fixed_text: str, text_reversed: str) -> str:
     '''
     ### Enhances the word with rules for reverse-parsing.
     '''
 
     added_suffix = ''
 
     if not (
@@ -293,18 +289,18 @@
             added_suffix = ''
         if fixed_text[cursor + 2] in config.AVRO_KAR and not cursor == 0:
             added_suffix = ''
 
     except IndexError:
         pass
 
-    return text_reversed if text_reversed is None else (text_reversed + added_suffix)
+    return text_reversed if not text_reversed else text_reversed + added_suffix
 
 
-def process_rules(rules: Any, fixed_text: str, cur: int = 0, cur_end: int = 1) -> Union[Any, None]:
+def process_rules(rules: Dict[str, Any], fixed_text: str, cur: int = 0, cur_end: int = 1) -> Optional[str]:
     '''
     ### Process rules matched in pattern and returns suitable replacement.
 
     If any rule's condition is satisfied, output the rules "replace",
     else output None.
     '''
```

### Comparing `avro.py-2023.4.3/avro/resources/__init__.py` & `avro.py-2023.6.12/avro/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `avro.py-2023.4.3/avro/resources/avrodict.py` & `avro.py-2023.6.12/avro/resources/avrodict.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 ## The Avro Dictionary (Adapted)
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
@@ -36,17 +36,17 @@
 # The dictionary variable.
 AVRO_DICT: Dict[str, str] = {
     "meta": {
         "file_name": "avrodict.py",
         "file_description": "Provides Avro Dictionary in native Python dictionary. Adapted from avrodict.json",
         "package": "avro.py",
         "license": "MIT License",
-        "source": "https://github.com/kaustavdm/pyAvroPhonetic/blob/master/pyavrophonetic/resources/avrodict.json",
+        "source": "https://github.com/hitblast/avro.py/blob/main/avro/resources/avrodict.py",
         "adapted_by": "HitBlast",
-        "updated": "20230403",
+        "updated": "20230421",
         "encoding": "utf-8"
     },
     "data": {
         "patterns": [
             {
                 "find": "bhl",
                 "replace": "ভ্ল"
@@ -113,16 +113,15 @@
             {
                 "find": "cc",
                 "replace": "চ্চ",
                 "reverse": "cc"
             },
             {
                 "find": "ch",
-                "replace": "ছ",
-                "reverse": "s"
+                "replace": "ছ"
             },
             {
                 "find": "c",
                 "replace": "চ",
                 "reverse": "ch"
             },
             {
@@ -2018,25 +2017,28 @@
             # }
         ],
 
         # Remapped words
         "exceptions": {
             "ফেসবুক": "Facebook",
             "গুগল": "Google",
-            "উইকিপিডিয়া": "Wikipedia"
+            "উইকিপিডিয়া": "Wikipedia",
+            "হোয়াটসঅ্যাপ": "Whatsapp",
+            "টুইটার": "Twitter",
+            "লিঙ্কডইন": "Linkedin"
         },
 
         # Constant values
         "vowel": "aeiou",
         "consonant": "bcdfghjklmnpqrstvwxyz",
         "casesensitive": "oiudgjnrstyz",
         "number": "0123456789",
 
         # For reverse parsing
-        "shorborno": "অআইঈউঊঊএঐওঔ",
+        "shorborno": "অআইঈউঊএঐওঔ",
         "kar": {
             'া',
             'ি',
             'ী',
             'ু',
             'ূ',
             'ৃ',
```

### Comparing `avro.py-2023.4.3/avro/utils/__init__.py` & `avro.py-2023.6.12/avro/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Utils package for avro.py
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.3/avro/utils/count.py` & `avro.py-2023.6.12/avro/utils/count.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Count functions (avro.utils) for avro.py
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
@@ -25,18 +25,19 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
 
-# Imports
+# Import local modules.
 from avro import config
 
 
+# Functions.
 def count_vowels(text) -> int:
     '''
     ### Count number of occurrences of vowels in a given string.
     '''
 
     count = 0
     for i in text:
```

### Comparing `avro.py-2023.4.3/avro/utils/validate.py` & `avro.py-2023.6.12/avro/utils/validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Validation functions (avro.utils) for avro.py
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
@@ -25,15 +25,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
 
-# Imports
+# Import local modules.
 from avro import config
 
 
 # Functions.
 def is_vowel(text: str) -> bool:
     '''
     ### Check if given string is a vowel.
```

### Comparing `avro.py-2023.4.3/avro.py.egg-info/PKG-INFO` & `avro.py-2023.6.12/avro.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2023.4.3
+Version: 2023.6.12
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,avro,avro phonetic,bangla,bangla phonetics,bengali,bengali phonetics
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div align="center">
 
-# <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="35px"/> avro.py
+# <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
 
 A modern Pythonic implementation of the popular Bengali phonetic-typing software **Avro Phonetic.**
 
 [![Downloads](https://static.pepy.tech/personalized-badge/avro-py?period=total&units=international_system&left_color=grey&right_color=black&left_text=Downloads)](https://pepy.tech/project/avro-py)
 ![Python Version](https://img.shields.io/pypi/pyversions/avro.py.svg?color=black&label=Python)
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
@@ -42,21 +42,19 @@
 
 </div>
 
 ## Overview
 
 **avro.py**, being a Python package, provides a text parser that converts English text written in Roman script to its phonetic equivalent of Bengali. It implements the **Avro Phonetic Dictionary Search Library** by [Mehdi Hasan Khan](https://github.com/mugli).
 
-The original project ([pyAvroPhonetic](https://github.com/kaustavdm/pyAvroPhonetic)) can only be used on versions up to **Python 2.7** and doesn't contain proper support for Python's third major version AKA Python 3. It is noteworthy that Python 2 has officially been deprecated by the original maintainers and its usage is being discouraged overall.
-
-<br>
+The original project ([pyAvroPhonetic](https://github.com/kaustavdm/pyAvroPhonetic)) can only be used on versions up to **Python 2.7** and doesn't contain proper support for Python's third major version AKA Python 3. It is noteworthy that Python 2 has officially been deprecated by the original maintainers and its usage is being discouraged overall. <br>
 
 ## Inspirations
 
-This package is inspired from Rifat Nabi's jsAvroPhonetic library and derives from Kaustav Das Modak's pyAvroPhonetic.
+This package is inspired from Rifat Nabi's jsAvroPhonetic library and derives from Kaustav Das Modak's pyAvroPhonetic. 
 
 <br>
 
 ## Installation
 
 This package requires **Python 3.8 or higher** to be used inside your development environment.
 
@@ -89,25 +87,24 @@
 
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 print(reversed_text)
 
 # amar sonar bangla.
 ```
 
-Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally!
+Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally! 
 
 <br>
 
 ## Contributing
 
 :octocat: *Fork -> Do your changes -> Send a Pull Request, it's that easy!* <br>
 
 ---
 
-
 **Additional Developer Notes**
 
 In short, avro.py doesn't depend on any third-party libraries. However, if you'd like to contribute to the project, you'll need a handful of such useful tools. <br>
 
 - [flake8](https://flake8.pycqa.org/en/latest/) - linter
 - [pytest](https://pypi.python.org/pypi/pytest) - testing framework
 - [black](https://github.com/psf/black) - formatting
@@ -119,17 +116,15 @@
 # Running pytest.
 $ python3 -m pytest --verbose
 
 # The results should appear onwards.
 # The --verbose / -v flag is used to show all the test results in detail.
 ```
 
-<br>
-
-### We're looking for bug hunters!
+### We're looking for bug hunters, by the way!
 
 If you come across any kind of bug or wanna request a feature, please let us know by opening an issue [here](https://github.com/hitblast/avro.py/issues). We do need more ideas to keep the project alive and running, don't we? :P
 
 ---
 
 <br>
```

### Comparing `avro.py-2023.4.3/setup.py` & `avro.py-2023.6.12/setup.py`

 * *Files identical despite different names*

### Comparing `avro.py-2023.4.3/tests/test_main.py` & `avro.py-2023.6.12/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Test cases for avro.main
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
@@ -185,10 +185,10 @@
 
 def test_reverse_func() -> None:
     '''
     ### Test reverse-parsing with sentences.
     '''
 
     assert 'ami banglay gan gai' == avro.reverse('আমি বাংলায় গান গাই')
-    assert 'rahim, tomake korim dakse. ekhon ki rowna debe?' == avro.reverse(
+    assert 'rahim, tomake korim dakche. ekhon ki rowna debe?' == avro.reverse(
         'রাহিম, তোমাকে করিম ডাকছে। এখন কি রওনা দেবে?'
     )
```

### Comparing `avro.py-2023.4.3/tests/test_utils_count.py` & `avro.py-2023.6.12/tests/test_utils_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Test cases for avro.utils.count
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.3/tests/test_utils_validate.py` & `avro.py-2023.6.12/tests/test_utils_validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Test cases for avro.utils.validate
 
 ---
 
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
+of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

