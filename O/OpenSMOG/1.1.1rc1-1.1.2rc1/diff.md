# Comparing `tmp/OpenSMOG-1.1.1rc1.tar.gz` & `tmp/OpenSMOG-1.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenSMOG-1.1.1rc1.tar", last modified: Mon Sep 19 22:53:35 2022, max compression
+gzip compressed data, was "OpenSMOG-1.1.2rc1.tar", last modified: Mon Jun 12 16:29:40 2023, max compression
```

## Comparing `OpenSMOG-1.1.1rc1.tar` & `OpenSMOG-1.1.2rc1.tar`

### file list

```diff
@@ -1,126 +1,290 @@
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.440249 OpenSMOG-1.1.1rc1/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1163 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/LICENSE
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       21 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/MANIFEST.in
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.432249 OpenSMOG-1.1.1rc1/OpenSMOG/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    55414 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/OpenSMOG.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6233 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/OpenSMOG_Reporter.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      172 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/__init__.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.432249 OpenSMOG-1.1.1rc1/OpenSMOG/share/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3369 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/OpenSMOG.xsd
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.432249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.436249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/energies
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23517 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.0.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.1.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.2.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.3.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.4.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.5.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.6.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.7.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.8.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.9.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)   169177 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/opentest.top
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    39684 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/opentest.xml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       75 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/smogcommands
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.436249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/energies
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.0.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.1.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.2.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.3.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.4.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.5.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.6.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.7.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.8.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.9.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)   169185 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/opentest.top
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    62444 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/opentest.xml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       83 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/smogcommands
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.436249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      116 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/energies
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.0.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.1.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.2.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.3.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.4.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.5.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.6.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.7.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.8.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.9.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    16208 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/opentest.top
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11053 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/opentest.xml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       75 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/smogcommands
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.436249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      110 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/energies
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.0.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.1.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.2.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.3.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.4.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.5.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.6.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.7.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.8.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.9.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    16216 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/opentest.top
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    15783 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/opentest.xml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       83 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/smogcommands
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.440249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/energies
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.0.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.1.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.10.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.2.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.3.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.4.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.5.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.6.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.7.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.8.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.9.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)   251521 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/opentest.top
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    36891 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/opentest.xml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       83 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/smogcommands
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.440249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/PDBs/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    42362 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/PDBs/2ci2.adj.pdb
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    37699 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/PDBs/DNA.terminal.BMG.pdb
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    19360 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/PDBs/RNA.adj.pdb
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.440249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      102 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/energies
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11502 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.0.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.1.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11507 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.10.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.2.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.3.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.4.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.5.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.6.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.7.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.8.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.9.gro
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    92635 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/opentest.top
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    16039 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/opentest.xml
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.440249 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2617 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.b
--rw-rw-r--   0 antonio   (1000) antonio   (1000)   211513 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.bif
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      765 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.extras
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      126 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.ions.def
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      719 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.nb
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3527 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.sif
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      326 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/smogcommands
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       72 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/listoftests
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2022-09-19 22:53:35.432249 OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6624 2022-09-19 22:53:35.000000 OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     4692 2022-09-19 22:53:35.000000 OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/SOURCES.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2022-09-19 22:53:35.000000 OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/dependency_links.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       47 2022-09-19 22:53:35.000000 OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/entry_points.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       11 2022-09-19 22:53:35.000000 OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/requires.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        9 2022-09-19 22:53:35.000000 OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/top_level.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2022-09-19 22:41:38.000000 OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/zip-safe
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6624 2022-09-19 22:53:35.440249 OpenSMOG-1.1.1rc1/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5872 2022-09-19 22:53:22.000000 OpenSMOG-1.1.1rc1/README.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       38 2022-09-19 22:53:35.440249 OpenSMOG-1.1.1rc1/setup.cfg
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1303 2022-09-19 22:41:05.000000 OpenSMOG-1.1.1rc1/setup.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.803424 OpenSMOG-1.1.2rc1/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1163 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/LICENSE
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       21 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/MANIFEST.in
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.775424 OpenSMOG-1.1.2rc1/OpenSMOG/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    54360 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/OpenSMOG.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6233 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/OpenSMOG_Reporter.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      172 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/__init__.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     8439 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/oscheck.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.779424 OpenSMOG-1.1.2rc1/OpenSMOG/share/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     4717 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/OpenSMOG.xsd
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.779424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.779424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23517 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   169177 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    39684 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       75 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.779424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.779424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/SBM_AA_dihe/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2722 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/SBM_AA_dihe/dihetest.b
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   211528 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/SBM_AA_dihe/dihetest.bif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      562 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/SBM_AA_dihe/dihetest.nb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2743 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/SBM_AA_dihe/dihetest.sif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23517 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23545 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/opentest.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    85151 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   207043 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      116 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD1/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.783424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.783424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/SBM_AA_dihe/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2734 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/SBM_AA_dihe/dihetest.b
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   211528 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/SBM_AA_dihe/dihetest.bif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      562 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/SBM_AA_dihe/dihetest.nb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2746 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/SBM_AA_dihe/dihetest.sif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23517 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23545 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/opentest.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    85142 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   207035 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      116 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CD4/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.783424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.783424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/SBM_AA+CustomDihedrals/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2527 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/SBM_AA+CustomDihedrals/test.b
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   211528 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/SBM_AA+CustomDihedrals/test.bif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      604 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/SBM_AA+CustomDihedrals/test.nb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3405 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/SBM_AA+CustomDihedrals/test.sif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23517 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23545 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/opentest.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    85185 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   160840 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      139 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.CustomDihedrals/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.787423 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      105 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23112 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23114 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    83468 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   201927 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       77 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.PBC/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.787423 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23532 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   169185 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    62444 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       83 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.787423 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      116 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    16208 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11053 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       75 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.791424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      110 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3012 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    16216 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    15783 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       83 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.791424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.10.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   251521 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    36891 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       83 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.791424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.791424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/SBM_AA_dihe/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2722 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/SBM_AA_dihe/dihetest.b
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   211528 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/SBM_AA_dihe/dihetest.bif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      562 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/SBM_AA_dihe/dihetest.nb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2743 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/SBM_AA_dihe/dihetest.sif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.10.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   161013 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   225764 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      127 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD1/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.795424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.795424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/SBM_AA_dihe/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2734 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/SBM_AA_dihe/dihetest.b
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   211528 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/SBM_AA_dihe/dihetest.bif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      562 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/SBM_AA_dihe/dihetest.nb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2746 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/SBM_AA_dihe/dihetest.sif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.10.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   161013 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   225764 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      127 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CD4/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.795424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.795424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/SBM_AA+CustomDihedrals/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2528 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/SBM_AA+CustomDihedrals/test.b
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   211528 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/SBM_AA+CustomDihedrals/test.bif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      604 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/SBM_AA+CustomDihedrals/test.nb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3166 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/SBM_AA+CustomDihedrals/test.sif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.10.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   161013 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   225764 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      150 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.799424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.799424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/SBM_AA+CustomDihedrals/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2447 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/SBM_AA+CustomDihedrals/test.b
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   211528 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/SBM_AA+CustomDihedrals/test.bif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      604 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/SBM_AA+CustomDihedrals/test.nb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3275 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/SBM_AA+CustomDihedrals/test.sif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.10.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    30912 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   161013 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   225764 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/opentest.xml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      151 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA.CustomDihedrals2/smogcommands
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.799424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/PDBs/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    42362 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/PDBs/2ci2.adj.pdb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    41637 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/PDBs/2ci2.split.pdb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    37699 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/PDBs/DNA.terminal.BMG.pdb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    19360 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/PDBs/RNA.adj.pdb
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.799424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      102 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/energies
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11502 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.0.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.1.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11507 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.10.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.2.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.3.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.4.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.5.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.6.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.7.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.8.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11506 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.9.gro
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    92635 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/opentest.top
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    16039 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/opentest.xml
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.799424 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2617 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.b
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   211513 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.bif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      765 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.extras
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      126 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.ions.def
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      719 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.nb
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3522 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.sif
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      326 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/smogcommands
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      217 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/listoftests
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-12 16:29:40.779424 OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6587 2023-06-12 16:29:40.000000 OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    12733 2023-06-12 16:29:40.000000 OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-06-12 16:29:40.000000 OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       47 2023-06-12 16:29:40.000000 OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/entry_points.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       11 2023-06-12 16:29:40.000000 OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/requires.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        9 2023-06-12 16:29:40.000000 OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/top_level.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-06-12 16:18:46.000000 OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/zip-safe
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6587 2023-06-12 16:29:40.803424 OpenSMOG-1.1.2rc1/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5872 2023-06-12 16:29:34.000000 OpenSMOG-1.1.2rc1/README.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       38 2023-06-12 16:29:40.803424 OpenSMOG-1.1.2rc1/setup.cfg
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1303 2023-06-12 16:06:41.000000 OpenSMOG-1.1.2rc1/setup.py
```

### Comparing `OpenSMOG-1.1.1rc1/LICENSE` & `OpenSMOG-1.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/OpenSMOG.py` & `OpenSMOG-1.1.2rc1/OpenSMOG/OpenSMOG.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright (c) 2020-2022 The Center for Theoretical Biological Physics (CTBP) - Rice University and Northeastern University
 # This file is from the OpenSMOG project, released under the MIT License. 
 
 R"""  
 The :class:`~.OpenSMOG` classes perform molecular dynamics using Structure-Based Models (SBM) for biomolecular simulations.
 :class:`~.OpenSMOG` uses force fields generated by SMOG 2, and it allows the simulations of a wide variety of potential forms, including commonly employed C-alpha and all-atom variants.
-Details about the default models in SMOG 2 can be found in the following resources:
+Details about the default models in SMOG 2 can be found at the following resource:
     - **SMOG server**: https://smog-server.org/smog2/
-    - **C-alpha**: Clementi, C., Nymeyer, H. and Onuchic, J.N., 2000. Topological and energetic factors: what determines the structural details of the transition state ensemble and “en-route” intermediates for protein folding? An investigation for small globular proteins. Journal of molecular biology, 298(5), pp.937-953.
-    - **All-Atom**: Whitford, P.C., Noel, J.K., Gosavi, S., Schug, A., Sanbonmatsu, K.Y. and Onuchic, J.N., 2009. An all‐atom structure‐based potential for proteins: bridging minimal models with all‐atom empirical forcefields. Proteins: Structure, Function, and Bioinformatics, 75(2), pp.430-441.
 """
 
 # with OpenMM 7.7.0, the import calls have changed. So, try both, if needed
 try:
     try:
         # >=7.7.0
         from openmm.app import *
