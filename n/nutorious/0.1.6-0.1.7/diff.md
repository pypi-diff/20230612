# Comparing `tmp/nutorious-0.1.6.tar.gz` & `tmp/nutorious-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutorious-0.1.6.tar", max compression
+gzip compressed data, was "nutorious-0.1.7.tar", max compression
```

## Comparing `nutorious-0.1.6.tar` & `nutorious-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-06-11 23:51:12.140631 nutorious-0.1.6/LICENSE
--rw-r--r--   0        0        0     6706 2023-06-11 23:51:12.140631 nutorious-0.1.6/README.md
--rw-r--r--   0        0        0      879 2023-06-11 23:51:12.144631 nutorious-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1558 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/__init__.py
--rw-r--r--   0        0        0      770 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/cli/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/config/__init__.py
--rw-r--r--   0        0        0      376 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/config/default.yml
--rw-r--r--   0        0        0      203 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/context/__init__.py
--rw-r--r--   0        0        0     4430 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/journal/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/report/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/report/base.py
--rw-r--r--   0        0        0     2555 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/report/daily.py
--rw-r--r--   0        0        0        0 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/report/diff.py
--rw-r--r--   0        0        0     1094 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/ui/__init__.py
--rw-r--r--   0        0        0      336 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/utils/collections.py
--rw-r--r--   0        0        0      570 2023-06-11 23:51:12.144631 nutorious-0.1.6/src/nutorious/utils/commons.py
--rw-r--r--   0        0        0     7484 1970-01-01 00:00:00.000000 nutorious-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 00:02:39.371817 nutorious-0.1.7/LICENSE
+-rw-r--r--   0        0        0     6727 2023-06-12 00:02:39.371817 nutorious-0.1.7/README.md
+-rw-r--r--   0        0        0      879 2023-06-12 00:02:39.375817 nutorious-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1558 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/__init__.py
+-rw-r--r--   0        0        0      770 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/cli/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/config/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/config/default.yml
+-rw-r--r--   0        0        0      203 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/context/__init__.py
+-rw-r--r--   0        0        0     4430 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/journal/__init__.py
+-rw-r--r--   0        0        0     1994 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/report/__init__.py
+-rw-r--r--   0        0        0     1475 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/report/base.py
+-rw-r--r--   0        0        0     2555 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/report/daily.py
+-rw-r--r--   0        0        0        0 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/report/diff.py
+-rw-r--r--   0        0        0     1094 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/ui/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/utils/collections.py
+-rw-r--r--   0        0        0      570 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/utils/commons.py
+-rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 nutorious-0.1.7/PKG-INFO
```

### Comparing `nutorious-0.1.6/LICENSE` & `nutorious-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/README.md` & `nutorious-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Nutorious
 =========
 
-Nutorious is a command-line tool to track your nutrition. This includes the usual kcal, protein, carbs, fats, but also any other ingredient of your choosing, i.e. sugar, salt, etc. I was inspired by the https://plaintextaccounting.org/, when at some point I wanted to start counting calories and realized that none of the phone apps are flexible/easy-to-use enough for my needs, especially after trying plaintext for accouting. Another inspiration came from [Calorific](https://github.com/peterkeen/calorific) to use simple yaml format for the journal files. The Calorific is a great tool, but I wanted a bit better UX.
+Nutorious is a command-line tool to track your nutrition in plaintext files. This includes the usual kcal, protein, carbs, fats, but also any other ingredient of your choosing, i.e. sugar, salt, etc. I was inspired by the https://plaintextaccounting.org/, when at some point I wanted to start counting calories and realized that none of the phone apps are flexible/easy-to-use enough for my needs, especially after trying plaintext for accouting. Another inspiration came from [Calorific](https://github.com/peterkeen/calorific) to use simple yaml format for the journal files. The Calorific is a great tool, but I wanted a bit better UX.
 
 
 ### Installation
 Nutorious is available in PyPI, so it can be installed the usual way using the `pip` command:
 ```bash
 pip install --upgrade nutorious
 ```
