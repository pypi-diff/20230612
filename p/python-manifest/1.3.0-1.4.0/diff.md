# Comparing `tmp/python_manifest-1.3.0-py3-none-any.whl.zip` & `tmp/python_manifest-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 19789 bytes, number of entries: 22
+Zip file size: 19891 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 manifest/__init__.py
--rw-r--r--  2.0 unx     9693 b- defN 80-Jan-01 00:00 manifest/base.py
+-rw-r--r--  2.0 unx    10808 b- defN 80-Jan-01 00:00 manifest/base.py
 -rw-r--r--  2.0 unx      460 b- defN 80-Jan-01 00:00 manifest/hooks/__init__.py
 -rw-r--r--  2.0 unx      549 b- defN 80-Jan-01 00:00 manifest/hooks/builtin.py
 -rw-r--r--  2.0 unx      382 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/__init__.py
 -rw-r--r--  2.0 unx     4581 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/operations.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/resolve.py
 -rw-r--r--  2.0 unx     2128 b- defN 80-Jan-01 00:00 manifest/hooks/interface.py
 -rw-r--r--  2.0 unx     2085 b- defN 80-Jan-01 00:00 manifest/instantiable.py
--rw-r--r--  2.0 unx    11827 b- defN 80-Jan-01 00:00 manifest/parse.py
+-rw-r--r--  2.0 unx    12035 b- defN 80-Jan-01 00:00 manifest/parse.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 manifest/py.typed
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 manifest/serializers/__init__.py
 -rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 manifest/serializers/base.py
 -rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 manifest/serializers/jsons.py
 -rw-r--r--  2.0 unx      353 b- defN 80-Jan-01 00:00 manifest/serializers/noop.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 manifest/serializers/tomls.py
 -rw-r--r--  2.0 unx      350 b- defN 80-Jan-01 00:00 manifest/serializers/yamls.py
 -rw-r--r--  2.0 unx     7718 b- defN 80-Jan-01 00:00 manifest/utils.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5565 b- defN 80-Jan-01 00:00 python_manifest-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1819 b- defN 16-Jan-01 00:00 python_manifest-1.3.0.dist-info/RECORD
-22 files, 53661 bytes uncompressed, 16829 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5565 b- defN 80-Jan-01 00:00 python_manifest-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.4.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1820 b- defN 16-Jan-01 00:00 python_manifest-1.4.0.dist-info/RECORD
+22 files, 54985 bytes uncompressed, 16931 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: manifest/serializers/yamls.py
 Comment: 
 
 Filename: manifest/utils.py
 Comment: 
 
-Filename: python_manifest-1.3.0.dist-info/LICENSE
+Filename: python_manifest-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: python_manifest-1.3.0.dist-info/METADATA
+Filename: python_manifest-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: python_manifest-1.3.0.dist-info/WHEEL
+Filename: python_manifest-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: python_manifest-1.3.0.dist-info/RECORD
+Filename: python_manifest-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## manifest/base.py

