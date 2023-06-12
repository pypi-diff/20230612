# Comparing `tmp/starbug2-0.4.0.tar.gz` & `tmp/starbug2-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbug2-0.4.0.tar", last modified: Thu Jun  8 13:00:33 2023, max compression
+gzip compressed data, was "starbug2-0.4.1.tar", last modified: Mon Jun 12 19:16:12 2023, max compression
```

## Comparing `starbug2-0.4.0.tar` & `starbug2-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.490545 starbug2-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-08 13:00:18.000000 starbug2-0.4.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 13:00:18.000000 starbug2-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 13:00:18.000000 starbug2-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-08 13:00:33.490545 starbug2-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-08 13:00:18.000000 starbug2-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.486544 starbug2-0.4.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-06-08 13:00:18.000000 starbug2-0.4.0/bin/starbug2
--rwxr-xr-x   0 runner    (1001) docker     (123)     4292 2023-06-08 13:00:18.000000 starbug2-0.4.0/bin/starbug2-match
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.486544 starbug2-0.4.0/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-08 13:00:18.000000 starbug2-0.4.0/extras/starbug2.completion
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 13:00:18.000000 starbug2-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 13:00:33.490545 starbug2-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-08 13:00:18.000000 starbug2-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.486544 starbug2-0.4.0/starbug2/
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.490545 starbug2-0.4.0/starbug2/param/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/param/default.param
--rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/starbug.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.490545 starbug2-0.4.0/starbug2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.490545 starbug2-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-08 13:00:18.000000 starbug2-0.4.0/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-08 13:00:18.000000 starbug2-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.101716 starbug2-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 19:15:57.000000 starbug2-0.4.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 19:15:57.000000 starbug2-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 19:15:57.000000 starbug2-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-12 19:16:12.101716 starbug2-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-12 19:15:57.000000 starbug2-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.097716 starbug2-0.4.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-06-12 19:15:57.000000 starbug2-0.4.1/bin/starbug2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5629 2023-06-12 19:15:57.000000 starbug2-0.4.1/bin/starbug2-match
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.097716 starbug2-0.4.1/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-12 19:15:57.000000 starbug2-0.4.1/extras/starbug2.completion
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 19:15:57.000000 starbug2-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 19:16:12.101716 starbug2-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-12 19:15:57.000000 starbug2-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.097716 starbug2-0.4.1/starbug2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.101716 starbug2-0.4.1/starbug2/param/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/param/default.param
+-rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/starbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-12 19:15:57.000000 starbug2-0.4.1/starbug2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.101716 starbug2-0.4.1/starbug2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 19:16:12.000000 starbug2-0.4.1/starbug2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:12.101716 starbug2-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-12 19:15:57.000000 starbug2-0.4.1/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-12 19:15:57.000000 starbug2-0.4.1/tests/test_utils.py
```

### Comparing `starbug2-0.4.0/LICENSE.txt` & `starbug2-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/PKG-INFO` & `starbug2-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1
-Name: starbug2
-Version: 0.4.0
-Summary: JWST PSF photometry in complex crowded fields.
-Author: Conor Nally
-Author-email: conor.nally@ed.ac.uk
-License: GNU General Public License v3.0
-Description-Content-Type: text/markdown
-
 # StarBugII
 
 JWST PSF photometry in dusty crowded fields.
