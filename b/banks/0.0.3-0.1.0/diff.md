# Comparing `tmp/banks-0.0.3.tar.gz` & `tmp/banks-0.1.0.tar.gz`

## Comparing `banks-0.0.3.tar` & `banks-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,34 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.0.3/MANIFEST.in
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/__about__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/env.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/prompt.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/extensions/__init__.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/extensions/generate.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/filters/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/filters/lemmatize.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/templates/blog.jinja
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/templates/generate_tweet.jinja
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/templates/summarize.jinja
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.0.3/src/banks/templates/summarize_lemma.jinja
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.0.3/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 banks-0.0.3/README.md
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 banks-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 banks-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.1.0/MANIFEST.in
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 banks-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 banks-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/__about__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/env.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/errors.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/loader.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/prompt.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/extensions/__init__.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/extensions/generate.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/filters/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/filters/lemmatize.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/templates/banks_macros.jinja
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/templates/blog.jinja
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/templates/generate_tweet.jinja
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/templates/run_prompt.jinja
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/templates/run_prompt_process.jinja
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/templates/summarize.jinja
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.1.0/src/banks/templates/summarize_lemma.jinja
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 banks-0.1.0/tests/test_default_templates.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 banks-0.1.0/tests/test_env.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 banks-0.1.0/tests/test_loader.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 banks-0.1.0/tests/test_run_prompt.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 banks-0.1.0/tests/test_default_templates/blog.jinja.out
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 banks-0.1.0/tests/test_default_templates/generate_tweet.jinja.out
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 banks-0.1.0/tests/test_default_templates/summarize.jinja.out
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 banks-0.1.0/tests/test_default_templates/summarize_lemma.jinja.out
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 banks-0.1.0/README.md
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 banks-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 banks-0.1.0/PKG-INFO
```

### Comparing `banks-0.0.3/src/banks/extensions/generate.py` & `banks-0.1.0/src/banks/extensions/generate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023-present Massimiliano Pippi <mpippi@gmail.com>
 #
 # SPDX-License-Identifier: MIT
-from jinja2 import nodes, lexer
-from jinja2.ext import Extension
 import openai
+from jinja2 import nodes
+from jinja2.ext import Extension
 
 CHAT_MODELS = [
     "gpt-4",
     "gpt-4-32k",
     "gpt-3.5-turbo",
 ]
 DEFAULT_MODEL = "gpt-3.5-turbo"
@@ -23,15 +23,15 @@
         lineno = next(parser.stream).lineno
 
         # The args passed to the extension:
         # - the prompt text used to generate new text
         # - (optional) the name of the model use to generate new text
         args = [parser.parse_expression()]
 
