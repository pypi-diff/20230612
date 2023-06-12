# Comparing `tmp/PRauto-0.212.tar.gz` & `tmp/PRauto-0.213.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.212.tar", last modified: Mon Jun 12 04:27:54 2023, max compression
+gzip compressed data, was "PRauto-0.213.tar", last modified: Mon Jun 12 05:13:51 2023, max compression
```

## Comparing `PRauto-0.212.tar` & `PRauto-0.213.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.087424 PRauto-0.212/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.212/LICENSE
--rw-rw-rw-   0        0        0      349 2023-06-12 04:27:54.087424 PRauto-0.212/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.059496 PRauto-0.212/PRauto.egg-info/
--rw-rw-rw-   0        0        0      349 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 04:27:53.000000 PRauto-0.212/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2604 2023-06-05 02:04:20.000000 PRauto-0.212/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.063502 PRauto-0.212/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.212/prauto/__init__.py
--rw-rw-rw-   0        0        0     3181 2023-06-05 02:01:10.000000 PRauto-0.212/prauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.070693 PRauto-0.212/prauto/prepauto/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.212/prauto/prepauto/__init__.py
--rw-rw-rw-   0        0        0    14202 2023-05-10 05:53:19.000000 PRauto-0.212/prauto/prepauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:27:54.085053 PRauto-0.212/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.212/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     3064 2023-06-05 02:01:33.000000 PRauto-0.212/prauto/retriever/__main__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.212/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     7842 2023-06-07 08:27:19.000000 PRauto-0.212/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.212/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-06-12 04:27:54.088431 PRauto-0.212/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-06-12 04:25:32.000000 PRauto-0.212/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.029045 PRauto-0.213/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.213/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-06-12 05:13:51.029045 PRauto-0.213/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.003719 PRauto-0.213/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2604 2023-06-05 02:04:20.000000 PRauto-0.213/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.005718 PRauto-0.213/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.213/prauto/__init__.py
+-rw-rw-rw-   0        0        0     3501 2023-06-12 05:08:39.000000 PRauto-0.213/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.013718 PRauto-0.213/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.213/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    14202 2023-05-10 05:53:19.000000 PRauto-0.213/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.027047 PRauto-0.213/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.213/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-06-05 02:01:33.000000 PRauto-0.213/prauto/retriever/__main__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.213/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     7842 2023-06-07 08:27:19.000000 PRauto-0.213/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.213/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 05:13:51.029045 PRauto-0.213/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-06-12 05:10:11.000000 PRauto-0.213/setup.py
```

### Comparing `PRauto-0.212/LICENSE` & `PRauto-0.213/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.212/README.md` & `PRauto-0.213/README.md`

 * *Files identical despite different names*

### Comparing `PRauto-0.212/prauto/__main__.py` & `PRauto-0.213/prauto/retriever/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,73 @@
 #!/usr/bin/env python
 
-from .retriever.get_fasta import *
-from .retriever.get_pdb import *
-from .retriever.get_ligand import *
+from .get_fasta import *
+from .get_pdb import *
+from .get_ligand import *
 from tqdm.auto import tqdm
 from tkinter import Tk
 from tkinter import filedialog
 
 root = Tk()
 root.withdraw()
 
 mult = '\n' * 3
 global search_key
 
 
 def main():
     global search_key
+    target_dir = filedialog.askdirectory(title='Select a directory to work with')
+    os.chdir(target_dir)
     print(f'Step1: Retrieve FASTA files{mult}')
     print(f"""
     
 ########################################################################################################
 
-This is a bulk data retrieval version of Prauto.
+ > Please input [ Protein Name ] and [ Gene Name ] of your target.
 
-To make prauto work properly, the Directory, Protein Name, and Gene Name 
-should have been entered in the format of prauto_order_form.csv
+
+    input 1  Protein Name with subtype :  ex. 5-hydroxytryptamine receptor 2A   
+                                                                             / Search term(uniprot API)
+                                                                               
+    input 2  Gene Name :  ex. HTR2A                                 
+                                     / Filtering term for Integrity of data 
                                                   
 #########################################################################################################
                                                                                             """)
