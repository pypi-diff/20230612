# Comparing `tmp/freeGPT-1.1.6.tar.gz` & `tmp/freeGPT-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.1.6.tar", last modified: Mon Jun  5 09:16:21 2023, max compression
+gzip compressed data, was "freeGPT-1.1.7.tar", last modified: Mon Jun 12 18:16:56 2023, max compression
```

## Comparing `freeGPT-1.1.6.tar` & `freeGPT-1.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.838091 freeGPT-1.1.6/
--rw-rw-rw-   0        0        0    35149 2023-06-05 09:10:43.000000 freeGPT-1.1.6/LICENSE
--rw-rw-rw-   0        0        0       98 2023-06-05 09:10:43.000000 freeGPT-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3399 2023-06-05 09:16:21.822446 freeGPT-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2324 2023-06-05 09:10:43.000000 freeGPT-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.791195 freeGPT-1.1.6/freeGPT/
--rw-rw-rw-   0        0        0     2319 2023-06-05 09:10:43.000000 freeGPT-1.1.6/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.806823 freeGPT-1.1.6/freeGPT/alpaca_7b/
--rw-rw-rw-   0        0        0     1530 2023-06-05 09:10:43.000000 freeGPT-1.1.6/freeGPT/alpaca_7b/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.822446 freeGPT-1.1.6/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     5171 2023-06-05 09:10:43.000000 freeGPT-1.1.6/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.822446 freeGPT-1.1.6/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     6799 2023-06-05 09:10:43.000000 freeGPT-1.1.6/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:16:21.806823 freeGPT-1.1.6/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3399 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 09:16:21.000000 freeGPT-1.1.6/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 09:16:21.838091 freeGPT-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1539 2023-06-05 09:10:43.000000 freeGPT-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:16:56.041886 freeGPT-1.1.7/
+-rw-rw-rw-   0        0        0    35149 2023-06-12 18:13:39.000000 freeGPT-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0       96 2023-06-12 18:13:39.000000 freeGPT-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4074 2023-06-12 18:16:56.039890 freeGPT-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2944 2023-06-12 18:13:39.000000 freeGPT-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:16:56.015885 freeGPT-1.1.7/freeGPT/
+-rw-rw-rw-   0        0        0     2319 2023-06-12 18:13:39.000000 freeGPT-1.1.7/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:16:56.031886 freeGPT-1.1.7/freeGPT/alpaca_7b/
+-rw-rw-rw-   0        0        0     1545 2023-06-12 18:13:39.000000 freeGPT-1.1.7/freeGPT/alpaca_7b/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:16:56.033886 freeGPT-1.1.7/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     5173 2023-06-12 18:13:39.000000 freeGPT-1.1.7/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:16:56.035887 freeGPT-1.1.7/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     6803 2023-06-12 18:13:39.000000 freeGPT-1.1.7/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:16:56.028885 freeGPT-1.1.7/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     4074 2023-06-12 18:16:55.000000 freeGPT-1.1.7/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-12 18:16:55.000000 freeGPT-1.1.7/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:16:55.000000 freeGPT-1.1.7/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-12 18:16:55.000000 freeGPT-1.1.7/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 18:16:55.000000 freeGPT-1.1.7/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:16:56.041886 freeGPT-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1577 2023-06-12 18:13:39.000000 freeGPT-1.1.7/setup.py
```

### Comparing `freeGPT-1.1.6/LICENSE` & `freeGPT-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.6/PKG-INFO` & `freeGPT-1.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.6
-Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
+Version: 1.1.7
+Summary: freeGPT is a Python package that gives free access to GPT and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
+Project-URL: Discord, http://dsc.gg/ruu3fstudio
 Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,alpaca-7b,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -20,20 +21,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
-A Python package that gives access to GPT3 &amp; GPT4 models for free.
+freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 <br>
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
+***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
 
 ## Source:
 *Both GPT models have internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
 | gpt3              | [you.com](https://you.com)                           |
@@ -44,50 +46,65 @@
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
+- [x] Make a discord bot.
 - [ ] Add a text to image generation model.
-- [ ] Make a discord bot.
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
+## Discord bot:
+- Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
+- This bot has ALL the models in this repository available.
+- Its interactive, fast and overall easy to use.
+- And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
+
 ## Examples:
 
 #### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
-    resp = gpt3.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp['text']}")
+    try:
+        # There is also a 'proxy' parameter.
+        resp = gpt3.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp['text'])}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 #### GPT-4:
 ```python
-# Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
-    token = Account.create(logging=True)
+    token = gpt4.Account.create(logging=True)
     prompt = input("👦 > ")
-    resp = gpt4.Completion.create(prompt=prompt, token=token)
-    print(f"🤖 > {resp.text}")
+    try:
+        resp = gpt4.Completion.create(prompt=prompt, token=token)
+        print(f"🤖 > {str(resp.text)}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 
 #### Alpaca-7b:
 ```python
 from freeGPT import alpaca_7b
 
 while True:
     prompt = input("👦 > ")