-        return nodes.Output([self.call_method('_generate', args)]).set_lineno(lineno)
+        return nodes.Output([self.call_method("_generate", args)]).set_lineno(lineno)
 
     def _generate(self, text, model_name=DEFAULT_MODEL):
         """Helper callback."""
         content = openai.ChatCompletion.create(
             model=model_name,
             messages=[
                 {"role": "system", "content": "You are a helpful assistant."},
```

### Comparing `banks-0.0.3/.gitignore` & `banks-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `banks-0.0.3/LICENSE.txt` & `banks-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `banks-0.0.3/README.md` & `banks-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 # banks
 
 [![PyPI - Version](https://img.shields.io/pypi/v/banks.svg)](https://pypi.org/project/banks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/banks.svg)](https://pypi.org/project/banks)
 
-Banks is a Python library to generate LLM prompts using a template language.
+[Banks](https://en.wikipedia.org/wiki/Arrival_(film)) is the linguist professor who will help you generate meaningful LLM prompts using a template language that makes sense.
+If you're still using `f-strings` for the job, keep reading.
 
 -----
 
 **Table of Contents**
 
 - [banks](#banks)
   - [Installation](#installation)
   - [Examples](#examples)
     - [Generate a blog writing prompt](#generate-a-blog-writing-prompt)
-    - [Reuse templates from files](#reuse-templates-from-files)
     - [Generate a summarizer prompt](#generate-a-summarizer-prompt)
     - [Lemmatize text while processing a template](#lemmatize-text-while-processing-a-template)
     - [Use a LLM to generate a text while rendering a prompt](#use-a-llm-to-generate-a-text-while-rendering-a-prompt)
+    - [Go meta: create a prompt and `generate` its response](#go-meta-create-a-prompt-and-generate-its-response)
+    - [Go meta(meta): process a LLM response](#go-metameta-process-a-llm-response)
+    - [Reuse templates from files](#reuse-templates-from-files)
   - [License](#license)
 
 ## Installation
 
 ```console
 pip install banks
 ```
 
-To use lemmatization and text generation you also need to:
-
-```console
-pip install openai simplemma
-```
-
 ## Examples
 
 ### Generate a blog writing prompt
 
 Given a generic template to instruct an LLM to generate a blog article, we
-use Banks to generate the actual prompt on our topic of choice, "Retrogame computing":
+use Banks to generate the actual prompt on our topic of choice, "retrogame computing":
 
 ```py
 from banks import Prompt
 
 
 p = Prompt("Write a 500-word blog post on {{ topic }}.\n\nBlog post:")
 topic = "retrogame computing"
@@ -51,43 +48,28 @@
 
 ```txt
 Write a 500-word blog post on retrogame computing.
 
 Blog post:
 ```
 
-### Reuse templates from files
-
-We can get the same result as the previous example loading the prompt template from file
-instead of hardcoding it into the Python code. For convenience, Banks comes with a few
-default templates distributed the package. We can load those templates from file like this:
-
-```py
-from banks import Prompt
-
-
-p = Prompt.from_template("blog.jinja")
-topic = "retrogame computing"
-print(p.text({"topic": topic}))
-```
-
 ### Generate a summarizer prompt
 
 Instead of hardcoding the content to summarize in the prompt itself, we can generate it
 starting from a generic one:
 
 
 ```py
 from banks import Prompt
 
 
 prompt_template = """
 Summarize the following documents:
 {% for document in documents %}
-{{document}}
+{{ document }}
 {% endfor %}
 Summary:
 """
 
 # In a real-world scenario, these would be loaded as external resources from files or network
 documents = [
     "A first paragraph talking about AI",
@@ -112,23 +94,30 @@
 
 Summary:
 ```
 
 ### Lemmatize text while processing a template
 
 Banks comes with predefined filters you can use to process data before generating the
-prompt. Say you want to use a lemmatizer on a document you want to summarize:
+prompt. Say you want to use a lemmatizer on a document before summarizing it, first
+you need to install `simplemma`:
+
+```sh
+pip install simplemma
+```
+
+then you can use the `lemmatize` filter in your templates like this:
 
 ```py
 from banks import Prompt
 
 
 prompt_template = """
 Summarize the following document:
-{{document | lemmatize}}
+{{ document | lemmatize }}
 Summary:
 """
 
 p = Prompt(prompt_template)
 print(p.text({"document": "The cats are running"}))
 ```
 
@@ -184,10 +173,94 @@
 ```
 
 If you paste Banks' output into ChatGPT you would get something like this:
 ```txt
 Climate change is a pressing global issue, but together we can create positive change! Let's embrace renewable energy, protect our planet, and build a sustainable future for generations to come. 🌍💚 #ClimateAction #PositiveFuture
 ```
 
+### Go meta: create a prompt and `generate` its response
+
+We can leverage Jinja's macro system to generate a prompt, send the result to OpenAI and get a response.
+Let's bring back the blog writing example:
+
+```py
+from banks import Prompt
+
+prompt_template = """
+{% from "banks_macros.jinja" import run_prompt with context %}
+
+{%- call run_prompt() -%}
+Write a 500-word blog post on {{ topic }}
+
+Blog post:
+{%- endcall -%}
+"""
+
+p = Prompt(prompt_template)
+print(p.text({"topic": "climate change"}))
+```
+
+The snippet above won't print the prompt, instead will generate the prompt text
+
+```
+Write a 500-word blog post on climate change
+
+Blog post:
+```
+
+and will send it to OpenAI using the `generate` extension, eventually returning its response:
+
+```
+Climate change is a phenomenon that has been gaining attention in recent years...
+...
+```
+
+### Go meta(meta): process a LLM response
+
+When generating a response from a prompt template, we can take a step further and
+post-process the LLM response by assinging it to a variable and applying filters
+to it:
+
+```py
+from banks import Prompt
+
+prompt_template = """
+{% from "banks_macros.jinja" import run_prompt with context %}
+
+{%- set prompt_result %}
+{%- call run_prompt() -%}
+Write a 500-word blog post on {{ topic }}
+
+Blog post:
+{%- endcall -%}
+{%- endset %}
+
+{# nothing is returned at this point: the variable 'prompt_result' contains the result #}
+
+{# let's use the prompt_result variable now #}
+{{ prompt_result | upper }}
+"""
+
+p = Prompt(prompt_template)
+print(p.text({"topic": "climate change"}))
+```
+
+The final answer from the LLM will be printed, this time all in uppercase.
+
+### Reuse templates from files
+
+We can get the same result as the previous example loading the prompt template from file
+instead of hardcoding it into the Python code. For convenience, Banks comes with a few
+default templates distributed the package. We can load those templates from file like this:
+
+```py
+from banks import Prompt
+
+
+p = Prompt.from_template("blog.jinja")
+topic = "retrogame computing"
+print(p.text({"topic": topic}))
+```
+
 ## License
 
 `banks` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `banks-0.0.3/pyproject.toml` & `banks-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "jinja2",
   "openai",
-  "simplemma",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/banks#readme"
 Issues = "https://github.com/unknown/banks/issues"
 Source = "https://github.com/unknown/banks"
 
@@ -74,15 +73,15 @@
 fmt = [
   "black {args:.}",
   "ruff --fix {args:.}",
   "style",
 ]
 all = [
   "style",
-  "typing",
+  # "typing",  # FIXME: re-enable once typing is good to go
 ]
 
 [tool.hatch.build.targets.wheel]
 only-include = ["src/banks", "src/templates"]
 
 [tool.hatch.build.targets.wheel.sources]
 "src" = ""
```

### Comparing `banks-0.0.3/PKG-INFO` & `banks-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banks
-Version: 0.0.3
+Version: 0.1.0
 Summary: A prompt programming language
 Project-URL: Documentation, https://github.com/unknown/banks#readme
 Project-URL: Issues, https://github.com/unknown/banks/issues
 Project-URL: Source, https://github.com/unknown/banks
 Author-email: Massimiliano Pippi <mpippi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -16,56 +16,52 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: jinja2
 Requires-Dist: openai
-Requires-Dist: simplemma
 Description-Content-Type: text/markdown
 
 # banks
 
 [![PyPI - Version](https://img.shields.io/pypi/v/banks.svg)](https://pypi.org/project/banks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/banks.svg)](https://pypi.org/project/banks)
 
-Banks is a Python library to generate LLM prompts using a template language.
+[Banks](https://en.wikipedia.org/wiki/Arrival_(film)) is the linguist professor who will help you generate meaningful LLM prompts using a template language that makes sense.
+If you're still using `f-strings` for the job, keep reading.
 
 -----
 
 **Table of Contents**
 
 - [banks](#banks)
   - [Installation](#installation)
   - [Examples](#examples)
     - [Generate a blog writing prompt](#generate-a-blog-writing-prompt)
-    - [Reuse templates from files](#reuse-templates-from-files)
     - [Generate a summarizer prompt](#generate-a-summarizer-prompt)
     - [Lemmatize text while processing a template](#lemmatize-text-while-processing-a-template)
     - [Use a LLM to generate a text while rendering a prompt](#use-a-llm-to-generate-a-text-while-rendering-a-prompt)
+    - [Go meta: create a prompt and `generate` its response](#go-meta-create-a-prompt-and-generate-its-response)
+    - [Go meta(meta): process a LLM response](#go-metameta-process-a-llm-response)
+    - [Reuse templates from files](#reuse-templates-from-files)
   - [License](#license)
 
 ## Installation
 
 ```console
 pip install banks
 ```
 
-To use lemmatization and text generation you also need to:
-
-```console
-pip install openai simplemma
-```
-
 ## Examples
 
 ### Generate a blog writing prompt
 
 Given a generic template to instruct an LLM to generate a blog article, we
-use Banks to generate the actual prompt on our topic of choice, "Retrogame computing":
+use Banks to generate the actual prompt on our topic of choice, "retrogame computing":
 
 ```py
 from banks import Prompt
 
 
 p = Prompt("Write a 500-word blog post on {{ topic }}.\n\nBlog post:")
 topic = "retrogame computing"
@@ -76,43 +72,28 @@
 
 ```txt
 Write a 500-word blog post on retrogame computing.
 
 Blog post:
 ```
 
-### Reuse templates from files
-
-We can get the same result as the previous example loading the prompt template from file
-instead of hardcoding it into the Python code. For convenience, Banks comes with a few
-default templates distributed the package. We can load those templates from file like this:
-
-```py
-from banks import Prompt
-
-
-p = Prompt.from_template("blog.jinja")
-topic = "retrogame computing"
-print(p.text({"topic": topic}))
-```
-
 ### Generate a summarizer prompt
 
 Instead of hardcoding the content to summarize in the prompt itself, we can generate it
 starting from a generic one:
 
 
 ```py
 from banks import Prompt
 
 
 prompt_template = """
 Summarize the following documents:
 {% for document in documents %}
-{{document}}
+{{ document }}
 {% endfor %}
 Summary:
 """
 
 # In a real-world scenario, these would be loaded as external resources from files or network
 documents = [
     "A first paragraph talking about AI",
@@ -137,23 +118,30 @@
 
 Summary:
 ```
 
 ### Lemmatize text while processing a template
 
 Banks comes with predefined filters you can use to process data before generating the
-prompt. Say you want to use a lemmatizer on a document you want to summarize:
+prompt. Say you want to use a lemmatizer on a document before summarizing it, first
+you need to install `simplemma`:
+
+```sh
+pip install simplemma
+```
+
+then you can use the `lemmatize` filter in your templates like this:
 
 ```py
 from banks import Prompt
 
 
 prompt_template = """
 Summarize the following document:
-{{document | lemmatize}}
+{{ document | lemmatize }}
 Summary:
 """
 
 p = Prompt(prompt_template)
 print(p.text({"document": "The cats are running"}))
 ```
 
@@ -209,10 +197,94 @@
 ```
 
 If you paste Banks' output into ChatGPT you would get something like this:
 ```txt
 Climate change is a pressing global issue, but together we can create positive change! Let's embrace renewable energy, protect our planet, and build a sustainable future for generations to come. 🌍💚 #ClimateAction #PositiveFuture
 ```
 
+### Go meta: create a prompt and `generate` its response
+
+We can leverage Jinja's macro system to generate a prompt, send the result to OpenAI and get a response.
+Let's bring back the blog writing example:
+
+```py
+from banks import Prompt
+
+prompt_template = """
+{% from "banks_macros.jinja" import run_prompt with context %}
+
+{%- call run_prompt() -%}
+Write a 500-word blog post on {{ topic }}
+
+Blog post:
+{%- endcall -%}
+"""
+
+p = Prompt(prompt_template)
+print(p.text({"topic": "climate change"}))
+```
+
+The snippet above won't print the prompt, instead will generate the prompt text
+
+```
+Write a 500-word blog post on climate change
+
+Blog post:
+```
+
+and will send it to OpenAI using the `generate` extension, eventually returning its response:
+
+```
+Climate change is a phenomenon that has been gaining attention in recent years...
+...
+```
+
+### Go meta(meta): process a LLM response
+
+When generating a response from a prompt template, we can take a step further and
+post-process the LLM response by assinging it to a variable and applying filters
+to it:
+
+```py
+from banks import Prompt
+
+prompt_template = """
+{% from "banks_macros.jinja" import run_prompt with context %}
+
+{%- set prompt_result %}
+{%- call run_prompt() -%}
+Write a 500-word blog post on {{ topic }}
+
+Blog post:
+{%- endcall -%}
+{%- endset %}
+
+{# nothing is returned at this point: the variable 'prompt_result' contains the result #}
+
+{# let's use the prompt_result variable now #}
+{{ prompt_result | upper }}
+"""
+
+p = Prompt(prompt_template)
+print(p.text({"topic": "climate change"}))
+```
+
+The final answer from the LLM will be printed, this time all in uppercase.
+
+### Reuse templates from files
+
+We can get the same result as the previous example loading the prompt template from file
+instead of hardcoding it into the Python code. For convenience, Banks comes with a few
+default templates distributed the package. We can load those templates from file like this:
+
+```py
+from banks import Prompt
+
+
+p = Prompt.from_template("blog.jinja")
+topic = "retrogame computing"
+print(p.text({"topic": topic}))
+```
+
 ## License
 
 `banks` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

