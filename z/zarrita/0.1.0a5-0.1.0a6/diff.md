# Comparing `tmp/zarrita-0.1.0a5.tar.gz` & `tmp/zarrita-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrita-0.1.0a5.tar", max compression
+gzip compressed data, was "zarrita-0.1.0a6.tar", max compression
```

## Comparing `zarrita-0.1.0a5.tar` & `zarrita-0.1.0a6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     2311 2023-06-08 08:19:54.182773 zarrita-0.1.0a5/README.md
--rw-r--r--   0        0        0      696 2023-06-09 12:23:32.908465 zarrita-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     1085 2023-06-07 11:49:09.452172 zarrita-0.1.0a5/zarrita/__init__.py
--rw-r--r--   0        0        0    19605 2023-06-09 11:30:35.987863 zarrita-0.1.0a5/zarrita/array.py
--rw-r--r--   0        0        0    13242 2023-06-08 12:06:11.862323 zarrita-0.1.0a5/zarrita/array_v2.py
--rw-r--r--   0        0        0    12363 2023-06-09 11:37:23.257106 zarrita-0.1.0a5/zarrita/codecs.py
--rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a5/zarrita/common.py
--rw-r--r--   0        0        0     4181 2023-06-07 15:17:15.193840 zarrita-0.1.0a5/zarrita/group.py
--rw-r--r--   0        0        0     4735 2023-06-07 15:17:10.125767 zarrita-0.1.0a5/zarrita/group_v2.py
--rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a5/zarrita/indexing.py
--rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a5/zarrita/metadata.py
--rw-r--r--   0        0        0    20531 2023-06-08 12:06:20.763281 zarrita-0.1.0a5/zarrita/sharding.py
--rw-r--r--   0        0        0     5391 2023-06-07 20:04:34.652580 zarrita-0.1.0a5/zarrita/store.py
--rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a5/zarrita/sync.py
--rw-r--r--   0        0        0     3827 2023-06-06 13:35:33.794530 zarrita-0.1.0a5/zarrita/value_handle.py
--rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 zarrita-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     2311 2023-06-11 20:17:59.556412 zarrita-0.1.0a6/README.md
+-rw-r--r--   0        0        0      737 2023-06-12 12:49:19.575716 zarrita-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     1144 2023-06-11 20:17:59.559200 zarrita-0.1.0a6/zarrita/__init__.py
+-rw-r--r--   0        0        0    19654 2023-06-11 20:17:59.559624 zarrita-0.1.0a6/zarrita/array.py
+-rw-r--r--   0        0        0    13103 2023-06-11 20:17:59.559984 zarrita-0.1.0a6/zarrita/array_v2.py
+-rw-r--r--   0        0        0    12363 2023-06-09 11:37:23.257106 zarrita-0.1.0a6/zarrita/codecs.py
+-rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a6/zarrita/common.py
+-rw-r--r--   0        0        0     3830 2023-06-11 20:17:59.560239 zarrita-0.1.0a6/zarrita/group.py
+-rw-r--r--   0        0        0     4353 2023-06-11 20:17:59.560496 zarrita-0.1.0a6/zarrita/group_v2.py
+-rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a6/zarrita/indexing.py
+-rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a6/zarrita/metadata.py
+-rw-r--r--   0        0        0    20531 2023-06-08 12:06:20.763281 zarrita-0.1.0a6/zarrita/sharding.py
+-rw-r--r--   0        0        0     8466 2023-06-11 20:17:59.560828 zarrita-0.1.0a6/zarrita/store.py
+-rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a6/zarrita/sync.py
+-rw-r--r--   0        0        0     3783 2023-06-11 20:17:59.561195 zarrita-0.1.0a6/zarrita/value_handle.py
+-rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 zarrita-0.1.0a6/PKG-INFO
```

### Comparing `zarrita-0.1.0a5/LICENSE` & `zarrita-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a5/README.md` & `zarrita-0.1.0a6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,36 @@
 store = zarrita.LocalStore('testdata') # or zarrita.RemoteStore('s3://bucket/test')
 ```
 
 ## Create an array
 
 ```python
 a = await zarrita.Array.create_async(
-    store,
-    'array',
+    store / 'array',
     shape=(6, 10),
     dtype='int32',
     chunk_shape=(2, 5),
     codecs=[zarrita.codecs.blosc_codec()],
     attributes={'question': 'life', 'answer': 42}
 )
 await a.async_[:, :].set(np.ones((6, 10), dtype='int32'))
 ```
 
 ## Open an array
 
 ```python
