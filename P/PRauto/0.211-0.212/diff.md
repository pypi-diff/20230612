# Comparing `tmp/PRauto-0.211.tar.gz` & `tmp/PRauto-0.212.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.211.tar", last modified: Mon Jun  5 02:03:26 2023, max compression
+gzip compressed data, was "PRauto-0.212.tar", last modified: Mon Jun 12 04:27:54 2023, max compression
```

## Comparing `PRauto-0.211.tar` & `PRauto-0.212.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.915933 PRauto-0.211/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.211/LICENSE
--rw-rw-rw-   0        0        0      349 2023-06-05 02:03:26.915168 PRauto-0.211/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.899472 PRauto-0.211/PRauto.egg-info/
--rw-rw-rw-   0        0        0      349 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2088 2023-04-21 03:50:22.000000 PRauto-0.211/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.902472 PRauto-0.211/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.211/prauto/__init__.py
--rw-rw-rw-   0        0        0     3181 2023-06-05 02:01:10.000000 PRauto-0.211/prauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.905471 PRauto-0.211/prauto/prepauto/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.211/prauto/prepauto/__init__.py
--rw-rw-rw-   0        0        0    14202 2023-05-10 05:53:19.000000 PRauto-0.211/prauto/prepauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.913456 PRauto-0.211/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.211/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     3064 2023-06-05 02:01:33.000000 PRauto-0.211/prauto/retriever/__main__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.211/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     5901 2023-06-02 02:00:27.000000 PRauto-0.211/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.211/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-06-05 02:03:26.915933 PRauto-0.211/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-06-05 02:02:19.000000 PRauto-0.211/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.087424 PRauto-0.212/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.212/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-06-12 04:27:54.087424 PRauto-0.212/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.059496 PRauto-0.212/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2604 2023-06-05 02:04:20.000000 PRauto-0.212/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.063502 PRauto-0.212/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.212/prauto/__init__.py
+-rw-rw-rw-   0        0        0     3181 2023-06-05 02:01:10.000000 PRauto-0.212/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.070693 PRauto-0.212/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.212/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    14202 2023-05-10 05:53:19.000000 PRauto-0.212/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.085053 PRauto-0.212/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.212/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-06-05 02:01:33.000000 PRauto-0.212/prauto/retriever/__main__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.212/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     7842 2023-06-07 08:27:19.000000 PRauto-0.212/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.212/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 04:27:54.088431 PRauto-0.212/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-06-12 04:25:32.000000 PRauto-0.212/setup.py
```

### Comparing `PRauto-0.211/LICENSE` & `PRauto-0.212/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.211/prauto/__main__.py` & `PRauto-0.212/prauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.211/prauto/prepauto/__main__.py` & `PRauto-0.212/prauto/prepauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.211/prauto/retriever/__main__.py` & `PRauto-0.212/prauto/retriever/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.211/prauto/retriever/get_fasta.py` & `PRauto-0.212/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.211/prauto/retriever/get_ligand.py` & `PRauto-0.212/prauto/retriever/get_ligand.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     targets = targets_api.get(
         target_components__accession=accession,
         target_type__in=['SINGLE PROTEIN', 'PROTEIN FAMILY']
     ).only("target_chembl_id")
     targets_id = list(set([target['target_chembl_id'] for target in targets]))
 
     if len(targets_id) != 0:
