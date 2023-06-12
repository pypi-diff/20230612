# Comparing `tmp/kanu-0.5.0.tar.gz` & `tmp/kanu-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanu-0.5.0.tar", last modified: Thu Jun  8 00:32:08 2023, max compression
+gzip compressed data, was "kanu-0.6.0.tar", last modified: Mon Jun 12 03:25:43 2023, max compression
```

## Comparing `kanu-0.5.0.tar` & `kanu-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-08 00:32:08.635644 kanu-0.5.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-08 00:31:53.000000 kanu-0.5.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)      853 2023-06-08 00:32:08.635495 kanu-0.5.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      537 2023-06-08 00:31:53.000000 kanu-0.5.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-08 00:32:08.634660 kanu-0.5.0/kanu/
--rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/__init__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     9960 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/__main__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     1959 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/chatgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)     8295 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/docgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)      844 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/utils.py
--rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/version.py
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-08 00:32:08.635302 kanu-0.5.0/kanu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)      853 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      264 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/entry_points.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-08 00:32:08.635702 kanu-0.5.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-08 00:31:53.000000 kanu-0.5.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-12 03:25:43.795226 kanu-0.6.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-12 03:25:27.000000 kanu-0.6.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)     2115 2023-06-12 03:25:43.795083 kanu-0.6.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)     1799 2023-06-12 03:25:27.000000 kanu-0.6.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-12 03:25:43.794261 kanu-0.6.0/kanu/
+-rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    10380 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/__main__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     2347 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/chatgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     8900 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/docgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     6943 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/utils.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-12 03:25:27.000000 kanu-0.6.0/kanu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-12 03:25:43.794874 kanu-0.6.0/kanu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)     2115 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      264 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/entry_points.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-12 03:25:43.000000 kanu-0.6.0/kanu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-12 03:25:43.795275 kanu-0.6.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-12 03:25:27.000000 kanu-0.6.0/setup.py
```

### Comparing `kanu-0.5.0/LICENSE` & `kanu-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kanu-0.5.0/kanu/__main__.py` & `kanu-0.6.0/kanu/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,22 +80,28 @@
         b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("ChatGPT", e.get(), self.model.get(), self.temperature.get(), self.prompt.get("1.0", "end-1c")))
         b.grid(row=14, column=0)
         b = tk.Button(self.container, text="Go back", command=lambda: self.homepage())
         b.grid(row=14, column=1)
 
     def parse_chatgpt_config(self):
         config = configparser.ConfigParser()
-        config.read(filedialog.askopenfilename())
+        file_path = filedialog.askopenfilename()
+        if not file_path:
+            return
+        config.read(file_path)
         self.deploy_agent("ChatGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"])
 
     def template_chatgpt_config(self):
+        file_path = filedialog.asksaveasfilename()
+        if not file_path:
+            return
         config = configparser.ConfigParser()
         config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": CHATGPT_PROMPT}
         config["USER"] = {"openai_key": ""}
-        with open(filedialog.asksaveasfilename(), "w") as f:
+        with open(file_path, "w") as f:
             config.write(f)
 
     def config_docgpt(self):
         self.container.pack_forget()
         self.container = tk.Frame(self.root)
         self.container.pack()
         l = tk.Label(self.container, text="DocGPT")
@@ -140,29 +146,35 @@
         self.temperature = tk.DoubleVar(self.container, value=0.5)
         e = tk.Entry(self.container, textvariable=self.temperature)
         e.grid(row=17, column=0, columnspan=2)
         l = tk.Label(self.container, text="OpenAI API key:")
         l.grid(row=18, column=0, columnspan=2)
         e = tk.Entry(self.container)
         e.grid(row=19, column=0, columnspan=2)
-        b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("DocGPT", e.get(), self.model.get(), self.prompt.get("1.0", "end-1c"), self.temperature.get()))
+        b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("DocGPT", e.get(), self.model.get(), self.prompt.get("1.0", "end-1c"), self.temperature.get(), 1000, 50))
         b.grid(row=20, column=0)
         b = tk.Button(self.container, text="Go back", command=lambda: self.homepage())
         b.grid(row=20, column=1)
 
     def parse_docgpt_config(self):
         config = configparser.ConfigParser()
-        config.read(filedialog.askopenfilename())
-        self.deploy_agent("DocGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"])
+        file_path = filedialog.askopenfilename()
+        if not file_path:
+            return
+        config.read(file_path)
+        self.deploy_agent("DocGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"], config["DEFAULT"]["chunk_size"], config["DEFAULT"]["chunk_overlap"])
 
     def template_docgpt_config(self):
+        file_path = filedialog.asksaveasfilename()
+        if not file_path:
+            return
         config = configparser.ConfigParser()
