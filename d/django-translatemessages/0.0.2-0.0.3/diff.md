# Comparing `tmp/django-translatemessages-0.0.2.tar.gz` & `tmp/django-translatemessages-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-translatemessages-0.0.2.tar", last modified: Mon Jun 12 08:57:36 2023, max compression
+gzip compressed data, was "django-translatemessages-0.0.3.tar", last modified: Mon Jun 12 14:47:46 2023, max compression
```

## Comparing `django-translatemessages-0.0.2.tar` & `django-translatemessages-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       53 2023-06-12 08:55:29.000000 django-translatemessages-0.0.2/CHANGELOG.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1071 2023-06-11 10:32:38.000000 django-translatemessages-0.0.2/LICENSE
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       89 2023-06-11 10:46:30.000000 django-translatemessages-0.0.2/MANIFEST.in
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3452 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2410 2023-06-12 08:55:29.000000 django-translatemessages-0.0.2/README.rst
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/django_translatemessages/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       22 2023-06-12 08:55:34.000000 django-translatemessages-0.0.2/django_translatemessages/__init__.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/django_translatemessages/management/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:02.000000 django-translatemessages-0.0.2/django_translatemessages/management/__init__.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/django_translatemessages/management/commands/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:14.000000 django-translatemessages-0.0.2/django_translatemessages/management/commands/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11238 2023-06-12 08:57:11.000000 django-translatemessages-0.0.2/django_translatemessages/management/commands/translatemessages.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/django_translatemessages.egg-info/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3452 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      557 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/SOURCES.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/dependency_links.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-11 14:28:09.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/not-zip-safe
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/requires.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       25 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/top_level.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/setup.cfg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2023-06-11 14:28:07.000000 django-translatemessages-0.0.2/setup.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       53 2023-06-12 08:55:29.000000 django-translatemessages-0.0.3/CHANGELOG.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1071 2023-06-11 10:32:38.000000 django-translatemessages-0.0.3/LICENSE
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       89 2023-06-11 10:46:30.000000 django-translatemessages-0.0.3/MANIFEST.in
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4117 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3075 2023-06-12 14:40:26.000000 django-translatemessages-0.0.3/README.rst
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/django_translatemessages/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       22 2023-06-12 14:07:48.000000 django-translatemessages-0.0.3/django_translatemessages/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/django_translatemessages/management/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:02.000000 django-translatemessages-0.0.3/django_translatemessages/management/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/django_translatemessages/management/commands/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:14.000000 django-translatemessages-0.0.3/django_translatemessages/management/commands/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11506 2023-06-12 13:57:29.000000 django-translatemessages-0.0.3/django_translatemessages/management/commands/translatemessages.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/django_translatemessages.egg-info/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4117 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      557 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/SOURCES.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/dependency_links.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-11 14:28:09.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/not-zip-safe
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/requires.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       25 2023-06-12 14:47:46.000000 django-translatemessages-0.0.3/django_translatemessages.egg-info/top_level.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-12 14:47:46.296572 django-translatemessages-0.0.3/setup.cfg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2023-06-11 14:28:07.000000 django-translatemessages-0.0.3/setup.py
```

### Comparing `django-translatemessages-0.0.2/LICENSE` & `django-translatemessages-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.2/PKG-INFO` & `django-translatemessages-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-translatemessages
-Version: 0.0.2
+Version: 0.0.3
 Summary: Translate Django .po files
 Home-page: https://github.com/elapouya/django-translatemessages
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: MIT
 Keywords: table,datatable,listing,data grid
 Platform: UNKNOWN
@@ -45,74 +45,88 @@
 
     poetry add django-translatemessages
 
 
 Configuration
 -------------
 
-You must declare in your `settings.py` what translator to use and its params.
+You must declare in your ``settings.py`` what translator to use and its params.
 Please refer to `deep-translator Translators <https://deep-translator.readthedocs.io/en/latest/usage.html>`_
-to know what parameters to specify (Note that `django-translatemessages` automatically add `source` and `target` parameters
+to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters
 
-To configure GoogleTranslator, add in your `settings.py`::
+To configure GoogleTranslator, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "GoogleTranslator",
             "params": {},
         },
     }
 
 
-To configure DeeplTranslator, you will need an API key, add in your `settings.py`::
+To configure DeeplTranslator, you will need an API key, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "DeeplTranslator",
             "params": {
                 "api_key": "your deepl api key",
             },
         },
     }
 
 A good pratice in a Django application is to encapsulate strings to be translated into square brakets,
 thus, you will noticed at once what strings has not been translated yet.
-You can ask `django-translatemessages` to extract the string to translate from the source string.
+You can ask ``django-translatemessages`` to extract the string to translate from the source string.
 Use a regex which selects with parentheses the text to extract. Note that if there is no match, the translation will not occur.
 
-For example if you want to translate `[my english string]` into `my french string` with deepl, put in `settings.py`::
+For example if you want to translate ``[my english string]`` into ``my french string`` with deepl, put in ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "extract_regex": r"\[(.*)\]",
         "translator": {
             "class": "DeeplTranslator",
             "params": {
                 "api_key": "your deepl api key",
             },
         },
     }
 
