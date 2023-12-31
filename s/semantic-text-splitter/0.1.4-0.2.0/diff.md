# Comparing `tmp/semantic_text_splitter-0.1.4.tar.gz` & `tmp/semantic_text_splitter-0.2.0.tar.gz`

## Comparing `semantic_text_splitter-0.1.4.tar` & `semantic_text_splitter-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 semantic_text_splitter-0.1.4/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-06-09 05:02:09.000000 semantic_text_splitter-0.1.4/.gitignore
--rw-r--r--   0     1001      123      262 2023-06-09 05:02:09.000000 semantic_text_splitter-0.1.4/CHANGELOG.md
--rw-r--r--   0     1001      123     3995 2023-06-09 05:02:09.000000 semantic_text_splitter-0.1.4/README.md
--rw-r--r--   0     1001      123      458 2023-06-09 05:02:09.000000 semantic_text_splitter-0.1.4/pyproject.toml
--rw-r--r--   0     1001      123     3029 2023-06-09 05:02:09.000000 semantic_text_splitter-0.1.4/semantic_text_splitter.pyi
--rw-r--r--   0     1001      123     8622 2023-06-09 05:02:09.000000 semantic_text_splitter-0.1.4/src/lib.rs
--rw-r--r--   0     1001      123      564 2023-06-09 05:02:09.000000 semantic_text_splitter-0.1.4/tests/test_integration.py
--rw-r--r--   0     1001      123     9987 2023-06-09 05:02:09.000000 semantic_text_splitter-0.1.4/Cargo.lock
--rw-r--r--   0        0        0     4882 1970-01-01 00:00:00.000000 semantic_text_splitter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     1025 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/CHANGELOG.md
+-rw-r--r--   0     1001      123     4027 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/README.md
+-rw-r--r--   0     1001      123      472 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     9035 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/semantic_text_splitter.pyi
+-rw-r--r--   0     1001      123    13390 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123   711396 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/tests/bert-base-cased.json
+-rw-r--r--   0     1001      123     1874 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/tests/test_integration.py
+-rw-r--r--   0     1001      123    23384 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.0/PKG-INFO
```

### Comparing `semantic_text_splitter-0.1.4/Cargo.toml` & `semantic_text_splitter-0.2.0/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [package]
 name = "semantic-text-splitter"
