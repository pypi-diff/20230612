# Comparing `tmp/wkt_scraper-1.0.1.tar.gz` & `tmp/wkt_scraper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkt_scraper-1.0.1.tar", last modified: Wed May 31 20:12:06 2023, max compression
+gzip compressed data, was "wkt_scraper-1.0.2.tar", last modified: Mon Jun 12 19:38:32 2023, max compression
```

## Comparing `wkt_scraper-1.0.1.tar` & `wkt_scraper-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-05-31 20:12:06.054674 wkt_scraper-1.0.1/
--rw-rw-r--   0 fatih     (1000) fatih     (1000)     1068 2023-05-27 22:07:08.000000 wkt_scraper-1.0.1/LICENSE
--rw-rw-r--   0 fatih     (1000) fatih     (1000)       18 2023-05-27 22:07:08.000000 wkt_scraper-1.0.1/MANIFEST.in
--rw-rw-r--   0 fatih     (1000) fatih     (1000)     1089 2023-05-31 20:12:06.054674 wkt_scraper-1.0.1/PKG-INFO
--rw-rw-r--   0 fatih     (1000) fatih     (1000)      568 2023-05-31 20:06:46.000000 wkt_scraper-1.0.1/README.md
-drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-05-31 20:12:06.050674 wkt_scraper-1.0.1/scraper/
--rw-rw-r--   0 fatih     (1000) fatih     (1000)       29 2023-05-27 22:07:08.000000 wkt_scraper-1.0.1/scraper/__init__.py
--rw-rw-r--   0 fatih     (1000) fatih     (1000)     1051 2023-05-31 14:00:56.000000 wkt_scraper-1.0.1/scraper/language.py
--rw-rw-r--   0 fatih     (1000) fatih     (1000)    14094 2023-05-31 19:50:14.000000 wkt_scraper-1.0.1/scraper/scraper.py
--rw-rw-r--   0 fatih     (1000) fatih     (1000)       38 2023-05-31 20:12:06.054674 wkt_scraper-1.0.1/setup.cfg
--rw-rw-r--   0 fatih     (1000) fatih     (1000)      811 2023-05-31 20:09:34.000000 wkt_scraper-1.0.1/setup.py
-drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-05-31 20:12:06.050674 wkt_scraper-1.0.1/wkt_scraper.egg-info/
--rw-rw-r--   0 fatih     (1000) fatih     (1000)     1089 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 fatih     (1000) fatih     (1000)      271 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 fatih     (1000) fatih     (1000)        1 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 fatih     (1000) fatih     (1000)       24 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/requires.txt
--rw-rw-r--   0 fatih     (1000) fatih     (1000)        8 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-12 19:38:32.859754 wkt_scraper-1.0.2/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1068 2023-05-27 22:07:08.000000 wkt_scraper-1.0.2/LICENSE
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       18 2023-05-27 22:07:08.000000 wkt_scraper-1.0.2/MANIFEST.in
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1097 2023-06-12 19:38:32.859754 wkt_scraper-1.0.2/PKG-INFO
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      567 2023-06-11 11:51:47.000000 wkt_scraper-1.0.2/README.md
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-12 19:38:32.855754 wkt_scraper-1.0.2/scraper/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       29 2023-05-27 22:07:08.000000 wkt_scraper-1.0.2/scraper/__init__.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1418 2023-06-11 11:48:55.000000 wkt_scraper-1.0.2/scraper/language.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)    15572 2023-06-12 19:27:13.000000 wkt_scraper-1.0.2/scraper/scraper.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       38 2023-06-12 19:38:32.859754 wkt_scraper-1.0.2/setup.cfg
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      820 2023-06-12 19:35:53.000000 wkt_scraper-1.0.2/setup.py
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-12 19:38:32.855754 wkt_scraper-1.0.2/wkt_scraper.egg-info/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1097 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      271 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)        1 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       24 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/requires.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)        8 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/top_level.txt
```

### Comparing `wkt_scraper-1.0.1/LICENSE` & `wkt_scraper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wkt_scraper-1.0.1/PKG-INFO` & `wkt_scraper-1.0.2/wkt_scraper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: wkt_scraper
-Version: 1.0.1
-Summary: Parse word information from Wiktionary. Currently only English and Turkish are supported.
+Name: wkt-scraper
+Version: 1.0.2
+Summary: Parse word information from Wiktionary. Currently only English, Spanish and Turkish are supported.
 Home-page: https://github.com/fatih-akgul/wkt_scraper
 Author: Fatih Akgul
 Author-email: akguls@gmail.com
 License: MIT
 Keywords: wiktionary scraper parser
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,14 @@
 Wiktionary Scraper is a basic scraper implementation to get word data from Wiktionary for a given word and language.  
 
 ## Installation
 You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
     
     pip install wkt_scraper
 
-In python code, to look up the word "complicated" from English to English:
+In python code, to look up the word "street" from English to Spanish:
 
     from scraper import Scraper
-    response = Scraper('en', 'en').scrape('complicated')
+    response = Scraper('en', 'es').scrape('street')
 