```diff
@@ -157,14 +157,44 @@
             post_process_hooks=post_process_hooks,
             **filesystem_options
         )
 
         return cls(**{**parsed_files, **kwargs})
 
     @classmethod
+    async def from_file(
+        cls: Type[T],
+        file_path: str | Path,
+        pre_process_hooks: list[Callable] = [],
+        post_process_hooks: list[Callable] = [],
+        filesystem_options: dict = {},
+        **kwargs
+    ) -> T:
+        """
+        Build the Manifest from a file.
+
+        :param file_path: The path to the file to parse
+        :type file_path: str
+        :param pre_process_hooks: A list of pre-process hooks to run before deserialization
+        :type pre_process_hooks: list[Callable]
+        :param post_process_hooks: A list of post-process hooks to run after deserialization
+        :type post_process_hooks: list[Callable]
+        :param kwargs: Additional keyword arguments to pass to the model
+        :type kwargs: dict[str, Any]
+        :return: The built Manifest
+        """
+        return await cls.from_files(
+            files=[file_path],
+            pre_process_hooks=pre_process_hooks,
+            post_process_hooks=post_process_hooks,
+            filesystem_options=filesystem_options,
+            **kwargs
+        )
+
+    @classmethod
     async def from_env(
         cls: Type[T],
         dotenv_files: list[str] = [],
         env_prefix: str = "CONFIG",
         env_delimiter: str = "__",
         **kwargs
     ) -> T:
@@ -266,27 +296,28 @@
         )
 
     async def to_file(
         self,
         file_path: str | Path,
         pre_process_hooks: list[Callable] = [],
         post_process_hooks: list[Callable] = [],
-        filesystem_options: dict = {}
+        filesystem_options: dict = {},
+        **kwargs
     ) -> int:
         """
         Save the Manifest to a file.
 
         :param file_path: The path to the file to save to
         :type file_path: str
         :param pre_process_hooks: A list of pre-process hooks to run before serialization
         :type pre_process_hooks: list[Callable]
         :param post_process_hooks: A list of post-process hooks to run after serialization
         :type post_process_hooks: list[Callable]
         :return: The number of bytes written to the file
         """
         return await dump_to_file(
             file=file_path,
-            data=self.normalize(),
+            data=self.normalize(**kwargs),
             pre_process_hooks=pre_process_hooks,
             post_process_hooks=post_process_hooks,
             **filesystem_options
         )
```

## manifest/parse.py

```diff
@@ -130,39 +130,42 @@
         with fsspec_open(file, "wb", **kwargs) as f:
             return f.write(content)
     return await run_in_thread(_)
 
 
 async def dump_to_file(
     file: str | Path,
-    data: dict,
+    data: Any,
     pre_process_hooks: list[Callable] = [],
     post_process_hooks: list[Callable] = [],
     default_serializer: Any = Undefined,
+    root_alias: str = "__root__",
     **kwargs
 ) -> int:
     """
     Persist data to a file by serializing it, writing it to the file, and returning the number
     of bytes written.
 
     :param file: The path to the file to be written to.
     :type file: str
     :param data: The data to be persisted to the file.
-    :type data: dict
+    :type data: Any
     :param serializer: The serializer to be used to serialize the data.
     :type serializer: Serializer
     :param pre_process_hooks: A list of hooks to be called before serializing the data.
     :type pre_process_hooks: list[Callable]
     :param post_process_hooks: A list of hooks to be called after serializing the data.
     :type post_process_hooks: list[Callable]
     :return: The number of bytes written to the file.
     :rtype: int
     """
     string_path = str(file)
-    assert isinstance(data, dict), "`data` must be a dictionary"
+
+    if isinstance(data, dict) and root_alias in data:
+        data = data[root_alias]
 
     # Get the serializer for the file type
     serializer = get_serializer_from_type(
         _type=determine_file_type(
             get_filename_suffix(string_path)
         ),
         _default=default_serializer
@@ -195,16 +198,17 @@
 
 
 async def load_from_file(
     file: str | Path,
     pre_process_hooks: list[Callable] = [],
     post_process_hooks: list[Callable] = [],
     default_serializer: Any = Undefined,
+    root_alias: str = "__root__",
     **kwargs
-) -> dict:
+) -> Any:
     """
     Parse a file by loading it, deserializing it, and returning the resulting dictionary.
 
     :param file: The path to the file to be parsed.
     :type file: str
     :param pre_process_hooks: A list of hooks to be called before deserializing the file.
     :type pre_process_hooks: list[Callable]
@@ -242,20 +246,24 @@
 
     try:
         # Pre-process the file contents
         for pre_hook in pre_process_hooks:
             raw_data = await execute_hook(pre_hook, raw_data)
 
         # Deserialize the file contents
-        data: dict = serializer.loads(raw_data)
+        data = serializer.loads(raw_data)
 
         # Handle empty files
         if not data:
             data = {}
 
+        # Handle files with different root types
+        if not isinstance(data, dict):
+            data = {root_alias: data}
+
         # Post-process the file contents
         for post_hook in post_process_hooks:
             data = await execute_hook(post_hook, data)
     finally:
         # Reset the current file context variable
         current_file.reset(token)
```