-The source language is `en` by default, but you can use another one in your `settings.py`::
+The source language is ``en`` by default, but you can use another one in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "source_lang": "fr",
         ...
     }
 
+**IMPORTANT :** By default, ``django-translatemessages`` will produce translations with the flag ``fuzzy``.
+This force the developer to validate manually each translation. To do so, edit each ``django.po`` file,
+search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
+Django will not display the translation. You can also use `poedit <https://poedit.net/>`_
+and press ``CTRL + RETURN`` on each highlighted translation you agree.
+
+To disable auto-fuzzy feature, use this in your ``settings.py``::
+
+    TRANSLATEMESSAGES_PARAMS = {
+        "auto_fuzzy": False,
+        ...
+    }
+
 
 Usage
 -----
 
 To auto-translate all languages in all apps::
 
     python ./manage.py translatemessages
 
-Do not forget to do a `makemessages` before if needed (See Django documentation)
+Do not forget to do a ``makemessages`` before if needed (See Django documentation)
+
+For more options, run ``python ./manage.py translatemessages -h``
 
-For more options, run `python ./manage.py translatemessages -h`
 
 News
 ----
 
 0.0.2 (2023-06-11)
 ------------------
 - First commit
```

### Comparing `django-translatemessages-0.0.2/README.rst` & `django-translatemessages-0.0.3/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -17,67 +17,80 @@
 
     poetry add django-translatemessages
 
 
 Configuration
 -------------
 
-You must declare in your `settings.py` what translator to use and its params.
+You must declare in your ``settings.py`` what translator to use and its params.
 Please refer to `deep-translator Translators <https://deep-translator.readthedocs.io/en/latest/usage.html>`_
-to know what parameters to specify (Note that `django-translatemessages` automatically add `source` and `target` parameters
+to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters
 
-To configure GoogleTranslator, add in your `settings.py`::
+To configure GoogleTranslator, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "GoogleTranslator",
             "params": {},
         },
     }
 
 
-To configure DeeplTranslator, you will need an API key, add in your `settings.py`::
+To configure DeeplTranslator, you will need an API key, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "DeeplTranslator",
             "params": {
                 "api_key": "your deepl api key",
             },
         },
     }
 
 A good pratice in a Django application is to encapsulate strings to be translated into square brakets,
 thus, you will noticed at once what strings has not been translated yet.
-You can ask `django-translatemessages` to extract the string to translate from the source string.
+You can ask ``django-translatemessages`` to extract the string to translate from the source string.
 Use a regex which selects with parentheses the text to extract. Note that if there is no match, the translation will not occur.
 
-For example if you want to translate `[my english string]` into `my french string` with deepl, put in `settings.py`::
+For example if you want to translate ``[my english string]`` into ``my french string`` with deepl, put in ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "extract_regex": r"\[(.*)\]",
         "translator": {
             "class": "DeeplTranslator",
             "params": {
                 "api_key": "your deepl api key",
             },
         },
     }
 
-The source language is `en` by default, but you can use another one in your `settings.py`::
+The source language is ``en`` by default, but you can use another one in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "source_lang": "fr",
         ...
     }
 
+**IMPORTANT :** By default, ``django-translatemessages`` will produce translations with the flag ``fuzzy``.
+This force the developer to validate manually each translation. To do so, edit each ``django.po`` file,
+search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
+Django will not display the translation. You can also use `poedit <https://poedit.net/>`_
+and press ``CTRL + RETURN`` on each highlighted translation you agree.
+
+To disable auto-fuzzy feature, use this in your ``settings.py``::
+
+    TRANSLATEMESSAGES_PARAMS = {
+        "auto_fuzzy": False,
+        ...
+    }
+
 
 Usage
 -----
 
 To auto-translate all languages in all apps::
 
     python ./manage.py translatemessages
 
-Do not forget to do a `makemessages` before if needed (See Django documentation)
+Do not forget to do a ``makemessages`` before if needed (See Django documentation)
 
-For more options, run `python ./manage.py translatemessages -h`
+For more options, run ``python ./manage.py translatemessages -h``
```

### Comparing `django-translatemessages-0.0.2/django_translatemessages/management/commands/translatemessages.py` & `django-translatemessages-0.0.3/django_translatemessages/management/commands/translatemessages.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         self.translator_params = settings.TRANSLATEMESSAGES_PARAMS["translator"].get(
             "params", {}
         )
 
         # Get other parameters from settings
         self.do_batch = settings.TRANSLATEMESSAGES_PARAMS.get("batch", False)
         self.source_lang = settings.TRANSLATEMESSAGES_PARAMS.get("source_lang", "en")
+        self.auto_fuzzy = settings.TRANSLATEMESSAGES_PARAMS.get("auto_fuzzy", True)
 
         extract_regex = settings.TRANSLATEMESSAGES_PARAMS.get("extract_regex")
         if isinstance(extract_regex, str):
             extract_regex = re.compile(extract_regex)
         if extract_regex and not options["no_filter"]:
 
             def filter_msgid(msgid):
