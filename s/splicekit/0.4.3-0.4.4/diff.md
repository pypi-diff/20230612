# Comparing `tmp/splicekit-0.4.3.tar.gz` & `tmp/splicekit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splicekit-0.4.3.tar", last modified: Thu Jun  8 07:40:46 2023, max compression
+gzip compressed data, was "splicekit-0.4.4.tar", last modified: Mon Jun 12 17:57:04 2023, max compression
```

## Comparing `splicekit-0.4.3.tar` & `splicekit-0.4.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.110929 splicekit-0.4.3/
--rw-rw-r--   0 rotg     (2023757) games       (20)    23142 2023-06-08 07:40:46.110340 splicekit-0.4.3/PKG-INFO
--rwxrwxr-x   0 rotg     (2023757) games       (20)    22744 2023-06-06 14:20:03.000000 splicekit-0.4.3/README.md
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-08 07:40:46.111031 splicekit-0.4.3/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1133 2023-05-25 08:08:20.000000 splicekit-0.4.3/setup.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.087030 splicekit-0.4.3/splicekit/
--rw-rw-r--   0 rotg     (2023757) games       (20)    13857 2023-06-08 07:08:02.000000 splicekit-0.4.3/splicekit/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.090636 splicekit-0.4.3/splicekit/clusterlogfc/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.3/splicekit/clusterlogfc/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.092167 splicekit-0.4.3/splicekit/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.3/splicekit/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.107484 splicekit-0.4.3/splicekit/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)      396 2023-01-31 12:27:24.000000 splicekit-0.4.3/splicekit/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.3/splicekit/core/anchors.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.3/splicekit/core/annotation.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.3/splicekit/core/delta_dar.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.3/splicekit/core/exons.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)    29902 2023-05-03 08:24:07.000000 splicekit-0.4.3/splicekit/core/features.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.3/splicekit/core/genes.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.3/splicekit/core/jbrowse2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     8978 2023-06-07 14:07:47.000000 splicekit-0.4.3/splicekit/core/jbrowse2_create.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.3/splicekit/core/juan.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-05-02 17:27:43.000000 splicekit-0.4.3/splicekit/core/junctions.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.3/splicekit/core/motifs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.3/splicekit/core/patterns.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.3/splicekit/core/promisc.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.3/splicekit/core/report.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.109005 splicekit-0.4.3/splicekit/judge/
--rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-05-02 18:05:54.000000 splicekit-0.4.3/splicekit/judge/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.3/splicekit/splicecompare
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5165 2023-06-08 07:07:45.000000 splicekit-0.4.3/splicekit/splicekit
--rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.3/splicekit/splicekit.config.template
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-08 07:40:35.000000 splicekit-0.4.3/splicekit/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.089992 splicekit-0.4.3/splicekit.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)    23142 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      826 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.3/splicekit.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/top_level.txt
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.026227 splicekit-0.4.4/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23142 2023-06-12 17:57:04.025850 splicekit-0.4.4/PKG-INFO
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    22744 2023-06-06 14:20:03.000000 splicekit-0.4.4/README.md
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-12 17:57:04.026327 splicekit-0.4.4/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1150 2023-06-12 17:55:56.000000 splicekit-0.4.4/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.003757 splicekit-0.4.4/splicekit/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    13857 2023-06-08 07:08:02.000000 splicekit-0.4.4/splicekit/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.007341 splicekit-0.4.4/splicekit/clusterlogfc/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.4/splicekit/clusterlogfc/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.008686 splicekit-0.4.4/splicekit/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.4/splicekit/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.023391 splicekit-0.4.4/splicekit/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      396 2023-01-31 12:27:24.000000 splicekit-0.4.4/splicekit/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.4/splicekit/core/anchors.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.4/splicekit/core/annotation.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.4/splicekit/core/delta_dar.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.4/splicekit/core/exons.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    29902 2023-05-03 08:24:07.000000 splicekit-0.4.4/splicekit/core/features.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.4/splicekit/core/genes.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.4/splicekit/core/jbrowse2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9033 2023-06-08 11:52:41.000000 splicekit-0.4.4/splicekit/core/jbrowse2_create.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.4/splicekit/core/juan.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-05-02 17:27:43.000000 splicekit-0.4.4/splicekit/core/junctions.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.4/splicekit/core/motifs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.4/splicekit/core/patterns.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.4/splicekit/core/promisc.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.4/splicekit/core/report.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1527 2023-05-09 07:27:49.000000 splicekit-0.4.4/splicekit/folders.setup
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.024482 splicekit-0.4.4/splicekit/judge/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-06-08 11:49:08.000000 splicekit-0.4.4/splicekit/judge/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.4/splicekit/splicecompare
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5165 2023-06-08 07:07:45.000000 splicekit-0.4.4/splicekit/splicekit
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.4/splicekit/splicekit.config.template
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-12 17:56:05.000000 splicekit-0.4.4/splicekit/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-12 17:57:04.006803 splicekit-0.4.4/splicekit.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23142 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.4/splicekit.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-06-12 17:57:03.000000 splicekit-0.4.4/splicekit.egg-info/top_level.txt
```

### Comparing `splicekit-0.4.3/PKG-INFO` & `splicekit-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.3
+Version: 0.4.4
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `splicekit-0.4.3/README.md` & `splicekit-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/setup.py` & `splicekit-0.4.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     author='Roche, PMDA Spliceosome team',
     scripts=["splicekit/splicekit", "splicekit/splicecompare"],
     author_email='gregor.rot@gmail.com',
     url='https://github.com/bedapub/splicekit',
     keywords=['splicekit', 'splicing', 'transcriptomics', 'bioinformatics'],
     include_package_data=True,
     package_data={
-        'splicekit': ['splicekit.config.template', 'version'],
+        'splicekit': ['folders.setup', 'splicekit.config.template', 'version'],
     },
     install_requires=["pybio", "scanRBP", "pysam", "numpy", "psutil", "bs4", "requests", "rangehttpserver"],
 )
```