@@ -31,20 +29,18 @@
 import numpy as np
 import xml.etree.ElementTree as ET
 from lxml import etree
 import sys
 from .OpenSMOG_Reporter import forcesReporter, stateReporter
 import re as regex
 from pathlib import Path
-from sys import stdout
-import subprocess
-from contextlib import redirect_stdout
+from .oscheck import SBMCHECK
 
 class SBM:
-    version="1.1.1rc1"
+    version="1.1.2rc1"
     R"""  
     The :class:`~.SBM` class performs Molecular dynamics simulations using structure-based (SMOG) models to investigate a broad range of biomolecular dynamics, including domain rearrangements in proteins, folding and ligand binding in RNA, and large-scale rearrangements in ribonucleoprotein assemblies. In its simplest form, a structure-based model defines a particular structure (usually obtained from X-ray, cryo-EM, or NMR methods) as the energetic global minimum. Find more information about SMOG models and OpenSMOG at http://smog-server.org 
     
     
     The :class:`~.SBM` sets the environment to start the molecular dynamics simulations.
     
     Args:
@@ -122,16 +118,39 @@
         self.forceApplied = False
         self.loaded = False
         self.folder = "."
         self.forceCount = 0
         self.pbc=pbc
         self.cmm=cmm
         self.nonbonded_present = False
-        self.setupCheck = False
-            
+
+# setup_openmm defaults
+        
+        self.forceDict = {}
+        self.forcesDict = {}
+ 
+        self.integrator = LangevinIntegrator(self.temperature,
+            self.gamma, self.dt)
+        self.integrator_type = 'langevin'
+
+        properties={}
+        properties["Precision"] = 'single'
+        self.properties = properties
+
+        plats = []
+        for i in range(Platform.getNumPlatforms()):
+            pn=Platform.getPlatform(i).getName()
+            plats.append(pn)
+
+        for tryplat in ['HIP','CUDA','OpenCL','CPU','Reference']:
+            if tryplat in plats:
+                self.platform = Platform.getPlatformByName(tryplat)
+                self.platformname=tryplat
+                break
+
     def help():
         R"""Prints information about using OpenSMOG.
         """
         print("""
 
 #############################################################################
 
@@ -149,15 +168,17 @@
 In terms of accounting, 1 \"ns\" is equal to 1000 reduced time units. For 
 detailed discussions of units, one can consult any number of recent papers 
 by the SMOG team, such as Yang et al. JCP 2019, 151, 085102, which estimated
 that one reduced unit corresponds to 50-1000 ps.
 
 Temperature: When initializing your simulation with the SBM class, the 
 temperature is provided in reduced units, where a typical protein will fold
