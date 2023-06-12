# Comparing `tmp/turbo_docs-0.9.0.tar.gz` & `tmp/turbo_docs-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-0.9.0.tar", last modified: Sun Jun 11 16:43:01 2023, max compression
+gzip compressed data, was "turbo_docs-0.9.1.tar", last modified: Mon Jun 12 21:25:56 2023, max compression
```

## Comparing `turbo_docs-0.9.0.tar` & `turbo_docs-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.849555 turbo_docs-0.9.0/
--rw-rw-rw-   0        0        0     3430 2023-06-11 16:43:01.847559 turbo_docs-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2933 2023-06-11 16:42:38.000000 turbo_docs-0.9.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 16:43:01.850557 turbo_docs-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-06-11 16:42:54.000000 turbo_docs-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.822259 turbo_docs-0.9.0/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.0/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.837005 turbo_docs-0.9.0/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.9.0/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0      596 2023-06-11 13:01:46.000000 turbo_docs-0.9.0/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0      898 2023-06-11 13:04:26.000000 turbo_docs-0.9.0/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.845469 turbo_docs-0.9.0/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.0/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      432 2023-06-11 12:56:58.000000 turbo_docs-0.9.0/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2022 2023-06-11 15:15:54.000000 turbo_docs-0.9.0/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1581 2023-05-29 19:09:31.000000 turbo_docs-0.9.0/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.833987 turbo_docs-0.9.0/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     3430 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.666760 turbo_docs-0.9.1/
+-rw-rw-rw-   0        0        0     2252 2023-06-12 21:25:56.665753 turbo_docs-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2023-06-12 21:24:42.000000 turbo_docs-0.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 21:25:56.667755 turbo_docs-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-06-12 21:24:58.000000 turbo_docs-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.641359 turbo_docs-0.9.1/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.1/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.655746 turbo_docs-0.9.1/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.9.1/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0      818 2023-06-12 21:24:00.000000 turbo_docs-0.9.1/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0      914 2023-06-12 21:11:03.000000 turbo_docs-0.9.1/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.663752 turbo_docs-0.9.1/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.1/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-06-12 21:10:08.000000 turbo_docs-0.9.1/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2022 2023-06-12 21:03:28.000000 turbo_docs-0.9.1/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      991 2023-06-12 20:59:48.000000 turbo_docs-0.9.1/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.652748 turbo_docs-0.9.1/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2252 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.9.0/README.md` & `turbo_docs-0.9.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,84 @@
+Metadata-Version: 2.1
+Name: turbo_docs
+Version: 0.9.1
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
 # Turbo Docs
 
-Turbo Docs is a Python tool designed to help developers generate a well-formatted README.md file for their repository and perform other tasks related to gathering information from their codebase.
+Turbo Docs is a Python package that helps you generate a well-formatted, user-friendly README.md file for your repository using GPT-3.5-turbo or GPT-4 (default). It also provides a command to copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
 
 ## Installation
 
-You can install Turbo Docs using pip:
+To install Turbo Docs, run the following command:
 
 ```bash
 pip install turbo_docs
 ```
 
+## Requirements
+
+Turbo Docs requires the following packages:
+
+- requests
+- openai
+- llm-blocks
+- click
+- pyperclip
+- redbaron
+- gitpython
+- toml
+- pathspec
+
+These packages will be installed automatically when you install Turbo Docs.
+
 ## Usage
 
-Turbo Docs provides command line options for various tasks, such as generating a README.md file, or copying the formatted directory text to the clipboard. To use Turbo Docs, run the following command in your terminal:
+To use Turbo Docs, run the following command in your terminal:
 
 ```bash
-turbo_docs [options]
+turbo_docs [OPTIONS]
 ```
 
-### Available Options
+### Options
 
-- `--copy`: Copy the formatted text of the entire directory to clipboard. This can be useful when working with GPT. Example:
+- `--copy`: Copy the directory text to the clipboard. Useful for working with ChatGPT.
+- `--readme`: Generate a README.md file. Useful for keeping documentation up to date.
+- `--gpt3`: Use the GPT-3.5 Turbo model instead of GPT-4.
 
