# Comparing `tmp/civicutils-1.0.2.tar.gz` & `tmp/civicutils-1.0.2.post1.tar.gz`

## Comparing `civicutils-1.0.2.tar` & `civicutils-1.0.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 civicutils-1.0.2/info_on_matching_framework.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/__init__.py
--rw-r--r--   0        0        0    40439 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/filtering.py
--rw-r--r--   0        0        0   111723 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/match.py
--rw-r--r--   0        0        0    16931 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/query.py
--rw-r--r--   0        0        0    33562 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/read_and_write.py
--rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/utils.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/data/data.yml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/data/example_cnv.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/data/example_expr.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 civicutils-1.0.2/civicutils/data/example_snv.txt
--rw-r--r--   0        0        0    82485 2020-02-02 00:00:00.000000 civicutils-1.0.2/dist_backup/civicutils-1.0.1-py3-none-any.whl
--rw-r--r--   0        0        0   961403 2020-02-02 00:00:00.000000 civicutils-1.0.2/dist_backup/civicutils-1.0.1.tar.gz
--rw-r--r--   0        0        0    82463 2020-02-02 00:00:00.000000 civicutils-1.0.2/dist_backup_2/civicutils-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   439302 2020-02-02 00:00:00.000000 civicutils-1.0.2/dist_backup_2/civicutils-1.0.0.tar.gz
--rw-r--r--   0        0        0   396868 2020-02-02 00:00:00.000000 civicutils-1.0.2/images/civicutils-workflow.png
--rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/data/civic_available_diseases_31052023.txt
--rw-r--r--   0        0        0    36985 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/scripts/Query_CIViCutils.py
--rw-r--r--   0        0        0    78674 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/scripts/civicutils_manuscript_figures.R
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/scripts/get_available_diseases_in_civic.py
--rw-r--r--   0        0        0   128034 2020-02-02 00:00:00.000000 civicutils-1.0.2/tcga_analysis/scripts/process_civic_predictions.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 civicutils-1.0.2/LICENSE.md
--rw-r--r--   0        0        0    45370 2020-02-02 00:00:00.000000 civicutils-1.0.2/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 civicutils-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    86899 2020-02-02 00:00:00.000000 civicutils-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/info_on_matching_framework.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/__init__.py
+-rw-r--r--   0        0        0    40439 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/filtering.py
+-rw-r--r--   0        0        0   111723 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/match.py
+-rw-r--r--   0        0        0    16931 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/query.py
+-rw-r--r--   0        0        0    33562 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/read_and_write.py
+-rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/utils.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/data/data.yml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/data/example_cnv.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/data/example_expr.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/civicutils/data/example_snv.txt
+-rw-r--r--   0        0        0    82485 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/dist_backup/civicutils-1.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0   961403 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/dist_backup/civicutils-1.0.1.tar.gz
+-rw-r--r--   0        0        0    82463 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/dist_backup_2/civicutils-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   439302 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/dist_backup_2/civicutils-1.0.0.tar.gz
+-rw-r--r--   0        0        0   396868 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/images/civicutils-workflow.png
+-rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/tcga_analysis/data/civic_available_diseases_31052023.txt
+-rw-r--r--   0        0        0    36985 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/tcga_analysis/scripts/Query_CIViCutils.py
+-rw-r--r--   0        0        0    78674 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/tcga_analysis/scripts/civicutils_manuscript_figures.R
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/tcga_analysis/scripts/get_available_diseases_in_civic.py
+-rw-r--r--   0        0        0   128034 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/tcga_analysis/scripts/process_civic_predictions.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/LICENSE.md
+-rw-r--r--   0        0        0    45378 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/README.md
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/pyproject.toml
+-rw-r--r--   0        0        0    86913 2020-02-02 00:00:00.000000 civicutils-1.0.2.post1/PKG-INFO
```

### Comparing `civicutils-1.0.2/info_on_matching_framework.md` & `civicutils-1.0.2.post1/info_on_matching_framework.md`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/civicutils/filtering.py` & `civicutils-1.0.2.post1/civicutils/filtering.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/civicutils/match.py` & `civicutils-1.0.2.post1/civicutils/match.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/civicutils/query.py` & `civicutils-1.0.2.post1/civicutils/query.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/civicutils/read_and_write.py` & `civicutils-1.0.2.post1/civicutils/read_and_write.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/civicutils/utils.py` & `civicutils-1.0.2.post1/civicutils/utils.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/civicutils/data/data.yml` & `civicutils-1.0.2.post1/civicutils/data/data.yml`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/dist_backup/civicutils-1.0.1-py3-none-any.whl` & `civicutils-1.0.2.post1/dist_backup/civicutils-1.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/dist_backup/civicutils-1.0.1.tar.gz` & `civicutils-1.0.2.post1/dist_backup/civicutils-1.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/dist_backup_2/civicutils-1.0.0-py3-none-any.whl` & `civicutils-1.0.2.post1/dist_backup_2/civicutils-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/dist_backup_2/civicutils-1.0.0.tar.gz` & `civicutils-1.0.2.post1/dist_backup_2/civicutils-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/images/civicutils-workflow.png` & `civicutils-1.0.2.post1/images/civicutils-workflow.png`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/tcga_analysis/data/civic_available_diseases_31052023.txt` & `civicutils-1.0.2.post1/tcga_analysis/data/civic_available_diseases_31052023.txt`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/tcga_analysis/scripts/Query_CIViCutils.py` & `civicutils-1.0.2.post1/tcga_analysis/scripts/Query_CIViCutils.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/tcga_analysis/scripts/civicutils_manuscript_figures.R` & `civicutils-1.0.2.post1/tcga_analysis/scripts/civicutils_manuscript_figures.R`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/tcga_analysis/scripts/get_available_diseases_in_civic.py` & `civicutils-1.0.2.post1/tcga_analysis/scripts/get_available_diseases_in_civic.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/tcga_analysis/scripts/process_civic_predictions.py` & `civicutils-1.0.2.post1/tcga_analysis/scripts/process_civic_predictions.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/LICENSE.md` & `civicutils-1.0.2.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.2/README.md` & `civicutils-1.0.2.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # CIViCutils
 
 ## General overview
 
 [CIViCutils](https://pypi.org/project/civicutils) is a Python package for rapid retrieval, annotation, prioritization and downstream processing of information from the expert-curated [CIViC knowledgebase](https://civicdb.org/welcome) (Clinical Interpretations of Variants in Cancer). CIViCutils can be integrated into novel and existing clinical workflows to provide variant-level disease-specific information about treatment response, pathogenesis, diagnosis, and prognosis of genomic aberrations (SNVs, InDels and CNVs), as well as differentially expressed genes. It streamlines interpreting large numbers of input alterations with querying and analyzing CIViC information, and enables the harmonization of input across different nomenclatures. Key features of CIViCutils include an automated matching framework for linking clinical evidence to input variants, as well as evaluating the accuracy of the resulting hits, and in-silico prediction of drug-target interactions tailored to individual patients and cancer subtypes of interest. For more details, see the CIViCutils publication.
 
-![README_diagram](https://github.com/ETH-NEXUS/civicutils/blob/master/images/civicutils-workflow.png)
-
+![README_diagram](https://github.com/ETH-NEXUS/civicutils/blob/master/images/civicutils-workflow.png?raw=true)
 
 ## Installation instructions
 
 ### Dependencies
 - [civicpy](https://github.com/griffithlab/civicpy):
 To install, first activate the relevant Python (>=3.7) environment and then use pip install:
```

