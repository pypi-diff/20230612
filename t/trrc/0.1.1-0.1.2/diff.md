# Comparing `tmp/trrc-0.1.1.tar.gz` & `tmp/trrc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trrc-0.1.1.tar", last modified: Sun Jun  4 19:45:51 2023, max compression
+gzip compressed data, was "trrc-0.1.2.tar", last modified: Sun Jun 11 22:23:00 2023, max compression
```

## Comparing `trrc-0.1.1.tar` & `trrc-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-04 19:45:51.242575 trrc-0.1.1/
--rw-r--r--   0 constantinhong   (501) staff       (20)    35149 2023-05-30 20:49:49.000000 trrc-0.1.1/LICENSE
--rw-r--r--   0 constantinhong   (501) staff       (20)    58835 2023-06-04 19:45:51.241928 trrc-0.1.1/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)    17050 2023-06-04 19:44:49.000000 trrc-0.1.1/README.md
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-04 19:45:51.220495 trrc-0.1.1/docs/
--rw-r--r--   0 constantinhong   (501) staff       (20)     4018 2023-06-04 19:36:54.000000 trrc-0.1.1/docs/trrc.1
--rw-r--r--   0 constantinhong   (501) staff       (20)     1334 2023-06-04 19:36:54.000000 trrc-0.1.1/pyproject.toml
--rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-06-04 19:45:51.242751 trrc-0.1.1/setup.cfg
--rw-r--r--   0 constantinhong   (501) staff       (20)     1578 2023-06-04 19:43:11.000000 trrc-0.1.1/setup.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-04 19:45:51.225741 trrc-0.1.1/tests/
--rw-r--r--   0 constantinhong   (501) staff       (20)     4620 2023-05-30 20:49:49.000000 trrc-0.1.1/tests/test_cardcontentsHandle.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     1041 2023-05-30 20:49:49.000000 trrc-0.1.1/tests/test_classAnkiConnect.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     3009 2023-05-30 20:49:49.000000 trrc-0.1.1/tests/test_create_parser.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     2803 2023-05-30 20:49:49.000000 trrc-0.1.1/tests/test_options.py
--rw-r--r--   0 constantinhong   (501) staff       (20)      806 2023-05-30 20:49:49.000000 trrc-0.1.1/tests/test_pipe_redirection.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     1968 2023-05-26 00:27:04.000000 trrc-0.1.1/tests/test_regexhtml.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     9970 2023-05-30 20:49:49.000000 trrc-0.1.1/tests/test_utils.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-04 19:45:51.231748 trrc-0.1.1/trrc/
--rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-06-01 00:15:14.000000 trrc-0.1.1/trrc/__init__.py
--rwxr-xr-x   0 constantinhong   (501) staff       (20)      354 2023-06-02 19:57:50.000000 trrc-0.1.1/trrc/__main__.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     4864 2023-05-30 20:49:49.000000 trrc-0.1.1/trrc/config_opts.py
--rw-r--r--   0 constantinhong   (501) staff       (20)    23774 2023-06-04 19:43:11.000000 trrc-0.1.1/trrc/create_parser.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     6846 2023-06-04 19:43:11.000000 trrc-0.1.1/trrc/parser_opts.py
--rwxr-xr-x   0 constantinhong   (501) staff       (20)    11937 2023-06-04 19:43:11.000000 trrc-0.1.1/trrc/utils.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-04 19:45:51.240549 trrc-0.1.1/trrc.egg-info/
--rw-r--r--   0 constantinhong   (501) staff       (20)    58835 2023-06-04 19:45:51.000000 trrc-0.1.1/trrc.egg-info/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)      522 2023-06-04 19:45:51.000000 trrc-0.1.1/trrc.egg-info/SOURCES.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-06-04 19:45:51.000000 trrc-0.1.1/trrc.egg-info/dependency_links.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       44 2023-06-04 19:45:51.000000 trrc-0.1.1/trrc.egg-info/entry_points.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       25 2023-06-04 19:45:51.000000 trrc-0.1.1/trrc.egg-info/requires.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        5 2023-06-04 19:45:51.000000 trrc-0.1.1/trrc.egg-info/top_level.txt
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.713771 trrc-0.1.2/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    35149 2023-05-30 20:49:49.000000 trrc-0.1.2/LICENSE
+-rw-r--r--   0 constantinhong   (501) staff       (20)    59089 2023-06-11 22:23:00.713415 trrc-0.1.2/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)    17304 2023-06-11 22:15:08.000000 trrc-0.1.2/README.md
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.702894 trrc-0.1.2/docs/
+-rw-r--r--   0 constantinhong   (501) staff       (20)     4018 2023-06-04 19:36:54.000000 trrc-0.1.2/docs/trrc.1
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1334 2023-06-11 22:09:38.000000 trrc-0.1.2/pyproject.toml
+-rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-06-11 22:23:00.713853 trrc-0.1.2/setup.cfg
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1578 2023-06-11 22:09:38.000000 trrc-0.1.2/setup.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.707266 trrc-0.1.2/tests/
+-rw-r--r--   0 constantinhong   (501) staff       (20)     4620 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_cardcontentsHandle.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1041 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_classAnkiConnect.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     3009 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_create_parser.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     2803 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_options.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)      806 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_pipe_redirection.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1968 2023-05-26 00:27:04.000000 trrc-0.1.2/tests/test_regexhtml.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     9970 2023-05-30 20:49:49.000000 trrc-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.710672 trrc-0.1.2/trrc/
+-rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-06-01 00:15:14.000000 trrc-0.1.2/trrc/__init__.py
+-rwxr-xr-x   0 constantinhong   (501) staff       (20)      354 2023-06-02 19:57:50.000000 trrc-0.1.2/trrc/__main__.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     4864 2023-05-30 20:49:49.000000 trrc-0.1.2/trrc/config_opts.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)    23892 2023-06-11 22:12:30.000000 trrc-0.1.2/trrc/create_parser.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     7080 2023-06-11 22:09:38.000000 trrc-0.1.2/trrc/parser_opts.py
+-rwxr-xr-x   0 constantinhong   (501) staff       (20)    11936 2023-06-11 22:12:30.000000 trrc-0.1.2/trrc/utils.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-11 22:23:00.712856 trrc-0.1.2/trrc.egg-info/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    59089 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)      522 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/SOURCES.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/dependency_links.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       44 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/entry_points.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       25 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/requires.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        5 2023-06-11 22:23:00.000000 trrc-0.1.2/trrc.egg-info/top_level.txt
```

### Comparing `trrc-0.1.1/LICENSE` & `trrc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/PKG-INFO` & `trrc-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trrc
-Version: 0.1.1
+Version: 0.1.2
 Summary: a command-line program for creating anki card using AnkiConnect API.
 Home-page: https://github.com/Constantin1489/trrc
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
@@ -709,14 +709,15 @@
     * [PIP](#pip)
     * [MANUAL_INSTALLATION](#manual-installation)
 * [USAGE](#usage)
 * [CONFIG_FILE](#config-file)
 * [LOCATIONS](#locations)
 * [OPTIONS](#options)
 * [FAQ](#faq)
+* [CANGELOG](#changelog)
 * [CONTRIBUTION](#contribution)
 
 ## INTRODUCTION
 
 **ToRRential Card processor**(**trrc**) is a command-line unix-like program to create anki cards using AnkiConnect plugin.(Think a yt-dlp, but this program is for adding cards into Anki.)
 
 I intent to make it as a Unix-like program. Therefore it **leverages a lot of Unix concepts**.
@@ -744,14 +745,16 @@
 You don't have to use all those fields.
 For example, if all field of a type is 'Front:Back:Source:Sound:Tags',
 you can use only some of them. e.g.: 'Front:Back:Tags'.
 ####
 Total cards: 1 Total fails: 1
 ```
 
+See [Youtube demonstration video of the author](https://www.youtube.com/watch?v=-3jCwUEAOHE)
+
 ***if you decide to use this app, I highly recommend to turn apikey option in your AnkiConnect to prevent malicious attack. (It's not a fault of this app nor AnkiConnect. If the port of AnkiConnect opens without an apikey, anybody can modify your anki deck.)*** See also [AnkiConnect Configure](docs/tips/AnkiConnect_configure/AnkiConnect_addon_configure_example.md)
 
 ## INSTALLATION
 
 ### pip
 `pip install trrc`
 
@@ -1103,16 +1106,20 @@
 
 But if your want to send a card using **trrc** from outside of your computer which is running Anki with AnkiConnect, you may need to modify firewall option on the computer or a router.
 
 ### How to make iOS shortcuts with **trrc**
 
 See [iOS_shortcuts_example](docs/tips/iOS_shortcuts_setting_example/iOS_shortcuts_example.md)
 
-### This software misses some characters.
+## Changelog
 
+| Version | Note                     | 
+|:--------|:-------------------------|
+| HEAD    | fix sync option error handle. | 
+| 0.1.1   | init                     | 
 
 ## Contribution
 
 Thank you for letting me know the bug! Please report the bug in [issue tracker](https://github.com/Constantin1489/trrc/issues).
 
 Personally I like this app as a method to add cards and use daily, so I will keep developing it. Because I'm trying to get a job, an update delivery can be slow. But after getting a job, I will learn some good clean code conventions and apply it.
```

### Comparing `trrc-0.1.1/README.md` & `trrc-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     * [PIP](#pip)
     * [MANUAL_INSTALLATION](#manual-installation)
 * [USAGE](#usage)
 * [CONFIG_FILE](#config-file)
 * [LOCATIONS](#locations)
 * [OPTIONS](#options)
 * [FAQ](#faq)
+* [CANGELOG](#changelog)
 * [CONTRIBUTION](#contribution)
 
 ## INTRODUCTION
 
 **ToRRential Card processor**(**trrc**) is a command-line unix-like program to create anki cards using AnkiConnect plugin.(Think a yt-dlp, but this program is for adding cards into Anki.)
 
 I intent to make it as a Unix-like program. Therefore it **leverages a lot of Unix concepts**.
@@ -40,14 +41,16 @@
 You don't have to use all those fields.
 For example, if all field of a type is 'Front:Back:Source:Sound:Tags',
 you can use only some of them. e.g.: 'Front:Back:Tags'.
 ####
 Total cards: 1 Total fails: 1
 ```
 
+See [Youtube demonstration video of the author](https://www.youtube.com/watch?v=-3jCwUEAOHE)
+
 ***if you decide to use this app, I highly recommend to turn apikey option in your AnkiConnect to prevent malicious attack. (It's not a fault of this app nor AnkiConnect. If the port of AnkiConnect opens without an apikey, anybody can modify your anki deck.)*** See also [AnkiConnect Configure](docs/tips/AnkiConnect_configure/AnkiConnect_addon_configure_example.md)
 
 ## INSTALLATION
 
 ### pip
 `pip install trrc`
 
@@ -399,16 +402,20 @@
 
 But if your want to send a card using **trrc** from outside of your computer which is running Anki with AnkiConnect, you may need to modify firewall option on the computer or a router.
 
 ### How to make iOS shortcuts with **trrc**
 
 See [iOS_shortcuts_example](docs/tips/iOS_shortcuts_setting_example/iOS_shortcuts_example.md)
 
-### This software misses some characters.
+## Changelog
 
+| Version | Note                     | 
+|:--------|:-------------------------|
+| HEAD    | fix sync option error handle. | 
+| 0.1.1   | init                     | 
 
 ## Contribution
 
 Thank you for letting me know the bug! Please report the bug in [issue tracker](https://github.com/Constantin1489/trrc/issues).
 
 Personally I like this app as a method to add cards and use daily, so I will keep developing it. Because I'm trying to get a job, an update delivery can be slow. But after getting a job, I will learn some good clean code conventions and apply it.
```

### Comparing `trrc-0.1.1/docs/trrc.1` & `trrc-0.1.2/docs/trrc.1`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/pyproject.toml` & `trrc-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trrc"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 maintainers = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 license = {file = "LICENSE"}
```

### Comparing `trrc-0.1.1/setup.py` & `trrc-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 setup(
     name = 'trrc',
-    version = '0.1.1',
+    version = '0.1.2',
     description='a command-line program for creating anki card using AnkiConnect API.',
     author='Constantin Hong',
     author_email='hongconstantin@gmail.com',
     url='https://github.com/Constantin1489/trrc',
     maintainer='Constantin Hong',
     maintainer_email='hongconstantin@gmail.com',
     readme = "README.md",
```

### Comparing `trrc-0.1.1/tests/test_cardcontentsHandle.py` & `trrc-0.1.2/tests/test_cardcontentsHandle.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/tests/test_classAnkiConnect.py` & `trrc-0.1.2/tests/test_classAnkiConnect.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/tests/test_create_parser.py` & `trrc-0.1.2/tests/test_create_parser.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/tests/test_options.py` & `trrc-0.1.2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/tests/test_pipe_redirection.py` & `trrc-0.1.2/tests/test_pipe_redirection.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/tests/test_regexhtml.py` & `trrc-0.1.2/tests/test_regexhtml.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/tests/test_utils.py` & `trrc-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/trrc/config_opts.py` & `trrc-0.1.2/trrc/config_opts.py`

 * *Files identical despite different names*

### Comparing `trrc-0.1.1/trrc/create_parser.py` & `trrc-0.1.2/trrc/create_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,14 +317,15 @@
                      'get_type_name' : { "action": "modelNames",
                                         "version": 6 },
                      'get_deck_list' : { "action": "deckNames",
                                         "version": 6 },
                      'get_fields_of_model' : { "action": "modelFieldNames",
                                               "version": 6,
                                               "params": { "modelName": parameter }},
+                     'sync' : {"action": "sync", "version": 6,'key' : parameter},
                      }
 
     return dict_template[action]
 
 def send_card_ankiconnect(ankiconnect_url, card_json, action, apikey: str):
 
     # if apikey exist then update it
@@ -550,23 +551,27 @@
 
     if re.search(r'{{c\d+::.*}}', card_contents):
         main_logger.debug('found a cloze')
         return 'cloze'
 
     return get_proper_cardtype(cardtype)
 
-def sync(ankiconnect_info, apikey=''):
+def sync(ankiconnect_url, apikey=''):
     """
     Sync an anki.
     :ankiconnect_info: TODO
     """
-    response = requests.post(ankiconnect_info,
-                             json={"action": "sync", "version": 6,'key' : apikey},
-                             timeout=(1,1))
-    print(f'sync: {response.text}')
+
+    response = send_card_ankiconnect(ankiconnect_url, '', 'sync', apikey)
+
+    if response.text == '{"result": null, "error": null}':
+        print('sync: triggered')
+        return
+
+    check_response(response.text, '', ankiconnect_url, apikey)
 
 DEFAULT_ALIAS = 'default'
 
 def parse_config(parsed_arg):
     """Parse config options from default config files and user option argument."""
 
     # If user doesn't set section, then use 'default' even the config file is a
```

### Comparing `trrc-0.1.1/trrc/parser_opts.py` & `trrc-0.1.2/trrc/parser_opts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,212 +1,215 @@
 """module for parser using argparse"""
 import argparse
 import logging
 
-VERSION_MESSAGE = """trrc - ToRRential Card processor 0.1.1
+VERSION_MESSAGE = """trrc - ToRRential Card processor 0.1.2
 Copyright (C) 2023  Constantin Hong
 License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>.
 This is free software: you are free to change and redistribute it.
 There is NO WARRANTY, to the extent permitted by law."""
 
 DESCRIPTION = "A command-line unix-like program to create Anki cards using AnkiConnect API."
 
-CLOZE_TYPE_HELP = "set a type of a fallback for a cloze type. the default is " \
-"'cloze'. if user set --field option, then the default won't work. even a string " \
+CLOZE_TYPE_HELP = "Set a type of a fallback for a cloze type. The default is " \
+"'cloze'. If user set --field option, then the default won't work. Even a string " \
 "contains cloze, the program will process as a field unless user set " \
 "--cloze-type"
 
+CARD_CONTENT_HELP = "A quoted string divided by IFS. The default IFS is a tab character. " \
+        "Instead of a string, it can also take a file consists of strings " \
+        "without '--FILE' option. A [CARD_CONTENT] of '-' stands for standa" \
+        "rd input. <<EOF in [CARD_CONTENT] will trigger Pseudo HEREDOC " \
+        "mode. See #pseudo-heredoc-mode in README."
+
 def create_parser():
     """
     create parser
     """
 
     parser = argparse.ArgumentParser(
             prog='trrc',
             description=DESCRIPTION,
             formatter_class=argparse.RawDescriptionHelpFormatter,
             )
 
     parser.add_argument(
             'cardContents', action='store', nargs='*',
-            help=(
-            "a string divided by IFS. the default IFS is a tab character. " \
-            "instead of a string, It can also take a file consists of strings " \
-            "without '--FILE' option."
-            ))
+            metavar="CARD_CONTENT",
+            help=CARD_CONTENT_HELP)
 
     parser.add_argument(
             '-D', '--deck',
             action='store', dest='deck',
             help=(
-            "set a Deck. the default is 'default'."
+            "Set a Deck. The default is 'default'."
             ))
 
     parser.add_argument(
             '-t', '--type',
             action='store', dest='cardtype',
             help=(
-            "set a card type. the default is 'Basic'."
+            "Set a card type. The default is 'Basic'."
             ))
 
     parser.add_argument(
             '-i', '--ip',
             action='store', dest='ip',
             help=(
-            "set a ip that AnkiConnect specified. the default is '127.0.0.1'."
+            "Set a ip that AnkiConnect specified. The default is '127.0.0.1'."
             ))
 
     parser.add_argument(
             '-p', '--port',
             action='store', dest='port', type=int,
             help=(
-            "set a port number that AnkiConnect specified. the default is '8765'."
+            "Set a port number that AnkiConnect specified. The default is '8765'."
             ))
 
     parser.add_argument(
             '-f', '--file',
             action='store', dest='file', nargs='*',
             help=(
-            'set a file that contains card contents.'
+            'Set a file that contains card contents.'
             ))
 
     parser.add_argument(
             '-c', '--config',
             metavar="FILE",
             action='store', dest='config',
             help=(
-            "set a config file to import config options. without this option, " \
-            "this program searches '~/.trrc'."
+            "Set a config file to import config options. Without this option, " \
+            "this program searches '~/.trrc', '$PWD/.trrc'."
             ))
 
     parser.add_argument(
             '--alias',
             metavar="SECTION",
             action='store', dest='alias',
             help=(
-            "set a section of a config file to apply options. without this " \
+            "Set a section of a config file to apply options. Without this " \
             "argument, the default is 'default'."
             ))
 
     parser.add_argument(
             '-F', '--IFS',
             action='store', dest='ifs',
             help=(
-            "set a delimiter of card contents to use any character other than " \
-            "a tab character. the default is a tab character."
+            "Set a delimiter of card contents to use any character other than " \
+            "a tab character. The default is a tab character."
             ))
 
     parser.add_argument(
             '--field',
             metavar="COLON:DELIMITER-SEPARATED:FIELDS",
             action='store', dest='field',
             help=(
-            "set a card field corresponding to the cardContents. the default " \
+            "Set a card field corresponding to the [CARD_CONTENT]. The default " \
             "is 'Front:Back:Tags'."
             ))
 
     parser.add_argument(
             '--cloze-field',
             metavar="COLON:DELIMITER-SEPARATED:FIELDS",
             action='store', dest='cloze_field',
             help=(
-            "set a cloze type card field corresponding to the cardContents. " \
+            "Set a cloze type card field corresponding to the [CARD_CONTENT]. " \
             "The default is 'Text:Back Extra:Tags'."
             ))
 
     parser.add_argument(
             '--cloze-type',
             action='store', dest='cloze_type',
             help=CLOZE_TYPE_HELP)
 
     parser.add_argument(
             '--toml-generate',
             action='store_true', dest='toml_generate',
             help=(
-            "print toml configs with current arguments. to set a section of " \
+            "Print toml configs with current arguments. To set a section of " \
             "it, use it with '--toml-section' option."
             ))
 
     parser.add_argument(
             '--toml-write',
             metavar="FILE",
             action='store', dest='toml_write',
             help=(
-            "write a config file with options used. to set a section, use " \
+            "Write a config file with options used. To set a section, use " \
             "'--toml-section'."
             ))
 
     parser.add_argument(
             '--toml-section',
             metavar="SECTION",
             action='store', dest='toml_section',
             help=(
-            "set a toml section. the default is 'untitled'."
+            "Set a toml section. The default is 'untitled'."
             ))
 
     parser.add_argument(
             '-H', '--render-HTML',
             action='store_true', dest='allow_HTML',
             help=(
-            "set to allow to render a HTML tag. the default doesn't allow " \
+            "Set to allow to render a HTML tag. The default doesn't allow " \
             "render a HTML tag, therefore <br> won't be a new line."
             ))
 
     parser.add_argument(
             '--apikey',
             action='store', dest='apikey',
             help=(
-            "set an api key for AnkiConnect. if it is specified, --debug " \
-            "options will mask it because of security concern."
+            "Set an api key for AnkiConnect. If it is specified, --debug " \
+            "option will mask it because of security concern."
             ))
 
     parser.add_argument(
             '--sync',
             action='store_true', dest='sync',
             help=(
-            "sync Anki. if there is a card to process, trrc syncs after " \
-            "adding the card. the default is not to sync."
+            "Sync Anki. If there is a card to process, trrc syncs after " \
+            "adding the card. The default is not to sync."
             ))
 
     parser.add_argument(
             '--force-add',
             action='store_true', dest='force_add',
             help=(
-            "create a card even if there is a duplicate in the deck."
+            "Create a card even if there is a duplicate in the deck."
             ))
 
     parser.add_argument(
             '--dry-run',
             action='store_true', dest='dryrun',
             help=(
-            'perform a trial run without sending to Anki.'
+            'Perform a trial run without sending to Anki.'
             ))
 
     parser.add_argument(
             '--read-file-in-a-content',
             action='store_true', dest='contents_file_import',
             help=(
-            "set to allow to replace a file in contents with its contents. a default setting doesn't read it"
+            "Set to allow to replace a file in contents with its contents. A default setting doesn't read it"
             ))
 
     parser.add_argument(
             '-v', '--verbose',
             action='store_const', dest='verbose', const=logging.INFO,
             help=(
-            'print a card being currently processed.'
+            'Print a card being currently processed.'
             ))
 
     parser.add_argument(
             '--debug', dest='debug', nargs='?', const=logging.DEBUG,
             metavar="FILE",
             help=(
-            'print debug information. if you specify FILE, trrc writes debug there.'
+            'Print debug information. If you specify FILE, trrc writes debug there.'
             ))
 
     parser.add_argument(
             '-V', '--version',
             action='version', dest='version', version=VERSION_MESSAGE,
             help=(
-            'print a version number and a license of trrc.'
+            'Print a version number and a license of trrc.'
             ))
 
     return parser
```

### Comparing `trrc-0.1.1/trrc/utils.py` & `trrc-0.1.2/trrc/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     ask_check_network = """
 AnkiConnect doesn't respond.
 
 Check list
 1. Is your Anki running now? your Anki must be running to use AnkiConnect.
 2. Is your AnkiConnect plugin installed in your Anki application and enabled?
 3. Are an ip and port in option or config files correct?
-4. Does your serverside allow port?
+4. Does your serverside open port?
 """
     connect_time_out = "It's a connection time out."
     unknown_network_error = """It's an unknown error.
 Please report it to https://github.com/Constantin1489/trrc/issues"""
     basictype = 'Basic type must have at least two fields'
     wrong_field = '"cannot create note because it is empty"'
     check_notetype = "ERROR: 'def _check_notetype' No predefined notetype is here"
```

### Comparing `trrc-0.1.1/trrc.egg-info/PKG-INFO` & `trrc-0.1.2/trrc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trrc
-Version: 0.1.1
+Version: 0.1.2
 Summary: a command-line program for creating anki card using AnkiConnect API.
 Home-page: https://github.com/Constantin1489/trrc
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
@@ -709,14 +709,15 @@
     * [PIP](#pip)
     * [MANUAL_INSTALLATION](#manual-installation)
 * [USAGE](#usage)
 * [CONFIG_FILE](#config-file)
 * [LOCATIONS](#locations)
 * [OPTIONS](#options)
 * [FAQ](#faq)
+* [CANGELOG](#changelog)
 * [CONTRIBUTION](#contribution)
 
 ## INTRODUCTION
 
 **ToRRential Card processor**(**trrc**) is a command-line unix-like program to create anki cards using AnkiConnect plugin.(Think a yt-dlp, but this program is for adding cards into Anki.)
 
 I intent to make it as a Unix-like program. Therefore it **leverages a lot of Unix concepts**.
@@ -744,14 +745,16 @@
 You don't have to use all those fields.
 For example, if all field of a type is 'Front:Back:Source:Sound:Tags',
 you can use only some of them. e.g.: 'Front:Back:Tags'.
 ####
 Total cards: 1 Total fails: 1
 ```
 
+See [Youtube demonstration video of the author](https://www.youtube.com/watch?v=-3jCwUEAOHE)
+
 ***if you decide to use this app, I highly recommend to turn apikey option in your AnkiConnect to prevent malicious attack. (It's not a fault of this app nor AnkiConnect. If the port of AnkiConnect opens without an apikey, anybody can modify your anki deck.)*** See also [AnkiConnect Configure](docs/tips/AnkiConnect_configure/AnkiConnect_addon_configure_example.md)
 
 ## INSTALLATION
 
 ### pip
 `pip install trrc`
 
@@ -1103,16 +1106,20 @@
 
 But if your want to send a card using **trrc** from outside of your computer which is running Anki with AnkiConnect, you may need to modify firewall option on the computer or a router.
 
 ### How to make iOS shortcuts with **trrc**
 
 See [iOS_shortcuts_example](docs/tips/iOS_shortcuts_setting_example/iOS_shortcuts_example.md)
 
-### This software misses some characters.
+## Changelog
 
+| Version | Note                     | 
+|:--------|:-------------------------|
+| HEAD    | fix sync option error handle. | 
+| 0.1.1   | init                     | 
 
 ## Contribution
 
 Thank you for letting me know the bug! Please report the bug in [issue tracker](https://github.com/Constantin1489/trrc/issues).
 
 Personally I like this app as a method to add cards and use daily, so I will keep developing it. Because I'm trying to get a job, an update delivery can be slow. But after getting a job, I will learn some good clean code conventions and apply it.
```

### Comparing `trrc-0.1.1/trrc.egg-info/SOURCES.txt` & `trrc-0.1.2/trrc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