-a = await zarrita.Array.open_async(store, 'array')
+a = await zarrita.Array.open_async(store / 'array')
 assert np.array_equal(await a.async_[:, :].get(), np.ones((6, 10), dtype='int32'))
 ```
 
 ## Create an array with sharding
 
 ```python
 a = await zarrita.Array.create_async(
-    store,
-    'sharding',
+    store / 'sharding',
     shape=(16, 16),
     dtype='int32',
     chunk_shape=(16, 16),
     chunk_key_encoding=('v2', '.'),
     codecs=[
         zarrita.codecs.sharding_codec(
             chunk_shape=(8, 8),
@@ -54,31 +52,31 @@
 await a.async_[:, :].set(data)
 assert np.array_equal(await a.async_[:, :].get(), data)
 ```
 
 ## Create a group
 
 ```python
-g = await zarrita.Group.create_async(store, 'group')
+g = await zarrita.Group.create_async(store / 'group')
 g2 = await g.create_group_async('group2')
 a = await g2.create_array_async(
     'array',
     shape=(16, 16),
     dtype='int32',
     chunk_shape=(16, 16),
 )
 await a.async_[:, :].set(np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
 ```
 
 ## Open a group
 
 ```python
-g = await zarrita.Group.open_async(store, 'group')
+g = await zarrita.Group.open_async(store / 'group')
 g2 = g['group2']
-a = g['group2/array']
+a = g['group2']['array']
 assert np.array_equal(await a.asnyc_[:, :].get(), np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
 ```
 
 # Credits
 
 This is a largely-rewritten fork of `zarrita` by [@alimanfoo](https://github.com/alimanfoo). It implements the Zarr v3 draft specification created by [@alimanfoo](https://github.com/alimanfoo), [@jstriebel](https://github.com/jstriebel), [@jbms](https://github.com/jbms) et al.
```

### Comparing `zarrita-0.1.0a5/pyproject.toml` & `zarrita-0.1.0a6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "zarrita"
-version = "0.1.0a5"
+version = "0.1.0a6"
 description = ""
 authors = ["Norman Rzepka <code@normanrz.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-fsspec = "^2022.2.0"
+python = ">=3.8,<3.12"
+fsspec = ">=2022.0.0"
 numpy = "^1.24.2"
-numcodecs = "^0.10.0"
-cattrs = "^22.2.0"
-attrs = "^22.2.0"
-crc32c = "^2.3.post0"
+numcodecs = "^0.11.0"
+cattrs = ">=22.2.0"
+attrs = ">=22.2.0"
+crc32c = ">=2.3"
 
 [tool.poetry.group.dev.dependencies]
-webknossos = "^0.12.3"
+wkw = "^1.1.22"
 pytest = "^7.2.1"
 black = "^23.1.0"
 mypy = "^1.0.1"
 isort = "^5.12.0"
 pudb = "^2022.1.3"
 zarr = "^2.14.2"
 pytest-asyncio = "^0.21.0"
 ruff = "^0.0.271"
+s3fs = ">=2022.0.0"
+universal_pathlib = "^0.0.23"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `zarrita-0.1.0a5/zarrita/__init__.py` & `zarrita-0.1.0a6/zarrita/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,31 +5,36 @@
     Array,
     ArrayRuntimeConfiguration,
     runtime_configuration,
 )
 from zarrita.array_v2 import ArrayV2  # noqa: F401
 from zarrita.group import Group  # noqa: F401
 from zarrita.group_v2 import GroupV2  # noqa: F401
-from zarrita.store import LocalStore, RemoteStore, Store  # noqa: F401
+from zarrita.store import (  # noqa: F401
+    LocalStore,
+    RemoteStore,
+    Store,
+    StoreLike,
+    StorePath,
+    make_store_path,
+)
 from zarrita.sync import sync as _sync
 
 
 async def open_auto_async(
-    store: Store,
-    path: str,
+    store: StoreLike,
     runtime_configuration_: Optional[ArrayRuntimeConfiguration] = None,
 ) -> Union[Array, ArrayV2, Group, GroupV2]:
+    store_path = make_store_path(store)
     try:
         return await Group.open_or_array(
-            store, path, runtime_configuration=runtime_configuration_
+            store_path, runtime_configuration=runtime_configuration_
         )
     except KeyError:
-        return await GroupV2.open_or_array(store, path)
-    raise KeyError
+        return await GroupV2.open_or_array(store_path)
 
 
 def open_auto(
-    store: Store,
-    path: str,
+    store: StoreLike,
     runtime_configuration_: Optional[ArrayRuntimeConfiguration] = None,
 ) -> Union[Array, ArrayV2, Group, GroupV2]:
-    return _sync(open_auto_async(store, path, runtime_configuration_))
+    return _sync(open_auto_async(store, runtime_configuration_))
```

### Comparing `zarrita-0.1.0a5/zarrita/array.py` & `zarrita-0.1.0a6/zarrita/array.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     RegularChunkGridConfigurationMetadata,
     RegularChunkGridMetadata,
     V2ChunkKeyEncodingConfigurationMetadata,
     V2ChunkKeyEncodingMetadata,
     dtype_to_data_type,
 )
 from zarrita.sharding import ShardingCodec
-from zarrita.store import Store
+from zarrita.store import StoreLike, StorePath, make_store_path
 from zarrita.sync import sync
 from zarrita.value_handle import (
     ArrayValueHandle,
     FileValueHandle,
     NoneValueHandle,
     ValueHandle,
 )
@@ -77,24 +77,22 @@
         return o.name
     raise TypeError
 
 
 @frozen
 class Array:
     metadata: ArrayMetadata
-    store: "Store"
-    path: str
+    store_path: StorePath
     runtime_configuration: ArrayRuntimeConfiguration
     codecs: List[Codec]
 
     @classmethod
     async def create_async(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         *,
         shape: ChunkCoords,
         dtype: Union[str, np.dtype],
         chunk_shape: ChunkCoords,
         fill_value: Optional[Any] = None,
         chunk_key_encoding: Union[
             Tuple[Literal["default"], Literal[".", "/"]],
@@ -102,16 +100,17 @@
         ] = ("default", "/"),
         codecs: Optional[Iterable[CodecMetadata]] = None,
         dimension_names: Optional[Iterable[str]] = None,
         attributes: Optional[Dict[str, Any]] = None,
         runtime_configuration: Optional[ArrayRuntimeConfiguration] = None,
         exists_ok: bool = False,
     ) -> "Array":
+        store_path = make_store_path(store)
         if not exists_ok:
-            assert not await store.exists_async(f"{path}/{ZARR_JSON}")
+            assert not await (store_path / ZARR_JSON).exists_async()
 
         data_type = (
             DataType[dtype]
             if isinstance(dtype, str)
             else DataType[dtype_to_data_type[dtype.str]]
         )
 
@@ -139,28 +138,26 @@
             fill_value=0 if fill_value is None else fill_value,
             codecs=list(codecs) if codecs else [],
             dimension_names=tuple(dimension_names) if dimension_names else None,
             attributes=attributes or {},
         )
         array = cls(
             metadata=metadata,
-            store=store,
-            path=path,
+            store_path=store_path,
             runtime_configuration=runtime_configuration or ArrayRuntimeConfiguration(),
             codecs=Codec.codecs_from_metadata(metadata.codecs),
         )
 
         await array._save_metadata()
         return array
 
     @classmethod
     def create(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         *,
         shape: ChunkCoords,
         dtype: Union[str, np.dtype],
         chunk_shape: ChunkCoords,
         fill_value: Optional[Any] = None,
         chunk_key_encoding: Union[
             Tuple[Literal["default"], Literal[".", "/"]],
@@ -170,16 +167,15 @@
         dimension_names: Optional[Iterable[str]] = None,
         attributes: Optional[Dict[str, Any]] = None,
         runtime_configuration: Optional[ArrayRuntimeConfiguration] = None,
         exists_ok: bool = False,
     ) -> "Array":
         return sync(
             cls.create_async(
-                store,
-                path,
+                store=store,
                 shape=shape,
                 dtype=dtype,
                 chunk_shape=chunk_shape,
                 fill_value=fill_value,
                 chunk_key_encoding=chunk_key_encoding,
                 codecs=codecs,
                 dimension_names=dimension_names,
@@ -188,89 +184,80 @@
                 exists_ok=exists_ok,
             )
         )
 
     @classmethod
     async def open_async(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         runtime_configuration: Optional[ArrayRuntimeConfiguration] = None,
     ) -> "Array":
-        zarr_json_bytes = await store.get_async(f"{path}/{ZARR_JSON}")
+        store_path = make_store_path(store)
+        zarr_json_bytes = await (store_path / ZARR_JSON).get_async()
         assert zarr_json_bytes is not None
         return cls.from_json(
-            store,
-            path,
+            store_path,
             json.loads(zarr_json_bytes),
             runtime_configuration=runtime_configuration or ArrayRuntimeConfiguration(),
         )
 
     @classmethod
     def open(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         runtime_configuration: Optional[ArrayRuntimeConfiguration] = None,
     ) -> "Array":
-        return sync(
-            cls.open_async(store, path, runtime_configuration=runtime_configuration)
-        )
+        return sync(cls.open_async(store, runtime_configuration=runtime_configuration))
 
     @classmethod
     def from_json(
         cls,
-        store: Store,
-        path: str,
+        store_path: StorePath,
         zarr_json: Any,
         runtime_configuration: ArrayRuntimeConfiguration,
     ) -> "Array":
         metadata = make_cattr().structure(zarr_json, ArrayMetadata)
         out = cls(
             metadata=metadata,
-            store=store,
-            path=path,
+            store_path=store_path,
             runtime_configuration=runtime_configuration,
             codecs=Codec.codecs_from_metadata(metadata.codecs),
         )
         out._validate_metadata()
         return out
 
     @classmethod
     async def open_auto_async(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         runtime_configuration: Optional[ArrayRuntimeConfiguration] = None,
     ) -> Union["Array", ArrayV2]:
-        v3_metadata_bytes = await store.get_async(f"{path}/{ZARR_JSON}")
+        store_path = make_store_path(store)
+        v3_metadata_bytes = await (store_path / ZARR_JSON).get_async()
         if v3_metadata_bytes is not None:
             return cls.from_json(
-                store,
-                path,
+                store_path,
                 json.loads(v3_metadata_bytes),
                 runtime_configuration=runtime_configuration
                 or ArrayRuntimeConfiguration(),
             )
-        return await ArrayV2.open_async(store, path)
+        return await ArrayV2.open_async(store_path)
 
     @classmethod
     async def open_auto(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         runtime_configuration: Optional[ArrayRuntimeConfiguration] = None,
     ) -> Union["Array", ArrayV2]:
-        return sync(cls.open_auto_async(store, path, runtime_configuration))
+        return sync(cls.open_auto_async(store, runtime_configuration))
 
     async def _save_metadata(self) -> None:
         self._validate_metadata()
 
-        await self.store.set_async(
-            f"{self.path}/{ZARR_JSON}",
+        await (self.store_path / ZARR_JSON).set_async(
             json.dumps(asdict(self.metadata), default=_json_convert).encode(),
         )
 
     def _validate_metadata(self) -> None:
         assert len(self.metadata.shape) == len(
             self.metadata.chunk_grid.configuration.chunk_shape
         ), "`chunk_shape` and `shape` need to have the same number of dimensions."
@@ -366,18 +353,24 @@
         )
 
         if out.shape:
             return out
         else:
             return out[()]
 
-    async def _read_chunk(self, chunk_coords, chunk_selection, out_selection, out):
+    async def _read_chunk(
+        self,
+        chunk_coords: ChunkCoords,
+        chunk_selection: SliceSelection,
+        out_selection: SliceSelection,
+        out: np.ndarray,
+    ):
         chunk_key_encoding = self.metadata.chunk_key_encoding
-        chunk_key = f"{self.path}/{chunk_key_encoding.encode_chunk_key(chunk_coords)}"
-        value_handle = FileValueHandle(self.store, chunk_key)
+        chunk_key = chunk_key_encoding.encode_chunk_key(chunk_coords)
+        value_handle: ValueHandle = FileValueHandle(self.store_path / chunk_key)
 
         if len(self.codecs) == 1 and isinstance(self.codecs[0], ShardingCodec):
             value_handle = await self.codecs[0].decode_partial(
                 value_handle, chunk_selection, self._core_metadata
             )
             chunk_array = await value_handle.toarray()
             if chunk_array is not None:
@@ -464,16 +457,16 @@
         value: np.ndarray,
         chunk_shape: ChunkCoords,
         chunk_coords: ChunkCoords,
         chunk_selection: SliceSelection,
         out_selection: SliceSelection,
     ):
         chunk_key_encoding = self.metadata.chunk_key_encoding
-        chunk_key = f"{self.path}/{chunk_key_encoding.encode_chunk_key(chunk_coords)}"
-        value_handle = FileValueHandle(self.store, chunk_key)
+        chunk_key = chunk_key_encoding.encode_chunk_key(chunk_coords)
+        value_handle = FileValueHandle(self.store_path / chunk_key)
 
         if is_total_slice(chunk_selection, chunk_shape):
             # write entire chunks
             if np.isscalar(value):
                 chunk_array = np.empty(
                     chunk_shape,
                     dtype=self.metadata.dtype,
@@ -546,29 +539,30 @@
 
         # Remove all chunks outside of the new shape
         chunk_shape = self.metadata.chunk_grid.configuration.chunk_shape
         chunk_key_encoding = self.metadata.chunk_key_encoding
         old_chunk_coords = set(all_chunk_coords(self.metadata.shape, chunk_shape))
         new_chunk_coords = set(all_chunk_coords(new_shape, chunk_shape))
 
+        async def _delete_key(key: str) -> None:
+            await (self.store_path / key).delete_async()
+
         await concurrent_map(
             [
-                (f"{self.path}/{chunk_key_encoding.encode_chunk_key(chunk_coords)}",)
+                (chunk_key_encoding.encode_chunk_key(chunk_coords),)
                 for chunk_coords in old_chunk_coords.difference(new_chunk_coords)
             ],
-            self.store.delete_async,
+            _delete_key,
             self.runtime_configuration.concurrency,
         )
 
         # Write new metadata
-        await self.store.set_async(
-            f"{self.path}/{ZARR_JSON}",
+        await (self.store_path / ZARR_JSON).set_async(
             json.dumps(asdict(new_metadata), default=_json_convert).encode(),
         )
         return attr.evolve(self, metadata=new_metadata)
 
     def reshape(self, new_shape: ChunkCoords) -> "Array":
         return sync(self.reshape_async(new_shape))
 
     def __repr__(self):
-        path = self.path
-        return f"<Array {path}>"
+        return f"<Array {self.store_path}>"
```

### Comparing `zarrita-0.1.0a5/zarrita/array_v2.py` & `zarrita-0.1.0a6/zarrita/array_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Selection,
     SliceSelection,
     make_cattr,
     to_thread,
 )
 from zarrita.indexing import BasicIndexer, is_total_slice
 from zarrita.metadata import ArrayV2Metadata
-from zarrita.store import Store
+from zarrita.store import StoreLike, StorePath, make_store_path
 from zarrita.sync import sync
 from zarrita.value_handle import (
     BufferValueHandle,
     FileValueHandle,
     NoneValueHandle,
     ValueHandle,
 )
@@ -49,36 +49,35 @@
         return await self.array.set_async(self.selection, value)
 
 
 @frozen
 class ArrayV2:
     metadata: ArrayV2Metadata
     attributes: Optional[Dict[str, Any]]
-    store: "Store"
-    path: str
+    store_path: StorePath
 
     @classmethod
     async def create_async(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         *,
         shape: ChunkCoords,
         dtype: np.dtype,
         chunks: ChunkCoords,
         dimension_separator: Literal[".", "/"] = ".",
         fill_value: Optional[Union[None, int, float]] = None,
         order: Literal["C", "F"] = "C",
         filters: Optional[List[Dict[str, Any]]] = None,
         compressor: Optional[Dict[str, Any]] = None,
         attributes: Optional[Dict[str, Any]] = None,
         exists_ok: bool = False,
     ) -> "ArrayV2":
+        store_path = make_store_path(store)
         if not exists_ok:
-            assert not await store.exists_async(f"{path}/{ZARRAY_JSON}")
+            assert not await (store_path / ZARRAY_JSON).exists_async()
 
         metadata = ArrayV2Metadata(
             shape=shape,
             dtype=dtype,
             chunks=chunks,
             order=order,
             dimension_separator=dimension_separator,
@@ -88,26 +87,24 @@
             else None,
             filters=[numcodecs.get_codec(filter).get_config() for filter in filters]
             if filters is not None
             else None,
         )
         array = cls(
             metadata=metadata,
-            store=store,
-            path=path,
+            store_path=store_path,
             attributes=attributes,
         )
         await array._save_metadata()
         return array
 
     @classmethod
     def create(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         *,
         shape: ChunkCoords,
         dtype: np.dtype,
         chunks: ChunkCoords,
         dimension_separator: Literal[".", "/"] = ".",
         fill_value: Optional[Union[None, int, float]] = None,
         order: Literal["C", "F"] = "C",
@@ -115,15 +112,14 @@
         compressor: Optional[Dict[str, Any]] = None,
         attributes: Optional[Dict[str, Any]] = None,
         exists_ok: bool = False,
     ) -> "ArrayV2":
         return sync(
             cls.create_async(
                 store,
-                path,
                 shape=shape,
                 dtype=dtype,
                 chunks=chunks,
                 order=order,
                 dimension_separator=dimension_separator,
                 fill_value=0 if fill_value is None else fill_value,
                 compressor=compressor,
@@ -132,54 +128,45 @@
                 exists_ok=exists_ok,
             )
         )
 
     @classmethod
     async def open_async(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
     ) -> "ArrayV2":
+        store_path = make_store_path(store)
         zarray_bytes, zattrs_bytes = await asyncio.gather(
-            store.get_async(f"{path}/{ZARRAY_JSON}"),
-            store.get_async(f"{path}/{ZATTRS_JSON}"),
+            (store_path / ZARRAY_JSON).get_async(),
+            (store_path / ZATTRS_JSON).get_async(),
         )
         assert zarray_bytes is not None
         return cls.from_json(
-            store,
-            path,
+            store_path,
             zarray_json=json.loads(zarray_bytes),
             zattrs_json=json.loads(zattrs_bytes) if zattrs_bytes is not None else None,
         )
 
     @classmethod
     def open(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
     ) -> "ArrayV2":
-        return sync(
-            cls.open_async(
-                store,
-                path,
-            )
-        )
+        return sync(cls.open_async(store))
 
     @classmethod
     def from_json(
         cls,
-        store: Store,
-        path: str,
+        store_path: StorePath,
         zarray_json: Any,
         zattrs_json: Optional[Any],
     ) -> "ArrayV2":
         metadata = make_cattr().structure(zarray_json, ArrayV2Metadata)
         out = cls(
-            store=store,
-            path=path,
+            store_path=store_path,
             metadata=metadata,
             attributes=zattrs_json,
         )
         out._validate_metadata()
         return out
 
     async def _save_metadata(self) -> None:
@@ -189,27 +176,23 @@
                     return o.str
                 else:
                     return o.descr
             raise TypeError
 
         self._validate_metadata()
 
-        await self.store.set_async(
-            f"{self.path}/{ZARRAY_JSON}",
+        await (self.store_path / ZARRAY_JSON).set_async(
             json.dumps(asdict(self.metadata), default=convert).encode(),
         )
         if self.attributes is not None and len(self.attributes) > 0:
-            await self.store.set_async(
-                f"{self.path}/{ZATTRS_JSON}",
+            await (self.store_path / ZATTRS_JSON).set_async(
                 json.dumps(self.attributes).encode(),
             )
         else:
-            await self.store.delete_async(
-                f"{self.path}/{ZATTRS_JSON}",
-            )
+            await (self.store_path / ZATTRS_JSON).delete_async()
 
     def _validate_metadata(self) -> None:
         assert len(self.metadata.shape) == len(
             self.metadata.chunks
         ), "`chunks` and `shape` need to have the same number of dimensions."
 
     @property
@@ -246,17 +229,24 @@
         )
 
         if out.shape:
             return out
         else:
             return out[()]
 
-    async def _read_chunk(self, chunk_coords, chunk_selection, out_selection, out):
-        chunk_key = f"{self.path}/{self._encode_chunk_key(chunk_coords)}"
-        value_handle = FileValueHandle(self.store, chunk_key)
+    async def _read_chunk(
+        self,
+        chunk_coords: ChunkCoords,
+        chunk_selection: SliceSelection,
+        out_selection: SliceSelection,
+        out: np.ndarray,
+    ):
+        value_handle = FileValueHandle(
+            self.store_path / self._encode_chunk_key(chunk_coords)
+        )
 
         chunk_array = await self._decode_chunk(await value_handle.tobytes())
         if chunk_array is not None:
             tmp = chunk_array[chunk_selection]
             out[out_selection] = tmp
         else:
             out[out_selection] = self.metadata.fill_value
@@ -336,16 +326,17 @@
         self,
         value: np.ndarray,
         chunk_shape: ChunkCoords,
         chunk_coords: ChunkCoords,
         chunk_selection: SliceSelection,
         out_selection: SliceSelection,
     ):
-        chunk_key = f"{self.path}/{self._encode_chunk_key(chunk_coords)}"
-        value_handle = FileValueHandle(self.store, chunk_key)
+        value_handle = FileValueHandle(
+            self.store_path / self._encode_chunk_key(chunk_coords)
+        )
 
         if is_total_slice(chunk_selection, chunk_shape):
             # write entire chunks
             if np.isscalar(value):
                 chunk_array = np.empty(
                     chunk_shape,
                     dtype=self.metadata.dtype,
@@ -416,9 +407,8 @@
     def _encode_chunk_key(self, chunk_coords: ChunkCoords) -> str:
         chunk_identifier = self.metadata.dimension_separator.join(
             map(str, chunk_coords)
         )
         return "0" if chunk_identifier == "" else chunk_identifier
 
     def __repr__(self):
-        path = self.path
-        return f"<Array_v2 {path}>"
+        return f"<Array_v2 {self.store_path}>"
```

### Comparing `zarrita-0.1.0a5/zarrita/codecs.py` & `zarrita-0.1.0a6/zarrita/codecs.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a5/zarrita/common.py` & `zarrita-0.1.0a6/zarrita/common.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a5/zarrita/group.py` & `zarrita-0.1.0a6/zarrita/group.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,117 @@
 import json
 from typing import Any, Dict, Literal, Optional, Union
 
 from attr import asdict, field, frozen
 
 from zarrita.array import Array, ArrayRuntimeConfiguration
 from zarrita.common import ZARR_JSON, make_cattr
-from zarrita.store import Store
+from zarrita.store import StoreLike, StorePath, make_store_path
 from zarrita.sync import sync
 
 
 @frozen
 class GroupMetadata:
     attributes: Dict[str, Any] = field(factory=dict)
     zarr_format: Literal[3] = 3
     node_type: Literal["group"] = "group"
 
 
 @frozen
 class Group:
     metadata: GroupMetadata
-    store: Store
-    path: str
+    store_path: StorePath
 
     @classmethod
     async def create_async(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         *,
         attributes: Optional[Dict[str, Any]] = None,
         exists_ok: bool = False,
     ) -> "Group":
+        store_path = make_store_path(store)
         if not exists_ok:
-            assert not await store.exists_async(f"{path}/{ZARR_JSON}")
+            assert not await (store_path / ZARR_JSON).exists_async()
         group = cls(
             metadata=GroupMetadata(attributes=attributes or {}),
-            store=store,
-            path=path,
+            store_path=store_path,
         )
         await group._save_metadata()
         return group
 
     @classmethod
     def create(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         *,
         attributes: Optional[Dict[str, Any]] = None,
         exists_ok: bool = False,
     ) -> "Group":
-        return sync(
-            cls.create_async(store, path, attributes=attributes, exists_ok=exists_ok)
-        )
+        return sync(cls.create_async(store, attributes=attributes, exists_ok=exists_ok))
 
     @classmethod
-    async def open_async(cls, store: "Store", path: str) -> "Group":
-        zarr_json_bytes = await store.get_async(f"{path}/{ZARR_JSON}")
+    async def open_async(cls, store: StoreLike) -> "Group":
+        store_path = make_store_path(store)
+        zarr_json_bytes = await (store_path / ZARR_JSON).get_async()
         assert zarr_json_bytes is not None
-        return cls.from_json(store, path, json.loads(zarr_json_bytes))
+        return cls.from_json(store_path, json.loads(zarr_json_bytes))
 
     @classmethod
-    def open(cls, store: "Store", path: str) -> "Group":
-        return sync(cls.open_async(store, path))
+    def open(cls, store: StoreLike) -> "Group":
+        return sync(cls.open_async(store))
 
     @classmethod
-    def from_json(cls, store: Store, path: str, zarr_json: Any) -> "Group":
+    def from_json(cls, store_path: StorePath, zarr_json: Any) -> "Group":
         group = cls(
             metadata=make_cattr().structure(zarr_json, GroupMetadata),
-            store=store,
-            path=path,
+            store_path=store_path,
         )
         return group
 
     @classmethod
     async def open_or_array(
         cls,
-        store: Store,
-        path: str,
+        store: StoreLike,
         runtime_configuration: Optional[ArrayRuntimeConfiguration] = None,
     ) -> Union[Array, "Group"]:
-        zarr_json_bytes = await store.get_async(f"{path}/{ZARR_JSON}")
+        store_path = make_store_path(store)
+        zarr_json_bytes = await (store_path / ZARR_JSON).get_async()
         if zarr_json_bytes is None:
             raise KeyError
         zarr_json = json.loads(zarr_json_bytes)
         if zarr_json["node_type"] == "group":
-            return cls.from_json(store, path, zarr_json)
+            return cls.from_json(store_path, zarr_json)
         if zarr_json["node_type"] == "array":
             return Array.from_json(
-                store,
-                path,
+                store_path,
                 zarr_json,
                 runtime_configuration=runtime_configuration
                 or ArrayRuntimeConfiguration(),
             )
         raise KeyError
 
     async def _save_metadata(self) -> None:
-        await self.store.set_async(
-            f"{self.path}/{ZARR_JSON}",
+        await (self.store_path / ZARR_JSON).set_async(
             json.dumps(asdict(self.metadata)).encode(),
         )
 
-    def _dereference_path(self, path: str) -> str:
-        assert isinstance(path, str)
-        path = f"{self.path}/{path}"
-        if len(path) > 1:
-            assert path[-1] != "/"
-        return path
-
     async def get_async(self, path: str) -> Union[Array, "Group"]:
-        path = self._dereference_path(path)
-        return await self.__class__.open_or_array(self.store, path)
+        return await self.__class__.open_or_array(self.store_path / path)
 
     def __getitem__(self, path: str) -> Union[Array, "Group"]:
         return sync(self.get_async(path))
 
     async def create_group_async(self, path: str, **kwargs) -> "Group":
-        path = self._dereference_path(path)
-        return await self.__class__.create_async(self.store, path, **kwargs)
+        return await self.__class__.create_async(self.store_path / path, **kwargs)
 
     def create_group(self, path: str, **kwargs) -> "Group":
         return sync(self.create_group_async(path))
 
     async def create_array_async(self, path: str, **kwargs) -> Array:
-        path = self._dereference_path(path)
-        return await Array.create_async(self.store, path, **kwargs)
+        return await Array.create_async(self.store_path / path, **kwargs)
 
     def create_array(self, path: str, **kwargs) -> Array:
         return sync(self.create_array_async(path, **kwargs))
 
     def __repr__(self):
-        path = self.path
-        return f"<Group {path}>"
+        return f"<Group {self.store_path}>"
```

### Comparing `zarrita-0.1.0a5/zarrita/group_v2.py` & `zarrita-0.1.0a6/zarrita/group_v2.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,143 +2,124 @@
 import json
 from typing import Any, Dict, Literal, Optional, Union
 
 from attr import asdict, frozen
 
 from zarrita.array_v2 import ArrayV2
 from zarrita.common import ZARRAY_JSON, ZATTRS_JSON, ZGROUP_JSON, make_cattr
-from zarrita.store import Store
+from zarrita.store import StoreLike, StorePath, make_store_path
 from zarrita.sync import sync
 
 
 @frozen
 class GroupV2Metadata:
     zarr_format: Literal[2] = 2
 
 
 @frozen
 class GroupV2:
     metadata: GroupV2Metadata
-    store: Store
-    path: str
+    store_path: StorePath
     attributes: Optional[Dict[str, Any]] = None
 
     @classmethod
     async def create_async(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         *,
         attributes: Optional[Dict[str, Any]] = None,
         exists_ok: bool = False,
     ) -> "GroupV2":
+        store_path = make_store_path(store)
         if not exists_ok:
-            assert not await store.exists_async(f"{path}/{ZGROUP_JSON}")
+            assert not await (store_path / ZGROUP_JSON).exists_async()
         group = cls(
-            metadata=GroupV2Metadata(), attributes=attributes, store=store, path=path
+            metadata=GroupV2Metadata(), attributes=attributes, store_path=store_path
         )
         await group._save_metadata()
         return group
 
     @classmethod
     def create(
         cls,
-        store: "Store",
-        path: str,
+        store: StoreLike,
         *,
         attributes: Optional[Dict[str, Any]] = None,
         exists_ok: bool = False,
     ) -> "GroupV2":
-        return sync(
-            cls.create_async(store, path, attributes=attributes, exists_ok=exists_ok)
-        )
+        return sync(cls.create_async(store, attributes=attributes, exists_ok=exists_ok))
 
     @classmethod
-    async def open_async(cls, store: "Store", path: str) -> "GroupV2":
-        zgroup_bytes = await store.get_async(f"{path}/{ZGROUP_JSON}")
+    async def open_async(cls, store: StoreLike) -> "GroupV2":
+        store_path = make_store_path(store)
+        zgroup_bytes = await (store_path / ZGROUP_JSON).get_async()
         assert zgroup_bytes is not None
-        zattrs_bytes = await store.get_async(f"{path}/{ZATTRS_JSON}")
+        zattrs_bytes = await (store_path / ZATTRS_JSON).get_async()
         metadata = json.loads(zgroup_bytes)
         attributes = json.loads(zattrs_bytes) if zattrs_bytes is not None else None
 
-        return cls.from_json(store, path, metadata, attributes)
+        return cls.from_json(store_path, metadata, attributes)
 
     @classmethod
-    def open(cls, store: "Store", path: str) -> "GroupV2":
-        return sync(cls.open_async(store, path))
+    def open(cls, store_path: StorePath) -> "GroupV2":
+        return sync(cls.open_async(store_path))
 
     @classmethod
     def from_json(
         cls,
-        store: Store,
-        path: str,
+        store_path: StorePath,
         zarr_json: Any,
         attributes: Optional[Dict[str, Any]] = None,
     ) -> "GroupV2":
         group = cls(
             metadata=make_cattr().structure(zarr_json, GroupV2Metadata),
-            store=store,
-            path=path,
+            store_path=store_path,
             attributes=attributes,
         )
         return group
 
     @staticmethod
-    async def open_or_array(store: Store, path: str) -> Union[ArrayV2, "GroupV2"]:
+    async def open_or_array(store: StoreLike) -> Union[ArrayV2, "GroupV2"]:
+        store_path = make_store_path(store)
         zgroup_bytes, zattrs_bytes = await asyncio.gather(
-            store.get_async(f"{path}/{ZGROUP_JSON}"),
-            store.get_async(f"{path}/{ZATTRS_JSON}"),
+            (store_path / ZGROUP_JSON).get_async(),
+            (store_path / ZATTRS_JSON).get_async(),
         )
         attributes = json.loads(zattrs_bytes) if zattrs_bytes is not None else None
         if zgroup_bytes is not None:
-            return GroupV2.from_json(store, path, json.loads(zgroup_bytes), attributes)
-        zarray_bytes = await store.get_async(f"{path}/{ZARRAY_JSON}")
+            return GroupV2.from_json(store_path, json.loads(zgroup_bytes), attributes)
+        zarray_bytes = await (store_path / ZARRAY_JSON).get_async()
         if zarray_bytes is not None:
-            return ArrayV2.from_json(store, path, json.loads(zarray_bytes), attributes)
+            return ArrayV2.from_json(store_path, json.loads(zarray_bytes), attributes)
         raise KeyError
 
     async def _save_metadata(self) -> None:
-        await self.store.set_async(
-            f"{self.path}/{ZGROUP_JSON}",
+        await (self.store_path / ZGROUP_JSON).set_async(
             json.dumps(asdict(self.metadata)).encode(),
         )
         if self.attributes is not None and len(self.attributes) > 0:
-            await self.store.set_async(
-                f"{self.path}/{ZATTRS_JSON}",
+            await (self.store_path / ZATTRS_JSON).set_async(
                 json.dumps(self.attributes).encode(),
             )
         else:
-            await self.store.delete_async(
-                f"{self.path}/{ZATTRS_JSON}",
-            )
-
-    def _dereference_path(self, path: str) -> str:
-        assert isinstance(path, str)
-        path = f"{self.path}/{path}"
-        if len(path) > 1:
-            assert path[-1] != "/"
-        return path
+            await (self.store_path / ZATTRS_JSON).delete_async()
 
     async def get_async(self, path: str) -> Union[ArrayV2, "GroupV2"]:
-        path = self._dereference_path(path)
-        return await self.__class__.open_or_array(self.store, path)
+        return await self.__class__.open_or_array(self.store_path / path)
 
     def __getitem__(self, path: str) -> Union[ArrayV2, "GroupV2"]:
         return sync(self.get_async(path))
 
     async def create_group_async(self, path: str, **kwargs) -> "GroupV2":
-        path = self._dereference_path(path)
-        return await self.__class__.create_async(self.store, path, **kwargs)
+        return await self.__class__.create_async(self.store_path / path, **kwargs)
 
     def create_group(self, path: str, **kwargs) -> "GroupV2":
         return sync(self.create_group_async(path))
 
     async def create_array_async(self, path: str, **kwargs) -> ArrayV2:
-        path = self._dereference_path(path)
-        return await ArrayV2.create_async(self.store, path, **kwargs)
+        return await ArrayV2.create_async(self.store_path / path, **kwargs)
 
     def create_array(self, path: str, **kwargs) -> "ArrayV2":
         return sync(self.create_array_async(path, **kwargs))
 
     def __repr__(self):
-        path = self.path
-        return f"<Group_v2 {path}>"
+        return f"<Group_v2 {self.store_path}>"
```

### Comparing `zarrita-0.1.0a5/zarrita/indexing.py` & `zarrita-0.1.0a6/zarrita/indexing.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a5/zarrita/metadata.py` & `zarrita-0.1.0a6/zarrita/metadata.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a5/zarrita/sharding.py` & `zarrita-0.1.0a6/zarrita/sharding.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a5/zarrita/store.py` & `zarrita-0.1.0a6/zarrita/store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,79 @@
 import asyncio
 import io
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 import fsspec
+from fsspec.asyn import AsyncFileSystem
 
 from zarrita.common import BytesLike, to_thread
 
 
+def _dereference_path(root: str, path: str) -> str:
+    assert isinstance(root, str)
+    assert isinstance(path, str)
+    path = f"{root}/{path}" if root != "" else path
+    path = path.rstrip("/")
+    return path
+
+
+class StorePath:
+    store: "Store"
+    path: str
+
+    def __init__(self, store: "Store", path: Optional[str] = None):
+        self.store = store
+        self.path = path or ""
+
+    @classmethod
+    def from_path(cls, pth: "Path") -> "StorePath":
+        return cls(Store.from_path(pth))
+
+    async def get_async(
+        self, byte_range: Optional[Tuple[int, int]] = None
+    ) -> Optional[BytesLike]:
+        return await self.store.get_async(self.path, byte_range)
+
+    async def set_async(
+        self, value: BytesLike, byte_range: Optional[Tuple[int, int]] = None
+    ) -> None:
+        await self.store.set_async(self.path, value, byte_range)
+
+    async def delete_async(self) -> None:
+        await self.store.delete_async(self.path)
+
+    async def exists_async(self) -> bool:
+        return await self.store.exists_async(self.path)
+
+    def __truediv__(self, other: str) -> "StorePath":
+        return self.__class__(self.store, _dereference_path(self.path, other))
+
+    def __str__(self) -> str:
+        return _dereference_path(str(self.store), self.path)
+
+    def __repr__(self) -> str:
+        return f"StorePath({self.store.__class__.__name__}, {repr(str(self))})"
+
+
 class Store:
+    @classmethod
+    def from_path(cls, pth: "Path") -> "Store":
+        try:
+            from upath import UPath
+
+            if isinstance(pth, UPath):
+                storage_options = pth._kwargs.copy()
+                storage_options.pop("_url", None)
+                return RemoteStore(str(pth), **storage_options)
+        except ImportError:
+            pass
+
+        return LocalStore(pth)
+
     async def multi_get_async(
         self, keys: List[Tuple[str, Optional[Tuple[int, int]]]]
     ) -> List[Optional[BytesLike]]:
         return await asyncio.gather(
             *[self.get_async(key, byte_range) for key, byte_range in keys]
         )
 
@@ -38,14 +99,17 @@
 
     async def delete_async(self, key: str) -> None:
         raise NotImplementedError
 
     async def exists_async(self, key: str) -> bool:
         raise NotImplementedError
 
+    def __truediv__(self, other: str) -> StorePath:
+        return StorePath(self, other)
+
 
 class LocalStore(Store):
     root: Path
     auto_mkdir: bool
 
     def __init__(self, root: Union[Path, str], auto_mkdir: bool = True):
         if isinstance(root, str):
@@ -120,16 +184,25 @@
         path = self.root / key
         await to_thread(path.unlink, True)
 
     async def exists_async(self, key: str) -> bool:
         path = self.root / key
         return await to_thread(path.exists)
 
+    def __str__(self) -> str:
+        return f"file://{self.root}"
+
+    def __repr__(self) -> str:
+        return f"LocalStore({repr(str(self))})"
+
 
 class RemoteStore(Store):
+    fs: AsyncFileSystem
+    root: str
+
     def __init__(self, url: str, **storage_options):
         assert isinstance(url, str)
 
         # instantiate file system
         fs, root = fsspec.core.url_to_fs(
             url, auto_mkdir=True, asynchronous=True, **storage_options
         )
@@ -137,15 +210,15 @@
         self.fs = fs
         self.root = root.rstrip("/")
 
     async def get_async(
         self, key: str, byte_range: Optional[Tuple[int, int]] = None
     ) -> Optional[BytesLike]:
         assert isinstance(key, str)
-        path = f"{self.root}/{key}"
+        path = _dereference_path(self.root, key)
 
         try:
             value = await (
                 self.fs._cat_file(path, byte_range[0], byte_range[1])
                 if byte_range
                 else self.fs._cat_file(path)
             )
@@ -154,25 +227,56 @@
 
         return value
 
     async def set_async(
         self, key: str, value: BytesLike, byte_range: Optional[Tuple[int, int]] = None
     ) -> None:
         assert isinstance(key, str)
-        path = f"{self.root}/{key}"
+        path = _dereference_path(self.root, key)
 
         # write data
         if byte_range:
             with self.fs._open(path, "r+b") as f:
                 f.seek(byte_range[0])
                 f.write(value)
         else:
             await self.fs._write_bytes(path, value)
 
     async def delete_async(self, key: str) -> None:
-        path = f"{self.root}/{key}"
+        path = _dereference_path(self.root, key)
         if await self.fs._exists(path):
             await self.fs._rm(path)
 
     async def exists_async(self, key: str) -> bool:
-        path = f"{self.root}/{key}"
+        path = _dereference_path(self.root, key)
         return await self.fs._exists(path)
+
+    def __str__(self) -> str:
+        protocol = (
+            self.fs.protocol[0]
+            if isinstance(self.fs.protocol, list)
+            else self.fs.protocol
+        )
+        return f"{protocol}://{self.root}"
+
+    def __repr__(self) -> str:
+        return f"RemoteStore({repr(str(self))})"
+
+
+StoreLike = Union[Store, StorePath, Path, str]
+
+
+def make_store_path(store_like: StoreLike) -> StorePath:
+    if isinstance(store_like, StorePath):
+        return store_like
+    elif isinstance(store_like, Store):
+        return StorePath(store_like)
+    elif isinstance(store_like, Path):
+        return StorePath(Store.from_path(store_like))
+    elif isinstance(store_like, str):
+        try:
+            from upath import UPath
+
+            return StorePath(Store.from_path(UPath(store_like)))
+        except ImportError:
+            return StorePath(LocalStore(Path(store_like)))
+    raise TypeError
```

### Comparing `zarrita-0.1.0a5/zarrita/sync.py` & `zarrita-0.1.0a6/zarrita/sync.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a5/zarrita/value_handle.py` & `zarrita-0.1.0a6/zarrita/value_handle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import abstractmethod
 from typing import Optional, Tuple
 
 import numpy as np
 
 from zarrita.common import BytesLike
-from zarrita.store import Store
+from zarrita.store import StorePath
 
 
 # ValueHandle abstracts over files, byte buffer, and arrays.
 # Makes it easy pass around as references with lazy reading (esp. for files).
 # Facilitates implementations of codec which either operate on arrays or bytes.
 class ValueHandle:
     @abstractmethod
@@ -30,44 +30,42 @@
     async def toarray(
         self, shape: Optional[Tuple[int, ...]] = None
     ) -> Optional[np.ndarray]:
         pass
 
 
 class FileValueHandle(ValueHandle):
-    store: "Store"
-    path: str
+    store_path: "StorePath"
     selection: Optional[slice] = None
 
-    def __init__(self, store: "Store", path: str):
+    def __init__(self, store_path: "StorePath"):
         super().__init__()
-        self.store = store
-        self.path = path
+        self.store_path = store_path
 
     def __getitem__(self, selection: slice) -> ValueHandle:
-        out = FileValueHandle(self.store, self.path)
+        out = FileValueHandle(self.store_path)
         out.selection = selection
         return out
 
     async def set_async(
         self,
         value: ValueHandle,
     ):
         buf = await value.tobytes()
         if buf:
-            await self.store.set_async(self.path, buf)
+            await self.store_path.set_async(buf)
         else:
-            await self.store.delete_async(self.path)
+            await self.store_path.delete_async()
 
     async def tobytes(self) -> Optional[bytes]:
         if self.selection:
-            return await self.store.get_async(
-                self.path, (self.selection.start, self.selection.stop)
+            return await self.store_path.get_async(
+                (self.selection.start, self.selection.stop)
             )
-        return await self.store.get_async(self.path)
+        return await self.store_path.get_async()
 
     async def toarray(
         self, shape: Optional[Tuple[int, ...]] = None
     ) -> Optional[np.ndarray]:
         buf = await self.tobytes()
         if buf is not None:
             return np.frombuffer(buf)
```

### Comparing `zarrita-0.1.0a5/PKG-INFO` & `zarrita-0.1.0a6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: zarrita
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: 
 License: MIT
 Author: Norman Rzepka
 Author-email: code@normanrz.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
-Requires-Dist: cattrs (>=22.2.0,<23.0.0)
-Requires-Dist: crc32c (>=2.3.post0,<3.0)
-Requires-Dist: fsspec (>=2022.2.0,<2023.0.0)
-Requires-Dist: numcodecs (>=0.10.0,<0.11.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=22.2.0)
+Requires-Dist: cattrs (>=22.2.0)
+Requires-Dist: crc32c (>=2.3)
+Requires-Dist: fsspec (>=2022.0.0)
+Requires-Dist: numcodecs (>=0.11.0,<0.12.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Zarrita
 
 Zarrita is an experimental implementation of [Zarr v3](https://zarr-specs.readthedocs.io/en/latest/v3/core/v3.0.html) including [sharding](https://zarr.dev/zeps/draft/ZEP0002.html). This is only a technical proof of concept meant for generating sample datasets. Not recommended for production use.
 
@@ -32,38 +33,36 @@
 store = zarrita.LocalStore('testdata') # or zarrita.RemoteStore('s3://bucket/test')
 ```
 
 ## Create an array
 
 ```python
 a = await zarrita.Array.create_async(
-    store,
-    'array',
+    store / 'array',
     shape=(6, 10),
     dtype='int32',
     chunk_shape=(2, 5),
     codecs=[zarrita.codecs.blosc_codec()],
     attributes={'question': 'life', 'answer': 42}
 )
 await a.async_[:, :].set(np.ones((6, 10), dtype='int32'))
 ```
 
 ## Open an array
 
 ```python
-a = await zarrita.Array.open_async(store, 'array')
+a = await zarrita.Array.open_async(store / 'array')
 assert np.array_equal(await a.async_[:, :].get(), np.ones((6, 10), dtype='int32'))
 ```
 
 ## Create an array with sharding
 
 ```python
 a = await zarrita.Array.create_async(
-    store,
-    'sharding',
+    store / 'sharding',
     shape=(16, 16),
     dtype='int32',
     chunk_shape=(16, 16),
     chunk_key_encoding=('v2', '.'),
     codecs=[
         zarrita.codecs.sharding_codec(
             chunk_shape=(8, 8),
@@ -75,31 +74,31 @@
 await a.async_[:, :].set(data)
 assert np.array_equal(await a.async_[:, :].get(), data)
 ```
 
 ## Create a group
 
 ```python
-g = await zarrita.Group.create_async(store, 'group')
+g = await zarrita.Group.create_async(store / 'group')
 g2 = await g.create_group_async('group2')
 a = await g2.create_array_async(
     'array',
     shape=(16, 16),
     dtype='int32',
     chunk_shape=(16, 16),
 )
 await a.async_[:, :].set(np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
 ```
 
 ## Open a group
 
 ```python
-g = await zarrita.Group.open_async(store, 'group')
+g = await zarrita.Group.open_async(store / 'group')
 g2 = g['group2']
-a = g['group2/array']
+a = g['group2']['array']
 assert np.array_equal(await a.asnyc_[:, :].get(), np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
 ```
 
 # Credits
 
 This is a largely-rewritten fork of `zarrita` by [@alimanfoo](https://github.com/alimanfoo). It implements the Zarr v3 draft specification created by [@alimanfoo](https://github.com/alimanfoo), [@jstriebel](https://github.com/jstriebel), [@jbms](https://github.com/jbms) et al.
```