-Last updated: v0.3.0
+Last updated: v0.4.1
 
 [![Python application](https://github.com/conornally/starbug2/actions/workflows/python-app.yml/badge.svg)](https://github.com/conornally/starbug2/actions/workflows/python-app.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/starbug2.svg)](https://pypi.python.org/pypi/starbug2/)
 [![Latest release](https://badgen.net/github/release/conornally/starbug2)](https://github.com/conornally/starbug2/releases)
 
 
 ## Installation
@@ -80,14 +71,26 @@
        --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
        --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
 
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
+
+
+StarbugII Matching 
+usage: starbug2-match [-BGfhv] [-o output] [-p file.param] [-s KEY=VAL] table.fits ...
+    -B  --band               : match in "BAND" mode (does not preserve a column for every frame)
+    -D  --dither             : match in "DITHER" mode (preserves a column for every frame)
+    -f  --full               : export full catalogue
+    -G  --generic            : match in "GENERIC" mode
+    -h  --help               : show help message
+    -o  --output  file.fits  : output matched catalogue
+    -p  --param   file.param : load starbug parameter file
+    -s  --set     option     : set value in parameter file at runtime (-s MATCH_THRESH=1)
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
```

### Comparing `starbug2-0.4.0/README.md` & `starbug2-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,20 @@
+Metadata-Version: 2.1
+Name: starbug2
+Version: 0.4.1
+Summary: JWST PSF photometry in complex crowded fields.
+Author: Conor Nally
+Author-email: conor.nally@ed.ac.uk
+License: GNU General Public License v3.0
+Description-Content-Type: text/markdown
+
 # StarBugII
 
 JWST PSF photometry in dusty crowded fields.
-Last updated: v0.3.0
+Last updated: v0.4.1
 
 [![Python application](https://github.com/conornally/starbug2/actions/workflows/python-app.yml/badge.svg)](https://github.com/conornally/starbug2/actions/workflows/python-app.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/starbug2.svg)](https://pypi.python.org/pypi/starbug2/)
 [![Latest release](https://badgen.net/github/release/conornally/starbug2)](https://github.com/conornally/starbug2/releases)
 
 
 ## Installation
@@ -71,14 +80,26 @@
        --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
        --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
 
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
+
+
+StarbugII Matching 
+usage: starbug2-match [-BGfhv] [-o output] [-p file.param] [-s KEY=VAL] table.fits ...
+    -B  --band               : match in "BAND" mode (does not preserve a column for every frame)
+    -D  --dither             : match in "DITHER" mode (preserves a column for every frame)
+    -f  --full               : export full catalogue
+    -G  --generic            : match in "GENERIC" mode
+    -h  --help               : show help message
+    -o  --output  file.fits  : output matched catalogue
+    -p  --param   file.param : load starbug parameter file
+    -s  --set     option     : set value in parameter file at runtime (-s MATCH_THRESH=1)
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
```

### Comparing `starbug2-0.4.0/bin/starbug2` & `starbug2-0.4.1/bin/starbug2`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/bin/starbug2-match` & `starbug2-0.4.1/bin/starbug2-match`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/python3 -Wignore
-"""Starbug2 Matching
-usage: starbug2-match [-Bfhv] [-o output] [-p file.param] [-s KEY=VAL] table.fits ...
+"""StarbugII Matching 
+usage: starbug2-match [-BGfhv] [-o output] [-p file.param] [-s KEY=VAL] table.fits ...
     -B  --band               : match in "BAND" mode (does not preserve a column for every frame)
     -D  --dither             : match in "DITHER" mode (preserves a column for every frame)
     -f  --full               : export full catalogue
     -G  --generic            : match in "GENERIC" mode
     -h  --help               : show help message
     -o  --output  file.fits  : output matched catalogue
     -p  --param   file.param : load starbug parameter file
     -s  --set     option     : set value in parameter file at runtime (-s MATCH_THRESH=1)
 """
 
 import os,sys,getopt,glob
 import numpy as np
 import pkg_resources
 from astropy.io import fits
-from astropy.table import Table, hstack
+from astropy.table import Table, hstack, vstack
 import starbug2
 from starbug2 import utils
 from starbug2 import matching
 
 VERBOSE=0x01
 KILLPROC=0x02
 
@@ -30,15 +30,15 @@
 EXPFULL = 0x100
 
 options=0
 
 parameter={}
 pfile=None
 output=None
-setdict={}
+setopt={}
 
 def usage():
     if options& VERBOSE: quit(__doc__)
     else: quit( __doc__.split("\n")[1])
 
 opts,args=getopt.getopt(sys.argv[1:], "BDfGhvo:p:s:", ("band","dither","full", "generic", "help","verbose",
                                                 "output=", "param=", "set="))
@@ -53,54 +53,80 @@
 
 
     if opt in ("-s","--set"): 
         if '=' in optarg:
             key,val=optarg.split('=')
             try: val=float(val)
             except: pass
-            setdict[key]=val
+            setopt[key]=val
 
         else: perror("unable to set parameter, use syntax -s KEY=VALUE\n")
 
     if opt in ("-B","--band"): options|=BANDMATCH
     if opt in ("-D","--dither"): options|=DITHERMATCH
     if opt in ("-G","--generic"): options|=GENERICMATCH
 
 if not len(args): usage()
 
 if pfile: parameters=utils.load_params(pfile)
 elif os.path.exists("./starbug.param"): parameters=utils.load_params("./starbug.param")
 else: parameters=utils.load_params("%s/default.param"%pkg_resources.resource_filename("starbug2", "param/"))
 
-if parameters: parameters.update(setdict)
+if parameters: parameters.update(setopt)
 else: 
     utils.perror("failed to load parameter file\n")
     quit("..quitting :(")
 
 tables=[Table.read(fname,format="fits") for fname in args]
 
 colnames=starbug2.match_cols
 colnames+=[ name for name in parameters["MATCH_COLS"].split() if name not in colnames]
 dthreshold=parameters["MATCH_THRESH"]
 nthreshold=parameters["NEXP_THRESH"]
 rmmatch=parameters["RM_MATCH"]
 
 if options & BANDMATCH:
-    filters= [ tab.meta.get("FILTER") for tab in tables ]
-    efilters=["e%s"%f for f in filters]
-    matched=matching.band_match(tables,dthreshold,["RA","DEC",*filters,*efilters])
+    filters=[]
+    tomatch={ starbug2.NIRCAM:[], starbug2.MIRI:[] }
+    _colnames=["RA","DEC"]
+    for i,tab in enumerate(tables):
+        if not ( (fltr:=tab.meta.get("FILTER")) and fltr in list(starbug2.filters.keys())):
+            if not (fltr:= set(tab.colnames) & set(starbug2.filters.keys()) ):
+                perror("Unable to determine FILTER for \"%s\"\n"%args[i])
+                continue
+        filters.append(fltr)
+        tomatch[starbug2.filters[fltr].instr].append(tab)
+        _colnames+=([fltr,"e%s"%fltr])
+    
+    if tomatch[starbug2.NIRCAM] and tomatch[starbug2.MIRI]:
+        utils.printf("Detected NIRCam to MIRI matching\n")
+        nircam_matched=matching.band_match(tomatch[starbug2.NIRCAM], colnames=_colnames)
+        puts()
+        miri_matched=matching.band_match(tomatch[starbug2.MIRI], colnames=_colnames)
+        puts()
+
+        if not (lockcol:=parameters.get("LOCKCOL")):
+            lockcol= sorted([f for f in filters if starbug2.filters[f].instr==starbug2.NIRCAM],key=lambda f: list(starbug2.filters.keys()).index(f))[-1]
+        mask= np.isnan(nircam_matched[lockcol])
+        load=utils.loading(len(miri_matched), msg="Combining NIRCAM-MIRI(%.2g\")"%dthreshold)
+        matched,_=matching.generic_match((nircam_matched[~mask],miri_matched), threshold=dthreshold, add_src=True, load=load)
+        matched.remove_column("NUM")
+        matched=vstack((matched, nircam_matched[mask]))
+    else:
+        matched=matching.band_match(tables, colnames=_colnames)
+        
     fname=output if output else "out.fits"
     utils.export_table(matched,fname=fname)
 
 else:
     if options & DITHERMATCH: av,full=matching.dither_match(tables, threshold=dthreshold, colnames=colnames)
     if options & GENERICMATCH: 
         options|=EXPFULL
-        full=matching.generic_match(tables,threshold=dthreshold, add_src=True)
-        av=None#_=matching.finish_matching(full, colnames=tables[0].colnames)
+        av,full=matching.generic_match(tables,threshold=dthreshold, add_src=True)
+        #av=None#_=matching.finish_matching(full, colnames=tables[0].colnames)
     else:
         av,full=matching.cascade_match(tables, threshold=dthreshold, colnames=colnames)
 
     dtypes=[]
     for name in full.colnames:
         if name=="Catalogue_Number": dtypes.append(str)
         elif name=="flag": dtypes.append(np.uint16)
```

### Comparing `starbug2-0.4.0/extras/starbug2.completion` & `starbug2-0.4.1/extras/starbug2.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/starbug2/__init__.py` & `starbug2-0.4.1/starbug2/__init__.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/starbug2/matching.py` & `starbug2-0.4.1/starbug2/matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Primarily this is the main routines for dither/band/generic matching which are at the core
 of starbug2 and starbug2-matc
 """
 import numpy as np
 import astropy.io.fits as fits
 import astropy.units as u
 from astropy.coordinates import SkyCoord
-from astropy.table import Column, Table, hstack
+from astropy.table import Column, Table, hstack, vstack
 
 import starbug2
 from starbug2.utils import *
 
 def exp_info(hdulist):
     """
     Get the exposure information about a hdulist 
@@ -67,22 +67,14 @@
 
         out[info["FILTER"]][info["OBSERVTN"]][info["VISIT"]][info["DETECTOR"]].append(cat)
         #index= modules.index(info["DETECTOR"]) if info["DETECTOR"] in modules else -1
         #out[info["FILTER"]][info["OBSERVTN"]][info["VISIT"]][info["EXPOSURE"]][index] = cat
     return out
 
 def _match(cat1, cat2):
-    """
-    if not len(cat1) and len(cat2): 
-        n=len(cat2)
-        return np.array((range(n), sys.maxsize*np.ones(n)*u.degree, sys.maxsize*np.ones(n)))
-    if not len(cat2) and len(cat1): 
-        n=len(cat1)
-        return np.array((range(n), sys.maxsize*np.ones(n)*u.degree, sys.maxsize*np.ones(n)))
-    """
     _ra_cols= list( name for name in cat1.colnames if "RA" in name)
     _dec_cols= list( name for name in cat1.colnames if "DEC" in name)
     _ra= np.nanmean( tab2array( cat1, colnames=_ra_cols), axis=1) # this still breaks if the source isnt matched in all the columns, the 999 will increase the average
     _dec=np.nanmean( tab2array( cat1, colnames=_dec_cols), axis=1)
     skycoord1=SkyCoord( ra=_ra*u.deg, dec=_dec*u.deg)
 
     _ra_cols= list( name for name in cat2.colnames if "RA" in name)
@@ -94,41 +86,45 @@
     return skycoord2.match_to_catalog_3d(skycoord1)
 
 def generic_match(catalogues, threshold=0.25, add_src=True, load=None):
     """
     """
     threshold=threshold*u.arcsec
     base=Table(None)
+    colnames=[]
 
     for n,cat in enumerate(catalogues,1):
         if "Catalogue_Number" in cat.colnames: cat.remove_column("Catalogue_Number")
         if not len(base):
             tmp=cat.copy()
         else:
-            #tmp=Table(tmp,dtype=[float]*len(tmp.colnames)).filled(np.nan) ## fill empty values with null
             idx,d2d,_=_match(base,cat)
             tmp=Table(np.full( (len(base),len(cat.colnames)), np.nan), names=cat.colnames)
 
             for src,IDX,sep in zip(cat,idx,d2d):
                 if load:
                     load()
                     load.show()
                 if (sep<=threshold) and (sep==min(d2d[idx==IDX])): ## GOOD MATCH
                     tmp[IDX]=src
                 elif add_src:   ##BAD MATCH / NEW SOURCE
                     tmp.add_row( src )
-        tmp.rename_columns( tmp.colnames, ["%s_%d"%(name,n) for name in tmp.colnames] )
-        base=hstack((base,tmp))
-        #base=Table(base,dtype=[float]*len(base.colnames)).filled(np.nan) ## fill empty values with null
 
-    for colname in base.colnames:
-        basename=colname[:colname.rfind("_")]
-        all_cols=find_colnames(base,basename)
-        if len(all_cols)==1: base.rename_column(colname,basename)
-    return reindex(base)
+        #colnames |= set(tmp.colnames)
+        for name in tmp.colnames: 
+            if name not in colnames: colnames.append(name)
+        tmp.rename_columns( tmp.colnames, ["%s_%d"%(name,n) for name in tmp.colnames] )
+        base=hstack((base,tmp)).filled(np.nan)
+        
+    return finish_matching(base,colnames)
+    #for colname in base.colnames:
+    #    basename=colname[:colname.rfind("_")]
+    #    all_cols=find_colnames(base,basename)
+    #    if len(all_cols)==1: base.rename_column(colname,basename)
+    #return reindex(base)
 
 
 
 def dither_match(catalogues, threshold, colnames):
     """
     This is the match for when you simultaneously detect sources over
     a series of pipeline stage2 dithers and wich to combine it into a single catalogue
@@ -200,15 +196,22 @@
                     else: 
                         tmp.add_row(src[colnames]) ##i can purely use add_row to simplifiy the code
         tmp.rename_columns(colnames, list("%s_%d"%(name,n) for name in colnames))
         base=hcascade((base,tmp), colnames=colnames)
     base=Table(base,dtype=[float]*len(base.colnames)).filled(np.nan)
     return finish_matching(base, colnames)
 
-def band_match(catalogues, threshold, colnames):
+def nircam_miri_match(nircam, miri, nircam_lockcol="F444W", miri_lockcol=None):
+    """
+    Matching between a nircam catalogue and a miri catalogue
+    It optionally requires a source to be present in one column in each catalougue
+    """
+    pass
+
+def band_match(catalogues, colnames=("RA","DEC")):
     """
     Given a list of catalogues (with filter names in the meta data), match them
     in order of decreasing astrometric accuracy. 
     If F115W, F444W, F770W are input, the F115W centroid positions will be 
     taken as "correct". If a source is not resolved in this band, the next most 
     astrometrically accurate position is taken, i.e. F444W
     """
@@ -219,26 +222,31 @@
     for tab in catalogues:
         if "FILTER" in tab.meta.keys():
             if tab.meta["FILTER"] in starbug2.filters: 
                 ii=list(starbug2.filters.keys()).index(tab.meta["FILTER"])
                 tables[ii]=tab
                 mask[ii]=True
             else: perror("Unknown filter '%s' (skipping)..\n"%tab.meta["FILTER"])
+        elif (_tmp:=set(starbug2.filters.keys()) & set(tab.colnames)):
+            ii=list(starbug2.filters.keys()).index(_tmp.pop())
+            tables[ii]=tab
+            mask[ii]=True
         else: perror("Cannot find 'FILTER' in table meta (skipping)..\n")
     s="Bands: "
     for fltr,tab in zip(starbug2.filters.keys(),tables):
         if tab: s+="%5s "%fltr
         #else: s+=". "
     puts(s)
 
     ### Match in increasing wavelength order
     base=Table(None)
     load=loading(sum( [len(t) for t in tables[mask][1:]]),"matching", res=100)
     for fltr,tab in zip(starbug2.filters.keys(),tables):
         if not tab: continue
+        tab.remove_rows( np.isnan(tab[fltr]) ) ## removing empty magnitude rows
         load.msg="matching:%s"%fltr
         _colnames= list( name for name in tab.colnames if name in colnames)
         if not len(base): 
             tmp=tab[_colnames].copy()
         else:
             idx,d2d,_=_match(base,tab)
             tmp=Table(np.full( (len(base),len(_colnames)), np.nan), names=_colnames)
@@ -265,24 +273,24 @@
         #base=hstack(( base,tmp[["flux","eflux"]] ))
         #mag,magerr=flux2ABmag(tmp["flux"], tmp["eflux"],fltr)
         #base.add_column(mag,name=fltr)
         #base.add_column(magerr,name="e%s"%fltr)
 
         #base.rename_column("flux","%s_flux"%fltr)
         #base.rename_column("eflux","%s_eflux"%fltr)
-        base=hstack(( base,tmp[[fltr,"e%s"%fltr]] ))
+        base=hstack(( base,tmp[[fltr,"e%s"%fltr]] ))#.filled(np.nan)
         base=Table(base,dtype=[float]*len(base.colnames)).filled(np.nan)
 
         ### Only keep the most astromectrically correct position
         if "RA" not in base.colnames: base=hstack(( tmp[["RA","DEC"]], base))
         else:
             _mask=np.logical_and( np.isnan(base["RA"]), tmp["RA"]!=np.nan)
             base["RA"][_mask]=tmp["RA"][_mask]
             base["DEC"][_mask]=tmp["DEC"][_mask]
-    return base
+    return base.filled(np.nan)
 
 def stage_match(stage2, stage3, threshold):
     """
     Match together a stage 2 and stage 3 catalogue
     if the star is resolved in just the stage 3, it takes on that value
     if the star is resolved in both, the stage3 is ignored
     """
@@ -335,17 +343,18 @@
             col=Column(flags, name=name)
             for fcol in ar.T: col|=fcol.astype(np.uint16)
         elif name=="NUM":
             col=Column(np.nansum(ar, axis=1), name=name)
         else: col=Column(np.nanmedian(ar, axis=1),name=name)
         
         av[name]=col
-    mag,magerr=flux2ABmag(av["flux"],av["eflux"], tab.meta["FILTER"])
-    av.add_column(mag,name=tab.meta["FILTER"])
-    av.add_column(magerr,name="e%s"%tab.meta["FILTER"])
+    if len(set(["flux","eflux"])&set(av.colnames))==2:
+        mag,magerr=flux2ABmag(av["flux"],av["eflux"], tab.meta["FILTER"])
+        av.add_column(mag,name=tab.meta["FILTER"])
+        av.add_column(magerr,name="e%s"%tab.meta["FILTER"])
     if "NUM" not in av.colnames:
         narr= np.nansum( np.invert( np.isnan(tab2array(tab,find_colnames(tab,colnames[0])))),axis=1)
         av.add_column(Column(narr, name="NUM"))
     return (av,tab)
 
 
 def remove_NUM(tab, N):
```

### Comparing `starbug2-0.4.0/starbug2/misc.py` & `starbug2-0.4.1/starbug2/misc.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/starbug2/param/default.param` & `starbug2-0.4.1/starbug2/param/default.param`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/starbug2/routines.py` & `starbug2-0.4.1/starbug2/routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/starbug2/starbug.py` & `starbug2-0.4.1/starbug2/starbug.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/starbug2/utils.py` & `starbug2-0.4.1/starbug2/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -281,19 +281,37 @@
     Add indexes into a table
     """
     if "Catalogue_Number" in table.colnames: table.remove_column("Catalogue_Number")
     column=Column(["CN%d"%i for i in range(len(table))], name="Catalogue_Number")
     table.add_column(column,index=0)
     return table
 
+def colour_index(table,keys):
+    """
+    Allow table indexing with A-B
+    """
+    out=Table()
+    for key in keys:
+        if key in table.colnames: out.add_column(table[key])
+        elif '-' in key:
+            a,b=key.split('-')
+            out.add_column(table[a]-table[b],name=key)
+    return out
+
 def get_MJysr2Jy_scalefactor(ext):
     """
     Find the unit scale factor to convert an image from MJy/sr to Jy
     """
     scalefactor=1
     if ext.header["BUNIT"]=="MJy/sr":
         scalefactor=1e6*float(ext.header["PIXAR_SR"])
     return scalefactor
 
 
+
+
 if __name__ == "__main__":
     print(starbug2.logo)
+    t=Table.read("test/dat/image-ap.fits",format="fits")
+    print(colour_index( t, ("flux", "flux-eflux") ) )
+    #print(colour_index(t
+
```

### Comparing `starbug2-0.4.0/starbug2.egg-info/PKG-INFO` & `starbug2-0.4.1/starbug2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.4.0
+Version: 0.4.1
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
 
 JWST PSF photometry in dusty crowded fields.
-Last updated: v0.3.0
+Last updated: v0.4.1
 
 [![Python application](https://github.com/conornally/starbug2/actions/workflows/python-app.yml/badge.svg)](https://github.com/conornally/starbug2/actions/workflows/python-app.yml)
 [![PyPI version fury.io](https://badge.fury.io/py/starbug2.svg)](https://pypi.python.org/pypi/starbug2/)
 [![Latest release](https://badgen.net/github/release/conornally/starbug2)](https://github.com/conornally/starbug2/releases)
 
 
 ## Installation
@@ -80,14 +80,26 @@
        --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
        --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
 
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
+
+
+StarbugII Matching 
+usage: starbug2-match [-BGfhv] [-o output] [-p file.param] [-s KEY=VAL] table.fits ...
+    -B  --band               : match in "BAND" mode (does not preserve a column for every frame)
+    -D  --dither             : match in "DITHER" mode (preserves a column for every frame)
+    -f  --full               : export full catalogue
+    -G  --generic            : match in "GENERIC" mode
+    -h  --help               : show help message
+    -o  --output  file.fits  : output matched catalogue
+    -p  --param   file.param : load starbug parameter file
+    -s  --set     option     : set value in parameter file at runtime (-s MATCH_THRESH=1)
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
```

### Comparing `starbug2-0.4.0/tests/test_routines.py` & `starbug2-0.4.1/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.0/tests/test_utils.py` & `starbug2-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