-version = "0.1.4"
+version = "0.2.0"
 authors = ["Ben Brandt <benjamin.j.brandt@gmail.com>"]
 edition = "2021"
 description = "Split text into semantic chunks, up to a desired chunk size. Supports calculating length by characters and tokens (when used with large language models)."
 repository = "https://github.com/benbrandt/text-splitter"
 license = "MIT"
 keywords = ["text", "split", "tokenizer", "nlp", "ai"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "semantic_text_splitter"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.19.0", features = ["abi3-py37"] }
-text-splitter = "0.4.0"
+text-splitter = { version = "0.4.1", features = ["tokenizers"] }
+tokenizers = { version = "0.13.3", default_features = false, features = [
+    "onig",
+] }
```

### Comparing `semantic_text_splitter-0.1.4/.gitignore` & `semantic_text_splitter-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.1.4/README.md` & `semantic_text_splitter-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# text-splitter
+# semantic-text-splitter
 
-[![Documentation Status](https://readthedocs.org/projects/text-splitter/badge/?version=latest)](https://text-splitter.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
+[![Documentation Status](https://readthedocs.org/projects/semantic-text-splitter/badge/?version=stable)](https://semantic-text-splitter.readthedocs.io/en/stable/?badge=stable) [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
 
 Large language models (LLMs) can be used for many tasks, but often have a limited context size that can be smaller than documents you might want to use. To use documents of larger length, you often have to split your text into chunks to fit within this context size.
 
 This crate provides methods for splitting longer pieces of text into smaller chunks, aiming to maximize a desired chunk size, but still splitting at semantically sensible boundaries whenever possible.
 
 ## Get Started
 
 ### By Number of Characters
 
 ```python
 from semantic_text_splitter import CharacterTextSplitter
 
 # Maximum number of characters in a chunk
 max_characters = 1000
-# Optionally can also have the splitter trim whitespace for you
-splitter = CharacterTextSplitter(trim_chunks=True)
+# Optionally can also have the splitter not trim whitespace for you
+splitter = CharacterTextSplitter(trim_chunks=False)
 
 chunks = splitter.chunks("your document text", max_characters)
 ```
 
 ### Using a Range for Chunk Capacity
 
 You also have the option of specifying your chunk capacity as a range.
```

### Comparing `semantic_text_splitter-0.1.4/src/lib.rs` & `semantic_text_splitter-0.2.0/semantic_text_splitter.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,209 +1,189 @@
-//! Python Bindings for text-splitter crate
+from typing import Any, List, Tuple, Union
 
-#![warn(
-    clippy::pedantic,
-    future_incompatible,
-    missing_debug_implementations,
-    missing_docs,
-    nonstandard_style,
-    rust_2018_compatibility,
-    rust_2018_idioms,
-    rust_2021_compatibility,
-    unused
-)]
-// pyo3 uses this
-#![allow(elided_lifetimes_in_paths)]
-
-use pyo3::prelude::*;
-use text_splitter::{Characters, ChunkCapacity, TextSplitter};
-
-/// Custom chunk capacity for python to make it easier to work
-/// with python arguments
-#[derive(Debug, FromPyObject)]
-enum PyChunkCapacity {
-    #[pyo3(transparent, annotation = "int")]
-    Int(usize),
-    #[pyo3(annotation = "tuple[int, int]")]
-    IntTuple(usize, usize),
-}
-
-impl ChunkCapacity for PyChunkCapacity {
-    fn start(&self) -> Option<usize> {
-        match self {
-            Self::Int(_) => None,
-            Self::IntTuple(start, _) => Some(*start),
-        }
-    }
-
-    fn end(&self) -> usize {
-        match self {
-            Self::Int(end) | Self::IntTuple(_, end) => *end,
-        }
-    }
-}
-
-/**
-Plain-text splitter. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
-
-### By Number of Characters
-
-```python
-from semantic_text_splitter import CharacterTextSplitter
-
-# Maximum number of characters in a chunk
-max_characters = 1000
-# Optionally can also have the splitter trim whitespace for you
-splitter = CharacterTextSplitter(trim_chunks=True)
-
-chunks = splitter.chunks("your document text", max_characters)
-```
-
-### Using a Range for Chunk Capacity
-
-You also have the option of specifying your chunk capacity as a range.
-
-Once a chunk has reached a length that falls within the range it will be returned.
-
-It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
-
-```python
-from semantic_text_splitter import CharacterTextSplitter
-
-# Optionally can also have the splitter trim whitespace for you
-splitter = CharacterTextSplitter()
-
-# Maximum number of characters in a chunk. Will fill up the
-# chunk until it is somewhere in this range.
-chunks = splitter.chunks("your document text", chunk_capacity=(200,1000))
-```
-**/
-#[pyclass]
-struct CharacterTextSplitter {
-    splitter: TextSplitter<Characters>,
-}
-
-#[pymethods]
-impl CharacterTextSplitter {
-    /// Specify whether chunks should have whitespace trimmed from the
-    /// beginning and end or not.
-    ///
-    /// If `False` (default), joining all chunks should return the original
-    /// string.
-    /// If `True`, all chunks will have whitespace removed from beginning and end.
-    #[new]
-    #[pyo3(signature = (trim_chunks=false))]
-    fn new(trim_chunks: bool) -> Self {
-        Self {
-            splitter: TextSplitter::default().with_trim_chunks(trim_chunks),
-        }
-    }
-
-    /// Generate a list of chunks from a given text. Each chunk will be up to the `chunk_capacity`.
-    ///
-    /// ## Method
-    ///
-    /// To preserve as much semantic meaning within a chunk as possible, a recursive approach is used, starting at larger semantic units and, if that is too large, breaking it up into the next largest unit. Here is an example of the steps used:
-    ///
-    /// 1. Split the text by a given level
-    /// 2. For each section, does it fit within the chunk size?
-    ///   a. Yes. Merge as many of these neighboring sections into a chunk as possible to maximize chunk length.
-    ///   b. No. Split by the next level and repeat.
-    ///
-    /// The boundaries used to split the text if using the top-level `split` method, in descending length:
-    ///
-    /// 1. Descending sequence length of newlines. (Newline is `\r\n`, `\n`, or `\r`) Each unique length of consecutive newline sequences is treated as its own semantic level.
-    /// 2. [Unicode Sentence Boundaries](https://www.unicode.org/reports/tr29/#Sentence_Boundaries)
-    /// 3. [Unicode Word Boundaries](https://www.unicode.org/reports/tr29/#Word_Boundaries)
-    /// 4. [Unicode Grapheme Cluster Boundaries](https://www.unicode.org/reports/tr29/#Grapheme_Cluster_Boundaries)
-    /// 5. Characters
-    ///
-    /// Splitting doesn't occur below the character level, otherwise you could get partial
-    /// bytes of a char, which may not be a valid unicode str.
-    fn chunks<'text, 'splitter: 'text>(
-        &'splitter self,
-        text: &'text str,
-        chunk_capacity: PyChunkCapacity,
-    ) -> Vec<&'text str> {
-        self.splitter.chunks(text, chunk_capacity).collect()
-    }
-}
-
-/**
-# text-splitter
-
-[![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
-
-Large language models (LLMs) can be used for many tasks, but often have a limited context size that can be smaller than documents you might want to use. To use documents of larger length, you often have to split your text into chunks to fit within this context size.
-
-This crate provides methods for splitting longer pieces of text into smaller chunks, aiming to maximize a desired chunk size, but still splitting at semantically sensible boundaries whenever possible.
-
-## Get Started
-
-### By Number of Characters
-
-```python
-from semantic_text_splitter import CharacterTextSplitter
-
-# Maximum number of characters in a chunk
-max_characters = 1000
-# Optionally can also have the splitter trim whitespace for you
-splitter = CharacterTextSplitter(trim_chunks=True)
-
-chunks = splitter.chunks("your document text", max_characters)
-```
-
-### Using a Range for Chunk Capacity
-
-You also have the option of specifying your chunk capacity as a range.
-
-Once a chunk has reached a length that falls within the range it will be returned.
-
-It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
-
-```python
-from semantic_text_splitter import CharacterTextSplitter
-
-# Optionally can also have the splitter trim whitespace for you
-splitter = CharacterTextSplitter()
-
-# Maximum number of characters in a chunk. Will fill up the
-# chunk until it is somewhere in this range.
-chunks = splitter.chunks(
-    "your document text",
-    chunk_capacity_start=200,
-    chunk_capacity_end=1000
-)
-```
-
-## Method
-
-To preserve as much semantic meaning within a chunk as possible, a recursive approach is used, starting at larger semantic units and, if that is too large, breaking it up into the next largest unit. Here is an example of the steps used:
-
-1. Split the text by a given level
-2. For each section, does it fit within the chunk size?
-   - Yes. Merge as many of these neighboring sections into a chunk as possible to maximize chunk length.
-   - No. Split by the next level and repeat.
-
-The boundaries used to split the text if using the top-level `chunks` method, in descending length:
-
-1. Descending sequence length of newlines. (Newline is `\r\n`, `\n`, or `\r`) Each unique length of consecutive newline sequences is treated as its own semantic level.
-2. [Unicode Sentence Boundaries](https://www.unicode.org/reports/tr29/#Sentence_Boundaries)
-3. [Unicode Word Boundaries](https://www.unicode.org/reports/tr29/#Word_Boundaries)
-4. [Unicode Grapheme Cluster Boundaries](https://www.unicode.org/reports/tr29/#Grapheme_Cluster_Boundaries)
-5. Characters
-
-Splitting doesn't occur below the character level, otherwise you could get partial bytes of a char, which may not be a valid unicode str.
-
-_Note on sentences:_ There are lots of methods of determining sentence breaks, all to varying degrees of accuracy, and many requiring ML models to do so. Rather than trying to find the perfect sentence breaks, we rely on unicode method of sentence boundaries, which in most cases is good enough for finding a decent semantic breaking point if a paragraph is too large, and avoids the performance penalties of many other methods.
-
-## Inspiration
-
-This crate was inspired by [LangChain's TextSplitter](https://python.langchain.com/en/latest/modules/indexes/text_splitters/examples/recursive_text_splitter.html). But, looking into the implementation, there was potential for better performance as well as better semantic chunking.
-
-A big thank you to the unicode-rs team for their [unicode-segmentation](https://crates.io/crates/unicode-segmentation) crate that manages a lot of the complexity of matching the Unicode rules for words and sentences.
-**/
-#[pymodule]
-fn semantic_text_splitter(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_class::<CharacterTextSplitter>()?;
-    Ok(())
-}
+class CharacterTextSplitter:
+    """Plain-text splitter. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
+
+    ### By Number of Characters
+
+    ```python
+    from semantic_text_splitter import CharacterTextSplitter
+
+    # Maximum number of characters in a chunk
+    max_characters = 1000
+    # Optionally can also have the splitter not trim whitespace for you
+    splitter = CharacterTextSplitter(trim_chunks=False)
+
+    chunks = splitter.chunks("your document text", max_characters)
+    ```
+
+    ### Using a Range for Chunk Capacity
+
+    You also have the option of specifying your chunk capacity as a range.
+
+    Once a chunk has reached a length that falls within the range it will be returned.
+
+    It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
+
+    ```python
+    from semantic_text_splitter import CharacterTextSplitter
+
+    # Optionally can also have the splitter trim whitespace for you
+    splitter = CharacterTextSplitter()
+
+    # Maximum number of characters in a chunk. Will fill up the
+    # chunk until it is somewhere in this range.
+    chunks = splitter.chunks("your document text", chunk_capacity=(200,1000))
+    ```
+
+    Args:
+        trim_chunks (bool, optional): Specify whether chunks should have whitespace trimmed from the
+            beginning and end or not. If False, joining all chunks will return the original
+            string. Defaults to True.
+    """
+
+    def __init__(self, trim_chunks: bool = True) -> None: ...
+    def chunks(
+        self, text: str, chunk_capacity: Union[int, Tuple[int, int]]
+    ) -> List[str]:
+        """Generate a list of chunks from a given text. Each chunk will be up to the `chunk_capacity`.
+
+        ## Method
+
+        To preserve as much semantic meaning within a chunk as possible, a recursive approach is used, starting at larger semantic units and, if that is too large, breaking it up into the next largest unit. Here is an example of the steps used:
+
+        1. Split the text by a given level
+        2. For each section, does it fit within the chunk size?
+        a. Yes. Merge as many of these neighboring sections into a chunk as possible to maximize chunk length.
+        b. No. Split by the next level and repeat.
+
+        The boundaries used to split the text if using the top-level `split` method, in descending length:
+
+        1. Descending sequence length of newlines. (Newline is `\r\n`, `\n`, or `\r`) Each unique length of consecutive newline sequences is treated as its own semantic level.
+        2. [Unicode Sentence Boundaries](https://www.unicode.org/reports/tr29/#Sentence_Boundaries)
+        3. [Unicode Word Boundaries](https://www.unicode.org/reports/tr29/#Word_Boundaries)
+        4. [Unicode Grapheme Cluster Boundaries](https://www.unicode.org/reports/tr29/#Grapheme_Cluster_Boundaries)
+        5. Characters
+
+        Splitting doesn't occur below the character level, otherwise you could get partial
+        bytes of a char, which may not be a valid unicode str.
+
+        Args:
+            text (str): Text to split.
+            chunk_capacity (int | (int, int)): The capacity of characters in each chunk. If a
+                single int, then chunks will be filled up as much as possible, without going over
+                that number. If a tuple of two integers is provided, a chunk will be considered
+                "full" once it is within the two numbers (inclusive range). So it will only fill
+                up the chunk until the lower range is met.
+
+        Returns:
+            A list of strings, one for each chunk. If `trim_chunks` was specified in the text
+            splitter, then each chunk will already be trimmed as well.
+        """
+
+class HuggingFaceTextSplitter:
+    """Text splitter based on a Hugging Face Tokenizer. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
+
+    ### By Number of Tokens
+
+    ```python
+    from semantic_text_splitter import HuggingFaceTextSplitter
+    from tokenizers import Tokenizer
+
+    # Maximum number of tokens in a chunk
+    max_characters = 1000
+    # Optionally can also have the splitter not trim whitespace for you
+    tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
+    splitter = HuggingFaceTextSplitter(tokenizer, trim_chunks=False)
+
+    chunks = splitter.chunks("your document text", max_characters)
+    ```
+
+    ### Using a Range for Chunk Capacity
+
+    You also have the option of specifying your chunk capacity as a range.
+
+    Once a chunk has reached a length that falls within the range it will be returned.
+
+    It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
+
+    ```python
+    from semantic_text_splitter import HuggingFaceTextSplitter
+    from tokenizers import Tokenizer
+
+    # Optionally can also have the splitter trim whitespace for you
+    tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
+    splitter = HuggingFaceTextSplitter(tokenizer)
+
+    # Maximum number of tokens in a chunk. Will fill up the
+    # chunk until it is somewhere in this range.
+    chunks = splitter.chunks("your document text", chunk_capacity=(200,1000))
+    ```
+
+    Args:
+        tokenizer (Tokenizer): A `tokenizers.Tokenizer` you want to use to count tokens for each
+            chunk.
+        trim_chunks (bool, optional): Specify whether chunks should have whitespace trimmed from the
+            beginning and end or not. If False, joining all chunks will return the original
+            string. Defaults to True.
+    """
+
+    def __init__(self, tokenizer, trim_chunks: bool = True) -> None: ...
+    @staticmethod
+    def from_str(json: str, trim_chunks: bool = True) -> HuggingFaceTextSplitter:
+        """Instantiate a new text splitter from the given Hugging Face Tokenizer JSON string.
+
+        Args:
+            json (str): A valid JSON string representing a previously serialized
+                Hugging Face Tokenizer
+
+        Returns:
+            The new text splitter
+        """
+    @staticmethod
+    def from_file(path: str, trim_chunks: bool = True) -> HuggingFaceTextSplitter:
+        """Instantiate a new text splitter from the Hugging Face tokenizer file at the given path.
+
+        Args:
+            path (str): A path to a local JSON file representing a previously serialized
+                Hugging Face tokenizer.
+
+        Returns:
+            The new text splitter
+        """
+    def chunks(
+        self, text: str, chunk_capacity: Union[int, Tuple[int, int]]
+    ) -> List[str]:
+        """Generate a list of chunks from a given text. Each chunk will be up to the `chunk_capacity`.
+
+        ## Method
+
+        To preserve as much semantic meaning within a chunk as possible, a recursive approach is used, starting at larger semantic units and, if that is too large, breaking it up into the next largest unit. Here is an example of the steps used:
+
+        1. Split the text by a given level
+        2. For each section, does it fit within the chunk size?
+        a. Yes. Merge as many of these neighboring sections into a chunk as possible to maximize chunk length.
+        b. No. Split by the next level and repeat.
+
+        The boundaries used to split the text if using the top-level `split` method, in descending length:
+
+        1. Descending sequence length of newlines. (Newline is `\r\n`, `\n`, or `\r`) Each unique length of consecutive newline sequences is treated as its own semantic level.
+        2. [Unicode Sentence Boundaries](https://www.unicode.org/reports/tr29/#Sentence_Boundaries)
+        3. [Unicode Word Boundaries](https://www.unicode.org/reports/tr29/#Word_Boundaries)
+        4. [Unicode Grapheme Cluster Boundaries](https://www.unicode.org/reports/tr29/#Grapheme_Cluster_Boundaries)
+        5. Characters
+
+        Splitting doesn't occur below the character level, otherwise you could get partial
+        bytes of a char, which may not be a valid unicode str.
+
+        Args:
+            text (str): Text to split.
+            chunk_capacity (int | (int, int)): The capacity of characters in each chunk. If a
+                single int, then chunks will be filled up as much as possible, without going over
+                that number. If a tuple of two integers is provided, a chunk will be considered
+                "full" once it is within the two numbers (inclusive range). So it will only fill
+                up the chunk until the lower range is met.
+
+        Returns:
+            A list of strings, one for each chunk. If `trim_chunks` was specified in the text
+            splitter, then each chunk will already be trimmed as well.
+        """
```

### Comparing `semantic_text_splitter-0.1.4/PKG-INFO` & `semantic_text_splitter-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: semantic-text-splitter
-Version: 0.1.4
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: black ; extra == 'test'
+Requires-Dist: tokenizers ; extra == 'test'
 Requires-Dist: pdoc ; extra == 'docs'
 Provides-Extra: test
 Provides-Extra: docs
 Summary: Split text into semantic chunks, up to a desired chunk size. Supports calculating length by characters and tokens (when used with large language models).
 Keywords: text,split,tokenizer,nlp,ai
 Author: Ben Brandt <benjamin.j.brandt@gmail.com>
 Author-email: Ben Brandt <benjamin.j.brandt@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/benbrandt/text-splitter
 
-# text-splitter
+# semantic-text-splitter
 
-[![Documentation Status](https://readthedocs.org/projects/text-splitter/badge/?version=latest)](https://text-splitter.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
+[![Documentation Status](https://readthedocs.org/projects/semantic-text-splitter/badge/?version=stable)](https://semantic-text-splitter.readthedocs.io/en/stable/?badge=stable) [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
 
 Large language models (LLMs) can be used for many tasks, but often have a limited context size that can be smaller than documents you might want to use. To use documents of larger length, you often have to split your text into chunks to fit within this context size.
 
 This crate provides methods for splitting longer pieces of text into smaller chunks, aiming to maximize a desired chunk size, but still splitting at semantically sensible boundaries whenever possible.
 
 ## Get Started
 
 ### By Number of Characters
 
 ```python
 from semantic_text_splitter import CharacterTextSplitter
 
 # Maximum number of characters in a chunk
 max_characters = 1000
-# Optionally can also have the splitter trim whitespace for you
-splitter = CharacterTextSplitter(trim_chunks=True)
+# Optionally can also have the splitter not trim whitespace for you
+splitter = CharacterTextSplitter(trim_chunks=False)
 
 chunks = splitter.chunks("your document text", max_characters)
 ```
 
 ### Using a Range for Chunk Capacity
 
 You also have the option of specifying your chunk capacity as a range.
```

