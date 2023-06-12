# Comparing `tmp/puan_pv_rs-0.1.3.tar.gz` & `tmp/puan_pv_rs-0.1.4.tar.gz`

## Comparing `puan_pv_rs-0.1.3.tar` & `puan_pv_rs-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 puan_pv_rs-0.1.3/Cargo.toml
--rw-r--r--   0     1001      123     1500 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/.gitignore
--rw-r--r--   0     1001      123      359 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/pyproject.toml
--rwxr-xr-x   0     1001      123      833 2023-06-09 06:39:06.000000 puan_pv_rs-0.1.3/run-maturin-action.sh
--rw-r--r--   0     1001      123     9065 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/src/lib.rs
--rw-r--r--   0     1001      123     7654 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 puan_pv_rs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 puan_pv_rs-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      123     1500 2023-06-12 14:39:30.000000 puan_pv_rs-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-12 14:39:30.000000 puan_pv_rs-0.1.4/.gitignore
+-rw-r--r--   0     1001      123      359 2023-06-12 14:39:30.000000 puan_pv_rs-0.1.4/pyproject.toml
+-rwxr-xr-x   0     1001      123      833 2023-06-12 14:40:01.000000 puan_pv_rs-0.1.4/run-maturin-action.sh
+-rw-r--r--   0     1001      123    10550 2023-06-12 14:39:30.000000 puan_pv_rs-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      123     7654 2023-06-12 14:39:30.000000 puan_pv_rs-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 puan_pv_rs-0.1.4/PKG-INFO
```

### Comparing `puan_pv_rs-0.1.3/.github/workflows/CI.yml` & `puan_pv_rs-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `puan_pv_rs-0.1.3/.gitignore` & `puan_pv_rs-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `puan_pv_rs-0.1.3/run-maturin-action.sh` & `puan_pv_rs-0.1.4/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `puan_pv_rs-0.1.3/src/lib.rs` & `puan_pv_rs-0.1.4/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -139,24 +139,37 @@
     pub fn new(composite_operands: Vec<Disjunction>, single_operands: Vec<String>) -> Self {
         Self {
             composite_operands,
             single_operands,
         }
     }
 
+    pub fn _variables(&self) -> Vec<String> {
+        let mut variables = self.single_operands.clone();
+        for operand in self.composite_operands.clone() {
+            variables.extend(operand.variables);
+        }
+        variables
+    }
+
     #[getter]
     pub fn composite_operands(&self) -> PyResult<Vec<Disjunction>> {
         Ok(self.composite_operands.clone())
     }
 
     #[getter]
     pub fn single_operands(&self) -> PyResult<Vec<String>> {
         Ok(self.single_operands.clone())
     }
 
+    #[getter]
+    pub fn variables(&self) -> PyResult<Vec<String>> {
+        return Ok(self._variables())
+    }
+
     pub fn hash(&self) -> u64 {
         hashit(self)
     }
 
     pub fn evaluate(&self, interpretation: Vec<String>) -> bool {
         self.single_operands.iter().all(|operand| interpretation.contains(operand)) &&
         self.composite_operands.iter().all(|operand| operand.evaluate(interpretation.clone()))
@@ -177,14 +190,27 @@
     pub fn new(composite_operands: Vec<Conjunction>, single_operands: Vec<String>) -> Self {
         Self {
             composite_operands,
             single_operands,
         }
     }
 
+    pub fn _variables(&self) -> Vec<String> {
+        let mut variables = self.single_operands.clone();
+        for operand in self.composite_operands.clone() {
+            variables.extend(operand.variables);
+        }
+        variables
+    }
+
+    #[getter]
+    pub fn variables(&self) -> PyResult<Vec<String>> {
+        return Ok(self._variables())
+    }
+
     #[getter]
     pub fn composite_operands(&self) -> PyResult<Vec<Conjunction>> {
         Ok(self.composite_operands.clone())
     }
 
     #[getter]
     pub fn single_operands(&self) -> PyResult<Vec<String>> {
@@ -216,14 +242,19 @@
         Self {
             conjuctive_compositions,
             keys,
         }
     }
 
     #[getter]
+    pub fn variables(&self) -> PyResult<Vec<String>> {
+        Ok(self.conjuctive_compositions._variables())
+    }
+
+    #[getter]
     pub fn conjunctive_compositions(&self) -> PyResult<ConjunctiveComposition> {
         Ok(self.conjuctive_compositions.clone())
     }
 
     #[getter]
     pub fn keys(&self) -> PyResult<Vec<String>> {
         Ok(self.keys.clone())
@@ -256,14 +287,19 @@
         Self {
             disjunctive_compositions,
             keys,
         }
     }
 
     #[getter]
+    pub fn variables(&self) -> PyResult<Vec<String>> {
+        Ok(self.disjunctive_compositions._variables())
+    }
+
+    #[getter]
     pub fn disjunctive_compositions(&self) -> PyResult<DisjunctiveComposition> {
         Ok(self.disjunctive_compositions.clone())
     }
 
     #[getter]
     pub fn keys(&self) -> PyResult<Vec<String>> {
         Ok(self.keys.clone())
@@ -302,18 +338,23 @@
         Ok(self.conjunctive_composition_string_values.clone())
     }
 
     pub fn hash(&self) -> u64 {
         hashit(self)
     }
 
-    pub fn evaluate(&self, interpretation: Vec<String>) -> Vec<Vec<String>> {
+    pub fn evaluate(&self, interpretation: Vec<String>) -> Vec<ConjunctiveCompositionKeys> {
         self.conjunctive_composition_string_values
             .iter()
-            .filter_map(|ccsv| ccsv.evaluate(interpretation.clone()))
+            .filter_map(|conjunctive_composition_string_value| {
+                match conjunctive_composition_string_value.evaluate(interpretation.clone()) {
+                    Some(_) => Some(conjunctive_composition_string_value.clone()),
+                    None => None,
+                }
+            })
             .collect()
     }
 }
 
 #[pyclass]
 #[derive(Clone, Hash)]
 pub struct DCKeysIterable {
@@ -335,18 +376,23 @@
         Ok(self.disjunctive_composition_string_values.clone())
     }
 
     pub fn hash(&self) -> u64 {
         hashit(self)
     }
 
-    pub fn evaluate(&self, interpretation: Vec<String>) -> Vec<Vec<String>> {
+    pub fn evaluate(&self, interpretation: Vec<String>) -> Vec<DisjunctiveCompositionKeys> {
         self.disjunctive_composition_string_values
             .iter()
-            .filter_map(|dcsv| dcsv.evaluate(interpretation.clone()))
+            .filter_map(|disjunctive_composition_string_value| {
+                match disjunctive_composition_string_value.evaluate(interpretation.clone()) {
+                    Some(_) => Some(disjunctive_composition_string_value.clone()),
+                    None => None,
+                }
+            })
             .collect()
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn puan_pv_rs(_py: Python, m: &PyModule) -> PyResult<()> {
```

### Comparing `puan_pv_rs-0.1.3/Cargo.lock` & `puan_pv_rs-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "puan-pv-rs"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
```

