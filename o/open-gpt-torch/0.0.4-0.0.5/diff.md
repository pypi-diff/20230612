# Comparing `tmp/open_gpt_torch-0.0.4.tar.gz` & `tmp/open_gpt_torch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.4.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.5.tar", max compression
```

## Comparing `open_gpt_torch-0.0.4.tar` & `open_gpt_torch-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0    10825 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/LICENSE
--rw-r--r--   0        0        0     7611 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/README.md
--rw-r--r--   0        0        0      929 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/__main__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0      953 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/cli/commands/playground.py
--rw-r--r--   0        0        0     2031 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     4378 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/factory.py
--rw-r--r--   0        0        0     2523 2023-06-05 11:05:16.676548 open_gpt_torch-0.0.4/open_gpt/helper.py
--rw-r--r--   0        0        0      490 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/logs.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     6038 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     9040 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0        0        0     5647 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     2511 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0     3657 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/generation.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     2143 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0      749 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/llama/modeling.py
--rw-r--r--   0        0        0     2094 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/loading.py
--rw-r--r--   0        0        0     1833 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0     3504 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0      653 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/rwkv/__init__.py
--rw-r--r--   0        0        0      659 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/rwkv/modeling.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0     2608 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0        0        0     3236 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/vicuna/loading.py
--rw-r--r--   0        0        0     1488 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0        0        0     3527 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1775 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0     2373 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0        0        0      171 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/executors/utils.py
--rw-r--r--   0        0        0     3429 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0        0 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/playground/__init__.py
--rw-r--r--   0        0        0     4686 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/playground/gradio.py
--rw-r--r--   0        0        0     7396 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/playground/gradio_chatbot.py
--rw-r--r--   0        0        0     2714 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/open_gpt/serve/playground/gradio_css.py
--rw-r--r--   0        0        0     3073 2023-06-05 11:05:16.680548 open_gpt_torch-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    20671 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-06-12 10:13:36.643150 open_gpt_torch-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7611 2023-06-12 10:13:36.643150 open_gpt_torch-0.0.5/README.md
+-rw-r--r--   0        0        0      929 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0      953 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/commands/playground.py
+-rw-r--r--   0        0        0     2223 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     5326 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/factory.py
+-rw-r--r--   0        0        0     2523 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/helper.py
+-rw-r--r--   0        0        0      490 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/logs.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0     2420 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/embedding.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     6038 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     9040 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0        0        0     5647 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     2545 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0    11346 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/generation.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     2877 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0      943 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/llama/modeling.py
+-rw-r--r--   0        0        0     2856 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     2564 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0     3504 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0      653 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/rwkv/__init__.py
+-rw-r--r--   0        0        0      659 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/rwkv/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     2608 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0        0        0     7439 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0        0        0     1521 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0        0        0     3507 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1977 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0     2373 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0        0        0      171 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/executors/utils.py
+-rw-r--r--   0        0        0     3429 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/playground/__init__.py
+-rw-r--r--   0        0        0     4686 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio.py
+-rw-r--r--   0        0        0     7396 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio_chatbot.py
+-rw-r--r--   0        0        0     2714 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio_css.py
+-rw-r--r--   0        0        0     3094 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    20700 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.5/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.4/LICENSE` & `open_gpt_torch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/README.md` & `open_gpt_torch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/__init__.py` & `open_gpt_torch-0.0.5/open_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/cli/application.py` & `open_gpt_torch-0.0.5/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.5/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/cli/commands/playground.py` & `open_gpt_torch-0.0.5/open_gpt/cli/commands/playground.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/cli/commands/serve.py` & `open_gpt_torch-0.0.5/open_gpt/cli/commands/serve.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,17 @@
             default=51002,
         ),
         option('enable_cors', None, 'Enable CORS.', flag=True),
         option(
             'precision', None, 'The precision of the model.', flag=False, default='fp16'
         ),
         option(
+            'adapter_name_or_path', None, 'The name or path of the adapter checkpoint.'
+        ),
+        option(
             'device_map',
             None,
             'The device map of the model.',
             flag=False,
             default='balanced',
         ),
         option(
@@ -52,14 +55,15 @@
         with create_flow(
             self.argument('model_name'),
             grpc_port=self.option('grpc_port'),
             http_port=self.option('http_port'),
             cors=self.option('enable_cors'),
             uses_with={
                 'precision': self.option('precision'),
+                'adapter_name_or_path': self.option('adapter_name_or_path'),
                 'device_map': self.option('device_map'),
             },
             replicas=self.option('replicas'),
         ) as flow:
             self.line(
                 f'<info>The model is ready to be used at port {self.option("grpc_port")} (gRPC) and {self.option("http_port")} (HTTP).</info>'
             )
```

### Comparing `open_gpt_torch-0.0.4/open_gpt/helper.py` & `open_gpt_torch-0.0.5/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.5/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/flamingo/flamingo_model.py` & `open_gpt_torch-0.0.5/open_gpt/models/flamingo/flamingo_model.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.5/open_gpt/models/flamingo/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.5/open_gpt/models/flamingo/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,18 @@
     no_split_module_classes = ["LlamaDecoderLayer"]
     image_processor = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def load_model_and_transforms(
-        self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
+        self,
+        model_name_or_path: str,
+        tokenizer_name_or_path: Optional[str] = None,
+        **kwargs
     ):
         from .loading import load_model_and_transforms
 
         self.model, self.tokenizer, self.image_processor = load_model_and_transforms(
             model_name_or_path,
             vision_model_name_or_path='ViT-L-14::openai',
             lang_model_name_or_path='facebook/llama-7b',
```

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/llama/loading.py` & `open_gpt_torch-0.0.5/open_gpt/models/llama/loading.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 def load_model_and_tokenizer(
     model_name_or_path: str,
     tokenizer_name_or_path: Optional[str] = None,
     device: Optional[torch.device] = None,
     precision: Optional[str] = None,
     dtype: Optional[torch.dtype] = None,
     device_map: Optional[Union[str, List[int]]] = None,
-    no_split_module_classes: Optional[List[str]] = None,
     **kwargs,
 ):
-    """Load a model and tokenizer from HuggingFace."""
+    """Load model and tokenizer from HuggingFace / local.
+
+    :param model_name_or_path: The model id or path to load the model from.
+    :param tokenizer_name_or_path: The tokenizer id or path to load the tokenizer from.
+    """
+
     from transformers import AutoModelForCausalLM
     from transformers.models.llama.tokenization_llama import LlamaTokenizer
 
     tokenizer = LlamaTokenizer.from_pretrained(
         model_name_or_path or tokenizer_name_or_path
     )
 
@@ -39,16 +43,28 @@
 
         quantization_config = BitsAndBytesConfig(
             load_in_8bit=True,
             llm_int8_enable_fp32_cpu_offload=True,
             llm_int8_skip_modules=["lm_head", "LlamaDecoderLayer"],
         )
     elif precision == 'bit4':
+        from packaging import version
         from transformers import BitsAndBytesConfig
 
+        from open_gpt import importlib_metadata
+
+        trf_version = importlib_metadata.version("transformers")
+        if 'dev' in trf_version:
+            trf_version = '.'.join(trf_version.split('.')[:-1])
+        supports_kbit = version.parse(trf_version) >= version.parse("4.30.0")
+        assert supports_kbit, (
+            f"Vicuna model k-bit quantization requires transformers >= v4.30.0, you have transformers=={trf_version}.\n"
+            f"You can install the latest transformers with `pip install git+https://github.com/huggingface/transformers`."
+        )
+
         quantization_config = BitsAndBytesConfig(
             load_in_4bit=True,
             bnb_4bit_compute_dtype=torch.bfloat16,
             bnb_4bit_use_double_quant=True,
             bnb_4bit_quant_type='nf4',
         )
```

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/llama/modeling.py` & `open_gpt_torch-0.0.5/open_gpt/models/llama/modeling.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,21 +8,28 @@
 class LlamaModel(BaseModel):
     no_split_module_classes = ["LlamaDecoderLayer"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def load_model_and_transforms(
-        self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
+        self,
+        model_name_or_path: str,
+        adapter_name_or_path: Optional[str] = None,
+        tokenizer_name_or_path: Optional[str] = None,
     ):
 
         from .loading import load_model_and_tokenizer
 
         self.model, self.tokenizer = load_model_and_tokenizer(
             model_name_or_path,
             tokenizer_name_or_path=tokenizer_name_or_path,
             dtype=self._dtype,
+            precision=self._precision,
             device=self._device,
             device_map=self._device_map,
         )
 
+        if adapter_name_or_path:
+            self.load_adapter(adapter_name_or_path)
+
         self.model.eval()
```

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/modeling.py` & `open_gpt_torch-0.0.5/open_gpt/models/modeling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,87 @@
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import torch
 from torch import nn
 
 from ..helper import auto_dtype_and_device
+from .embedding import EmbeddingMixin
 from .generation import GenerationMixin
 
 if TYPE_CHECKING:
     from transformers import AutoModelForCausalLM, AutoTokenizer
 
 
-class BaseModel(nn.Module, GenerationMixin):
+class BaseModel(nn.Module, GenerationMixin, EmbeddingMixin):
     model: 'AutoModelForCausalLM'
     tokenizer: 'AutoTokenizer'
 
     def __init__(
         self,
         model_name_or_path: str,
+        adapter_name_or_path: Optional[str] = None,
         tokenizer_name_or_path: Optional[str] = None,
         precision: str = 'fp16',
         device: Optional[torch.device] = None,
         device_map: Optional[Union[str, List[int]]] = None,
         eval_mode: bool = True,
         **kwargs,
     ):
         """Create a model of the given name."""
 
         super().__init__()
 
         self._model_name_or_path = model_name_or_path
+        self._adapter_name_or_path = adapter_name_or_path
 
         self._precision = precision
         self._dtype, self._device = auto_dtype_and_device(precision, device)
 
         self._device_map = device_map
 
         self._eval_mode = eval_mode
 
         self.load_model_and_transforms(
-            model_name_or_path, tokenizer_name_or_path=tokenizer_name_or_path
+            model_name_or_path,
+            adapter_name_or_path=adapter_name_or_path,
+            tokenizer_name_or_path=tokenizer_name_or_path,
         )
 
         self.post_init(**kwargs)
 
     def load_model_and_transforms(
-        self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
+        self,
+        model_name_or_path: str,
+        adapter_name_or_path: Optional[str] = None,
+        tokenizer_name_or_path: Optional[str] = None,
     ):
         from .loading import load_model_and_tokenizer
 
         self.model, self.tokenizer = load_model_and_tokenizer(
             model_name_or_path,
             tokenizer_name_or_path=tokenizer_name_or_path,
             precision=self._precision,
             dtype=self._dtype,
             device=self._device,
             device_map=self._device_map,
         )
 
+        if adapter_name_or_path is not None:
+            self.load_adapter(adapter_name_or_path)
+
         # turn the eval mode off `eval_mode=False` in training
         if self._eval_mode:
             self.model.eval()
 
     def post_init(self, **kwargs):
         pass
+
+    def load_adapter(self, adapter_name_or_path: str):
+        from peft import PeftModel
+
+        self.model = PeftModel.from_pretrained(
+            self.model,
+            adapter_name_or_path,
+            device_map={'': self._device or 0}
+            if (self._device_map is None)
+            else self._device_map,
+        )
```

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/moss/modeling.py` & `open_gpt_torch-0.0.5/open_gpt/models/moss/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/pythia/modeling.py` & `open_gpt_torch-0.0.5/open_gpt/models/pythia/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/rwkv/modeling.py` & `open_gpt_torch-0.0.5/open_gpt/models/rwkv/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/stablelm/modeling.py` & `open_gpt_torch-0.0.5/open_gpt/models/stablelm/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/models/vicuna/modeling.py` & `open_gpt_torch-0.0.5/open_gpt/models/vicuna/modeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,19 +27,21 @@
     ```python
     import open_gpt
 
     model = open_gpt.create_model(
         'lmsys/vicuna-7b-delta-v1.1', precision='fp16', device_map='balanced'
     )
     ```
-
     """
 
     def load_model_and_transforms(
-        self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
+        self,
+        model_name_or_path: str,
+        tokenizer_name_or_path: Optional[str] = None,
+        **kwargs
     ):
         from .loading import load_model_and_tokenizer
 
         self.model, self.tokenizer = load_model_and_tokenizer(
             model_name_or_path,
             tokenizer_name_or_path=tokenizer_name_or_path,
             dtype=self._dtype,
```

### Comparing `open_gpt_torch-0.0.4/open_gpt/profile.py` & `open_gpt_torch-0.0.5/open_gpt/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,16 @@
     # Time
     measures = {"time": time.time() - start_measures["time"]}
 
     gc.collect()
     torch.cuda.empty_cache()
 
     # CPU mem
-    measures["cpu"] = (
-        psutil.Process().memory_info().rss - start_measures["cpu"]
-    ) / 2**20
-    measures["cpu-peak"] = (cpu_peak_tracker.stop() - start_measures["cpu"]) / 2**20
+    measures["cpu"] = (psutil.Process().memory_info().rss - start_measures["cpu"]) / GB
+    measures["cpu-peak"] = (cpu_peak_tracker.stop() - start_measures["cpu"]) / GB
 
     # GPU mem
     for i in range(torch.cuda.device_count()):
         measures[str(i)] = (
             torch.cuda.memory_allocated(i) - start_measures[str(i)]
         ) / GB
         measures[f"{i}-peak"] = (
```

### Comparing `open_gpt_torch-0.0.4/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.5/open_gpt/serve/executors/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,31 +12,37 @@
 
 
 class CausualLMExecutor(Executor):
     def __init__(
         self,
         model_name_or_path: str = '',
         minibatch_size: int = 1,
+        adapter_name_or_path: Optional[str] = None,
         device_map: Optional[Union[str, List[int]]] = None,
         precision: Optional[str] = None,
         num_workers: int = 4,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         assert (
             model_name_or_path
         ), '`model_name_or_path` must be provided to initialize the model and tokenizer.'
 
         self._model_name_or_path = model_name_or_path
+        self._adapter_name_or_path = adapter_name_or_path
         self._minibatch_size = minibatch_size
         self._thread_pool = ThreadPool(processes=num_workers)
 
         self.model = create_model(
-            model_name_or_path, precision=precision, device_map=device_map, **kwargs
+            model_name_or_path,
+            precision=precision,
+            adapter_name_or_path=adapter_name_or_path,
+            device_map=device_map,
+            **kwargs,
         )
 
         # warmup the model to avoid the first-time slowness
         self.model.generate(['Hello world!'])
 
     @requests(on='/generate')
     def generate(self, docs: 'DocumentArray', parameters: Dict = {}, **kwargs):
```

### Comparing `open_gpt_torch-0.0.4/open_gpt/serve/executors/flamingo.py` & `open_gpt_torch-0.0.5/open_gpt/serve/executors/flamingo.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/serve/gateway.py` & `open_gpt_torch-0.0.5/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/serve/playground/gradio.py` & `open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/serve/playground/gradio_chatbot.py` & `open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio_chatbot.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/open_gpt/serve/playground/gradio_css.py` & `open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio_css.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.4/pyproject.toml` & `open_gpt_torch-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.4"
+version = "0.0.5"
 description = "An open-source cloud-native of large multi-modal models (LMMs) serving framework."
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
@@ -51,23 +51,24 @@
 inference-client = "^0.0.4"
 pydantic = "^1.10.0"
 loguru = "^0.5"
 cleo = "^2.0.0"
 click = "^8.1.3"
 numpy = "^1.21.2"
 einops = "^0.6.0"
-transformers = "^4.29.0"
-open_clip_torch = "^2.16"
-bitsandbytes = "^0.38.0"
-accelerate = "^0.18.0"
+transformers = "^4.30.1"
+open_clip_torch = ">2.16.0"
+bitsandbytes = ">=0.39.0"
+accelerate = "^0.20.3"
 tqdm = "^4.62.3"
+peft = "^0.3.0"
 
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
-open-flamingo = { version = "^0.0", optional = true }
+open-flamingo = { version = "^0.0.2", optional = true }
 gradio = { version = "^3.30.0", optional = true }
 mdtex2html = { version = "^1.2.0", optional = true }
 markdown2 = { version = "^2.4.0", optional = true }
 
 [tool.poetry.extras]
 flamingo = ["open-flamingo"]
 playground = ["gradio", "mdtex2html", "markdown2"]
```

### Comparing `open_gpt_torch-0.0.4/PKG-INFO` & `open_gpt_torch-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.4
+Version: 0.0.5
 Summary: An open-source cloud-native of large multi-modal models (LMMs) serving framework.
 Home-page: https://github.com/jina-ai/opengpt
 License: Apache-2.0
 Keywords: Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-inference,llama,vicuna,stabellm
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0
@@ -22,32 +22,33 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: flamingo
 Provides-Extra: playground
-Requires-Dist: accelerate (>=0.18.0,<0.19.0)
-Requires-Dist: bitsandbytes (>=0.38.0,<0.39.0)
+Requires-Dist: accelerate (>=0.20.3,<0.21.0)
+Requires-Dist: bitsandbytes (>=0.39.0)
 Requires-Dist: cleo (>=2.0.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docarray (>=0.21.0,<0.22.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra == "playground"
 Requires-Dist: inference-client (>=0.0.4,<0.0.5)
 Requires-Dist: jina (>=3.15.0,<4.0.0)
 Requires-Dist: loguru (>=0.5,<0.6)
 Requires-Dist: markdown2 (>=2.4.0,<3.0.0) ; extra == "playground"
 Requires-Dist: mdtex2html (>=1.2.0,<2.0.0) ; extra == "playground"
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
-Requires-Dist: open-flamingo (>=0.0,<0.1) ; extra == "flamingo"
-Requires-Dist: open_clip_torch (>=2.16,<3.0)
+Requires-Dist: open-flamingo (>=0.0.2,<0.0.3) ; extra == "flamingo"
+Requires-Dist: open_clip_torch (>2.16.0)
+Requires-Dist: peft (>=0.3.0,<0.4.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
-Requires-Dist: transformers (>=4.29.0,<5.0.0)
+Requires-Dist: transformers (>=4.30.1,<5.0.0)
 Project-URL: Repository, https://github.com/jina-ai/opengpt
 Description-Content-Type: text/markdown
 
 # ☄️ OpenGPT
 
 <p align="center">
 <a href="https://github.com/jina-ai/opengpt"><img src="https://github.com/jina-ai/opengpt/blob/main/.github/images/logo.png?" alt="OpenGPT: An open-source cloud-native large-scale multimodal model serving framework" width="300px"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.4 Summary: An open-
+Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.5 Summary: An open-
 source cloud-native of large multi-modal models (LMMs) serving framework. Home-
 page: https://github.com/jina-ai/opengpt License: Apache-2.0 Keywords:
 Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-
 inference,llama,vicuna,stabellm Author: Jina AI Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
@@ -11,27 +11,28 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Provides-Extra: flamingo Provides-Extra: playground
-Requires-Dist: accelerate (>=0.18.0,<0.19.0) Requires-Dist: bitsandbytes
-(>=0.38.0,<0.39.0) Requires-Dist: cleo (>=2.0.0,<3.0.0) Requires-Dist: click
+Requires-Dist: accelerate (>=0.20.3,<0.21.0) Requires-Dist: bitsandbytes
+(>=0.39.0) Requires-Dist: cleo (>=2.0.0,<3.0.0) Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: docarray (>=0.21.0,<0.22.0) Requires-Dist:
 einops (>=0.6.0,<0.7.0) Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra ==
 "playground" Requires-Dist: inference-client (>=0.0.4,<0.0.5) Requires-Dist:
 jina (>=3.15.0,<4.0.0) Requires-Dist: loguru (>=0.5,<0.6) Requires-Dist:
 markdown2 (>=2.4.0,<3.0.0) ; extra == "playground" Requires-Dist: mdtex2html
 (>=1.2.0,<2.0.0) ; extra == "playground" Requires-Dist: numpy (>=1.21.2,<2.0.0)
-Requires-Dist: open-flamingo (>=0.0,<0.1) ; extra == "flamingo" Requires-Dist:
-open_clip_torch (>=2.16,<3.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0)
-Requires-Dist: tqdm (>=4.62.3,<5.0.0) Requires-Dist: transformers
-(>=4.29.0,<5.0.0) Project-URL: Repository, https://github.com/jina-ai/opengpt
-Description-Content-Type: text/markdown # âï¸ OpenGPT
+Requires-Dist: open-flamingo (>=0.0.2,<0.0.3) ; extra == "flamingo" Requires-
+Dist: open_clip_torch (>2.16.0) Requires-Dist: peft (>=0.3.0,<0.4.0) Requires-
+Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tqdm (>=4.62.3,<5.0.0)
+Requires-Dist: transformers (>=4.30.1,<5.0.0) Project-URL: Repository, https://
+github.com/jina-ai/opengpt Description-Content-Type: text/markdown # âï¸
+OpenGPT
   [OpenGPT:_An_open-source_cloud-native_large-scale_multimodal_model_serving
                                   framework]
 > "A playful and whimsical vector art of a Stochastic Tigger, wearing a t-shirt
 with a "GPT" text printed logo, surrounded by colorful geometric shapes. âar
 1:1 âupbeta" > > â Prompts and logo art was produced with [PromptPerfect]
 (https://promptperfect.jina.ai/) & [Stable Diffusion X](https://clipdrop.co/
 stable-diffusion) ![](https://img.shields.io/badge/Made%20with-JinaAI-
```