-    resp = alpaca_7b.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp}")
+    try:
+        resp = alpaca_7b.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp)}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.6/README.md` & `freeGPT-1.1.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
-A Python package that gives access to GPT3 &amp; GPT4 models for free.
+freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 <br>
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
+***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
 
 ## Source:
 *Both GPT models have internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
 | gpt3              | [you.com](https://you.com)                           |
@@ -22,50 +23,65 @@
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
+- [x] Make a discord bot.
 - [ ] Add a text to image generation model.
-- [ ] Make a discord bot.
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
+## Discord bot:
+- Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
+- This bot has ALL the models in this repository available.
+- Its interactive, fast and overall easy to use.
+- And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
+
 ## Examples:
 
 #### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
-    resp = gpt3.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp['text']}")
+    try:
+        # There is also a 'proxy' parameter.
+        resp = gpt3.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp['text'])}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 #### GPT-4:
 ```python
-# Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
-    token = Account.create(logging=True)
+    token = gpt4.Account.create(logging=True)
     prompt = input("👦 > ")
-    resp = gpt4.Completion.create(prompt=prompt, token=token)
-    print(f"🤖 > {resp.text}")
+    try:
+        resp = gpt4.Completion.create(prompt=prompt, token=token)
+        print(f"🤖 > {str(resp.text)}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 
 #### Alpaca-7b:
 ```python
 from freeGPT import alpaca_7b
 
 while True:
     prompt = input("👦 > ")
-    resp = alpaca_7b.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp}")
+    try:
+        resp = alpaca_7b.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp)}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.6/freeGPT/__init__.py` & `freeGPT-1.1.7/freeGPT/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from freeGPT import gpt3, gpt4, alpaca_7b
 
 __author__ = "Ruu3f"
-__version__ = "1.1.6"
+__version__ = "1.1.7"
 __all__ = ["Provider", "Completion"]
 
 
 class Provider(Enum):
     """Enum class representing the available GPT providers."""
 
     ALPACA_7B = "alpaca_7b"
```

### Comparing `freeGPT-1.1.6/freeGPT/alpaca_7b/__init__.py` & `freeGPT-1.1.7/freeGPT/alpaca_7b/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
             "Sec-Ch-Ua-Mobile": "?0",
             "Sec-Ch-Ua-Platform": "Windows",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "cross-site",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36",
         }
-        r = requests.post(
+        resp = requests.post(
             "https://us-central1-arched-keyword-306918.cloudfunctions.net/run-inference-1",
             headers=headers,
             json={"prompt": prompt},
         ).json()
         try:
-            return r["completion"]
-        except:
+            return resp["completion"]
+        except KeyError:
             raise Exception("Unable to fetch the response.")
```

### Comparing `freeGPT-1.1.6/freeGPT/gpt3/__init__.py` & `freeGPT-1.1.7/freeGPT/gpt3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os, re, json
+from typing import Optional, List, Dict, Any
+from uuid import uuid4
 
 try:
     from tls_client import Session
 except ImportError:
     os.system("pip install tls_client --no-cache-dir")
-from uuid import uuid4
-from pydantic import BaseModel
+
 from fake_useragent import UserAgent
-from typing import Optional, List, Dict, Any
 
 
 class Completion:
     """A class that provides methods for creating completion requests."""
 
     @staticmethod
     def create(
@@ -19,20 +19,20 @@
         page: int = 1,
         count: int = 10,
         safe_search: str = "Moderate",
         on_shopping_page: bool = False,
         mkt: str = "",
         response_filter: str = "WebPages,Translations,TimeZone,Computation,RelatedSearches",
         domain: str = "youchat",
-        query_trace_id: str = None,
-        chat: List[str] = None,
+        query_trace_id: Optional[str] = None,
+        chat: Optional[List[str]] = None,
         include_links: bool = False,
         detailed: bool = False,
         proxy: Optional[str] = None,
-    ) -> dict:
+    ) -> Dict[str, Any]:
         """
         Creates a completion request.
 
         Args:
             prompt (str): The prompt text for the completion.
             page (int, optional): The page number for pagination. Defaults to 1.
             count (int, optional): The number of results per page. Defaults to 10.
@@ -53,23 +53,23 @@
         Raises:
             Exception: If unable to get the response.
         """
         if chat is None:
             chat = []
 
         proxies = (
-            {"http": "http://" + proxy, "https": "http://" + proxy} if proxy else {}
+            {"http": "http://" + proxy, "https": "http://" + proxy} if proxy else None
         )
 
         client = Session(client_identifier="chrome_108")
         client.headers = Completion.__get_headers()
         client.proxies = proxies
 
         response = client.get(
-            f"https://you.com/api/streamingSearch",
+            "https://you.com/api/streamingSearch",
             params={
                 "q": prompt,
                 "page": page,
                 "count": count,
                 "safeSearch": safe_search,
                 "onShoppingPage": on_shopping_page,
                 "mkt": mkt,
@@ -82,26 +82,25 @@
             },
         )
 
         if "youChatToken" not in response.text:
             raise Exception("Unable to fetch the response.")
 
         you_chat_serp_results = re.search(
-            r"(?<=event: youChatSerpResults\ndata:)(.*\n)*?(?=event: )", response.text
+            r"(?<=event: youChatSerpResults)\ndata:)(.*\n)*?(?=event: )",
+            response.text,
         ).group()
         third_party_search_results = re.search(
             r"(?<=event: thirdPartySearchResults\ndata:)(.*\n)*?(?=event: )",
             response.text,
         ).group()
 
         text = "".join(re.findall(r'{"youChatToken": "(.*?)"}', response.text))
 