-  ```
-  turbo_docs --copy
-  ```
+### Example
 
-- `--readme`: Generate a well-formatted README.md file for the repository. Example:
+To generate a README.md file using GPT-3.5 Turbo, run the following command:
 
-  ```
-  turbo_docs --readme
-  ```
+```bash
+turbo_docs --readme --gpt3
+```
 
 ## Configuration
 
-To configure Turbo Docs, create a `turbo_docs.toml` file in the root of your project and specify the files and directories to ignore. The following example shows how to exclude different types of files and directories:
+You can configure Turbo Docs by creating a `turbo_docs.toml` file in your repository. This file allows you to specify files and folders to ignore when generating the README.md file or copying the directory text to the clipboard.
+
+Example `turbo_docs.toml`:
 
 ```toml
-ignore = 
+ignore = [
     "__pycache__",
     "venv",
     "build",
     "dist",
     "*.egg-info",
     ".git",
     "README.md",  # This is recommended so that --readme doesn't include the readme file itself
 ]
 ```
 
-## Files and Folders Overview
-
-Here's an overview of the files and folders in the Turbo Docs repository:
-
-- `turbo_docs\commands\readme.py`: Contains the `readme` function that generates a README.md file using the OpenAI API.
-- `turbo_docs\commands\__init__.py`: The init file for the `turbo_docs.commands` package.
-- `turbo_docs\generate.py`: The main module containing the `driver` function which is the entry point for the script.
-- `turbo_docs\utils\cli_options.py`: Contains the functions for adding command-line options, such as `copy` and `readme`.
-- `turbo_docs\utils\directory.py`: Contains utility functions for working with directories and reading text from files.
-- `turbo_docs\utils\openai_api.py`: Contains utility functions for interacting with the OpenAI API.
-- `turbo_docs\__init__.py`: The init file for the `turbo_docs` package.
-- `.gitignore`: A list of files and directories to be ignored by GIT.
-- `exclude.toml`: Example toml configuration file for specifying files or directories to exclude.
-- `requirements.txt`: Lists all the required Python packages for Turbo Docs.
-- `setup.py`: Sets up the Turbo Docs Python package.
-- `turbo_docs.toml`: The Turbo Docs configuration file.
-
-## Dependencies
-
-Turbo Docs uses the following Python packages:
-
-- `requests`
-- `openai`
-- `click`
-- `pyperclip`
-- `redbaron`
-- `gitpython`
-- `toml`
-- `pathspec`
-
-Please make sure these packages are installed before running Turbo Docs.
-
 ## License
 
-Turbo Docs is released under the MIT License. See the LICENSE file for more details.
+Turbo Docs is released under the MIT License.
```

### Comparing `turbo_docs-0.9.0/setup.py` & `turbo_docs-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.9.0",
+	version="0.9.1",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-0.9.0/turbo_docs/generate.py` & `turbo_docs-0.9.1/turbo_docs/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,35 @@
 from turbo_docs.commands import readme as readme_module
 from turbo_docs.utils import directory, cli_options
 
 
 @click.command()
 @cli_options.copy
 @cli_options.readme
+@cli_options.gpt3
 def driver(
         copy: bool,
         readme: bool,
+        gpt3: bool,
 ) -> None:
     """
     Pull text from all files in the current directory and apply the following commands:
 
     'turbo_docs --copy' copies the text to clipboard
         Useful for wokring with ChatGPT
 
     'turbo_docs --readme' generates a README.md file
         Useful for keeping documentation up to date
     """
     dir_text = directory.get_repo_text()
 
     if copy:
         pyperclip.copy(dir_text)
-        print("(--copy) Directory text copied to clipboard")
+        print("Directory copied to clipboard")
 
     if readme:
-        readme_module.readme(dir_text)
-        print("(--readme) README.md file generated")
+        readme_module.readme(dir_text, gpt3)
+        print("Generated README.md")
 
 
 if __name__ == '__main__':
     driver()
```

### Comparing `turbo_docs-0.9.0/turbo_docs/utils/directory.py` & `turbo_docs-0.9.1/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