-at around 1 reduced unit. 
+at around 1 reduced unit. For a detailed discussion of how one should
+interpret temperature in SMOG models, see Jackson et al. Int. J. Mol. Sci. 
+2015, 16, 6868-6889. 
 
 Energy: OpenSMOG will report all energies in reduced units. However, OpenMM 
 libraries may still label the energies as units of kJ/mol. This label should
 be ignored, unless you calibrated your SMOG model to use this energy scale. 
 
 
                                 Usage Example 
@@ -169,18 +190,19 @@
 
 Choose some basic runtime settings.  We will call our system 2ci2
 >SMOGrun = SBM(name='2ci2', time_step=0.002, collision_rate=1.0, r_cutoff=1.2, temperature=0.5)
 
 Note: By default, PBC is not turned on.  If you want to include PBCs, then use:
 >SMOGrun = SBM(name='2ci2', time_step=0.002, collision_rate=1.0, r_cutoff=1.2, temperature=0.5, pbc=True)
 
-Select a platform and GPU IDs (if needed)
+Select a platform and GPU IDs (if needed) - This is optional. If not given, then OpenSMOG will try to pick
+the fastest platform, and the precision will be set to single.
 >SMOGrun.setup_openmm(platform='cuda',GPUindex='default')
 
-Decide where to save your data (here, output_2ci2)
+Decide where to save your data (here, output_2ci2) - This is optional. If not given, will write to current dir.
 >SMOGrun.saveFolder('output_2ci2')
 
 You may optionally set some input file names to variables
 >SMOG_grofile = '2ci2.gro'
 >SMOG_topfile = '2ci2.top'
 >SMOG_xmlfile = '2ci2.xml'
 
@@ -209,20 +231,21 @@
 
 To save the state file:
 >statefilename='smog.state'
 >SMOGrun.simulation.saveState(statefilename)
 
 To save the checkpoint file:
 >checkpointfilename='smog.checkpoint'
->SMOGrun.saveCheckpoint(checkpointfilename)
+>SMOGrun.simulation.saveCheckpoint(checkpointfilename)
 
 If you saved a state or checkpoint in a previous run, here is an example 
 for how to continue the simulation. 
 >from OpenSMOG import SBM
 >SMOGrun2 = SBM(name='2ci2', time_step=0.002, collision_rate=1.0, r_cutoff=1.2, temperature=0.5)
+note: setup_openmm and saveFolder are optional
 >SMOGrun2.setup_openmm(platform='cuda',GPUindex='default')
 >SMOGrun2.saveFolder('output_2ci2')
 >SMOG_grofile = '2ci2.gro'
 >SMOG_topfile = '2ci2.top'
 >SMOG_xmlfile = '2ci2.xml'
 >SMOGrun2.loadSystem(Grofile=SMOG_grofile, Topfile=SMOG_topfile, Xmlfile=SMOG_xmlfile)
 >SMOGrun2.createSimulation()
@@ -246,109 +269,134 @@
 For more information and help, see the OpenSMOG and SMOG 2 websites.
 OpenSMOG: https://opensmog.readthedocs.io/en/latest/
 SMOG 2: https://smog-server.org
 
 If you have questions/suggestions, you can also email us at info@smog-server.org
 """) 
 
+    def opensmogcheck():
+        SBMCHECK.run()
 
     def opensmog_quit(message):
         print("\n\nOpenSMOG error: {}\n\n".format(message))
         sys.exit(1)
 
     def minimize(self,tolerance=1.0,maxIterations=0):
+        print("Starting minimization using L-BFGS method")
         R"""Wrapper for L-BFGS energy minimization.
 
          Args:
 
             tolerance (float, required):
                 Stopping criteria value between iterations. When the error between iteration is below this value, the minimization stops. (Default value: :code:`1.0`).
             maxIteration (int, required):
                 Number of maximum steps to be performed in the minimization simulation. (Default value: :code:`0`).   
         """
         self.simulation.minimizeEnergy(tolerance=tolerance,maxIterations=maxIterations)
         # it is very important that we reset the velocities. minimization warps the velocity values
         self.simulation.context.setVelocitiesToTemperature(self.temperature*kelvin)
+        print("Minimization completed")
 
-    def setup_openmm(self, platform='opencl', precision='single', GPUindex='default', integrator="langevin"):
+    def setup_openmm(self, platform="", precision="", GPUindex="", integrator=""):
         
         R"""Sets up the parameters of the simulation OpenMM platform.
+    This is optional.  If it is not used, then the following defaults will be used:
+        precision: single
+        integrator: Langevin
+        platform: a guess of the fastest platform available
+        GPUindex: Default
 
         Args:
 
             platform (str, optional):
                 Platform to use in the simulations. Opitions are *CUDA*, *OpenCL*, *HIP*, *CPU*, *Reference*. (Default value: :code:`OpenCL`). 
             precision (str, optional):
                 Numerical precision type of the simulation. Options are *single*, *mixed*, *double*. (Default value: :code:`single`).  For details check the `OpenMM Documentation <http://docs.openmm.org/latest/developerguide/developer.html#numerical-precision>`__. 
             GPUIndex (str, optional):
                 Set of Platform device index IDs. Ex: 0,1,2 for the system to use the devices 0, 1 and 2. 
             integrator (str, or integrator object):
                 Integrator to use in the simulations. Options are *langevin*, *langevinMiddle,  *variableLangevin* and, *brownian*. You may also build your own integrator object and pass it, rather than use a named integrator. (Default value: :code:`langevin`).
         """
 
-        precision = precision.lower()
-        if precision not in ["mixed", "single", "double"]:
-            SBM.opensmog_quit("Precision must be mixed, single or double")
-            
         properties = {}
-        properties["Precision"] = precision
-        if GPUindex.lower() != "default":
-            properties["DeviceIndex"] = GPUindex
+        if precision == "":
+            # use the default value that was set with _init_
+            properties["Precision"] = self.properties["Precision"]
+        else:
+            precision = precision.lower()
+            if precision not in ["mixed", "single", "double"]:
+                print("Precision must be mixed, single or double.\nTry running setup_openmm again.")
+                return
+            properties["Precision"] = precision
+
+        if GPUindex != "" and GPUindex.lower() != "default":
+            if isinstance(GPUindex,int):
+                 properties["DeviceIndex"] = GPUindex
+            else:
+                 print('Setup incomplete!\nGPUindex must be an integer. Given: {}\nTry rerunning setup_openmm again.'.format(GPUindex))
+                 return
             
         self.properties = properties
 
+        platslower = []
+        plats = []
+        for i in range(Platform.getNumPlatforms()):
+            pn=Platform.getPlatform(i).getName()
+            plats.append(pn)
+            platslower.append(pn.lower())
+        if not (platform.lower() in platslower):
+            print("\"{}\" is not a registered platform.\nRegistered platforms are:".format(platform))
+            for i in plats:
+                print("\t{}".format(i))
+            print("Try rerunning setup_openmm again.")
+            return    
+ 
         if platform.lower() == "opencl":
-            platformObject = Platform.getPlatformByName('OpenCL')
-
+            nametmp='OpenCL'
         elif platform.lower() == "reference":
-            platformObject = Platform.getPlatformByName('Reference')
+            nametmp='Reference'
             self.properties = {}
-
         elif platform.lower() == "cuda":
-            platformObject = Platform.getPlatformByName('CUDA')
-
+            nametmp='CUDA'
         elif platform.lower() == "cpu":
-            platformObject = Platform.getPlatformByName('CPU')
+            nametmp='CPU'
             self.properties = {}
-
         elif platform.lower() == "hip":
-            platformObject = Platform.getPlatformByName('HIP')
-
+            nametmp='HIP'
         else:
-            SBM.opensmog_quit("Unknown platform")
+            nametmp=platform
         
-        self.platform = platformObject
+        self.platform = Platform.getPlatformByName(nametmp)
+        self.platformname = nametmp
+
         if isinstance(integrator,str): 
             if integrator.lower() == "langevin":
                 self.integrator = LangevinIntegrator(self.temperature,
                     self.gamma, self.dt)
             elif integrator.lower() == "langevinmiddle": 
                 self.integrator = LangevinMiddleIntegrator(self.temperature,
                     self.gamma, self.dt)
             elif integrator.lower() == "variablelangevin": 
                 self.integrator = VariableLangevinIntegrator(self.temperature,
                     self.gamma, self.dt)
             elif integrator.lower() == "brownian": 
                 self.integrator = BrownianIntegrator(self.temperature,
                     self.gamma, self.dt)
-            else:
+            elif integrator != "": 
                 SBM.opensmog_quit("Unknown/unsupported integrator name: {}".format(integrator))
-            self.integrator_type = integrator
-                
+            if integrator != "": 
+                self.integrator_type = integrator
         else:
             self.integrator = integrator
             self.integrator_type = "UserDefined"
 
-        self.setupCheck = True  
-        self.forceDict = {}
-        self.forcesDict = {}
-        
     def saveFolder(self, folder):
 
         R"""Sets the folder path to save data.