-    order_form = filedialog.askopenfilename(title='Select the order_form')
-    with open(order_form, "r", encoding='UTF-8') as f:
-        lines = f.readlines()[1:]
-        for line in lines:
-            target_dir = line.split(",")[0]
-            os.chdir(target_dir)
-
-            search_key = line.split(",")[1]
-            gene_name = line.split(",")[2].strip('\n')
-            dir_name = line.split(",")[2].strip('\n')
-            fasta_file_path = download_fasta(search_key, dir_name)
-            fasta_file_path = remove_outlier(search_key, gene_name, fasta_file_path)
-            pdb_dir = os.path.dirname(fasta_file_path)
-
-            print(f'Step2: Retrieve PDB files{mult}')
-            accessions_list = extract_accessions(fasta_file_path)
-            for accession in accessions_list:
-                pdb_ids = search_pdb_by_accession(accession)
-                if pdb_ids:
-                    print(f'\nFound {len(pdb_ids)} PDB entries for {accession}')
-                    download_pdb_files_by_acc(pdb_ids, accession, pdb_dir)
-
-            print(f'Step3: Retrieve sdf files{mult}')
-            for accession in accessions_list:
-                sdf_file = os.path.join(pdb_dir, "ligands", f"{gene_name}_{accession}_ligands.sdf")
-                if os.path.exists(sdf_file):
-                    continue
-                else:
-                    retry_count = 0
-                    max_retries = 100
-                    while retry_count < max_retries:
-                        try:
-                            download_chembl_compounds(accession, pdb_dir, gene_name)
-                            break  # Download successful, exit the retry loop
-                        except Exception as e:
-                            print(f"Error occurred: {str(e)}")
-                            print(f"Retrying in 5 seconds... (retry count: {retry_count + 1}/{max_retries})")
-                            time.sleep(5)  # Wait for 5 seconds before retrying
-                            retry_count += 1
-                    else:
-                        print(f"Failed to download compounds for accession {accession} after {max_retries} retries.")
+    search_key = input('input 1  Protein Name with subtype :')
+    gene_name = input('input 2  Gene Name :')
+    dir_name = input('input Directory Name for FASTA file: ')
+    fasta_file_path = download_fasta(search_key, dir_name)
+    fasta_file_path = remove_outlier(search_key,gene_name,fasta_file_path)
+    pdb_dir = os.path.dirname(fasta_file_path)
+
+    print(f'Step2: Retrieve PDB files{mult}')
+    accessions_list = extract_accessions(fasta_file_path)
+    for accession in accessions_list:
+        pdb_ids = search_pdb_by_accession(accession)
+        if pdb_ids:
+            print(f'\nFound {len(pdb_ids)} PDB entries for {accession}')
+            download_pdb_files_by_acc(pdb_ids, accession, pdb_dir)
+
+    print(f'Step3: Retrieve sdf files{mult}')
+    for accession in accessions_list:
+        sdf_file = os.path.join(pdb_dir, "ligands", f"{gene_name}_{accession}_ligands.sdf")
+        if os.path.exists(sdf_file):
+            continue
+        else:
+            retry_count = 0
+            max_retries = 100
+            while retry_count < max_retries:
+                try:
+                    download_chembl_compounds(accession, pdb_dir, gene_name)
+                    break  # Download successful, exit the retry loop
+                except Exception as e:
+                    print(f"Error occurred: {str(e)}")
+                    print(f"Retrying in 5 seconds... (retry count: {retry_count + 1}/{max_retries})")
+                    time.sleep(5)  # Wait for 5 seconds before retrying
+                    retry_count += 1
+            else:
+                print(f"Failed to download compounds for accession {accession} after {max_retries} retries.")
 
 if __name__ == "__main__":
     main()
```

### Comparing `PRauto-0.212/prauto/prepauto/__main__.py` & `PRauto-0.213/prauto/prepauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.212/prauto/retriever/get_fasta.py` & `PRauto-0.213/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.212/prauto/retriever/get_ligand.py` & `PRauto-0.213/prauto/retriever/get_ligand.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.212/prauto/retriever/get_pdb.py` & `PRauto-0.213/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.212/setup.py` & `PRauto-0.213/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages, Extension
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.212',
+        version = '0.213',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

