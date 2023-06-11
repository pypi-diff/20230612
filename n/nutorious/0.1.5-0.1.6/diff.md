# Comparing `tmp/nutorious-0.1.5.tar.gz` & `tmp/nutorious-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutorious-0.1.5.tar", max compression
+gzip compressed data, was "nutorious-0.1.6.tar", max compression
```

## Comparing `nutorious-0.1.5.tar` & `nutorious-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      171 2023-06-11 07:38:28.878531 nutorious-0.1.5/README.md
--rw-r--r--   0        0        0      827 2023-06-11 07:38:28.878531 nutorious-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1173 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/__init__.py
--rw-r--r--   0        0        0      754 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/cli/__init__.py
--rw-r--r--   0        0        0     1187 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/config/__init__.py
--rw-r--r--   0        0        0      376 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/config/default.yml
--rw-r--r--   0        0        0      204 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/context/__init__.py
--rw-r--r--   0        0        0     4436 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/journal/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/report/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/report/base.py
--rw-r--r--   0        0        0     2556 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/report/daily.py
--rw-r--r--   0        0        0        0 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/report/diff.py
--rw-r--r--   0        0        0     1094 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/ui/__init__.py
--rw-r--r--   0        0        0      503 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/ui/ui.py
--rw-r--r--   0        0        0      337 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/utils/collections.py
--rw-r--r--   0        0        0      197 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/utils/commons.py
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 nutorious-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-11 23:51:12.140631 nutorious-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6706 2023-06-11 23:51:12.140631 nutorious-0.1.6/README.md
+-rw-r--r--   0        0        0      879 2023-06-11 23:51:12.144631 nutorious-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1558 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/__init__.py
+-rw-r--r--   0        0        0      770 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/cli/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/config/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/config/default.yml
+-rw-r--r--   0        0        0      203 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/context/__init__.py
+-rw-r--r--   0        0        0     4430 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/journal/__init__.py
+-rw-r--r--   0        0        0     1994 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/report/__init__.py
+-rw-r--r--   0        0        0     1475 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/report/base.py
+-rw-r--r--   0        0        0     2555 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/report/daily.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/report/diff.py
+-rw-r--r--   0        0        0     1094 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/ui/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/utils/collections.py
+-rw-r--r--   0        0        0      570 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/utils/commons.py
+-rw-r--r--   0        0        0     7484 1970-01-01 00:00:00.000000 nutorious-0.1.6/PKG-INFO
```

### Comparing `nutorious-0.1.5/src/nutorious/__init__.py` & `nutorious-0.1.6/src/nutorious/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,57 @@
+import sys
 from datetime import datetime
 
 import click
-
+from cattrs import transform_error
+from cattrs.errors import BaseValidationError
 from nutorious.cli import option_date, option_journal_path, option_watch
 from nutorious.report.daily import DailyReportOptions, display_daily_report
+from nutorious.utils.commons import mkstring
 
 
 @click.group()
-def main():
+def nutorious_cli():
     pass
 
 
-@main.command()
+@nutorious_cli.command()
 @option_journal_path()
 @option_date("--date", "--d", help="Date of the report. Default is 'today'.")
 @option_watch()
 def report(journal_path, date, watch):
     """
     Shows report on a date, closest to specified date.
     """
 
     date = datetime.today().date() if date is None else date.date()
 
     display_daily_report(DailyReportOptions(journal_path, watch, date))
 
 
-@main.command()
+@nutorious_cli.command()
 @option_journal_path()
 @option_date("--date1", "--d1", help="Date1 of the diff report. Default: yesterday.")
 @option_date("--date2", "--d2", help="Date2 of the diff report. Default: today.")
 @option_watch()
 def diff(journal_path, date1, date2, watch):
     """Shows difference report between two dates"""
 
     click.echo(f"Diff report:")
     click.echo(f"  Journal: {journal_path}")
     click.echo(f"    Date1: {date1}")
     click.echo(f"    Date2: {date2}")
     click.echo(f"    Watch: {watch}")
 
 
