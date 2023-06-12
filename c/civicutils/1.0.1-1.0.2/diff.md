# Comparing `tmp/civicutils-1.0.1.tar.gz` & `tmp/civicutils-1.0.2.tar.gz`

## Comparing `civicutils-1.0.1.tar` & `civicutils-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 civicutils-1.0.1/info_on_matching_framework.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/__init__.py
--rw-r--r--   0        0        0    40439 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/filtering.py
--rw-r--r--   0        0        0   111701 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/match.py
--rw-r--r--   0        0        0    16931 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/query.py
--rw-r--r--   0        0        0    33562 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/read_and_write.py
--rw-r--r--   0        0        0    20645 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/utils.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/data/data.yml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/data/example_cnv.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/data/example_expr.txt
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/data/example_snv.txt
--rw-r--r--   0        0        0    82463 2020-02-02 00:00:00.000000 civicutils-1.0.1/dist_backup/civicutils-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   439302 2020-02-02 00:00:00.000000 civicutils-1.0.1/dist_backup/civicutils-1.0.0.tar.gz
--rw-r--r--   0        0        0   396868 2020-02-02 00:00:00.000000 civicutils-1.0.1/images/civicutils-workflow.png
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/.DS_Store
--rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/data/civic_available_diseases_31052023.txt
--rw-r--r--   0        0        0    36985 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/scripts/Query_CIViCutils.py
--rw-r--r--   0        0        0    78674 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/scripts/civicutils_manuscript_figures.R
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/scripts/get_available_diseases_in_civic.py
--rw-r--r--   0        0        0   128034 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/scripts/process_civic_predictions.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 civicutils-1.0.1/LICENSE.md
--rw-r--r--   0        0        0    45370 2020-02-02 00:00:00.000000 civicutils-1.0.1/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 civicutils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    86899 2020-02-02 00:00:00.000000 civicutils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 civicutils-1.0.2/info_on_matching_framework.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/__init__.py
+-rw-r--r--   0        0        0    40439 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/filtering.py
+-rw-r--r--   0        0        0   111723 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/match.py
+-rw-r--r--   0        0        0    16931 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/query.py
+-rw-r--r--   0        0        0    33562 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/read_and_write.py
+-rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/utils.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/data/data.yml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/data/example_cnv.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/data/example_expr.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/data/example_snv.txt
+-rw-r--r--   0        0        0    82485 2020-02-02 00:00:00.000000 civicutils-1.0.2/dist_backup/civicutils-1.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0   961403 2020-02-02 00:00:00.000000 civicutils-1.0.2/dist_backup/civicutils-1.0.1.tar.gz
+-rw-r--r--   0        0        0    82463 2020-02-02 00:00:00.000000 civicutils-1.0.2/dist_backup_2/civicutils-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   439302 2020-02-02 00:00:00.000000 civicutils-1.0.2/dist_backup_2/civicutils-1.0.0.tar.gz
+-rw-r--r--   0        0        0   396868 2020-02-02 00:00:00.000000 civicutils-1.0.2/images/civicutils-workflow.png
+-rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/data/civic_available_diseases_31052023.txt
+-rw-r--r--   0        0        0    36985 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/scripts/Query_CIViCutils.py
+-rw-r--r--   0        0        0    78674 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/scripts/civicutils_manuscript_figures.R
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/scripts/get_available_diseases_in_civic.py
+-rw-r--r--   0        0        0   128034 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/scripts/process_civic_predictions.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 civicutils-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0    45370 2020-02-02 00:00:00.000000 civicutils-1.0.2/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 civicutils-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    86899 2020-02-02 00:00:00.000000 civicutils-1.0.2/PKG-INFO
```

### Comparing `civicutils-1.0.1/info_on_matching_framework.md` & `civicutils-1.0.2/info_on_matching_framework.md`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/civicutils/filtering.py` & `civicutils-1.0.2/civicutils/filtering.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/civicutils/match.py` & `civicutils-1.0.2/civicutils/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,15 +829,15 @@
     select_tier = check_tier_selection(select_tier, sorted_tiers)
 
     match_map = {}
     matched_ids = []     # keep track of all matched variant ids across genes and tiers
 
     # Check if an existing var_map was provided or if CIViC needs to be queried
     if (var_map is None) or (not var_map):
-        from query import query_civic
+        from civicutils.query import query_civic
         # gene -> variant -> null
         all_genes = list(var_data.keys())
         var_map = query_civic(all_genes, identifier_type)
     else:
         check_is_dict(var_map, "var_map")
 
     # gene -> variant -> null
@@ -931,15 +931,15 @@
             # Keep track of all the variant ids matched across genes and tiers
             for var_id in all_ids:
                 if var_id not in matched_ids:
                     matched_ids.append(var_id)
 
     # At this point, all input gene + variants in var_data have been matched to CIViC
     # Filter var_map used to match CIViC info based on the matched variant ids (to avoid returning unnecessary records)
-    from filtering import filter_civic
+    from civicutils.filtering import filter_civic
     var_map = filter_civic(var_map, var_id_in=matched_ids, output_empty=False)
 
     # Return match_map, list of all matched variant ids, and associated variant records retrieved from CIViC (or provided by user), already filtered for the matched variants
     return (match_map, matched_ids, var_map)
 
 
 def filter_match(match, select_tier):
```