### Comparing `splicekit-0.4.3/splicekit/__init__.py` & `splicekit-0.4.4/splicekit/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/clusterlogfc/__init__.py` & `splicekit-0.4.4/splicekit/clusterlogfc/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/config/__init__.py` & `splicekit-0.4.4/splicekit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/anchors.py` & `splicekit-0.4.4/splicekit/core/anchors.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/annotation.py` & `splicekit-0.4.4/splicekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/delta_dar.py` & `splicekit-0.4.4/splicekit/core/delta_dar.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/exons.py` & `splicekit-0.4.4/splicekit/core/exons.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/features.py` & `splicekit-0.4.4/splicekit/core/features.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/genes.py` & `splicekit-0.4.4/splicekit/core/genes.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/jbrowse2.py` & `splicekit-0.4.4/splicekit/core/jbrowse2.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/jbrowse2_create.py` & `splicekit-0.4.4/splicekit/core/jbrowse2_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     bamCoverage_binSize= 3
     fsh = open(f"jobs/jobs_jbrowse/process.sh", "wt")
     for sample in bam_files:
         bam_fname = bam_dir +'/'+ sample
         cram_fname = dirs_to_check[2] + '/'+sample.replace('.bam', '.cram')
         bigwig_fname = dirs_to_check[2] +'/'+ sample.replace('.bam', '.bw')
         if (not (os.path.exists(cram_fname) and os.path.exists(bigwig_fname))) or (force_samples == True):
