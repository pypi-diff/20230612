# Comparing `tmp/pandasai-0.5.0.tar.gz` & `tmp/pandasai-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.5.0.tar", max compression
+gzip compressed data, was "pandasai-0.5.1.tar", max compression
```

## Comparing `pandasai-0.5.0.tar` & `pandasai-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1055 2023-06-08 16:51:38.818063 pandasai-0.5.0/LICENSE
--rw-r--r--   0        0        0     9138 2023-06-08 16:51:38.818063 pandasai-0.5.0/README.md
--rw-r--r--   0        0        0    19135 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/__init__.py
--rw-r--r--   0        0        0     1678 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/constants.py
--rw-r--r--   0        0        0     1494 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3774 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5432 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1827 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1487 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3040 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4325 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10701 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1838 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1482 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2869 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      595 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      734 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1786 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1333 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1603 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      505 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1414 2023-06-08 16:51:38.822064 pandasai-0.5.0/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1456 2023-06-08 16:51:38.822064 pandasai-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10038 1970-01-01 00:00:00.000000 pandasai-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-12 16:07:34.242269 pandasai-0.5.1/LICENSE
+-rw-r--r--   0        0        0     9138 2023-06-12 16:07:34.242269 pandasai-0.5.1/README.md
+-rw-r--r--   0        0        0    19967 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/__init__.py
+-rw-r--r--   0        0        0     1423 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3837 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1825 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4354 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10683 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1482 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2869 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      595 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1737 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1262 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1554 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1343 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1557 2023-06-12 16:07:34.250269 pandasai-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10060 1970-01-01 00:00:00.000000 pandasai-0.5.1/PKG-INFO
```

### Comparing `pandasai-0.5.0/LICENSE` & `pandasai-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.0/README.md` & `pandasai-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.0/pandasai/__init__.py` & `pandasai-0.5.1/pandasai/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,101 @@
 # -*- coding: utf-8 -*-
 """
 PandasAI is a wrapper around a LLM to make dataframes conversational
 
-This module includes the implementation of basis  PandasAI class with methods to run the LLMs
-models on Pandas dataframes. Following LLMs are implemented so far.
+This module includes the implementation of basis  PandasAI class with methods to run
+the LLMs models on Pandas dataframes. Following LLMs are implemented so far.
 
 Example:
 
-    This module is the Entry point of the `pandasai` package. Following is an example of how to
-    use this Class.
+    This module is the Entry point of the `pandasai` package. Following is an example
+    of how to use this Class.
 
     ```python
     import pandas as pd
     from pandasai import PandasAI
 
     # Sample DataFrame
     df = pd.DataFrame({
-        "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain",
-        "Canada", "Australia", "Japan", "China"],
-        "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416,
-        1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+        "country": ["United States", "United Kingdom", "France", "Germany", "Italy",
+        "Spain", "Canada", "Australia", "Japan", "China"],
+        "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832,
+        1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440,
+        14631844184064],
         "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
     })
 
     # Instantiate a LLM
     from pandasai.llm.openai import OpenAI
     llm = OpenAI(api_token="YOUR_API_TOKEN")
 
     pandas_ai = PandasAI(llm)
     pandas_ai(df, prompt='Which are the 5 happiest countries?')
 
     ```
 """
 import ast
 import io
+import logging
 import re
 import sys
 import uuid
 from contextlib import redirect_stdout
 from typing import List, Optional, Union
 
 import astor
-import matplotlib.pyplot as plt
 import pandas as pd
-
 from .constants import (
-    ENVIRONMENT_DEFAULTS,
     WHITELISTED_BUILTINS,
     WHITELISTED_LIBRARIES,
-    WHITELISTED_OPTIONAL_LIBRARIES,
 )
 from .exceptions import BadImportError, LLMNotFoundError
-from .helpers._optional import import_optional_dependency
+from .helpers._optional import import_dependency
 from .helpers.anonymizer import anonymize_dataframe_head
 from .helpers.cache import Cache
 from .helpers.notebook import Notebook
 from .helpers.save_chart import add_save_chart
 from .llm.base import LLM
 from .middlewares.base import Middleware
