# Comparing `tmp/aichat-cli-0.4.5.tar.gz` & `tmp/aichat-cli-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aichat-cli-0.4.5.tar", last modified: Sat Jun 10 20:01:59 2023, max compression
+gzip compressed data, was "aichat-cli-0.4.6.tar", last modified: Mon Jun 12 12:16:37 2023, max compression
```

## Comparing `aichat-cli-0.4.5.tar` & `aichat-cli-0.4.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 20:01:59.004407 aichat-cli-0.4.5/
--rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     4378 2023-06-10 20:01:59.004407 aichat-cli-0.4.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 20:01:59.002282 aichat-cli-0.4.5/aichat_cli.egg-info/
--rw-rw-rw-   0        0        0     4378 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 20:01:58.000000 aichat-cli-0.4.5/aichat_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 20:01:59.005405 aichat-cli-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-06-10 19:48:02.000000 aichat-cli-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:37.063806 aichat-cli-0.4.6/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0     5218 2023-06-12 12:16:37.062805 aichat-cli-0.4.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:37.061806 aichat-cli-0.4.6/aichat_cli.egg-info/
+-rw-rw-rw-   0        0        0     5218 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:16:37.063806 aichat-cli-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-06-12 12:16:06.000000 aichat-cli-0.4.6/setup.py
```

### Comparing `aichat-cli-0.4.5/LICENSE` & `aichat-cli-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aichat-cli-0.4.5/PKG-INFO` & `aichat-cli-0.4.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.5
+Version: 0.4.6
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ai Chat CLI
 
+[![PyPI version](https://img.shields.io/pypi/v/aichat-cli.svg)](https://pypi.org/project/aichat-cli/)
 [![Did i find a bad token today ?](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml/badge.svg)](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml)
 
 A command-line interface chatbot. It allows you to have interactive conversations with different bots, including GPT4 FOR FREE
 
 Check the web version [here](https://github.com/TheLime1/gptCensorFree) (WIP).
 
 Thanks to [@Lomusire](https://github.com/Lomusire) for providing premium tokens ❤️.
@@ -45,17 +46,38 @@
 ```
 pip install -r requirements.txt
 ```
 
 4. Run the CLI app:
 
 ```
-python gpt_cli.py
+python chatcli.py
 ```
 
+## OR download it using pip📥📦
+
+```
+pip install aichat-cli --upgrade
+```
+
+<details>
+<summary>📦#####How to add pip package to PATH#####📦</summary>
+
+1. Open the command prompt.
+2. Type `pip show aichat-cli` and press Enter. This will show you the location of the package.
+3. Copy the path of the package.
+4. Open the Start menu and search for “Environment Variables”.
+5. Click on “Edit the system environment variables”.
+6. Click on “Environment Variables” button.
+7. Under “System Variables”, scroll down and find “Path” and click on “Edit”.
+8. Click on “New” and paste the path of the package that you copied earlier.
+9.  Click on “OK” to save changes.
+</details>
+
+
 <details>
 <summary>🔐#####How To generate tokens manually#####🔐</summary>
 
 ---
 ### poe token
 
 Log into [Poe](https://poe.com/) on any web browser, then open your browser's developer tools (also known as "inspect") and look for the value of the `p-b` cookie in the following menus:
@@ -108,15 +130,15 @@
 
 If you don't provide any command-line arguments, the app will prompt you to choose a bot and enter a message interactively.
 
 Once the conversation starts, you can continue the interaction by typing your messages or selecting options from the menu. The menu options include changing the bot or exporting the conversation to a .txt file.
 
 ## Notes📌
 
-- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` in `/token_gen` script provided.
+- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` in `/aichat/token_gen` script provided.
 
 - The CLI app also supports the use of premium tokens , so you can be able to use GPT4.
 
 - The conversation history is stored within the app and is not persistent between sessions.
 
 Feel free to customize and enhance the GPT CLI app according to your needs. Happy **chatting**!
```

### Comparing `aichat-cli-0.4.5/aichat_cli.egg-info/PKG-INFO` & `aichat-cli-0.4.6/aichat_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.5
+Version: 0.4.6
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ai Chat CLI
 
+[![PyPI version](https://img.shields.io/pypi/v/aichat-cli.svg)](https://pypi.org/project/aichat-cli/)
 [![Did i find a bad token today ?](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml/badge.svg)](https://github.com/TheLime1/gpt-cli/actions/workflows/bad_token.yml)
 
 A command-line interface chatbot. It allows you to have interactive conversations with different bots, including GPT4 FOR FREE
 
 Check the web version [here](https://github.com/TheLime1/gptCensorFree) (WIP).
 
 Thanks to [@Lomusire](https://github.com/Lomusire) for providing premium tokens ❤️.
@@ -45,17 +46,38 @@
 ```
 pip install -r requirements.txt
 ```
 
 4. Run the CLI app:
 
 ```
-python gpt_cli.py
+python chatcli.py
 ```
 
+## OR download it using pip📥📦
+
+```
+pip install aichat-cli --upgrade
+```
+
+<details>
+<summary>📦#####How to add pip package to PATH#####📦</summary>
+
+1. Open the command prompt.
+2. Type `pip show aichat-cli` and press Enter. This will show you the location of the package.
+3. Copy the path of the package.
+4. Open the Start menu and search for “Environment Variables”.
+5. Click on “Edit the system environment variables”.
+6. Click on “Environment Variables” button.
+7. Under “System Variables”, scroll down and find “Path” and click on “Edit”.
+8. Click on “New” and paste the path of the package that you copied earlier.
+9.  Click on “OK” to save changes.
+</details>
+
+
 <details>
 <summary>🔐#####How To generate tokens manually#####🔐</summary>
 
 ---
 ### poe token
 
 Log into [Poe](https://poe.com/) on any web browser, then open your browser's developer tools (also known as "inspect") and look for the value of the `p-b` cookie in the following menus:
@@ -108,15 +130,15 @@
 
 If you don't provide any command-line arguments, the app will prompt you to choose a bot and enter a message interactively.
 
 Once the conversation starts, you can continue the interaction by typing your messages or selecting options from the menu. The menu options include changing the bot or exporting the conversation to a .txt file.
 
 ## Notes📌
 
-- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` in `/token_gen` script provided.
+- If the app cannot find the `token.txt` file or the file is empty, it will automatically generate a new token using the `token_gen.py` in `/aichat/token_gen` script provided.
 
 - The CLI app also supports the use of premium tokens , so you can be able to use GPT4.
 
 - The conversation history is stored within the app and is not persistent between sessions.
 
 Feel free to customize and enhance the GPT CLI app according to your needs. Happy **chatting**!
```

### Comparing `aichat-cli-0.4.5/setup.py` & `aichat-cli-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="aichat-cli",
-    version="0.4.5",
+    version="0.4.6",
     author="TheLime1",
     license="GPLv3",
     description="A CLI app that allows you to have interactive conversations with different AI bots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