-Currently only English and Turkish are supported. 
+Currently only English, Spanish and Turkish are supported. 
 Supporting more languages will require additional work and testing.
```

### Comparing `wkt_scraper-1.0.1/README.md` & `wkt_scraper-1.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 Wiktionary Scraper is a basic scraper implementation to get word data from Wiktionary for a given word and language.  
 
 ## Installation
 You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
     
     pip install wkt_scraper
 
-In python code, to look up the word "complicated" from English to English:
+In python code, to look up the word "street" from English to Spanish:
 
     from scraper import Scraper
-    response = Scraper('en', 'en').scrape('complicated')
+    response = Scraper('en', 'es').scrape('street')
 
-Currently only English and Turkish are supported. 
+Currently only English, Spanish and Turkish are supported. 
 Supporting more languages will require additional work and testing.
```

### Comparing `wkt_scraper-1.0.1/scraper/language.py` & `wkt_scraper-1.0.2/scraper/language.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,31 +16,46 @@
         alpha2='en',
         name='English',
         etymology='Etymology',
         pronunciation='Pronunciation',
         derived_terms='Derived_terms',
         proverbs='Proverbs',
     ),
+    'es': Language(
+        alpha2='es',
+        name='Spanish',
+        etymology='Etimología',
+        pronunciation='Pronunciación',
+        derived_terms='Términos_derivados',
+        proverbs='Proverbios',
+    ),
     'tr': Language(
         alpha2='tr',
         name='Turkish',
         etymology='Köken',
         pronunciation='Söyleniş',
         derived_terms='Türetilmiş_kavramlar',
         proverbs='Atasözleri',
     ),
 }
 
 language_names = {
     'tr': {
-        'tr': 'Türkçe',
         'en': 'İngilizce',
+        'es': 'İspanyolca',
+        'tr': 'Türkçe',
     },
     'en': {
-        'tr': 'Turkish',
         'en': 'English',
+        'es': 'Spanish',
+        'tr': 'Turkish',
     },
+    'es': {
+        'en': 'Inglés',
+        'es': 'Español',
+        'tr': 'Turco',
+    }
 }
 
 
 def get_language(alpha2: str) -> Language:
     return languages.get(alpha2)
```

### Comparing `wkt_scraper-1.0.1/scraper/scraper.py` & `wkt_scraper-1.0.2/scraper/scraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -197,36 +197,51 @@
             'related_terms': 'Related_terms',
             'synonyms': 'Synonyms',
             'antonyms': 'Antonyms',
             'proverbs': self._to_language.proverbs,
             'derived_terms': self._to_language.derived_terms,
         }
 
+        self.response = {
+            'word': '',
+            'from_language': from_language,
+            'to_language': to_language,
+            'meanings': []
+        }
+
     def scrape(self, word: str) -> Dict[str, Any]:
         root = get_root_element(self._get_url(word))
         self._remove_other_languages(root)
         label = root.find(id=self._from_language_name)
-        response = {
-            'word': word,
-            'from_language': self._from_language.alpha2,
-            'to_language': self._to_language.alpha2,
-            'meanings': []
-        }
+        self.response['word'] = word
         if label is not None:
             siblings: ResultSet[PageElement] = label.parent.find_next_siblings(['h2', 'h3', 'hr'])
             processed_headers = []
             for sibling in siblings:
                 if sibling.name in ['hr', 'h2']:
                     break
                 else:
                     sibling_text = str(sibling)
                     if sibling_text not in processed_headers:
-                        response = self._process_header(sibling, response, processed_headers)
+                        self._process_header(sibling, processed_headers)
                     processed_headers.append(sibling_text)
-        return response
+        if not self._response_has_audio():
+            self._process_pronunciation(root)
+        return self.response
+
+    def _response_has_audio(self) -> bool:
+        if 'pronunciation' not in self.response:
+            return False
+        for pronunciation in self.response['pronunciation']:
+            for pronunciation_value in pronunciation['values']:
+                if 'value' in pronunciation_value and (
+                        '.mp3' in pronunciation_value['value']
+                        or '.ogg' in pronunciation_value['value']):
+                    return True
+        return False
 
     def _remove_other_languages(self, root: PageElement):
         languages: ResultSet[Tag] = root.find_all(name='h2')
         for language in languages:
             language_container: Tag = language.find(id=self._from_language_name)
             if language_container is None:
                 # Remove until next language h2
@@ -236,23 +251,21 @@
                     if sibling.name == 'h2':
                         break
                     sibling.extract()
 
     def _get_url(self, word: str) -> str:
         return f'https://{self._to_language.alpha2}.wiktionary.org/wiki/{word}'
 
-    def _process_header(self, header: PageElement, response: Dict[str, Any], processed_headers) -> Dict[str, Any]:
+    def _process_header(self, header: PageElement, processed_headers):
         if self._is_pronunciation_header(header):
-            response['pronunciation'] = get_pronunciation(header)
+            self.response['pronunciation'] = get_pronunciation(header)
         elif self._is_etymology_header(header):
-            response['meanings'].append(self._get_meaning_with_etymology(header, processed_headers))
+            self.response['meanings'].append(self._get_meaning_with_etymology(header, processed_headers))
         elif is_part_of_speech_header(header):