+from .middlewares.charts import ChartsMiddleware
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
 
 
-# pylint: disable=too-many-instance-attributes disable=too-many-arguments
 class PandasAI:
     """
     PandasAI is a wrapper around a LLM to make dataframes conversational.
 
 
-    This is an entry point of `pandasai` object. This class consists of methods to interface the
-    LLMs with Pandas     dataframes. A pandas dataframe metadata i.e. df.head() and prompt is
-    passed on to chosen LLMs API end point to     generate a Python code to answer the questions
-    asked. The resultant python code is run on actual data and answer is converted into a
-    conversational form.
+    This is an entry point of `pandasai` object. This class consists of methods
+    to interface the LLMs with Pandas     dataframes. A pandas dataframe metadata i.e.
+    df.head() and prompt is passed on to chosen LLMs API end point to generate a Python
+    code to answer the questions asked. The resultant python code is run on actual data
+    and answer is converted into a conversational form.
 
     Note:
         Do not include the `self` parameter in the ``Args`` section.
     Args:
         _llm (obj): LLMs option to be used for API access
         _verbose (bool, optional): To show the intermediate outputs e.g. python code
         generated and execution step on the prompt. Default to False
-        _is_conversational_answer (bool, optional): Whether to return answer in conversational
-        form. Default to False
+        _is_conversational_answer (bool, optional): Whether to return answer in
+        conversational form. Default to False
         _enforce_privacy (bool, optional): Do not display the data on prompt in case of
         Sensitive data. Default to False
-        _max_retries (int, optional): max no. of tries to generate code on failure. Default to 3
+        _max_retries (int, optional): max no. of tries to generate code on failure.
+        Default to 3
         _is_notebook (bool, optional): Whether to run code in notebook. Default to False
-        _original_instructions (dict, optional): The dict of instruction to run. Default to None
-        last_code_generated (str, optional): Pass last Code if generated. Default to None
+        _original_instructions (dict, optional): The dict of instruction to run. Default
+        to None
+        last_code_generated (str, optional): Pass last Code if generated. Default to
+        None
         last_run_code (str, optional): Pass the last execution / run. Default to None
         code_output (str, optional): The code output if any. Default to None
         last_error (str, optional): Error of running code last time. Default to None
         prompt_id (str, optional): Unique ID to differentiate calls. Default to None
 
 
     Returns (str): Response to a Question related to Data
@@ -113,15 +114,16 @@
         "num_rows": None,
         "num_columns": None,
         "rows_to_display": None,
     }
     _cache: Cache = Cache()
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
-    _middlewares: List[Middleware] = None
+    _middlewares: List[Middleware] = [ChartsMiddleware()]
+    _additional_dependencies: List[dict] = []
     last_code_generated: Optional[str] = None
     last_run_code: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
     def __init__(
         self,
@@ -135,20 +137,38 @@
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
-            conversational (bool): Whether to return answer in conversational form. Default to False
-            verbose (bool): To show the intermediate outputs e.g. python code generated and
-             execution step on the prompt.  Default to False
-            enforce_privacy (bool): Execute the codes with Privacy Mode ON.  Default to False
-            save_charts (bool): Save the charts generated in the notebook. Default to False
+            conversational (bool): Whether to return answer in conversational form.
+            Default to False
+            verbose (bool): To show the intermediate outputs e.g. python code
+            generated and execution step on the prompt.  Default to False
+            enforce_privacy (bool): Execute the codes with Privacy Mode ON.
+            Default to False
+            save_charts (bool): Save the charts generated in the notebook.
+            Default to False
         """
+
+        # configure the logging
+        # noinspection PyArgumentList
+        # https://stackoverflow.com/questions/61226587/pycharm-does-not-recognize-logging-basicconfig-handlers-argument
+        handlers = [logging.FileHandler("pandasai.log")]
+        if verbose:
+            handlers.append(logging.StreamHandler(sys.stdout))
+        logging.basicConfig(
+            level=logging.INFO,
+            format="%(asctime)s [%(levelname)s] %(message)s",
+            datefmt="%Y-%m-%d %H:%M:%S",
+            handlers=handlers,
+        )
+        self._logger = logging.getLogger(__name__)
+
         if llm is None:
             raise LLMNotFoundError(
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
         self._llm = llm
         self._is_conversational_answer = conversational
         self._verbose = verbose
@@ -194,18 +214,18 @@
     ) -> Union[str, pd.DataFrame]:
         """
         Run the PandasAI to make Dataframes Conversational.
 
         Args:
             data_frame (pd.Dataframe): A pandas Dataframe
             prompt (str): A prompt to query about the Dataframe
-            is_conversational_answer (bool): Whether to return answer in conversational form.
-            Default to False
-            show_code (bool): To show the intermediate python code generated on the prompt.
-            Default to False
+            is_conversational_answer (bool): Whether to return answer in conversational
+            form. Default to False
+            show_code (bool): To show the intermediate python code generated on the
+            prompt. Default to False
             anonymize_df (bool): Running the code with Sensitive Data. Default to True
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
         Returns (str): Answer to the Input Questions about the DataFrame
 
         """