+def main():
+    try:
+        nutorious_cli.main()
+    except BaseValidationError as e:
+        errors = mkstring(transform_error(e), sep="\n")
+        sys.exit(errors)
+    except Exception as e:
+        sys.exit(str(e))
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `nutorious-0.1.5/src/nutorious/config/__init__.py` & `nutorious-0.1.6/src/nutorious/config/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from importlib.resources import files
 from pathlib import Path
 
 import cattrs
 import yaml
 from attrs import define, field
-
 from nutorious.utils.collections import merge_dicts
+from nutorious.utils.commons import load_yaml_data
 
 
 @define
 class Config:
     meals: list[str]
     ui: UiConfig
 
@@ -47,12 +47,12 @@
 
 def load_config(journal_path: str) -> Config:
     default_config_text = (files("nutorious.config") / "default.yml").read_text("UTF-8")
     config_data = yaml.safe_load(default_config_text)
 
     journal_config_path = Path(journal_path) / "config.yml"
     if journal_config_path.exists():
-        journal_config_data = yaml.safe_load(journal_config_path.read_text("UTF-8"))
+        journal_config_data = load_yaml_data(journal_config_path)
         config_data = merge_dicts(config_data, journal_config_data)
 
     config = cattrs.structure(config_data, Config)
     return config
```

### Comparing `nutorious-0.1.5/src/nutorious/journal/__init__.py` & `nutorious-0.1.6/src/nutorious/journal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import re
 from datetime import date
 from datetime import datetime
 from pathlib import Path
 
 import cattrs
-import yaml
 from attrs import Factory, define
-from pydash import py_
-
 from nutorious.config import Config
 from nutorious.model import Journal, Day, Food, Meal
+from nutorious.utils.commons import load_yaml_data
+from pydash import py_
 
 ItemData = list[str]
 DayData = dict[str, ItemData]
 Data = dict[date, DayData]
 
 weight_spec_pattern = re.compile(r"^(\d+(?:\.\d+)?)g$")
 count_spec_pattern = re.compile(r"^(\d+(?:\.\d+)?)x$")
@@ -49,17 +48,16 @@
     journal_config_path = Path(journal_path) / "config.yml"
 
     data_file_paths = Path(journal_path).glob("**/*.yml")
 
     data_raw = {}
     for data_file_path in data_file_paths:
         if data_file_path != journal_config_path:
-            with open(data_file_path, "r") as f:
-                file_data = yaml.safe_load(f)
-                data_raw = data_raw | file_data
+            file_data = load_yaml_data(data_file_path)
+            data_raw = data_raw | file_data
 
     return cattrs.structure(data_raw, Data)
 
 
 def __build_journal(data: Data, meal_names: list[str]) -> Journal:
     sorted_by_dt = sorted(data.items())
```

### Comparing `nutorious-0.1.5/src/nutorious/model/__init__.py` & `nutorious-0.1.6/src/nutorious/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.5/src/nutorious/report/base.py` & `nutorious-0.1.6/src/nutorious/report/base.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.5/src/nutorious/report/daily.py` & `nutorious-0.1.6/src/nutorious/report/daily.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from datetime import date
 
 from attrs import define
-from pydash import py_
-from rich import box
-from rich.table import Table
-
 from nutorious.config import ColumnConfig, Config
 from nutorious.context import Context
 from nutorious.model import Day, Meal, Food
 from nutorious.report.base import BaseOptions, display_report
 from nutorious.ui import create_tree_row
+from pydash import py_
+from rich import box
+from rich.table import Table
 
 
 @define
 class DailyReportOptions(BaseOptions):
     dt: date
```

### Comparing `nutorious-0.1.5/src/nutorious/ui/__init__.py` & `nutorious-0.1.6/src/nutorious/ui/__init__.py`

 * *Files identical despite different names*