-            response['meanings'].append(self._get_meaning_without_etymology(header))
-
-        return response
+            self.response['meanings'].append(self._get_meaning_without_etymology(header))
 
     def _is_pronunciation_header(self, header: PageElement) -> bool:
         if header.find_all('span', string=self._to_language.pronunciation):
             return True
         return False
 
     def _get_meaning_without_etymology(self, header: PageElement) -> [Dict[str, Any]]:
@@ -292,29 +305,31 @@
             self._process_meaning_values(next_sibling, result)
         return result
 
     def _process_meaning_values(self, word_p: PageElement, meaning: Dict[str, Any]):
         next_sibling: PageElement = word_p
         if next_sibling.name == 'p':
             meaning['metadata'] = next_sibling.get_text().strip()
-        if next_sibling.name in ['p', 'div', 'pre', 'figure']:
+        if next_sibling.name in ['p', 'div', 'pre', 'figure', 'table']:
             next_sibling = next_sibling.find_next_sibling(name=['ol', 'dl'])
-        if next_sibling.name in ['ol', 'dl']:
+        meaning_sibling = next_sibling
+        while meaning_sibling and meaning_sibling.name in ['ol', 'dl']:
             # element_tag = 'dd' if next_sibling.name == 'dl' else 'li'
-            lis: ResultSet[PageElement] = next_sibling.find_all(name=['dd', 'li'], recursive=False)
+            lis: ResultSet[PageElement] = meaning_sibling.find_all(name=['dd', 'li'], recursive=False)
             for li in lis:
                 remove_descendants_with_class(li, 'HQToggle')
                 remove_parent_of_descendant_with_class(li, 'citation-whole')
                 examples = find_usage_examples(li)
 
                 value = {
                     'text': li.get_text().strip(),
                     'examples': examples
                 }
                 meaning['definitions'].append(value)
+            meaning_sibling = meaning_sibling.find_next_sibling()
             self._process_additional_data(next_sibling, meaning)
 
     def _process_additional_data(self, after_meaning_values: PageElement, meaning: Dict[str, Any]) -> None:
         if after_meaning_values is not None and meaning['definitions']:
             next_sibling = after_meaning_values
             while next_sibling is not None and not self._is_meaning_switcher(next_sibling):
                 for response_field, html_id in self._additional_data.items():
@@ -327,7 +342,27 @@
                or self._is_etymology_header(header) \
                or is_part_of_speech_header(header)
 
     def _is_etymology_header(self, header: PageElement) -> bool:
         if header.find_all('span', string=re.compile(self._to_language.etymology + '.*')):
             return True
         return False
+
+    def _process_pronunciation(self, root: BeautifulSoup) -> None:
+        audio_entries = root.find_all('audio')
+        pronunciations = []
+        if 'pronunciation' in self.response:
+            pronunciations = self.response['pronunciation']
+        for audio_entry in audio_entries:
+            sources = audio_entry.find_all('source')
+            if not sources:
+                continue
+            pronunciation_values = []
+            pronunciation = {'type': 'Audio', 'values': pronunciation_values}
+            for source in sources:
+                pronunciation_values.append({
+                    'type': source.attrs['type'],
+                    'value': source.attrs['src'],
+                })
+            pronunciations.append(pronunciation)
+
+        self.response['pronunciation'] = pronunciations
```

### Comparing `wkt_scraper-1.0.1/setup.py` & `wkt_scraper-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='wkt_scraper',
-    version='1.0.1',
-    description='Parse word information from Wiktionary. Currently only English and Turkish are supported.',
+    version='1.0.2',
+    description='Parse word information from Wiktionary. Currently only English, Spanish and Turkish are supported.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='wiktionary scraper parser',
     author='Fatih Akgul',
     author_email='akguls@gmail.com',
     license='MIT',
     classifiers=[
```

### Comparing `wkt_scraper-1.0.1/wkt_scraper.egg-info/PKG-INFO` & `wkt_scraper-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: wkt-scraper
-Version: 1.0.1
-Summary: Parse word information from Wiktionary. Currently only English and Turkish are supported.
+Name: wkt_scraper
+Version: 1.0.2
+Summary: Parse word information from Wiktionary. Currently only English, Spanish and Turkish are supported.
 Home-page: https://github.com/fatih-akgul/wkt_scraper
 Author: Fatih Akgul
 Author-email: akguls@gmail.com
 License: MIT
 Keywords: wiktionary scraper parser
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,14 @@
 Wiktionary Scraper is a basic scraper implementation to get word data from Wiktionary for a given word and language.  
 
 ## Installation
 You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
     
     pip install wkt_scraper
 
-In python code, to look up the word "complicated" from English to English:
+In python code, to look up the word "street" from English to Spanish:
 
     from scraper import Scraper
-    response = Scraper('en', 'en').scrape('complicated')
+    response = Scraper('en', 'es').scrape('street')
 
-Currently only English and Turkish are supported. 
+Currently only English, Spanish and Turkish are supported. 
 Supporting more languages will require additional work and testing.
```