+    This is option.  If not used, output will be written to current directory.
 
         Args:
 
             folder (str, required):
                 Folder path to save the simulation data. If the folder path does not exist, the function will create the directory. 
         """
         Path(folder).mkdir( parents=True, exist_ok=True )
@@ -377,28 +425,24 @@
                 return True
         
         if _checknames(Grofile, Topfile, Xmlfile) and  self.warn :
             print('WARNING: The Gro, Top and Xml files have different prefixes. Most people use the same name, so this may be a mistake.')
 
         self.inputNames = [Grofile, Topfile, Xmlfile]
 
-        if (self.setupCheck):
-
-            self._check_file(Grofile, '.gro')
-            self.loadGro(Grofile)
+        self._check_file(Grofile, '.gro')
+        self.loadGro(Grofile)
 
-            self._check_file(Topfile, '.top')
-            self.loadTop(Topfile)
+        self._check_file(Topfile, '.top')
+        self.loadTop(Topfile)
 
-            self._check_file(Xmlfile, '.xml')
-            self.loadXml(Xmlfile)
+        self._check_file(Xmlfile, '.xml')
+        self.loadXml(Xmlfile)
 
-            print("Loaded force field and config files.")
-        else:
-            SBM.opensmog_quit("setup_openmm() is not defined. Please set it before using LoadSystem()\n")
+        print("Loaded force field and config files.")
         
         
     def _check_file(self, filename, ext):
         if not (filename.lower().endswith(ext)):
             SBM.opensmog_quit('Wrong file extension: {} must to be {} extension'.format(filename, ext))
 
         
@@ -411,14 +455,15 @@
             Grofile (file, required):
                 Initial structure for the MD simulations in *.gro* file format. This is typically generated by SMOG2 with the flag :code:`-OpenSMOG`.  (Default value: :code:`None`).
         """
         if not os.path.exists(Grofile):
             SBM.opensmog_quit("Could not find gro file {}".format(Grofile))
            
         try:
+            print("Will try to load coordinates from {}".format(Grofile))
             self.Gro = GromacsGroFile(Grofile)
         except:
             SBM.opensmog_quit("Failed to load {}".format(Grofile))
 
     def loadTop(self, Topfile):
         R"""Loads the  *.top* file format in the OpenMM system platform. The input files are generated using SMOG2 software with the flag :code:`-OpenSMOG`. Details on how to create the files can be found in the `SMOG2 User Manual <https://smog-server.org/smog2/>`__.
         Tutorial on how to generate the inputs files can be found on the smog-server page, or `here <https://opensmog.readthedocs.io>`__.
@@ -427,14 +472,15 @@
 
             Topfile (file, required):
                 Topology *.top* file format generated by SMOG2 software with the flag :code:`-OpenSMOG`. The topology file defines the interactions between atoms, but the "Contacts" and nonbonded potentials can be provided with the *.xml* file. (Default value: :code:`None`).
         """
         if not os.path.exists(Topfile):
             SBM.opensmog_quit("Could not find top file {}".format(Topfile))
            
+        print("Will try to load force field from {}".format(Topfile))
         if self.pbc == True:
             print('This simulation will use periodic boundary conditions')
             self.Top = GromacsTopFile(Topfile,unitCellDimensions=self.Gro.getUnitCellDimensions())
             self.system = self.Top.createSystem(nonbondedMethod=CutoffPeriodic,nonbondedCutoff=self.rcutoff,removeCMMotion = self.cmm)
         else:
             print('This simulation will not use Periodic boundary conditions')
             self.Top = GromacsTopFile(Topfile)
@@ -459,17 +505,27 @@
         nb_data=self.data['nonbond']
         n_forces =  len(nb_data[0])
         forces = {}
         for n in range(n_forces):
             forces[nb_data[0][n]] = [nb_data[1][n], nb_data[2][n], nb_data[3][n]]
         self.nonbond = forces
 
-    def _customSmogForce(self, name, data):
+    def _splitForces_dihedrals(self):
+        #Custom Dihedrals
+        dihedrals_data=self.data['dihedrals']
+        n_forces =  len(dihedrals_data[3])
+        forces = {}
+        for n in range(n_forces):
+            forces[dihedrals_data[3][n]] = [dihedrals_data[0][n], dihedrals_data[1][n], dihedrals_data[2][n]]
+        self.dihedrals = forces
+
+    def _customSmogForce(self, name, data, pbc):
         #first set the equation
         contacts_ff = CustomBondForce(data[0])