### Comparing `civicutils-1.0.2/pyproject.toml` & `civicutils-1.0.2.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "civicutils"
-version = "1.0.2"
+version = "1.0.2.post1"
 description = "Python package for querying, matching and downstream processing of CIViC information."
 requires-python = ">=3.7"
 dependencies = ["civicpy>=3.0.0"]
 readme = "README.md"
 license = {file = "LICENSE.md"}
 authors = [
   { name="María Lourdes Rosano-Gonzalez", email="lourdes.rosanogonzalez@gmail.com" },
```

### Comparing `civicutils-1.0.2/PKG-INFO` & `civicutils-1.0.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civicutils
-Version: 1.0.2
+Version: 1.0.2.post1
 Summary: Python package for querying, matching and downstream processing of CIViC information.
 Project-URL: Homepage, https://github.com/ETH-NEXUS/civicutils
 Project-URL: Bug Tracker, https://github.com/ETH-NEXUS/civicutils/issues
 Author-email: María Lourdes Rosano-Gonzalez <lourdes.rosanogonzalez@gmail.com>, "Vipin T. Sreedharan" <vipin.sreedharan@nexus.ethz.ch>, Antoine Hanns <hanns@nexus.ethz.ch>, "Daniel J. Stekhoven" <stekhoven@nexus.ethz.ch>, Franziska Singer <singer@nexus.ethz.ch>
 Maintainer-email: Antoine Hanns <hanns@nexus.ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -691,16 +691,15 @@
 
 # CIViCutils
 
 ## General overview
 
 [CIViCutils](https://pypi.org/project/civicutils) is a Python package for rapid retrieval, annotation, prioritization and downstream processing of information from the expert-curated [CIViC knowledgebase](https://civicdb.org/welcome) (Clinical Interpretations of Variants in Cancer). CIViCutils can be integrated into novel and existing clinical workflows to provide variant-level disease-specific information about treatment response, pathogenesis, diagnosis, and prognosis of genomic aberrations (SNVs, InDels and CNVs), as well as differentially expressed genes. It streamlines interpreting large numbers of input alterations with querying and analyzing CIViC information, and enables the harmonization of input across different nomenclatures. Key features of CIViCutils include an automated matching framework for linking clinical evidence to input variants, as well as evaluating the accuracy of the resulting hits, and in-silico prediction of drug-target interactions tailored to individual patients and cancer subtypes of interest. For more details, see the CIViCutils publication.
 
-![README_diagram](https://github.com/ETH-NEXUS/civicutils/blob/master/images/civicutils-workflow.png)
-
+![README_diagram](https://github.com/ETH-NEXUS/civicutils/blob/master/images/civicutils-workflow.png?raw=true)
 
 ## Installation instructions
 
 ### Dependencies
 - [civicpy](https://github.com/griffithlab/civicpy):
 To install, first activate the relevant Python (>=3.7) environment and then use pip install:
```