-        config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": DOCGPT_PROMPT}
+        config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": DOCGPT_PROMPT, "chunk_size": 1000, "chunk_overlap": 50}
         config["USER"] = {"openai_key": ""}
-        with open(filedialog.asksaveasfilename(), "w") as f:
+        with open(file_path, "w") as f:
             config.write(f)
 
     def deploy_agent(self, agent, *args, **kwargs):
         if agent == "ChatGPT":
             from .chatgpt import ChatGPT
             chatgpt = ChatGPT(self, *args, **kwargs)
             chatgpt.run()
```

### Comparing `kanu-0.5.0/kanu/chatgpt.py` & `kanu-0.6.0/kanu/chatgpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 import tkinter as tk
 
 import openai
 
+from .utils import Settings
+
 class ChatGPT:
     def __init__(self, kanu, openai_key, model, temperature, prompt):
         self.kanu = kanu
         self.model = model
         self.temperature = temperature
         self.prompt = prompt
         openai.api_key = openai_key
+        self.settings = Settings(self)
 
     def run(self):
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
         l = tk.Label(self.kanu.container, text="ChatGPT")
-        l.grid(row=0, column=0, columnspan=3)
+        l.grid(row=0, column=0, columnspan=4)
         self.session = tk.Text(self.kanu.container, width=70, height=20)
-        self.session.grid(row=1, column=0, columnspan=3)
-        e = tk.Entry(self.kanu.container, width=54)
-        e.grid(row=2, column=0, columnspan=3)
+        self.session.grid(row=1, column=0, columnspan=4)
+        self.session.tag_config("user", **self.settings.get_user_kwargs())
+        self.session.tag_config("bot", **self.settings.get_bot_kwargs())
+        user_input = tk.Entry(self.kanu.container, width=54)
+        user_input.grid(row=2, column=0, columnspan=4)
         self.messages = []
-        b = tk.Button(self.kanu.container, text="Send", command=lambda: self.send_message(e))
+        b = tk.Button(self.kanu.container, text="Send", command=lambda: self.send_message(user_input))
         b.grid(row=3, column=0)
         b = tk.Button(self.kanu.container, text="Clear", command=lambda: self.clear_session())
         b.grid(row=3, column=1)
         b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.kanu.config_chatgpt())
         b.grid(row=3, column=2)
+        b = tk.Button(self.kanu.container, text="Settings", command=lambda: self.settings.page())
+        b.grid(row=3, column=3)
 
     def send_message(self, entry):
         if not self.messages:
             self.messages.append({"role": "system", "content": self.prompt})
         self.messages += [{"role": "user", "content": entry.get()}]
         bot_response = openai.ChatCompletion.create(
             model=self.model,
             messages=self.messages,
             temperature=self.temperature,
         )
         response = bot_response["choices"][0]["message"]["content"]
         self.messages += [{"role": "assistant", "content": response}]
-        self.session.insert(tk.END, "You: " + entry.get() + "\n")
-        self.session.insert(tk.END, f"Bot: " + response + "\n")
+        self.session.insert(tk.END, "You: " + entry.get() + "\n", "user")
+        self.session.insert(tk.END, f"Bot: " + response + "\n", "bot")
         entry.delete(0, tk.END)
 
     def clear_session(self):
         self.session.delete(1.0, tk.END)
         self.messages.clear()
```

### Comparing `kanu-0.5.0/kanu/docgpt.py` & `kanu-0.6.0/kanu/docgpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,33 +9,38 @@
 from langchain.chains import ConversationalRetrievalChain
 from langchain.prompts import PromptTemplate
 from langchain.memory import ConversationBufferMemory
 
 from langchain.document_loaders import (
     TextLoader,
     PDFMinerLoader,
-    UnstructuredWordDocumentLoader
+    UnstructuredWordDocumentLoader,
+    CSVLoader,
 )
 
-from .utils import Tooltip
+from .utils import Tooltip, Settings
 
 DOCUMENT_LOADERS = {
     ".txt": (TextLoader, {"encoding": "utf8"}),
     ".pdf": (PDFMinerLoader, {}),
     ".doc": (UnstructuredWordDocumentLoader, {}),
     ".docx": (UnstructuredWordDocumentLoader, {}),
+    ".csv": (CSVLoader, {}),
 }
 
 class DocGPT:
-    def __init__(self, kanu, openai_key, model, temperature, prompt):
+    def __init__(self, kanu, openai_key, model, temperature, prompt, default_chunk_size, default_chunk_overlap):
         self.kanu = kanu
         self.model = model
         self.temperature = temperature
         self.prompt = prompt
+        self.default_chunk_size = default_chunk_size
+        self.default_chunk_overlap = default_chunk_overlap
         os.environ["OPENAI_API_KEY"] = openai_key
+        self.settings = Settings(self)
 
     def run(self):
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
         l = tk.Label(self.kanu.container, text="DocGPT")
         l.grid(row=0, column=0, columnspan=3)
