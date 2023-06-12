# Comparing `tmp/gpt4-api-0.1.8.tar.gz` & `tmp/gpt4-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.1.8.tar", last modified: Wed Jun  7 01:59:54 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.1.9.tar", last modified: Mon Jun 12 07:30:24 2023, max compression
```

## Comparing `gpt4-api-0.1.8.tar` & `gpt4-api-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.8/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    10292 2023-06-07 01:39:20.000000 gpt4-api-0.1.8/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.8/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.9/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    10470 2023-06-12 07:29:22.000000 gpt4-api-0.1.9/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.9/setup.py
```

### Comparing `gpt4-api-0.1.8/api/gpt.py` & `gpt4-api-0.1.9/api/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         self.frequency_penalty = frequency_penalty
         # 要生成的文本的数量。默认为1，表示生成一段文本
         self.n = n
         # 是否将生成的文本作为流返回，而不是一次性返回所有文本。默认为False，表示一次性返回所有文本
         # 系统默认内容
         self.system_content = system_content
         self.total_tokens = 0
+        self.prompt_tokens = 0
+        self.completion_tokens = 0
         self.call_back = call_back
         self.threads = []
         self.__worker_flag = True
 
     def __worker(self, run_func):
         while True:
             try:
@@ -82,15 +84,15 @@
             thread = threading.Thread(target=self.__worker, args=(run_func,))
             thread.start()
             self.threads.append(thread)
         for thread in self.threads:
             thread.join()
         # if self.task_is_empty():
         #     self.__worker_flag = False
-        logging.info("Total tokens consumed in this round: %s" % self.total_tokens)
+        logging.info("Total tokens consumed in this round total_token: %s prompt_tokens: %s completion_tokens: %s" % (self.total_tokens, self.prompt_tokens, self.completion_tokens))
 
     @staticmethod
     def process_token(keys):
         usable_openai_keys = {}
         for key in keys:
             usable_openai_keys[key] = 0
         if len(usable_openai_keys) == 0:
@@ -158,18 +160,17 @@
                 elapsed_time = time.time() - start_time
                 response_str = response['choices'][0]['message']['content']
                 messages.append({"role": response['choices'][0]['message']['role'], "content": response_str})
                 completion_tokens = response['usage']['completion_tokens']
                 prompt_tokens = response['usage']['prompt_tokens']
                 total_tokens = response['usage']['total_tokens']
                 self.total_tokens += total_tokens
-                logging.info("request case 【%s】 cost time: %s second" % (case_name, int(elapsed_time)))
-                logging.info("prompt tokens: %s" % prompt_tokens)
-                logging.info("completion tokens: %s" % completion_tokens)
-                logging.info("total tokens: %s" % total_tokens)
+                self.prompt_tokens += prompt_tokens
+                self.completion_tokens += completion_tokens
+                logging.info("request case 【%s】 cost time: %s second, prompt tokens: %s completion tokens: %s total tokens: %s" % (case_name, int(elapsed_time), prompt_tokens, completion_tokens, total_tokens))
                 self.usable_openai_keys[open_ai_key] = total_tokens
                 if call_back_func and self.call_back:
                     call_back_func = self.call_back.get(call_back_func, None)
                     if call_back_func:
                         call_back_func(call_black_parameter(response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name))
             except openai.error.RateLimitError as e:
                 logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request exceeded rate limit: {e} api_key: {open_ai_key}")
```

### Comparing `gpt4-api-0.1.8/setup.py` & `gpt4-api-0.1.9/setup.py`

 * *Files identical despite different names*