+        contacts_ff.setUsesPeriodicBoundaryConditions(pbc)
 
         #second set the number of variable
         for pars in data[1]:
             contacts_ff.addPerBondParameter(pars)
 
         #third, apply the bonds from each pair of atoms and the related variables.
         pars = [pars for pars in data[1]]
@@ -484,14 +540,39 @@
         if self.constants_present==True:
             for const_key in self.data['constants']:
                 contacts_ff.addGlobalParameter(const_key,self.data['constants'][const_key])
         self.forcesDict[name] =  contacts_ff
         contacts_ff.setForceGroup(self.forceCount)
         self.forceCount +=1
 
+    def _customSmogForce_cd(self, name, data, pbc):
+        #first set the equation
+        dihedrals_ff = CustomTorsionForce(data[0])
+        dihedrals_ff.setUsesPeriodicBoundaryConditions(pbc)
+        #second set the number of variable
+        for pars in data[1]:
+            dihedrals_ff.addPerTorsionParameter(pars)
+
+        #third, apply the bonds from each pair of atoms and the related variables.
+        pars = [pars for pars in data[1]]
+
+        for iteraction in data[2]:
+            atom_index_i = int(iteraction['i'])-1 
+            atom_index_j = int(iteraction['j'])-1
+            atom_index_k = int(iteraction['k'])-1 
+            atom_index_l = int(iteraction['l'])-1
+            parameters = [float(iteraction[k]) for k in pars]
+
+            dihedrals_ff.addTorsion(atom_index_i, atom_index_j, atom_index_k, atom_index_l, parameters)
+
+        self.forcesDict[name] =  dihedrals_ff
+        dihedrals_ff.setForceGroup(self.forceCount)
+        self.forceCount +=1
+
+
     def _customSmogForce_nb(self, name, data):
         #first set the equation
         nonbond_ff = CustomNonbondedForce(data[0])
 
         #Define per particle parameters
         nonbond_ff.addPerParticleParameter('q')
         nonbond_ff.addPerParticleParameter('type')
@@ -575,17 +656,17 @@
         molecules_keys=[self.Top._molecules[i][0] for i in range(len(self.Top._molecules)) ]
         molecules_mul=[self.Top._molecules[i][1] for i in range(len(self.Top._molecules)) ]
         ## Loop over molecules
         for i in range(len(molecules_keys)):
             molecule=molecules_keys[i]
             mult=molecules_mul[i]
             # Loop over atoms in each molecule
-            for atom in self.Top._moleculeTypes[molecule].atoms:
-                # If atoms are repeated, then include the same entrie (CL,CL,CL,... or MG,MG,MG,...)
-                for _ in range(mult):
+            for _ in range(mult):
+                # If multiple copies of a molecule are defined in the system (in the top file), then include the atoms in that molecule multiple times. (CL,CL,CL,... or MG,MG,MG,... or CA, CB, CA, CB, CA, CB...). Notes, these two for loops were improperly nested in versions 1.1.1 and earlier
+                for atom in self.Top._moleculeTypes[molecule].atoms:
                     atom_types.append(atom[1])
         for i in range(self.system.getNumParticles()):
             # GET ATOM TYPE
             at_type=np.where(atom_types[i]==self.atom_types)[0][0]
             # GET ATOM CHARGE
             charge=atom_charges[i]
             # ADD PARTICLE TO EACH FORCE WITH CORRESPONDING CHARGE AND TYPE
@@ -608,14 +689,15 @@
 
         Args:
 
             Xmlfile (file, required):
                 The *.xml* file can contain information that defines the "Contact" and nonbonded potentials. The *.xml* file is generated by SMOG2 software with the flag :code:`-OpenSMOG`, which support custom potential energy functions. (Default value: :code:`None`).
         """
 
+        print("Will try to load OpenSMOG-specific force field terms from {}".format(Xmlfile))
         def validate(Xmlfile):
             path = "share/OpenSMOG.xsd"
             pt = os.path.dirname(os.path.realpath(__file__))
             filepath = os.path.join(pt,path)
 
             xmlschema_doc = etree.parse(filepath)
             xmlschema = etree.XMLSchema(xmlschema_doc)
@@ -628,15 +710,20 @@
             log = xmlschema.error_log
             return result,log
 
         def import_xml2OpenSMOG(file_xml):
             XML_potential = ET.parse(file_xml)
             root = XML_potential.getroot()
             xml_data={}
-
+            if 'OpenSMOGversion' in root.attrib:
+                OSv=root.attrib['OpenSMOGversion']
+                if OSv != SBM.version:
+                    print("WARNING: You are using OpenSMOG v{}, but the input SMOG2-generated XML file indidates that it is for use with v{}. You may want to use the current versions of OpenSMOG and SMOG 2.\n".format(SBM.version,OSv)) 
+            else:
+                print('WARNING: No OpenSMOG version listed in the XML file.  This probably means it was generated with a version of SMOG 2 that is earlier than 2.4.6. Your XML file should still be compatible with this version of OpenSMOG, but you may want to update your version of SMOG 2.')
             ## Constants
             self.constants_present=False
             if root.find('constants') != None:
                 self.constants_present=True
                 constants={}
                 constants_xml = root.find('constants')
                 for const in constants_xml.iter('constant'):
@@ -706,34 +793,74 @@
                     internal_NBParam=[]
                     for nbpar in nonbond_xml[i].iter('nonbond_param'):
                         internal_NBParam.append(nbpar.attrib)
                     NBParameters.append(internal_NBParam)
                 xml_data['nonbond']=[NonBond_Num,NBExpression,NBExpressionParameters,NBParameters]
             else:
                 self.nonbond_present=False
+
+
+            ## Custom Dihedrals 
+            CDForce_Names=[]
+            CDExpression=[]
+            CDParameters=[]
+            ijkl=[]
+            
+            self.dihedrals_present=False
+            if root.find('dihedrals') == None:
+                print('''        No dihedral definitions found in XML file. Will only use dihedral information provided in the top file''')
+            else:
+                self.dihedrals_present=True
+                dihedrals_xml=root.find('dihedrals')
+                for i in range(len(dihedrals_xml)):
+                    for name in dihedrals_xml[i].iter('dihedrals_type'):
+                        CDForce_Names.append(name.attrib['name'])
+
+                    for expr in dihedrals_xml[i].iter('expression'):
+                        CDExpression.append(expr.attrib['expr'])
+                        
+                    CDinternal_Param=[]
+                    for par in dihedrals_xml[i].iter('parameter'):
+                        CDinternal_Param.append(par.text)
+                    CDParameters.append(CDinternal_Param)
+
+                    internal_ijkl=[]
+                    for atoms_ijkl in dihedrals_xml[i].iter('interaction'):
+                            internal_ijkl.append(atoms_ijkl.attrib)
+                    ijkl.append(internal_ijkl)
+
+                xml_data['dihedrals']=[CDExpression,CDParameters,ijkl,CDForce_Names]
+
             return xml_data
 
         if not (self.forceApplied):
             result,log=validate(Xmlfile)
 
             if not result:
                 SBM.opensmog_quit("The xml file does not adhere to the required schema (same as that used by SMOG 2). Error message:\n\n"+str(log)+"\n\n This typically means your xml file was corrupted, or you are using an incompatible version of SMOG 2.  See smog-server.org for a list of OpenSMOG-SMOG2 versions that are compatible.")
             
             self.data = import_xml2OpenSMOG(Xmlfile)
             if self.contacts_present==True: 
                 self._splitForces_contacts()
                 for force in self.contacts:
-                    print("Creating Contacts force {:} from xml file".format(force))
-                    self._customSmogForce(force, self.contacts[force])
+                    print("        Creating Contacts force {:} from xml file".format(force))
+                    self._customSmogForce(force, self.contacts[force],self.pbc)
+                    self.system.addForce(self.forcesDict[force])
+
+            if self.dihedrals_present==True: 
+                self._splitForces_dihedrals()
+                for force in self.dihedrals:
+                    print("        Creating Dihedrals force {:} from xml file".format(force))
+                    self._customSmogForce_cd(force, self.dihedrals[force], self.pbc)
                     self.system.addForce(self.forcesDict[force])
             
             if self.nonbond_present==True: 
                 self._splitForces_nb()
                 for force in self.nonbond:
-                    print("Creating Nonbonded force {:} from xml file".format(force))
+                    print("        Creating Nonbonded force {:} from xml file.\n        This will replace any nonbonded definitions given in the .top file\n".format(force))
                     self._customSmogForce_nb(force, self.nonbond[force])
                     self.system.addForce(self.forcesDict['Nonbonded'+str(force)])
                 ## REMOVE OTHER NONBONDED FORCES
                 self.system.removeForce(0)
                 self.system.removeForce(0)
             
             self.forceApplied = True
@@ -876,15 +1003,15 @@
         self.started=1 
 
         R"""Run the molecular dynamics simulation.
 
         Args:
 
             nsteps (int, required):