@@ -58,21 +63,21 @@
         self.new_database_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
         self.new_database_label.grid(row=4, column=1)
         b = tk.Button(self.kanu.container, text="Browse", command=self.specify_new_database_directory)
         b.grid(row=4, column=2)
         l = tk.Label(self.kanu.container, text="Chunk size ⓘ:")
         Tooltip(l, "The maximum number of characters in each chunk.")
         l.grid(row=5, column=0)
-        self.chunk_size = tk.IntVar(self.kanu.container, value=1000)
+        self.chunk_size = tk.IntVar(self.kanu.container, value=self.default_chunk_size)
         e = tk.Entry(self.kanu.container, textvariable=self.chunk_size)
         e.grid(row=5, column=1, columnspan=2)
         l = tk.Label(self.kanu.container, text="Chunk overlap ⓘ:")
         Tooltip(l, "The number of overlapping characters between adjacent chunks.")
         l.grid(row=6, column=0)
-        self.chunk_overlap = tk.IntVar(self.kanu.container, value=50)
+        self.chunk_overlap = tk.IntVar(self.kanu.container, value=self.default_chunk_overlap)
         e = tk.Entry(self.kanu.container, textvariable=self.chunk_overlap)
         e.grid(row=6, column=1, columnspan=2)
         self.option1_button = tk.Button(self.kanu.container, text="Go with Option 1", command=self.go_with_option1)
         self.option1_button.grid(row=7, column=0, columnspan=3)
         self.option1_button["state"] = tk.DISABLED
         m = tk.Message(self.kanu.container, width=300, text="Option 2. Use an existing database")
         m.grid(row=8, column=0, columnspan=3)
@@ -97,48 +102,52 @@
             chain_type="stuff",
             combine_docs_chain_kwargs={"prompt": PromptTemplate(template=self.prompt, input_variables=["context", "question"])}
         )
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
         l = tk.Label(self.kanu.container, text="DocGPT")
-        l.grid(row=0, column=0, columnspan=3)    
+        l.grid(row=0, column=0, columnspan=4)    
         self.session = tk.Text(self.kanu.container, width=70, height=20)
-        self.session.grid(row=1, column=0, columnspan=3)
-        e = tk.Entry(self.kanu.container, width=54)
-        e.grid(row=2, column=0, columnspan=3)
-        b = tk.Button(self.kanu.container, text="Send", command=lambda: self.send_message(e))
+        self.session.grid(row=1, column=0, columnspan=4)
+        self.session.tag_config("user", **self.settings.get_user_kwargs())
+        self.session.tag_config("bot", **self.settings.get_bot_kwargs())
+        user_input = tk.Entry(self.kanu.container, width=54)
+        user_input.grid(row=2, column=0, columnspan=4)
+        b = tk.Button(self.kanu.container, text="Send", command=lambda: self.send_message(user_input))
         b.grid(row=3, column=0)
         b = tk.Button(self.kanu.container, text="Clear", command=lambda: self.clear_session())
         b.grid(row=3, column=1)
         b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.run())
         b.grid(row=3, column=2)
+        b = tk.Button(self.kanu.container, text="Settings", command=lambda: self.settings.page())
+        b.grid(row=3, column=3)
 
     def send_message(self, entry):
-        self.session.insert(tk.END, "You: " + entry.get() + "\n")
+        self.session.insert(tk.END, "You: " + entry.get() + "\n", "user")
         response = self.qa(entry.get())["answer"]
-        self.session.insert(tk.END, "Bot: " + response + "\n")
+        self.session.insert(tk.END, "Bot: " + response + "\n", "bot")
         entry.delete(0, tk.END)
 
     def go_with_option1(self):
         documents = []
         for root, dirs, files in os.walk(self.document_directory):
             for file in files:
                 file_path = os.path.join(root, file)
                 file_ext = os.path.splitext(file_path)[1]
                 if file_ext not in DOCUMENT_LOADERS:
                     continue
                 loader_class, loader_kwargs = DOCUMENT_LOADERS[file_ext]
                 loader = loader_class(file_path, **loader_kwargs)
-                document = loader.load()[0]
-                documents.append(document)
+                document = loader.load()
+                documents.extend(document)
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=self.chunk_size.get(), chunk_overlap=self.chunk_overlap.get())
         texts = text_splitter.split_documents(documents)
         db = Chroma.from_documents(texts, OpenAIEmbeddings(), persist_directory=self.database_directory)
-        db.add_documents(texts)    
+        db.add_documents(texts)
         db.persist()
         db = None
         self.query()
 
     def go_with_option2(self):
         self.query()
```

### Comparing `kanu-0.5.0/setup.py` & `kanu-0.6.0/setup.py`

 * *Files identical despite different names*