@@ -278,15 +298,15 @@
                 )
 
                 self._cache.set(prompt, code)
 
             if show_code and self._in_notebook:
                 self.notebook.create_new_cell(code)
 
-            for middleware in self._middlewares if self._middlewares else []:
+            for middleware in self._middlewares:
                 code = middleware(code)
 
             answer = self.run_code(
                 code,
                 data_frame,
                 use_error_correction_framework=use_error_correction_framework,
             )
@@ -295,15 +315,15 @@
 
             if is_conversational_answer is None:
                 is_conversational_answer = self._is_conversational_answer
             if is_conversational_answer:
                 answer = self.conversational_answer(prompt, answer)
                 self.log(f"Conversational answer: {answer}")
             return answer
-        except Exception as exception:  # pylint: disable=broad-except
+        except Exception as exception:
             self.last_error = str(exception)
             print(exception)
             return (
                 "Unfortunately, I was not able to answer your question, "
                 "because of the following error:\n"
                 f"\n{exception}\n"
             )
@@ -312,16 +332,14 @@
         """
         Add middlewares to PandasAI instance.
 
         Args:
             *middlewares: A list of middlewares
 
         """
-        if self._middlewares is None:
-            self._middlewares = []
         self._middlewares.extend(middlewares)
 
     def clear_cache(self):
         """
         Clears the cache of the PandasAI instance.
         """
         self._cache.clear()
@@ -355,43 +373,55 @@
             prompt,
             is_conversational_answer,
             show_code,
             anonymize_df,
             use_error_correction_framework,
         )
 
-    def _is_unsafe_import(self, node: ast.stmt) -> bool:
+    def _check_imports(self, node: Union[ast.Import, ast.ImportFrom]):
         """
-        Remove non-whitelisted imports from the code to prevent malicious code execution
+        Add whitelisted imports to _additional_dependencies.
 
         Args:
-            node (object): ast.stmt
+            node (object): ast.Import or ast.ImportFrom
 
-        Returns (bool): A flag if unsafe_imports found.
+        Raises:
+            BadImportError: If the import is not whitelisted
 
         """
+        # clear recent optional dependencies
+        self._additional_dependencies = []
+
+        if isinstance(node, ast.Import):
+            module = node.names[0].name
+        else:
+            module = node.module
+
+        library = module.split(".")[0]
+
+        if library == "pandas":
+            return
 
-        if isinstance(node, (ast.Import, ast.ImportFrom)):
+        if library in WHITELISTED_LIBRARIES:
             for alias in node.names:
-                if (
-                    alias.name in WHITELISTED_BUILTINS
-                    or alias.name in ENVIRONMENT_DEFAULTS
-                ):
-                    return True
-                if alias.name in WHITELISTED_OPTIONAL_LIBRARIES:
-                    import_optional_dependency(alias.name)
-                    continue
-                if alias.name.split(".")[0] not in WHITELISTED_LIBRARIES:
-                    raise BadImportError(alias.name)
+                self._additional_dependencies.append(
+                    {
+                        "module": module,
+                        "name": alias.name,
+                        "alias": alias.asname or alias.name,
+                    }
+                )
+            return
 
-        return False
+        if library not in WHITELISTED_BUILTINS:
+            raise BadImportError(library)
 
     def _is_df_overwrite(self, node: ast.stmt) -> bool:
         """
-        Remove df declarations from the code to prevent malicious code execution. A helper method.
+        Remove df declarations from the code to prevent malicious code execution.
 
         Args:
             node (object): ast.stmt
 
         Returns (bool):
 
         """