## Comparing `python_manifest-1.3.0.dist-info/LICENSE` & `python_manifest-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_manifest-1.3.0.dist-info/METADATA` & `python_manifest-1.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-manifest
-Version: 1.3.0
+Version: 1.4.0
 Summary: A modern toolkit for working with application manifests and configurations.
 Home-page: https://github.com/emergentmethods/python-manifest
 License: MIT
 Author: Timothy Pogue
 Author-email: tim@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `python_manifest-1.3.0.dist-info/RECORD` & `python_manifest-1.4.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 manifest/__init__.py,sha256=lPR8D6XQ8nBPlRQEKelo78kQ0gMKANeprcMEZKRevwo,230
-manifest/base.py,sha256=e2S0xQtEWXO49_LJOpvUVVGBalxtHAAvKbzgD7_qKd8,9693
+manifest/base.py,sha256=TuG5sE6PS-qo4XoP9fVBdmcQo_x90Z2pw79qv_yLN6M,10808
 manifest/hooks/__init__.py,sha256=xGWUkgzWM7Dp_cMDvqk8bRzi9fiX8GYBzOcVmtWJwuo,460
 manifest/hooks/builtin.py,sha256=EqeD6B9BnA21MdVZiZ54Gz1w7hNnjMBkc64PIzKC-Zw,549
 manifest/hooks/expressions/__init__.py,sha256=hvVL1tr9aCSH7EFeph99CJvKWCP_V4m5KStZx9Hmsqw,382
 manifest/hooks/expressions/operations.py,sha256=PoVZ69D7MTrl5iWze34Gl10WA6sdH7l505T1jKQNiUU,4581
 manifest/hooks/expressions/resolve.py,sha256=VF0l2MTeGGVqCCjQEeFj0Dxqlbz4Hq_jX022Dr0gIu8,3238
 manifest/hooks/interface.py,sha256=xKE-3E3yUV4FuLJWPiMR5UCe6pa-cwSIoP4zK0zxzuM,2128
 manifest/instantiable.py,sha256=TlzW04amYQF26X_iqJU2MMsvplCMogUM6XTwljdwFcc,2085
-manifest/parse.py,sha256=ZV-fFct6ci2s-C65hbuTQMTNnXExgBtc_fWxSfntL2M,11827
+manifest/parse.py,sha256=aBjUcUThYdLazCJFOGpgSZRC6mQVLIIyzAx5tUzQ4Uk,12035
 manifest/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 manifest/serializers/__init__.py,sha256=4d2mNeR4nZTdHC7Dg5ab7_whcXF_BsXvrhm8whJMeas,386
 manifest/serializers/base.py,sha256=So6sMP502D0fXN84Np0a_c5IGyq4gLWmMXfDwN6xAPg,272
 manifest/serializers/jsons.py,sha256=iK5Tswidrc3CLqeg4YaBNH7Ev6C7cVAQo6pEmDjncIM,503
 manifest/serializers/noop.py,sha256=x0sqDyLDFI-g6K5EnXUex3UVmwLvq-nMFoBj_iNpTys,353
 manifest/serializers/tomls.py,sha256=QxSGa4nWs3SqJAF-Y_64zGfEn_BgPOVs5-bxvS7X6Ro,356
 manifest/serializers/yamls.py,sha256=th77AOLV4I10t_SOLIlqQAsiSGzACzia71vGIi-1Cf0,350
 manifest/utils.py,sha256=bs7Pan15CW8sNldVq0-xuVzYL24vjxpVlzstyHDsH-M,7718
-python_manifest-1.3.0.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
-python_manifest-1.3.0.dist-info/METADATA,sha256=3fztSnjyCSnIXq7wDc23-TbNagkMqMS9zPp1IPCrvr0,5565
-python_manifest-1.3.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-python_manifest-1.3.0.dist-info/RECORD,,
+python_manifest-1.4.0.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
+python_manifest-1.4.0.dist-info/METADATA,sha256=QVTlEkZOmVYghYK8gnR6dYoaQ6zZENV7r-kJyUtxQJw,5565
+python_manifest-1.4.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+python_manifest-1.4.0.dist-info/RECORD,,
```