@@ -258,14 +259,16 @@
                 )
             ]
             nb_translations += len(entries)
             texts = [entry.msgid for entry in entries]
             translated_texts = self.translate_text_batch(texts, translator)
             for entry, translated_text in zip(entries, translated_texts):
                 entry.msgstr = translated_text
+                if self.auto_fuzzy:
+                    entry.flags.append("fuzzy")
                 self.stdout.write(
                     colorize(f"{entry.msgid}", fg="blue"),
                     ending="",
                 )
                 self.stdout.write(colorize(f"-> {translated_text}", fg="cyan"))
         else:
             for entry in po:
@@ -280,14 +283,16 @@
                         if translator.source != translator.target:
                             translated_text = self.translate_text(
                                 filtered_msgid, translator
                             )
                         else:
                             translated_text = filtered_msgid
                         entry.msgstr = translated_text
+                        if self.auto_fuzzy:
+                            entry.flags.append("fuzzy")
                         self.stdout.write(colorize(f"-> {translated_text}", fg="cyan"))
 
         if nb_translations:
             self.stdout.write(
                 self.style.SUCCESS(f"{nb_translations} strings translated")
             )
             if self.options["dry_run"]:
```

### Comparing `django-translatemessages-0.0.2/django_translatemessages.egg-info/PKG-INFO` & `django-translatemessages-0.0.3/django_translatemessages.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-translatemessages
-Version: 0.0.2
+Version: 0.0.3
 Summary: Translate Django .po files
 Home-page: https://github.com/elapouya/django-translatemessages
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: MIT
 Keywords: table,datatable,listing,data grid
 Platform: UNKNOWN
@@ -45,74 +45,88 @@
 
     poetry add django-translatemessages
 
 
 Configuration
 -------------
 
-You must declare in your `settings.py` what translator to use and its params.
+You must declare in your ``settings.py`` what translator to use and its params.
 Please refer to `deep-translator Translators <https://deep-translator.readthedocs.io/en/latest/usage.html>`_
-to know what parameters to specify (Note that `django-translatemessages` automatically add `source` and `target` parameters
+to know what parameters to specify (Note that ``django-translatemessages`` automatically add ``source`` and ``target`` parameters
 
-To configure GoogleTranslator, add in your `settings.py`::
+To configure GoogleTranslator, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "GoogleTranslator",
             "params": {},
         },
     }
 
 
-To configure DeeplTranslator, you will need an API key, add in your `settings.py`::
+To configure DeeplTranslator, you will need an API key, add in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "translator": {
             "class": "DeeplTranslator",
             "params": {
                 "api_key": "your deepl api key",
             },
         },
     }
 
 A good pratice in a Django application is to encapsulate strings to be translated into square brakets,
 thus, you will noticed at once what strings has not been translated yet.
-You can ask `django-translatemessages` to extract the string to translate from the source string.
+You can ask ``django-translatemessages`` to extract the string to translate from the source string.
 Use a regex which selects with parentheses the text to extract. Note that if there is no match, the translation will not occur.
 
-For example if you want to translate `[my english string]` into `my french string` with deepl, put in `settings.py`::
+For example if you want to translate ``[my english string]`` into ``my french string`` with deepl, put in ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "extract_regex": r"\[(.*)\]",
         "translator": {
             "class": "DeeplTranslator",
             "params": {
                 "api_key": "your deepl api key",
             },
         },
     }
 
-The source language is `en` by default, but you can use another one in your `settings.py`::
+The source language is ``en`` by default, but you can use another one in your ``settings.py``::
 
     TRANSLATEMESSAGES_PARAMS = {
         "source_lang": "fr",
         ...
     }
 
+**IMPORTANT :** By default, ``django-translatemessages`` will produce translations with the flag ``fuzzy``.
+This force the developer to validate manually each translation. To do so, edit each ``django.po`` file,
+search for the line ``#, fuzzy`` and remove it if you agree with the proposed translation. If you do not do this,
+Django will not display the translation. You can also use `poedit <https://poedit.net/>`_
+and press ``CTRL + RETURN`` on each highlighted translation you agree.
+
+To disable auto-fuzzy feature, use this in your ``settings.py``::
+
+    TRANSLATEMESSAGES_PARAMS = {
+        "auto_fuzzy": False,
+        ...
+    }
+
 
 Usage
 -----
 
 To auto-translate all languages in all apps::
 
     python ./manage.py translatemessages
 
-Do not forget to do a `makemessages` before if needed (See Django documentation)
+Do not forget to do a ``makemessages`` before if needed (See Django documentation)
+
+For more options, run ``python ./manage.py translatemessages -h``
 
-For more options, run `python ./manage.py translatemessages -h`
 
 News
 ----
 
 0.0.2 (2023-06-11)
 ------------------
 - First commit
```

### Comparing `django-translatemessages-0.0.2/django_translatemessages.egg-info/SOURCES.txt` & `django-translatemessages-0.0.3/django_translatemessages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.2/setup.py` & `django-translatemessages-0.0.3/setup.py`

 * *Files identical despite different names*