-            os.system(f'rm -r {bigwig_fname}')
-            os.system(f'rm -r {cram_fname}')
+            os.system(f'rm {bigwig_fname} >/dev/null 2>&1')
+            os.system(f'rm {cram_fname} >/dev/null 2>&1')
             print(f'[jbrowse] create sample processing job for {sample}')
             fout = open("jobs/jobs_jbrowse/{sample}.job".format(sample=sample), "wt")
             job_bw_out = job_bw.format(container=container, bamCoverage_binSize=bamCoverage_binSize, sample=sample,
                                         bam_fname=bam_fname,cram_fname=cram_fname, bigwig_fname=bigwig_fname, genome_fa=genome_fa)
             fout.write(job_bw_out)
             fout.close()        
             job_sh_bw_out = job_sh_bw.format(container=container, sample=sample, bamCoverage_binSize=bamCoverage_binSize,
@@ -91,16 +91,16 @@
 
     # initialize config.json with adding fasta file --------------------------------------------------------------------------------------------------------------------------------------
     if (not os.path.exists('jbrowse2/splicekit_data/config.json')) or (force_annotation==True):
         
         # clean up previous jobs
         os.system(f'rm -r jbrowse2/splicekit_data/*')
         for sample in bam_files:
-            os.system(f'rm logs/logs_jbrowse/{sample}.out')
-            os.system(f'rm logs/logs_jbrowse/{sample}.err')
+            os.system(f'rm logs/logs_jbrowse/{sample}.out >/dev/null 2>&1')
+            os.system(f'rm logs/logs_jbrowse/{sample}.err >/dev/null 2>&1')
 
         print('[jbrowse] creating config.json in jbrowse2/splicekit_data')
 
         if os.path.isabs(genome_fa): # check if genome_fa path is absolute or relative
             os.system(f'cd jbrowse2/splicekit_data; {container} jbrowse add-assembly {genome_fa} --name GenomeSequence --load symlink') # initialize config.json with genome sequence
         else:
             os.system(f'cd jbrowse2/splicekit_data; {container} jbrowse add-assembly ../../{genome_fa} --name GenomeSequence --load symlink') # initialize config.json with genome sequence
@@ -145,10 +145,7 @@
     # run  sample jobs if available
     if (not os.path.exists('jbrowse2/splicekit_data/config.json')) or (force_samples):
         if splicekit.config.platform=="cluster":
             os.system('export BSUB_QUIET=Y; jobs=( $(ls jobs/jobs_jbrowse/*.job) ); g=10; for((i=0; i < ${#jobs[@]}; i+=g)); do part=( "${jobs[@]:i:g}" ); for job_fname in ${part[*]}; do echo "[jbrowse] submitted $job_fname"; bsub -K < ${job_fname} & done; wait; echo "[jbrowse] processing next 10"; done; echo "[jbrowse] processing complete"')
         if splicekit.config.platform=="desktop":
             os.system("source jobs/jobs_jbrowse/process.sh")
     create_jbrowse_config(force_annotation)
-
-
-
```

### Comparing `splicekit-0.4.3/splicekit/core/juan.py` & `splicekit-0.4.4/splicekit/core/juan.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/junctions.py` & `splicekit-0.4.4/splicekit/core/junctions.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/motifs.py` & `splicekit-0.4.4/splicekit/core/motifs.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/patterns.py` & `splicekit-0.4.4/splicekit/core/patterns.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/promisc.py` & `splicekit-0.4.4/splicekit/core/promisc.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/core/report.py` & `splicekit-0.4.4/splicekit/core/report.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/judge/__init__.py` & `splicekit-0.4.4/splicekit/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/splicecompare` & `splicekit-0.4.4/splicekit/splicecompare`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/splicekit` & `splicekit-0.4.4/splicekit/splicekit`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit/splicekit.config.template` & `splicekit-0.4.4/splicekit/splicekit.config.template`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.3/splicekit.egg-info/PKG-INFO` & `splicekit-0.4.4/splicekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.3
+Version: 0.4.4
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `splicekit-0.4.3/splicekit.egg-info/SOURCES.txt` & `splicekit-0.4.4/splicekit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 splicekit/__init__.py
+splicekit/folders.setup
 splicekit/splicecompare
 splicekit/splicekit
 splicekit/splicekit.config.template
 splicekit/version
 splicekit.egg-info/PKG-INFO
 splicekit.egg-info/SOURCES.txt
 splicekit.egg-info/dependency_links.txt
```

