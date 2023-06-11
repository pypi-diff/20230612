# Comparing `tmp/contact_magic-0.3.6.tar.gz` & `tmp/contact_magic-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.3.6.tar", max compression
+gzip compressed data, was "contact_magic-0.3.7.tar", max compression
```

## Comparing `contact_magic-0.3.6.tar` & `contact_magic-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.6/README.md
--rw-r--r--   0        0        0      273 2023-06-11 11:14:26.606174 contact_magic-0.3.6/contact_magic/__init__.py
--rw-r--r--   0        0        0      977 2023-06-11 21:37:40.893254 contact_magic-0.3.6/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.6/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5201 2023-06-11 11:20:08.656242 contact_magic-0.3.6/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-11 11:09:58.728061 contact_magic-0.3.6/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.6/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2177 2023-06-11 12:02:22.673968 contact_magic-0.3.6/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.3.6/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.6/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.6/contact_magic/logger.py
--rw-r--r--   0        0        0    12256 2023-06-11 21:37:24.907383 contact_magic-0.3.6/contact_magic/models.py
--rw-r--r--   0        0        0     3047 2023-06-11 21:07:35.643112 contact_magic-0.3.6/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.6/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.6/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.6/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.6/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.6/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.6/contact_magic/utils.py
--rw-r--r--   0        0        0     1710 2023-06-11 21:37:24.903591 contact_magic-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.7/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.3.7/contact_magic/__init__.py
+-rw-r--r--   0        0        0      977 2023-06-11 22:24:14.818768 contact_magic-0.3.7/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.7/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5201 2023-06-11 11:20:08.656242 contact_magic-0.3.7/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-11 22:03:43.467264 contact_magic-0.3.7/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.7/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2177 2023-06-11 12:02:22.673968 contact_magic-0.3.7/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.3.7/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.7/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.7/contact_magic/logger.py
+-rw-r--r--   0        0        0    12289 2023-06-11 22:22:02.798555 contact_magic-0.3.7/contact_magic/models.py
+-rw-r--r--   0        0        0     3080 2023-06-11 22:22:02.791793 contact_magic-0.3.7/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.7/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.7/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.7/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.7/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.7/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.7/contact_magic/utils.py
+-rw-r--r--   0        0        0     1710 2023-06-11 21:59:48.589016 contact_magic-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.7/PKG-INFO
```

### Comparing `contact_magic-0.3.6/README.md` & `contact_magic-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/asyncio.py` & `contact_magic-0.3.7/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/conf/settings.py` & `contact_magic-0.3.7/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/helpers.py` & `contact_magic-0.3.7/contact_magic/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,35 +45,35 @@
         data=settings_data[1:], columns=settings_data[0]
     ).replace("", np.nan)
 
     for i in range(0, len(df_settings_data.columns), 2):
         scraper_col_values = list(df_settings_data.iloc[:, i].values)
         if not scraper_col_values:
             continue
-        new_entry = {"col_name": df_settings_data.columns[i], "allowed_scrapers": []}
+        new_entry = {"col_name": df_settings_data.columns[i], "sentence_wizards": []}
         scrapers_seen = set()
         for position, scraper in enumerate(scraper_col_values):
             if (
                 scraper not in SETTINGS.ALLOWED_SCRAPER_NAMES
                 or scraper in scrapers_seen
             ):
                 continue
             premise_url = df_settings_data.iloc[position, i + 1]
             if pd.isnull(premise_url):
                 continue
             if scraper == "FALLBACK":
-                new_entry["allowed_scrapers"].append(
+                new_entry["sentence_wizards"].append(
                     {"scraper_name": scraper, "fallback_template": premise_url}
                 )
             else:
-                new_entry["allowed_scrapers"].append(
+                new_entry["sentence_wizards"].append(
                     {"scraper_name": scraper, "premise_url": premise_url}
                 )
             scrapers_seen.add(scraper)
-        if new_entry.get("allowed_scrapers"):
+        if new_entry.get("sentence_wizards"):
             settings.append(new_entry)
     return PersonalizationSettings(datapoints=settings)
 
 
 def worksheet_to_dataframe(
     main_workflow_sheet: gspread.Spreadsheet, tab_name="WorkingSheet"
 ) -> pd.DataFrame:
```

### Comparing `contact_magic-0.3.6/contact_magic/integrations/copyfactory.py` & `contact_magic-0.3.7/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.3.7/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/integrations/sheets.py` & `contact_magic-0.3.7/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/models.py` & `contact_magic-0.3.7/contact_magic/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     @property
     def convert_to_original(self):
         return (
             pd.Series(data=self.data) if self._original_type == pd.Series else self.data
         )
 
 
-class Scraper(BaseModel):
+class SentenceWizard(BaseModel):
     """
     A reference to a scraper endpoint in SalesScrapers and a Copyfactory premiseURL.
     """
 
     scraper_name: str | None = Field(
         description="This is the endpoint from sales-scrapers", example="get-case-study"
     )
@@ -191,15 +191,15 @@
         for key, processor in self.field_processors.items():
             item = find_item(row.data, key)
             if item is not None:
                 if validation_model := processors.get(
                     processor.get("type", None), None
                 ):
                     value, is_value_valid = validation_model(
-                        processor=processor, value=item, scraper=self
+                        processor=processor, value=item, scraper=self, row_data=row.data
                     ).process()
                     if is_value_valid is False:
                         return row, False
                     row.data = replace_values(row.data, {key: value})
         return row, True
 
     async def execute(
@@ -235,22 +235,22 @@
     targeting a column and a list of allowed scrapers.
     """
 
     col_name: str = Field(
         description="The column name you want for the datapoint.",
         example="Personalization1",
     )
-    allowed_scrapers: list[Scraper]
+    sentence_wizards: list[SentenceWizard]
 
     @property
     def get_col_name_as_source(self) -> str:
         return f"source__{self.col_name}"
 
     async def build_datapoint(self, row: DataRow):
-        for scraper in self.allowed_scrapers:
+        for scraper in self.sentence_wizards:
             logger.info(
                 "processing_row",
                 row_number=row.index + 2,
                 scraper_name=scraper.scraper_name,
                 column_name=self.col_name,
                 status="STARTING",
             )
```

### Comparing `contact_magic-0.3.6/contact_magic/preprocessors.py` & `contact_magic-0.3.7/contact_magic/preprocessors.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from abc import abstractmethod
 from typing import Any
 
 from pydantic import BaseModel
 from pydantic.fields import ModelField
 from pydantic.main import validate_model
 
-from contact_magic import Scraper
+from contact_magic import SentenceWizard
 
 
 class BaseProcessor(BaseModel):
     """
     Base validator to inherit from. Define the 'validate' method to return a boolean.
     """
 
     value: Any = None
     processor: dict
-    scraper: Scraper
+    scraper: SentenceWizard
+    row_data: dict
 
     _is_valid: bool = True
 
     def process(self) -> tuple[Any, bool]:
         if not self._is_valid:
             return self.value, self._is_valid
         return self.validate(**self.processor)
```

### Comparing `contact_magic-0.3.6/contact_magic/scripts/agency.py` & `contact_magic-0.3.7/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/scripts/run_workflows.py` & `contact_magic-0.3.7/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.3.7/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/contact_magic/utils.py` & `contact_magic-0.3.7/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.6/pyproject.toml` & `contact_magic-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.3.6"
+version = "0.3.7"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.3.6/PKG-INFO` & `contact_magic-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.3.6
+Version: 0.3.7
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