-                 Number of steps to be performed in the simulation. (Default value: :code:`10**7`)
+                 Number of steps to be performed in the simulation. 
             report (bool, optional):
                 Whether to print the simulation progress. (Default value: :code:`True`).
             interval (int, optional):
                  Frequency to print the simulation progress. (Default value: :code:`10**4`)
         """
 
         if report:
@@ -966,204 +1093,39 @@
             f.write('\nOutput Files:\n')
             f.write('-------------\n')
             for n in self.outputNames:
                 f.write(os.path.basename(n)+"\n")
 
             sys.stdout = ori
 
-    # this is for testing that OpenSMOG and SMOG2 are working together.
-    # the interested user may also be interested in how to compare energies
-    def opensmogcheck():
-        # define some functions that will be used for testing purposes
-        def runSMOG(sysname):
-            # based on the sysname, find the flags and run SMOG2
-            with open(sysname+"smogcommands", "r") as f:
-                for line in f:
-                    pt = os.path.dirname(os.path.realpath(__file__))
-                    line=regex.sub("OSDIR", pt, line)
-        
-                    command = line.split()
-        
-                    try:
-                        out=subprocess.run(command,stdout=subprocess.PIPE,stderr=subprocess.PIPE,check=True)    
-                    except subprocess.CalledProcessError as e:
-                        print("SMOG 2 failed to generate OpenSMOG input!!!!\n")
-                        print("STDERR:\n")
-                        print((e.stderr).decode())
-                        print("STDOUT:\n")
-                        print((e.stdout).decode())
-                        sys.exit(1)    
-        
-        
-        def prepOpenSMOG(runsmog,sysname,platform,PBC):
-            # make and return a system.
-            if runsmog:
-                topname="opentest.top"
-                xmlname="opentest.xml"
-            else:
-                topname=sysname+"opentest.top"
-                xmlname=sysname+"opentest.xml"
-        
-        
-            f = open(os.devnull, 'w')
-            with redirect_stdout(f):
-                sbm_test = SBM(name='testss', time_step=0.002, collision_rate=1.0, r_cutoff=2, temperature=0.1, pbc = PBC, warn = False)
-                sbm_test.setup_openmm(platform=platform,GPUindex='default')
-                sbm_test.saveFolder('.')
-                sbm_test.loadSystem(Grofile=sysname+"frame.0.gro", Topfile=topname, Xmlfile=xmlname)
-                sbm_test.createSimulation()
-            return sbm_test
-        
-        def comparevalues(ref,open):
-            absdiff=abs(float(ref)-float(open))
-            reldiff=abs(absdiff/float(ref))
-            if absdiff < maxabsdiff or reldiff < maxreldiff:
-                return 1
-            else:
-                print("BAD VALUES:"+ref.rstrip()+" (reference) and "+open+" (OpenSMOG)")
-                return 0 
-        
-        def which(exe):
-            for dir in os.getenv("PATH").split(':'):
-                if (os.path.exists(os.path.join(dir, exe))):
-                    print ('SMOG2 version found:%s/%s\n' % (dir, exe))
-                    return 1
-        
-            print ('''
-NOTE: Did not find smog2 in path. Will test OpenSMOG library,
-but not the generation of force fields with SMOG2.  Use
-smog-check to ensure SMOG 2 is also functioning properly.
-''')
-            return 0    
-       
-        # maxreldiff is the max relative deviation allowed
-        maxreldiff=0.00001
-        # maxabsdiff is the max absolute deviation allowed
-        maxabsdiff=0.002
-        
-        
-        # The name of each test is listed in tests/listoftests
-        # each line defines a test, which is a subdir of tests/
-        # each subdirectory has a "flags" file that gives the exact 
-        # flags used when calling smog2
-        # energies contains the gromacs-generated (or any reference 
-        # calculation) energies for the 10 frame..gro files
-        
-        print(
-'''
-                       OpenSMOG-check
-
-This will use the version of SMOG2 that is found in the path and 
-try to generate OpenSMOG force fields. It will then calculate the 
-energy using the OpenSMOG force field for reference configurations 
-of each system. Finally, it will check if the potential energies
-are the same as a set of predefined reference values (typically 
-from Gromacs).
-''') 
-
-
-        # nummatch is the total number of energies that 
-        # will need to be close, in order to pass
-        # it is incremented as tests are applied
-        nummatch=0
-        # mcount is the number of matching energies
-        mcount=0
-    
-        runsmog = which("smog2")
-        print('What platform would you like to test?')
-        print("\tOptions: OpenCL, HIP, CUDA, CPU, reference")
-        plats = ['opencl', 'hip', 'cuda', 'cpu', 'reference']
-        for line in sys.stdin:
-            platform = line.rstrip()
-            break
-        if not (platform.lower() in plats):
-            print('''Unrecognized platform! 
-Options are (case-insensitive): 
-OpenCL, HIP, CUDA, CPU, reference
-
-Unable to perform tests.
-''')
-            sys.exit(1)    
-    
-        print("Will test platform \""+platform+"\"\n")
-        listoftests = "share/tests/listoftests"
-        pt = os.path.dirname(os.path.realpath(__file__))
-        listoftests = os.path.join(pt,listoftests)
-    
-        list = open(listoftests, "r")
-    
-        for testname in list:
-            testname=testname.strip()
-    
-            PBC=False
-            if regex.search(".PBC$",testname):
-                PBC=True
-    
-            sysname = "share/tests/"+testname+"/"
-            pt = os.path.dirname(os.path.realpath(__file__))
-            sysname = os.path.join(pt,sysname)
-            nummatch+=10
-            print("STARTING TEST FOR SYSTEM IN "+testname)
-            if runsmog:
-                runSMOG(sysname)
-            sbm_test = prepOpenSMOG(runsmog,sysname,platform,PBC)
-            energies = open(sysname+"energies", "r")
-            for frame in range(10):
-                newgro = app.GromacsGroFile(sysname+"frame."+str(frame)+".gro")
-                sbm_test.simulation.context.setPositions(newgro.positions)
-                new=newgro.getPeriodicBoxVectors()
-                sbm_test.simulation.context.setPeriodicBoxVectors(new[0],new[1],new[2])
-                e_pot_frame = sbm_test.simulation.context.getState(getEnergy=True).getPotentialEnergy()
-                num=str(e_pot_frame).split(" ",1)[0]
-                openv=energies.readline()
-                mcount += comparevalues(openv,num)
-            print("COMPLETED TEST FOR SYSTEM IN "+testname+"\n")
-                    # these two lines can be uncommented, if we want to regenerate the reference templates for fall-back option
-            #subprocess.run("cp opentest.xml "+sysname,shell=True)
-            #subprocess.run("cp opentest.top "+sysname,shell=True)
-                    ##############
-            if runsmog:
-                subprocess.run('rm opentest*',shell=True)
-    
-        print(str(mcount) + " of " + str(nummatch) + " values matched")
-    
-        if nummatch == 0:    
-            print("\n\nNO TESTS PERFORMED.  SOMETHING WENT WRONG!!!!\n\n")
-            sys.exit(1)    
-        elif mcount == nummatch:
-            print("\n\nPASSED ALL CHECKS!!!!\n\n")
-            sys.exit(0)    
-        else: 
-            print("\n\nFAILED CHECKS!!!!\n\n")
-            sys.exit(1)    
-    
             
 #end of subroutines
 
 
     print('{:^96s}'.format("****************************************************************************************"))
     print('{:^96s}'.format("**** *** *** *** *** *** *** *** OpenSMOG (v"+version+") *** *** *** *** *** *** *** ****"))
     print('')
-    print('{:^96s}'.format("The OpenSMOG classes are used to perform molecular dynamics simulations using"))
+    print('{:^96s}'.format("The OpenSMOG class is used to perform molecular dynamics simulations using"))
     print('{:^96s}'.format("Structure-Based Models (SBM) for biomolecular systems,"))
     print('{:^96s}'.format("and it allows for the simulation of a wide variety of potential forms."))
     print('{:^96s}'.format("OpenSMOG uses force field files generated by SMOG 2."))
-    print('{:^96s}'.format("OpenSMOG documentation is available at https://opensmog.readthedocs.io"))
+    print('{:^96s}'.format("OpenSMOG documentation is available at"))
+    print('{:^96s}'.format("https://opensmog.readthedocs.io and https://smog-server.org"))
     print('')
     print('{:^96s}'.format("OpenSMOG is described in: Oliveira and Contessoto et al,"))
     print('{:^96s}'.format("SMOG 2 and OpenSMOG: Extending the limits of structure-based models."))
     print('{:^96s}'.format("Protein Science, 31, 158-172 (2022) DOI:10.1002/pro.4209"))
     print('')
     print('{:^96s}'.format("This package is the product of contributions from a number of people, including:"))
     print('{:^96s}'.format("Jeffrey Noel, Mariana Levi, Antonio Oliveira, Vinícius Contessoto,"))
     print('{:^96s}'.format("Esteban Dodero-Rojas, Mohit Raghunathan, Joyce Yang, Prasad Bandarkar,"))
     print('{:^96s}'.format("Udayan Mohanty, Ailun Wang, Heiko Lammert, Ryan Hayes,"))
     print('{:^96s}'.format("Jose Onuchic & Paul Whitford"))
     print('')
-    print('{:^96s}'.format("Copyright (c) 2021, The SMOG development team at"))
+    print('{:^96s}'.format("Copyright (c) 2021, 2022, The SMOG development team at"))
     print('{:^96s}'.format("Rice University and Northeastern University"))
     print("\n\n")
     print('{:^96s}'.format("For more information, including descriptions of units and examples of"))
     print('{:^96s}'.format("how to launch a simulation with OpenSMOG, issue the command SBM.help()"))
     print('{:^96s}'.format("To check your installation of OpenSMOG/SMOG2, use SBM.opensmogcheck()"))
     print('{:^96s}'.format("Additional information available at https://smog-server.org"))
     print('{:^96s}'.format("****************************************************************************************"))
```

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/OpenSMOG_Reporter.py` & `OpenSMOG-1.1.2rc1/OpenSMOG/OpenSMOG_Reporter.py`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.0.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.0.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.1.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.1.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.2.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.2.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.3.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.3.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.4.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.4.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.5.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.5.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.6.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.6.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.7.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.7.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.8.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.8.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/frame.9.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/frame.9.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/opentest.top` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/opentest.top`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA/opentest.xml` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA/opentest.xml`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.0.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.0.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.1.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.1.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.2.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.2.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.3.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.3.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.4.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.4.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.5.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.5.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.6.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.6.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.7.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.7.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.8.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.8.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.9.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/frame.9.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/opentest.top` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/opentest.top`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/opentest.xml` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.AA.gaussian/opentest.xml`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.0.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.0.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.1.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.1.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.2.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.2.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.3.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.3.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.4.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.4.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.5.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.5.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.6.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.6.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.7.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.7.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.8.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.8.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/frame.9.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/frame.9.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/opentest.top` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/opentest.top`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA/opentest.xml` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA/opentest.xml`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.0.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.0.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.1.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.1.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.2.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.2.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.3.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.3.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.4.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.4.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.5.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.5.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.6.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.6.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.7.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.7.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.8.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.8.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.9.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/frame.9.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/opentest.top` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/opentest.top`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/opentest.xml` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/2ci2.CA.gaussian/opentest.xml`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.0.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.0.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.1.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.1.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.10.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.10.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.2.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.2.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.3.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.3.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.4.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.4.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.5.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.5.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.6.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.6.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.7.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.7.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.8.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.8.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.9.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/frame.9.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/opentest.top` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/opentest.top`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/DNA-BMG.AA/opentest.xml` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/DNA-BMG.AA/opentest.xml`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/PDBs/2ci2.adj.pdb` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/PDBs/2ci2.adj.pdb`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/PDBs/DNA.terminal.BMG.pdb` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/PDBs/DNA.terminal.BMG.pdb`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/PDBs/RNA.adj.pdb` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/PDBs/RNA.adj.pdb`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.0.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.0.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.1.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.1.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.10.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.10.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.2.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.2.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.3.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.3.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.4.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.4.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.5.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.5.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.6.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.6.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.7.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.7.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.8.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.8.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/frame.9.gro` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/frame.9.gro`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/opentest.top` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/opentest.top`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/opentest.xml` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/opentest.xml`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.b` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.b`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.bif` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.bif`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.extras` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.extras`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.nb` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.nb`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.sif` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.sif`

 * *Files 1% similar despite different names*

#### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.sif` & `OpenSMOG-1.1.2rc1/OpenSMOG/share/tests/RNAion.PBC/sbm.test/test.sif`

```diff
@@ -53,9 +53,9 @@
     <!-- NOTE: If another template is provided with the -t_contacts flag, then these settings will be ignored-->
     <Contacts method="shadow" contactDistance="6" shadowRadius="1" shadowRadiusBonded="0.5"/>
     <bondsThreshold shortBond="0.08" longBond="0.2"/>
     <anglesThreshold smallAngles="90" largeAngles="140"/>
     <contactsThreshold shortContacts="0.1"/>
   </settings>
   <!-- Custom Potential Info -->
-  <CustomNonBonded OpenSMOGparameters="C6,C12,C18,B1,C1,R1,B2,C2,R2,B3,C3,R3,B4,C4,R4,B5,C5,R5" OpenSMOGcombrule=" none " OpenSMOGpotential="K_coul*q1*q2/dielectric*(1/r-1/r_c)    +(1-2*select(C18,1,0))*C12*(1/r^12-1/r_c^12)    +C18*(1/r^18-1/r_c^18)    +B1*exp(-C1*(r-R1)^2)    +B2*exp(-C2*(r-R2)^2)    +B3*exp(-C3*(r-R3)^2)    +B4*exp(-C4*(r-R4)^2)    +B5*exp(-C5*(r-R5)^2)    " nbcutoff="2.0"/>
+  <CustomNonBonded OpenSMOGparameters="C6,C12,C18,B1,C1,R1,B2,C2,R2,B3,C3,R3,B4,C4,R4,B5,C5,R5" OpenSMOGcombrule=" none " OpenSMOGpotential="K_coul*q1*q2/dielectric*(1/r-1/r_c)    +(1-2*select(C18,1,0))*C12*(1/r^12-1/r_c^12)    +C18*(1/r^18-1/r_c^18)    +B1*exp(-C1*(r-R1)^2)    +B2*exp(-C2*(r-R2)^2)    +B3*exp(-C3*(r-R3)^2)    +B4*exp(-C4*(r-R4)^2)    +B5*exp(-C5*(r-R5)^2)    " r_c="2.0"/>
 </sif>
```

### Comparing `OpenSMOG-1.1.1rc1/OpenSMOG.egg-info/PKG-INFO` & `OpenSMOG-1.1.2rc1/OpenSMOG.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: OpenSMOG
-Version: 1.1.1rc1
+Version: 1.1.2rc1
 Summary: Structure-based Models for Biomolecules using OpenMM
 Home-page: https://github.com/smog-server/OpenSMOG
 Author: ['Antonio Bento de Oliveira Junior', 'Vinicius de Godoi Contessoto']
 Author-email: antonio.oliveira@rice.edu,contessoto@rice.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
@@ -170,9 +168,7 @@
 Resources
 =========
 
 - `Reference Documentation <https://opensmog.readthedocs.io/>`__: Examples, tutorials, and class details.
 - `Installing OpenSMOG <https://opensmog.readthedocs.io/en/latest/GettingStarted/install.html#installing-opensmog>`__: Instructions for installing **OpenSMOG**.
 - `Installing SMOG2 <https://opensmog.readthedocs.io/en/latest/GettingStarted/install.html#installing-smog2>`__: Instructions for installing **SMOG2**.
 - `Issue tracker <https://github.com/smog-server/OpenSMOG/issues>`__: Report issues/bugs or request features.
-
-
```

### Comparing `OpenSMOG-1.1.1rc1/PKG-INFO` & `OpenSMOG-1.1.2rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: OpenSMOG
-Version: 1.1.1rc1
+Version: 1.1.2rc1
 Summary: Structure-based Models for Biomolecules using OpenMM
 Home-page: https://github.com/smog-server/OpenSMOG
 Author: ['Antonio Bento de Oliveira Junior', 'Vinicius de Godoi Contessoto']
 Author-email: antonio.oliveira@rice.edu,contessoto@rice.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
@@ -170,9 +168,7 @@
 Resources
 =========
 
 - `Reference Documentation <https://opensmog.readthedocs.io/>`__: Examples, tutorials, and class details.
 - `Installing OpenSMOG <https://opensmog.readthedocs.io/en/latest/GettingStarted/install.html#installing-opensmog>`__: Instructions for installing **OpenSMOG**.
 - `Installing SMOG2 <https://opensmog.readthedocs.io/en/latest/GettingStarted/install.html#installing-smog2>`__: Instructions for installing **SMOG2**.
 - `Issue tracker <https://github.com/smog-server/OpenSMOG/issues>`__: Report issues/bugs or request features.
-
-
```

### Comparing `OpenSMOG-1.1.1rc1/README.rst` & `OpenSMOG-1.1.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `OpenSMOG-1.1.1rc1/setup.py` & `OpenSMOG-1.1.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from os import path
 
 this_dir = path.abspath(path.dirname(__file__))
 with open(path.join(this_dir, "README.rst")) as f:
     long_description = f.read()
 
-__version__ = "1.1.1rc1"
+__version__ = "1.1.2rc1"
 for line in open(path.join("OpenSMOG", "__init__.py")):
     if line.startswith("__version__"):
         exec(line.strip())
 
 setup(
     name="OpenSMOG",
     version=__version__,
```