@@ -411,66 +441,72 @@
 
         Returns (str): Returns a Clean Code String
 
         """
 
         tree = ast.parse(code)
 
-        new_body = [
-            node
-            for node in tree.body
-            if not (self._is_unsafe_import(node) or self._is_df_overwrite(node))
-        ]
+        new_body = []
+
+        for node in tree.body:
+            if isinstance(node, (ast.Import, ast.ImportFrom)):
+                self._check_imports(node)
+                continue
+            if self._is_df_overwrite(node):
+                continue
+            new_body.append(node)
 
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree).strip()
 
     def run_code(
         self,
         code: str,
         data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
     ) -> str:
         """
-        A method to execute the python code generated by LLMs to answer the question about the
-        input dataframe. Run the code in the current context and return the result.
+        A method to execute the python code generated by LLMs to answer the question
+        about the input dataframe. Run the code in the current context and return the
+        result.
 
         Args:
             code (str): A python code to execute
             data_frame (pd.DataFrame): A full Pandas DataFrame
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
         Returns (str): String representation of the result of the code execution.
 
         """
 
-        # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
-
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
-            code = add_save_chart(code, self._prompt_id)
+            code = add_save_chart(code, self._prompt_id, not self._verbose)
 
         # Get the code to run removing unsafe imports and df overwrites
         code_to_run = self._clean_code(code)
         self.last_run_code = code_to_run
         self.log(
             f"""
 Code running:
 ```
 {code_to_run}
 ```"""
         )
 
         environment: dict = {
+            "pd": pd,
             **{
-                alias: sys.modules[library]
-                for library, alias in ENVIRONMENT_DEFAULTS.items()
+                lib["alias"]: getattr(import_dependency(lib["module"]), lib["name"])
+                if hasattr(import_dependency(lib["module"]), lib["name"])
+                else import_dependency(lib["module"])
+                for lib in self._additional_dependencies
             },
             "__builtins__": {
                 **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
             },
         }
 
         if multiple:
@@ -486,15 +522,15 @@
             count = 0
             while count < self._max_retries:
                 try:
                     # Execute the code
                     exec(code_to_run, environment)
                     code = code_to_run
                     break
-                except Exception as e:  # pylint: disable=W0718 disable=C0103
+                except Exception as e:
                     if not use_error_correction_framework:
                         raise e
 
                     count += 1
 
                     if multiple:
                         error_correcting_instruction = (
@@ -531,21 +567,20 @@
 
         match = re.match(r"^print\((.*)\)$", last_line)
         if match:
             last_line = match.group(1)
 
         try:
             return eval(last_line, environment)
-        except Exception:  # pylint: disable=W0718
+        except Exception:
             return captured_output
 
     def log(self, message: str):
         """Log a message"""
-        if self._verbose:
-            print(message)
+        self._logger.info(message)
 
     def process_id(self) -> str:
         """Return the id of this PandasAI object."""
         return self._process_id
 
     def last_prompt_id(self) -> str:
         """Return the id of the last prompt that was run."""
```

### Comparing `pandasai-0.5.0/pandasai/exceptions.py` & `pandasai-0.5.1/pandasai/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,9 +64,10 @@
         __init__ method of BadImportError Class
 
         Args:
             library_name (str): Name of the library that is not in the whitelist.
         """
         self.library_name = library_name
         super().__init__(
-            f"Generated code includes import of {library_name} which is not in whitelist."
+            f"Generated code includes import of {library_name} which"
+            " is not in whitelist."
         )
```

### Comparing `pandasai-0.5.0/pandasai/helpers/_optional.py` & `pandasai-0.5.1/pandasai/helpers/_optional.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
 VERSIONS = {
     "sklearn": "1.2.2",
     "statsmodels": "0.14.0",
     "seaborn": "0.12.2",
     "plotly": "5.14.1",
     "ggplot": "0.11.5",
+    "numpy": "1.21.2",
+    "matplotlib": "3.7.3",
+    "scipy": "1.9.0",
 }
 
 # A mapping from import name to package name (on PyPI) for packages where
 # these two names are different.
 
 INSTALL_MAPPING = {}
 