-        extra = {
-            "youChatSerpResults": json.loads(you_chat_serp_results),
-        }
+        extra = {"youChatSerpResults": json.loads(you_chat_serp_results)}
 
         result = {
             "text": text.replace("\\n", "\n").replace("\\\\", "\\").replace('\\"', '"')
         }
 
         if include_links:
             result["links"] = json.loads(third_party_search_results)["search"][
@@ -110,15 +109,15 @@
 
         if detailed:
             result["extra"] = extra
 
         return result
 
     @staticmethod
-    def __get_headers() -> dict:
+    def __get_headers() -> Dict[str, str]:
         """
         Returns the headers for the completion request.
 
         Returns:
             dict: The headers as a dictionary.
         """
         return {
```

### Comparing `freeGPT-1.1.6/freeGPT/gpt4/__init__.py` & `freeGPT-1.1.7/freeGPT/gpt4/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import os, re, json
+import os, re
 
 try:
     from tls_client import Session
 except ImportError:
     os.system("pip install tls_client --no-cache-dir")
 
-from uuid import uuid4
 from requests import post
 from time import time, sleep
-from fake_useragent import UserAgent
-from pymailtm import MailTm, Message
-from typing import Any, List, Generator, Optional
 from pydantic import BaseModel
+from pymailtm import MailTm, Message
+from fake_useragent import UserAgent
+from typing import Any, List, Optional
 
 
 class Choice(BaseModel):
     text: str
     index: int
     logprobs: Any
     finish_reason: str
@@ -217,7 +216,9 @@
                             "total_tokens": len(prompt) + len(token),
                         },
                     }
                 )
                 return final_response
 
         raise Exception("Unable to fetch the response.")
+
+print(Completion.create(prompt="hi").text)
```

### Comparing `freeGPT-1.1.6/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.1.7/freeGPT.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.6
-Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
+Version: 1.1.7
+Summary: freeGPT is a Python package that gives free access to GPT and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
+Project-URL: Discord, http://dsc.gg/ruu3fstudio
 Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,alpaca-7b,gpt4free,freegpt,chatgpt,python,alpaca,openai,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -20,20 +21,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
-A Python package that gives access to GPT3 &amp; GPT4 models for free.
+freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 <br>
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
+***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
 
 ## Source:
 *Both GPT models have internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
 | gpt3              | [you.com](https://you.com)                           |
@@ -44,50 +46,65 @@
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
+- [x] Make a discord bot.
 - [ ] Add a text to image generation model.
-- [ ] Make a discord bot.
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
+## Discord bot:
+- Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
+- This bot has ALL the models in this repository available.
+- Its interactive, fast and overall easy to use.
+- And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
+
 ## Examples:
 
 #### GPT-3:
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
-    resp = gpt3.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp['text']}")
+    try:
+        # There is also a 'proxy' parameter.
+        resp = gpt3.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp['text'])}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 #### GPT-4:
 ```python
-# Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
-    token = Account.create(logging=True)
+    token = gpt4.Account.create(logging=True)
     prompt = input("👦 > ")
-    resp = gpt4.Completion.create(prompt=prompt, token=token)
-    print(f"🤖 > {resp.text}")
+    try:
+        resp = gpt4.Completion.create(prompt=prompt, token=token)
+        print(f"🤖 > {str(resp.text)}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 
 #### Alpaca-7b:
 ```python
 from freeGPT import alpaca_7b
 
 while True:
     prompt = input("👦 > ")
-    resp = alpaca_7b.Completion.create(prompt=prompt)
-    print(f"🤖 > {resp}")
+    try:
+        resp = alpaca_7b.Completion.create(prompt=prompt)
+        print(f"🤖 > {str(resp)}")
+    except Exception as e:
+        print(f"🤖 > {str(e)}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.6/setup.py` & `freeGPT-1.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.1.6",
-    description="freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.",
+    version="1.1.7",
+    description="freeGPT is a Python package that gives free access to GPT and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
         "artificial-intelligence",
@@ -48,9 +48,10 @@
         "curl_cffi",
         "requests",
         "fake-useragent",
     ],
     project_urls={
         "Source": "https://github.com/Ruu3f/freeGPT",
         "Issues": "https://github.com/Ruu3f/freeGPT/issues",
+        "Discord": "http://dsc.gg/ruu3fstudio",
     },
 )
```