-        target_columns_list = ['molecule_chembl_id', 'molecule_name', 'molecule_max_phase', 'molecular_weight', 'alogp',
+        target_columns_list = ['assay_chembl_id', 'molecule_chembl_id', 'molecule_name', 'molecule_max_phase', 'molecular_weight', 'alogp',
                                'standard_type', 'standard_relation', 'standard_value', 'standard_units',
                                'pchembl_value', 'assay_type', 'target_name', 'target_organism', 'target_type']
 
         for target in targets_id:
 
             bioactivities = bioactivities_api.filter(target_chembl_id=target,
                                                      standard_type__in=["IC50", "EC50", "Ki", "Kd"],
@@ -43,14 +43,15 @@
                 *target_columns_list)
 
             bioactivities_list = list(bioactivities)
 
             compound_columns_list = ["molecule_chembl_id", 'molecule_structures', 'molecule_properties', 'mw_freebase']
             for bioactivity_chunk in chunked_iterable(bioactivities_list, 100):
                 compounds = compounds_api.filter(
+                    molecule_type='Small molecule',
                     molecule_chembl_id__in=[x['molecule_chembl_id'] for x in bioactivity_chunk],
                     molecule_properties__mw_freebase__lte=700,
                     molfile__isnull=False
                 ).only(*compound_columns_list)
 
                 compounds_list = [record for record in compounds]
 
@@ -62,33 +63,61 @@
                             mol_id = record['molecule_chembl_id']
                             file_name = f"{accession}_{mol_id}.sdf"
                             file_path = os.path.join(save_path, "ligands", file_name)
                             if os.path.exists(file_path):
                                 continue
                             mol_file = ''
                             molfile = record['molecule_structures']['molfile']
-                            mw_freebase = f"> <mw_freebase>\n{record['molecule_properties']['mw_freebase']}\n"
+                            targets_chembl = f"> <target_chembl_id>\n{target}\n"
+                            # target_accession 추후에 뺄지 정하기
+                            target_accession = f"\n> <target_accession>\n{accession}\n"
+                            mw_freebase = f"\n> <mw_freebase>\n{record['molecule_properties']['mw_freebase']}\n"
                             alogp = f"\n> <alogp>\n{record['molecule_properties']['alogp']}\n"
                             mol_file += molfile
+                            mol_file += targets_chembl
+                            mol_file += target_accession
                             mol_file += mw_freebase
                             mol_file += alogp
                             mol_file += "\n> <bioactivities>\n"
 
-                            pChEMBL_value = 0
+                            pChEMBL_ki = 0
+                            pChEMBL_kd = 0
+                            pChEMBL_ec = 0
+                            pChEMBL_ic = 0
+
                             for i in bioactivities_list:
                                 if i['molecule_chembl_id'] == record['molecule_chembl_id']:
-                                    bioactivities_str = f"assay_type: {i['assay_type']}, pchembl_value: {i['pchembl_value']}, {i['standard_type']}{i['standard_relation']}{i['standard_value']}{i['standard_units']}\n"
+                                    bioactivities_str = f"assay_chembl_id: {i['assay_chembl_id']}, assay_type: {i['assay_type']}, pchembl_value: {i['pchembl_value']}, {i['standard_type']}{i['standard_relation']}{i['standard_value']}{i['standard_units']}\n"
                                     mol_file += bioactivities_str
-                                    if i['pchembl_value'] is not None:
-                                        if float(i['pchembl_value']) > float(pChEMBL_value):
-                                            pChEMBL_value = str(i['pchembl_value'])
-                            if pChEMBL_value == 0 or pChEMBL_value == '0':
-                                pChEMBL_value = 'None'
-                            pChEMBL_value_str = f"\n> <pChEMBL_value>\n{pChEMBL_value}\n"
-                            mol_file += pChEMBL_value_str
+
+                                    if i['standard_type'] =='Ki' and i['pchembl_value'] is not None:
+                                            if float(i['pchembl_value']) > float(pChEMBL_ki):
+                                                pChEMBL_ki = str(i['pchembl_value'])
+
+                                    if i['standard_type'] =='Kd' and i['pchembl_value'] is not None:
+                                            if float(i['pchembl_value']) > float(pChEMBL_kd):
+                                                pChEMBL_kd = str(i['pchembl_value'])
+
+                                    if i['standard_type'] =='IC50' and i['pchembl_value'] is not None:
+                                            if float(i['pchembl_value']) > float(pChEMBL_ic):
+                                                pChEMBL_ic = str(i['pchembl_value'])
+
+                                    if i['standard_type'] =='EC50' and i['pchembl_value'] is not None:
+                                            if float(i['pchembl_value']) > float(pChEMBL_ec):
+                                                pChEMBL_ec = str(i['pchembl_value'])
+
+                            pChEMBL_value_Ki = f"\n> <pChEMBL_value_Ki>\n{pChEMBL_ki}\n".replace("\n0\n", "\nNone\n")
+                            pChEMBL_value_Kd = f"\n> <pChEMBL_value_Kd>\n{pChEMBL_kd}\n".replace("\n0\n", "\nNone\n")
+                            pChEMBL_value_IC50 = f"\n> <pChEMBL_value_IC50>\n{pChEMBL_ic}\n".replace("\n0\n", "\nNone\n")
+                            pChEMBL_value_EC50 = f"\n> <pChEMBL_value_EC50>\n{pChEMBL_ec}\n".replace("\n0\n", "\nNone\n")
+
+                            mol_file += pChEMBL_value_Ki
+                            mol_file += pChEMBL_value_Kd
+                            mol_file += pChEMBL_value_IC50
+                            mol_file += pChEMBL_value_EC50
 
                             with open(file_path, 'w') as outfile:
                                 outfile.write(mol_file)
     merge_sdf_files(os.path.join(save_path, "ligands"), gene_name, accession)
 
 def merge_sdf_files(sdf_directory, gene_name, accession):
     # List the filenames of the input SDF files
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PRauto-0.211/prauto/retriever/get_pdb.py` & `PRauto-0.212/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.211/setup.py` & `PRauto-0.212/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages, Extension
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.211',
+        version = '0.212',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