@@ -36,15 +39,15 @@
 
     if version is None:
         raise ImportError(f"Can't determine version for {module.__name__}")
 
     return version
 
 
-def import_optional_dependency(
+def import_dependency(
     name: str,
     extra: str = "",
     errors: str = "raise",
     min_version: str | None = None,
 ):
     """
     Import an optional dependency.
```

### Comparing `pandasai-0.5.0/pandasai/helpers/anonymizer.py` & `pandasai-0.5.1/pandasai/helpers/anonymizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 This module contains helper functions for anonymizing data and generating random data
-before sending it to the LLM (An External API). Only df.head() is sent to LLM API,
- hence the df.head() is processed to remove any personal or sensitive information.
+ before sending it to the LLM (An External API).
+
+Only df.head() is sent to LLM API, hence the df.head() is processed
+ to remove any personal or sensitive information.
 
 """
 
 import random
 import re
 import string
```

### Comparing `pandasai-0.5.0/pandasai/helpers/cache.py` & `pandasai-0.5.1/pandasai/helpers/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import glob
 import os
 import shelve
 from os.path import dirname
 
 
 class Cache:
-    """Cache class for caching queries. It is used to cache queries to avoid save time and money.
+    """Cache class for caching queries. It is used to cache queries
+    to save time and money.
 
     Args:
         filename (str): filename to store the cache.
     """
 
     def __init__(self, filename="cache"):
         # define cache directory and create directory if it does not exist
```

### Comparing `pandasai-0.5.0/pandasai/helpers/from_excel.py` & `pandasai-0.5.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.0/pandasai/helpers/notebook.py` & `pandasai-0.5.1/pandasai/helpers/notebook.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,41 +7,40 @@
 
 
 class Notebook:
 
     """Baseclass to implement Notebook helper functions"""
 
     def in_notebook(self) -> bool:
-
         """
         Checks whether the code is running inside a notebook environment.
 
-        Returns (bool): True if the code is running inside a Jupyter notebook, False otherwise.
+        Returns (bool): True if the code is running inside a Jupyter notebook,
+        False otherwise.
         """
         try:
             if "IPKernelApp" not in get_ipython().config:
                 return False
         except (ImportError, AttributeError):
             return False
         return True
 
     def create_new_cell(self, contents: str) -> None:
-
         """
-        Creates a new code cell in the Jupyter notebook and populates it with the specified
-        contents.
+        Creates a new code cell in the Jupyter notebook and populates
+        it with the specified contents.
         Args:
             contents (str): The contents to be added to the new code cell.
 
         ImportError:
             If the IPython module is not installed.
 
         AttributeError:
-            If the 'get_ipython()' call raises an AttributeError, which can happen if the code is
-            not running inside a Jupyter notebook.
+            If the 'get_ipython()' call raises an AttributeError, which can happen
+            if the code is not running inside a Jupyter notebook.
 
         Returns: None
 
         """
 
         payload = {"source": "set_next_input", "text": contents, "replace": False}
         try:
```

### Comparing `pandasai-0.5.0/pandasai/helpers/save_chart.py` & `pandasai-0.5.1/pandasai/helpers/save_chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Helper functions to save charts to a file, if plt.show() is called."""
 import ast
+import logging
 import os
 from itertools import zip_longest
 from os.path import dirname
 from typing import Union
 
 import astor
 
@@ -44,21 +45,23 @@
         return all(
             compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
         )
 
     return node1 == node2
 
 
-def add_save_chart(code: str, folder_name: str) -> str:
+def add_save_chart(code: str, folder_name: str, print_save_dir: bool = True) -> str:
     """
     Add line to code that save charts to a file, if plt.show() is called.
 
     Args:
         code (str): Code to add line to.
         folder_name (str): Name of folder to save charts to.
+        print_save_dir (bool): Print the save directory to the console.
+            Defaults to True.
 
     Returns:
         str: Code with line added.
 
     """
 
     # define chart save directory
@@ -90,11 +93,14 @@
                 filename += f"_{chr(counter)}"
                 counter += 1
 
             chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
             new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
         new_body.append(node)
 
-    new_body.append(ast.parse(f"print(r'Charts saved to: {chart_save_dir}')"))
+    chart_save_msg = f"Charts saving to: {chart_save_dir}"
+    if print_save_dir:
+        print(chart_save_msg)
+    logging.info(chart_save_msg)
 
     new_tree = ast.Module(body=new_body)
     return astor.to_source(new_tree).strip()
```

### Comparing `pandasai-0.5.0/pandasai/llm/azure_openai.py` & `pandasai-0.5.1/pandasai/llm/azure_openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """OpenAI LLM via Microsoft Azure Cloud
 
-This module is to run the OpenAI API when using Microsoft Cloud infrastructure. Azure has
-implemented the openai API access to its platform.
+This module is to run the OpenAI API when using Microsoft Cloud infrastructure.
+Azure has implemented the openai API access to its platform.
 For details https://learn.microsoft.com/en-us/azure/cognitive-services/openai/reference.
 
 Example:
     Use below example to call AzureOpenAI class
 
     >>> from pandasai.llm.azure_openai import AzureOpenAI
 
@@ -37,24 +37,26 @@
 
     def __init__(
         self,
         api_token: Optional[str] = None,
         api_base: Optional[str] = None,
         api_version: Optional[str] = None,
         deployment_name: str = None,
-        **kwargs, ):
-
+        **kwargs,
+    ):
         """
         __init__ method of AzureOpenAI Class
 
         Args:
             api_token (str): Azure OpenAI API token.
             api_base (str): Base url of the Azure endpoint.
-                It should look like the following: <https://YOUR_RESOURCE_NAME.openai.azure.com/>
-            api_version (str): Version of the Azure OpenAI API. Be aware the API version may change.
+                It should look like the following:
+                <https://YOUR_RESOURCE_NAME.openai.azure.com/>
+            api_version (str): Version of the Azure OpenAI API. Be aware the API
+            version may change.
             deployment_name: Custom name of the deployed model
             **kwargs: Inference Parameters
         """
 
         self.api_token = api_token or os.getenv("AZURE_OPENAI_KEY") or None
         self.api_base = api_base or os.getenv("AZURE_OPENAI_ENDPOINT") or None
         self.api_version = api_version or "2023-03-15-preview"
@@ -92,24 +94,22 @@
                 f"Invalid Azure OpenAI Base Endpoint {api_base}"
             ) from ex
 
         self._set_params(**kwargs)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
-
         """Get the default parameters for calling OpenAI API
 
         Returns: A dict of Default Params
 
         """
         return {**super()._default_params, "engine": self.engine}
 
     def call(self, instruction: str, value: str, suffix: str = "") -> str:
-
         """
         Call the Azure OpenAI LLM.
 
         Args:
             instruction (str): Instruction to pass
             value (str): Value to pass
             suffix(str): Suffix to pass
```

### Comparing `pandasai-0.5.0/pandasai/llm/base.py` & `pandasai-0.5.1/pandasai/llm/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Base class to implement a new LLM
 
-This module is the base class to integrate the various LLMs API. This module also includes the
-Base LLM classes for OpenAI, HuggingFace and Google PaLM.
+This module is the base class to integrate the various LLMs API. This module also
+includes the Base LLM classes for OpenAI, HuggingFace and Google PaLM.
 
 Example:
 
     ```
     from .base import BaseOpenAI
 
     class CustomLLM(BaseOpenAI):
@@ -24,15 +24,15 @@
 
 from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
-from ..helpers._optional import import_optional_dependency
+from ..helpers._optional import import_dependency
 from ..prompts.base import Prompt
 
 
 class LLM:
     """Base class to implement a new LLM."""
 
     last_prompt: Optional[str] = None
@@ -326,15 +326,15 @@
 
         """
 
         if not api_key:
             raise APIKeyNotFoundError("Google Palm API key is required")
 
         err_msg = "Install google-generativeai >= 0.1 for Google Palm API"
-        genai = import_optional_dependency("google.generativeai", extra=err_msg)
+        genai = import_dependency("google.generativeai", extra=err_msg)
 
         genai.configure(api_key=api_key)
         self.genai = genai
 
     def _valid_params(self):
         return ["temperature", "top_p", "top_k", "max_output_tokens"]
```

### Comparing `pandasai-0.5.0/pandasai/llm/fake.py` & `pandasai-0.5.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.0/pandasai/llm/falcon.py` & `pandasai-0.5.1/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.0/pandasai/llm/google_palm.py` & `pandasai-0.5.1/pandasai/llm/google_palm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Google Palm LLM
 
-This module is to run the Google PaLM API hosted and maintained by Google. To read more on Google
-PaLM follow
+This module is to run the Google PaLM API hosted and maintained by Google.
+To read more on Google PaLM follow
 https://developers.generativeai.google/products/palm.
 
 Example:
     Use below example to call GooglePalm Model
 
     >>> from pandasai.llm.google_palm import GooglePalm
 
 """
 from .base import BaseGoogle
 
 
 class GooglePalm(BaseGoogle):
     """Google Palm LLM
-    BaseGoogle class is extended for Google Palm model. The default and only model support at the
-    moment is models/text-bison-001.
+    BaseGoogle class is extended for Google Palm model. The default and only model
+    support at the moment is models/text-bison-001.
 
     """
 
     model: str = "models/text-bison-001"
 
     def __init__(self, api_key: str, **kwargs):
         """
@@ -29,17 +29,15 @@
             api_key (str): API Key
             **kwargs: Extended Parameters inferred from BaseGoogle Class
         """
         self._configure(api_key=api_key)
         self._set_params(**kwargs)
 
     def _valid_params(self):
-        """Returns if the Parameters are valid or Not
-
-        """
+        """Returns if the Parameters are valid or Not"""
         return super()._valid_params() + ["model"]
 
     def _validate(self):
         """
         A method to Validate the Model
 
         """
```

### Comparing `pandasai-0.5.0/pandasai/llm/open_assistant.py` & `pandasai-0.5.1/pandasai/llm/open_assistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Open Assistant LLM
 
-This module is to run the HuggingFace OpenAssistant API hosted and maintained by HuggingFace.co.
-To generate HF_TOKEN go to https://huggingface.co/settings/tokens after creating Account on
-the platform.
+This module is to run the HuggingFace OpenAssistant API hosted and maintained by
+HuggingFace.co. To generate HF_TOKEN go to https://huggingface.co/settings/tokens after
+creating Account on the platform.
 
 Example:
     Use below example to call OpenAssistant Model
 
     >>> from pandasai.llm.open_assistant import OpenAssistant
 """
```

### Comparing `pandasai-0.5.0/pandasai/llm/openai.py` & `pandasai-0.5.1/pandasai/llm/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 load_dotenv()
 
 
 class OpenAI(BaseOpenAI):
     """OpenAI LLM using BaseOpenAI Class.
 
     An API call to OpenAi API is sent and response is recorded and returned.
-    The default chat model is **gpt-3.5-turbo** while **text-davinci-003** is only supported
-    completion model.
+    The default chat model is **gpt-3.5-turbo** while **text-davinci-003** is only
+    supported completion model.
     The list of supported Chat models includes ["gpt-4", "gpt-4-0314", "gpt-4-32k",
      "gpt-4-32k-0314","gpt-3.5-turbo", "gpt-3.5-turbo-0301"].
 
     """
 
     _supported_chat_models = [
         "gpt-4",
```

### Comparing `pandasai-0.5.0/pandasai/llm/starcoder.py` & `pandasai-0.5.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.0/pandasai/middlewares/base.py` & `pandasai-0.5.1/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.0/pandasai/middlewares/streamlit.py` & `pandasai-0.5.1/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.0/pandasai/prompts/base.py` & `pandasai-0.5.1/pandasai/prompts/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 
 from pandasai.exceptions import MethodNotImplementedError
 
 
 class Prompt:
     """Base class to implement a new Prompt"""
 
-    # pylint: disable=too-few-public-methods
-
     text = None
     _args = {}
 
-    def __init__(self, **kwargs): # pylint: disable=super-init-not-called
-
+    def __init__(self, **kwargs):
         """
         __init__ method of Base class of Prompt Module
         Args:
             **kwargs: Inferred Keyword Arguments
         """
         if kwargs:
             self._args = kwargs
```

### Comparing `pandasai-0.5.0/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.5.1/pandasai/prompts/correct_error_prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above
 mentioned error. Do not generate the same code again. Make sure to prefix the requested python
 code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
 ```
-"""
-# pylint:disable=duplicate-code
+"""  # noqa: E501
 from datetime import date
 
 from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 
 from .base import Prompt
 
 
 class CorrectErrorPrompt(Prompt):
     """Prompt to Correct Python code on Error"""
-    # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
 
@@ -44,15 +42,15 @@
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
 Make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
-"""
+"""  # noqa: E501
 
     def __init__(self, **kwargs):
         super().__init__(
             **kwargs,
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
             today_date=date.today()
```

### Comparing `pandasai-0.5.0/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.5.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 
 from .base import Prompt
 
 
 class CorrectMultipleDataframesErrorPrompt(Prompt):
     """Prompt to generate Python code"""
-    # pylint: disable=too-few-public-methods
 
     text: str = """
 You are provided with the following pandas dataframes:"""
 
     def __init__(
         self,
         code: str,
         error_returned: Exception,
         question: str,
         df_head: list[pd.DataFrame],
-    ): # pylint: disable=super-init-not-called
+    ):
         for i, dataframe in enumerate(df_head, start=1):
             row, col = dataframe.shape
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
 This is the result of `print(df{i}.head())`:
 {dataframe}"""
 
@@ -36,13 +35,13 @@
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
 Make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
-"""
+"""  # noqa: E501
 
         self.text += instruction
 
     def __str__(self):
         return self.text
```

### Comparing `pandasai-0.5.0/pandasai/prompts/generate_python_code.py` & `pandasai-0.5.1/pandasai/prompts/generate_python_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,37 +6,35 @@
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the
 dataframe `df`. Using the provided dataframe, df, return the python code and make sure to prefix
 the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG}
 exactly to get the answer to the following question:
 ```
-"""
-# pylint:disable=duplicate-code
+"""  # noqa: E501
 
 from datetime import date
 
 from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 
 from .base import Prompt
 
 
 class GeneratePythonCodePrompt(Prompt):
     """Prompt to generate Python code"""
-    # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the dataframe `df`.
 Using the provided dataframe, df, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
-"""
+"""  # noqa: E501
 
     def __init__(self, **kwargs):
         super().__init__(
             **kwargs,
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
             today_date=date.today()
```

### Comparing `pandasai-0.5.0/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.5.1/pandasai/prompts/multiple_dataframes.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 
 from .base import Prompt
 
 
 class MultipleDataframesPrompt(Prompt):
     """Prompt to generate Python code"""
-    # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
 You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
 Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
-"""
+"""  # noqa: E501
 
-    def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
+    def __init__(self, dataframes: list[pd.DataFrame]):
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
 This is the result of `print(df{i}.head())`:
 {dataframe}"""
```

### Comparing `pandasai-0.5.0/pyproject.toml` & `pandasai-0.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.5.0"
+version = "0.5.1"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -13,48 +13,49 @@
 pandas = "1.5.3"
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
 
-
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
-pylint = "^2.17.3"
+ruff = "^0.0.220"
 pytest = "^7.3.1"
-isort = "^5.12.0"
 pytest-mock = "^3.10.0"
 pytest-env = "^0.8.1"
 click = "^8.1.3"
 
 [tool.poetry.extras]
 google = ["google-generativeai"]
+tests = ["numpy", "seaborn"]
 
 [tool.poetry.group.whitelist.dependencies]
 statsmodels = {version = "^0.14.0", optional = true}
 scikit-learn = {version = "^1.2.2", optional = true}
 seaborn = {version = "^0.12.2", optional = true}
 plotly = {version = "^5.14.1", optional = true}
 ggplot = {version = "^0.11.5", optional = true}
+numpy = {version = "^1.17", optional = true}
+scipy = {version = "^1.9.0", optional = true}
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.0"
 mkdocstrings-python = "0.7.1"
 markdown-include = "^0.6.0"
 
 [tool.poetry.scripts]
 pai = "pai.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.pylint]
-ignore = "tests_*"
+[tool.ruff]
+exclude = ["tests_*"]
 
 [tool.pytest.ini_options]
 env = [
     "HUGGINGFACE_API_KEY=",
     "OPENAI_API_KEY="
 ]
```

### Comparing `pandasai-0.5.0/PKG-INFO` & `pandasai-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
+Provides-Extra: tests
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