### Comparing `civicutils-1.0.1/civicutils/query.py` & `civicutils-1.0.2/civicutils/query.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/civicutils/read_and_write.py` & `civicutils-1.0.2/civicutils/read_and_write.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/civicutils/utils.py` & `civicutils-1.0.2/civicutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
 
 def translate_aa(aminoacid):
     """
     Given a 1-letter aminoacid code, check if it is a valid one and translate into a 3-letter code.
     :param aminoacid:     Aminoacid code in 1-letter format.
     :return:              Translated 3-letter aminoacid code.
     """
-    from read_and_write import get_dict_aminoacids
+    from civicutils.read_and_write import get_dict_aminoacids
     # Import the dictionary of aminoacid codes provided in the config "data.yml" file
     dict_codes = get_dict_aminoacids()
     aa_new = None
     check_empty_input(aminoacid, "aminoacid", is_required=True)
     if aminoacid.upper() in dict_codes.keys():
         aa_new = dict_codes[aminoacid.upper()]
```

### Comparing `civicutils-1.0.1/civicutils/data/data.yml` & `civicutils-1.0.2/civicutils/data/data.yml`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/dist_backup/civicutils-1.0.0-py3-none-any.whl` & `civicutils-1.0.2/dist_backup_2/civicutils-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/dist_backup/civicutils-1.0.0.tar.gz` & `civicutils-1.0.2/dist_backup_2/civicutils-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/images/civicutils-workflow.png` & `civicutils-1.0.2/images/civicutils-workflow.png`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/tcga_analysis/data/civic_available_diseases_31052023.txt` & `civicutils-1.0.2/tcga_analysis/data/civic_available_diseases_31052023.txt`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/tcga_analysis/scripts/Query_CIViCutils.py` & `civicutils-1.0.2/tcga_analysis/scripts/Query_CIViCutils.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/tcga_analysis/scripts/civicutils_manuscript_figures.R` & `civicutils-1.0.2/tcga_analysis/scripts/civicutils_manuscript_figures.R`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/tcga_analysis/scripts/get_available_diseases_in_civic.py` & `civicutils-1.0.2/tcga_analysis/scripts/get_available_diseases_in_civic.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/tcga_analysis/scripts/process_civic_predictions.py` & `civicutils-1.0.2/tcga_analysis/scripts/process_civic_predictions.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/LICENSE.md` & `civicutils-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/README.md` & `civicutils-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.1/pyproject.toml` & `civicutils-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "civicutils"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python package for querying, matching and downstream processing of CIViC information."
 requires-python = ">=3.7"
 dependencies = ["civicpy>=3.0.0"]
 readme = "README.md"
 license = {file = "LICENSE.md"}
 authors = [
   { name="María Lourdes Rosano-Gonzalez", email="lourdes.rosanogonzalez@gmail.com" },
```

### Comparing `civicutils-1.0.1/PKG-INFO` & `civicutils-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civicutils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package for querying, matching and downstream processing of CIViC information.
 Project-URL: Homepage, https://github.com/ETH-NEXUS/civicutils
 Project-URL: Bug Tracker, https://github.com/ETH-NEXUS/civicutils/issues
 Author-email: María Lourdes Rosano-Gonzalez <lourdes.rosanogonzalez@gmail.com>, "Vipin T. Sreedharan" <vipin.sreedharan@nexus.ethz.ch>, Antoine Hanns <hanns@nexus.ethz.ch>, "Daniel J. Stekhoven" <stekhoven@nexus.ethz.ch>, Franziska Singer <singer@nexus.ethz.ch>
 Maintainer-email: Antoine Hanns <hanns@nexus.ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