@@ -109,15 +109,15 @@
     - 200 pepper
     - 20 oil
     - 2x
 ```
 
 #### Food registry
 After the food is defined it can be referenced on current or any future dates. 
-```yml
+```yaml
 2023-03-03:
   egg-rice:
     - 200 rice
     - 3 eggs
     - 600g # gets bigger after preparation
   lunch:
     - 200 egg-rice
@@ -128,15 +128,15 @@
 
 2023-03-05:
   lunch:
     - 200 egg-rice # more leftovers
 ```
 
 If the food is redefined, all future references will use this new version. The idea is that usually you have just one "bread" in your kitchen, but it can have different contents. So once the old one is finished and you bought the new one, you just add it with the same name "bread".
-```yml
+```yaml
 2023-03-03:
   bread: [ 200 kcal, 7.6 prot, 42.7 carb, 9 fat ]
   breakfast:
     - 50 bread # 100 kcal 
 
 2023-03-04:
   breakfast:
```

### Comparing `nutorious-0.1.6/pyproject.toml` & `nutorious-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nutorious"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Dzmitry Paulenka"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dzmitry-paulenka/nutorious"
 
 [tool.poetry.dependencies]
```

### Comparing `nutorious-0.1.6/src/nutorious/__init__.py` & `nutorious-0.1.7/src/nutorious/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/src/nutorious/cli/__init__.py` & `nutorious-0.1.7/src/nutorious/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/src/nutorious/config/__init__.py` & `nutorious-0.1.7/src/nutorious/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/src/nutorious/journal/__init__.py` & `nutorious-0.1.7/src/nutorious/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/src/nutorious/model/__init__.py` & `nutorious-0.1.7/src/nutorious/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/src/nutorious/report/base.py` & `nutorious-0.1.7/src/nutorious/report/base.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/src/nutorious/report/daily.py` & `nutorious-0.1.7/src/nutorious/report/daily.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/src/nutorious/ui/__init__.py` & `nutorious-0.1.7/src/nutorious/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/src/nutorious/utils/commons.py` & `nutorious-0.1.7/src/nutorious/utils/commons.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.6/PKG-INFO` & `nutorious-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutorious
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/dzmitry-paulenka/nutorious
 License: MIT
 Author: Dzmitry Paulenka
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
 Project-URL: Repository, https://github.com/dzmitry-paulenka/nutorious
 Description-Content-Type: text/markdown
 
 Nutorious
 =========
 
-Nutorious is a command-line tool to track your nutrition. This includes the usual kcal, protein, carbs, fats, but also any other ingredient of your choosing, i.e. sugar, salt, etc. I was inspired by the https://plaintextaccounting.org/, when at some point I wanted to start counting calories and realized that none of the phone apps are flexible/easy-to-use enough for my needs, especially after trying plaintext for accouting. Another inspiration came from [Calorific](https://github.com/peterkeen/calorific) to use simple yaml format for the journal files. The Calorific is a great tool, but I wanted a bit better UX.
+Nutorious is a command-line tool to track your nutrition in plaintext files. This includes the usual kcal, protein, carbs, fats, but also any other ingredient of your choosing, i.e. sugar, salt, etc. I was inspired by the https://plaintextaccounting.org/, when at some point I wanted to start counting calories and realized that none of the phone apps are flexible/easy-to-use enough for my needs, especially after trying plaintext for accouting. Another inspiration came from [Calorific](https://github.com/peterkeen/calorific) to use simple yaml format for the journal files. The Calorific is a great tool, but I wanted a bit better UX.
 
 
 ### Installation
 Nutorious is available in PyPI, so it can be installed the usual way using the `pip` command:
 ```bash
 pip install --upgrade nutorious
 ```
@@ -131,15 +131,15 @@
     - 200 pepper
     - 20 oil
     - 2x
 ```
 
 #### Food registry
 After the food is defined it can be referenced on current or any future dates. 
-```yml
+```yaml
 2023-03-03:
   egg-rice:
     - 200 rice
     - 3 eggs
     - 600g # gets bigger after preparation
   lunch:
     - 200 egg-rice
@@ -150,15 +150,15 @@
 
 2023-03-05:
   lunch:
     - 200 egg-rice # more leftovers
 ```
 
 If the food is redefined, all future references will use this new version. The idea is that usually you have just one "bread" in your kitchen, but it can have different contents. So once the old one is finished and you bought the new one, you just add it with the same name "bread".
-```yml
+```yaml
 2023-03-03:
   bread: [ 200 kcal, 7.6 prot, 42.7 carb, 9 fat ]
   breakfast:
     - 50 bread # 100 kcal 
 
 2023-03-04:
   breakfast:
```

