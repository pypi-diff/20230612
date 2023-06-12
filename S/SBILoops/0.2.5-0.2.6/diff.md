# Comparing `tmp/SBILoops-0.2.5.tar.gz` & `tmp/SBILoops-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBILoops-0.2.5.tar", last modified: Fri Jun  9 18:19:54 2023, max compression
+gzip compressed data, was "SBILoops-0.2.6.tar", last modified: Mon Jun 12 15:14:39 2023, max compression
```

## Comparing `SBILoops-0.2.5.tar` & `SBILoops-0.2.6.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.105078 SBILoops-0.2.5/
--rw-r--r--   0 patrick    (501) staff       (20)       84 2023-06-08 19:32:47.000000 SBILoops-0.2.5/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-09 18:19:54.107233 SBILoops-0.2.5/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 22:00:16.000000 SBILoops-0.2.5/README.md
--rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-09 18:19:54.108826 SBILoops-0.2.5/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)      620 2023-06-09 18:18:26.000000 SBILoops-0.2.5/setup.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.797863 SBILoops-0.2.5/src/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.811051 SBILoops-0.2.5/src/SBILoops/
--rw-r--r--   0 patrick    (501) staff       (20)    12913 2023-06-09 18:18:48.000000 SBILoops-0.2.5/src/SBILoops/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.838497 SBILoops-0.2.5/src/SBILoops/beans/
--rw-r--r--   0 patrick    (501) staff       (20)     4502 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/beans/Executable.py
--rw-r--r--   0 patrick    (501) staff       (20)    11705 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/beans/File.py
--rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/beans/IndexedNum.py
--rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/beans/JSONer.py
--rw-r--r--   0 patrick    (501) staff       (20)    14934 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/beans/Path.py
--rw-r--r--   0 patrick    (501) staff       (20)     2928 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/beans/StorableObject.py
--rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/beans/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2.5/src/SBILoops/beans/butler.py
--rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/beans/singleton.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.853344 SBILoops-0.2.5/src/SBILoops/data/
--rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/data/Alphabet.py
--rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/data/AminoAcids.py
--rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/data/AtomVariants.py
--rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/data/Element.py
--rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/data/Properties.py
--rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/data/SetDict.py
--rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/data/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.891369 SBILoops-0.2.5/src/SBILoops/databases/
--rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/databases/CATHlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     8418 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/DrugBanklink.py
--rw-r--r--   0 patrick    (501) staff       (20)    13623 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/Enzymelink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5579 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/GOlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5361 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/PDBTMlink.py
--rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/databases/PDBeChemConnect.py
--rw-r--r--   0 patrick    (501) staff       (20)     6723 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/PDBeChemlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     9135 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/PDBlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     1801 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/SCOPlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5741 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/TaxIDlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7108 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7073 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/__Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/databases/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7155 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/dblink.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.898149 SBILoops-0.2.5/src/SBILoops/databases/uniprot/
--rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/databases/uniprot/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4783 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/uniprot/connect.py
--rw-r--r--   0 patrick    (501) staff       (20)     8173 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/databases/uniprot/uniprot.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.907661 SBILoops-0.2.5/src/SBILoops/error/
--rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/error/BlastError.py
--rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/error/FileError.py
--rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/error/SeqAliError.py
--rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/error/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.915163 SBILoops-0.2.5/src/SBILoops/external/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.926621 SBILoops-0.2.5/src/SBILoops/external/CDhit/
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/external/CDhit/CDhit.py
--rw-r--r--   0 patrick    (501) staff       (20)     2261 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/external/CDhit/CDhitExe.py
--rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/external/CDhit/CDhitHomolog.py
--rw-r--r--   0 patrick    (501) staff       (20)     2227 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/external/CDhit/CDhitList.py
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/external/CDhit/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.933703 SBILoops-0.2.5/src/SBILoops/external/DSSP/
--rw-r--r--   0 patrick    (501) staff       (20)     3326 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/external/DSSP/DSSP.py
--rw-r--r--   0 patrick    (501) staff       (20)     3608 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/external/DSSP/DSSPExe.py
--rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/external/DSSP/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      338 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/external/README.md
--rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/external/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.945331 SBILoops-0.2.5/src/SBILoops/external/blast/
--rw-r--r--   0 patrick    (501) staff       (20)     9121 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/external/blast/BlastExe.py
--rw-r--r--   0 patrick    (501) staff       (20)    12572 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/external/blast/BlastHit.py
--rw-r--r--   0 patrick    (501) staff       (20)    23494 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/external/blast/BlastResult.py
--rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/external/blast/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     8076 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/external/blast/blast_parser.py
--rw-r--r--   0 patrick    (501) staff       (20)      312 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/external/configSBI.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.950159 SBILoops-0.2.5/src/SBILoops/math/
--rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/math/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/math/stats.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.960166 SBILoops-0.2.5/src/SBILoops/sequence/
--rw-r--r--   0 patrick    (501) staff       (20)     6337 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/sequence/Fasta.py
--rw-r--r--   0 patrick    (501) staff       (20)     4877 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/sequence/IndexedSeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)    15049 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/sequence/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/sequence/Sequence.py
--rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/sequence/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.969796 SBILoops-0.2.5/src/SBILoops/sequence/alignment/
--rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/sequence/alignment/Needleman_Wunsch.py
--rw-r--r--   0 patrick    (501) staff       (20)    43530 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/sequence/alignment/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/sequence/alignment/SimilarityMatrix.py
--rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/sequence/alignment/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.979294 SBILoops-0.2.5/src/SBILoops/structure/
--rw-r--r--   0 patrick    (501) staff       (20)    20850 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/PDB.py
--rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.990819 SBILoops-0.2.5/src/SBILoops/structure/atom/
--rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/atom/Atom.py
--rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/atom/AtomOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/atom/AtomOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     3764 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/atom/AtomSeries.py
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/atom/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.007348 SBILoops-0.2.5/src/SBILoops/structure/chain/
--rw-r--r--   0 patrick    (501) staff       (20)    19968 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/chain/Chain.py
--rw-r--r--   0 patrick    (501) staff       (20)    13270 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/chain/ChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)     2765 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/chain/ChainOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     6879 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/chain/ChainOfProtein.py
--rw-r--r--   0 patrick    (501) staff       (20)     4992 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/chain/ProteinChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/chain/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.014667 SBILoops-0.2.5/src/SBILoops/structure/contacts/
--rw-r--r--   0 patrick    (501) staff       (20)     9012 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/Complex.py
--rw-r--r--   0 patrick    (501) staff       (20)     3410 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/InnerContacts.py
--rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.026399 SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/
--rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/Contact.py
--rw-r--r--   0 patrick    (501) staff       (20)     3808 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/ContactAA.py
--rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/ContactAH.py
--rw-r--r--   0 patrick    (501) staff       (20)     3277 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/ContactAN.py
--rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.033053 SBILoops-0.2.5/src/SBILoops/structure/contacts/inner/
--rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/inner/PHInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/inner/PPInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/inner/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.044915 SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/
--rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/Interface.py
--rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/PHInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    11117 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/PNInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/PPInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.050823 SBILoops-0.2.5/src/SBILoops/structure/geometry/
--rw-r--r--   0 patrick    (501) staff       (20)    11104 2023-06-09 18:18:01.000000 SBILoops-0.2.5/src/SBILoops/structure/geometry/RMSD.py
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-06-08 18:05:00.000000 SBILoops-0.2.5/src/SBILoops/structure/geometry/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      662 2023-06-08 18:05:43.000000 SBILoops-0.2.5/src/SBILoops/structure/geometry/basics.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.074576 SBILoops-0.2.5/src/SBILoops/structure/header/
--rw-r--r--   0 patrick    (501) staff       (20)     2284 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/BioMolecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     3831 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/DBreference.py
--rw-r--r--   0 patrick    (501) staff       (20)     2015 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/Experiment.py
--rw-r--r--   0 patrick    (501) staff       (20)    14756 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/Header.py
--rw-r--r--   0 patrick    (501) staff       (20)     1201 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/HeteroAtom.py
--rw-r--r--   0 patrick    (501) staff       (20)      948 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/MiniRes.py
--rw-r--r--   0 patrick    (501) staff       (20)     7647 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/Molecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     8534 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     2423 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/Site.py
--rw-r--r--   0 patrick    (501) staff       (20)    18695 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/header/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    14370 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/parse_mmCIF.py
--rw-r--r--   0 patrick    (501) staff       (20)     8543 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/parse_pdb.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.090331 SBILoops-0.2.5/src/SBILoops/structure/protein/
--rw-r--r--   0 patrick    (501) staff       (20)    19074 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/protein/Arch.py
--rw-r--r--   0 patrick    (501) staff       (20)    19202 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/protein/SShelper.py
--rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/protein/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/protein/Sequencer.py
--rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/protein/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:54.102513 SBILoops-0.2.5/src/SBILoops/structure/residue/
--rw-r--r--   0 patrick    (501) staff       (20)    10773 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/residue/Residue.py
--rw-r--r--   0 patrick    (501) staff       (20)    10725 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/residue/ResidueOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)     5359 2023-06-05 21:34:52.000000 SBILoops-0.2.5/src/SBILoops/structure/residue/ResidueOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2.5/src/SBILoops/structure/residue/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 18:19:53.817550 SBILoops-0.2.5/src/SBILoops.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-09 18:19:53.000000 SBILoops-0.2.5/src/SBILoops.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     4981 2023-06-09 18:19:53.000000 SBILoops-0.2.5/src/SBILoops.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-09 18:19:53.000000 SBILoops-0.2.5/src/SBILoops.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-09 18:19:53.000000 SBILoops-0.2.5/src/SBILoops.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        9 2023-06-09 18:19:53.000000 SBILoops-0.2.5/src/SBILoops.egg-info/top_level.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:39.079376 SBILoops-0.2.6/
+-rw-r--r--   0 patrick    (501) staff       (20)       84 2023-06-08 19:32:47.000000 SBILoops-0.2.6/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-12 15:14:39.079971 SBILoops-0.2.6/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 22:00:16.000000 SBILoops-0.2.6/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-12 15:14:39.081189 SBILoops-0.2.6/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)      620 2023-06-12 15:13:56.000000 SBILoops-0.2.6/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.735129 SBILoops-0.2.6/src/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.751114 SBILoops-0.2.6/src/SBILoops/
+-rw-r--r--   0 patrick    (501) staff       (20)    12913 2023-06-12 15:13:33.000000 SBILoops-0.2.6/src/SBILoops/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.783476 SBILoops-0.2.6/src/SBILoops/beans/
+-rw-r--r--   0 patrick    (501) staff       (20)     4502 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/beans/Executable.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11705 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/beans/File.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/beans/IndexedNum.py
+-rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/beans/JSONer.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14934 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/beans/Path.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2928 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/beans/StorableObject.py
+-rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/beans/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2.6/src/SBILoops/beans/butler.py
+-rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/beans/singleton.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.807116 SBILoops-0.2.6/src/SBILoops/data/
+-rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/data/Alphabet.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/data/AminoAcids.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/data/AtomVariants.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/data/Element.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/data/Properties.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/data/SetDict.py
+-rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/data/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.841649 SBILoops-0.2.6/src/SBILoops/databases/
+-rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/databases/CATHlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8418 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/DrugBanklink.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13623 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/Enzymelink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5579 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/GOlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5361 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/PDBTMlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/databases/PDBeChemConnect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6723 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/PDBeChemlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9135 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/PDBlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1801 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/SCOPlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5741 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/TaxIDlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7108 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7073 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/__Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/databases/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7155 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/dblink.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.849130 SBILoops-0.2.6/src/SBILoops/databases/uniprot/
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/databases/uniprot/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4783 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/uniprot/connect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8173 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/databases/uniprot/uniprot.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.858419 SBILoops-0.2.6/src/SBILoops/error/
+-rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/error/BlastError.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/error/FileError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/error/SeqAliError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/error/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.867049 SBILoops-0.2.6/src/SBILoops/external/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.878264 SBILoops-0.2.6/src/SBILoops/external/CDhit/
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/external/CDhit/CDhit.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2261 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/external/CDhit/CDhitExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/external/CDhit/CDhitHomolog.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2227 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/external/CDhit/CDhitList.py
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/external/CDhit/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.885649 SBILoops-0.2.6/src/SBILoops/external/DSSP/
+-rw-r--r--   0 patrick    (501) staff       (20)     3326 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/external/DSSP/DSSP.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3608 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/external/DSSP/DSSPExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/external/DSSP/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      338 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/external/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/external/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.899379 SBILoops-0.2.6/src/SBILoops/external/blast/
+-rw-r--r--   0 patrick    (501) staff       (20)     9121 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/external/blast/BlastExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12572 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/external/blast/BlastHit.py
+-rw-r--r--   0 patrick    (501) staff       (20)    23494 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/external/blast/BlastResult.py
+-rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/external/blast/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8076 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/external/blast/blast_parser.py
+-rw-r--r--   0 patrick    (501) staff       (20)      312 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/external/configSBI.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.902550 SBILoops-0.2.6/src/SBILoops/math/
+-rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/math/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/math/stats.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.913289 SBILoops-0.2.6/src/SBILoops/sequence/
+-rw-r--r--   0 patrick    (501) staff       (20)     6337 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/sequence/Fasta.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4877 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/sequence/IndexedSeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15049 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/sequence/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/sequence/Sequence.py
+-rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/sequence/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.924077 SBILoops-0.2.6/src/SBILoops/sequence/alignment/
+-rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/sequence/alignment/Needleman_Wunsch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    43530 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/sequence/alignment/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/sequence/alignment/SimilarityMatrix.py
+-rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/sequence/alignment/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.937519 SBILoops-0.2.6/src/SBILoops/structure/
+-rw-r--r--   0 patrick    (501) staff       (20)    23889 2023-06-12 15:09:50.000000 SBILoops-0.2.6/src/SBILoops/structure/PDB.py
+-rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.953574 SBILoops-0.2.6/src/SBILoops/structure/atom/
+-rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/atom/Atom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/atom/AtomOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/atom/AtomOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3764 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/atom/AtomSeries.py
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/atom/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.969217 SBILoops-0.2.6/src/SBILoops/structure/chain/
+-rw-r--r--   0 patrick    (501) staff       (20)    19968 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/chain/Chain.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13270 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/chain/ChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2765 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/chain/ChainOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6879 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/chain/ChainOfProtein.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4992 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/chain/ProteinChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/chain/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.976768 SBILoops-0.2.6/src/SBILoops/structure/contacts/
+-rw-r--r--   0 patrick    (501) staff       (20)     9012 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/Complex.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3410 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/InnerContacts.py
+-rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.990109 SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/
+-rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/Contact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3808 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/ContactAA.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/ContactAH.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3277 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/ContactAN.py
+-rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.998148 SBILoops-0.2.6/src/SBILoops/structure/contacts/inner/
+-rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/inner/PHInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/inner/PPInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/inner/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:39.013073 SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/
+-rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/Interface.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/PHInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11117 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/PNInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/PPInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:39.021039 SBILoops-0.2.6/src/SBILoops/structure/geometry/
+-rw-r--r--   0 patrick    (501) staff       (20)    11104 2023-06-09 18:18:01.000000 SBILoops-0.2.6/src/SBILoops/structure/geometry/RMSD.py
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-06-08 18:05:00.000000 SBILoops-0.2.6/src/SBILoops/structure/geometry/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      662 2023-06-08 18:05:43.000000 SBILoops-0.2.6/src/SBILoops/structure/geometry/basics.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:39.051844 SBILoops-0.2.6/src/SBILoops/structure/header/
+-rw-r--r--   0 patrick    (501) staff       (20)     2284 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/BioMolecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3831 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/DBreference.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2015 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/Experiment.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14756 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/Header.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1201 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/HeteroAtom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      948 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/MiniRes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7647 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/Molecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8534 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2423 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/Site.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18695 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/header/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14370 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/parse_mmCIF.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8543 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/parse_pdb.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:39.065235 SBILoops-0.2.6/src/SBILoops/structure/protein/
+-rw-r--r--   0 patrick    (501) staff       (20)    19074 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/protein/Arch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19202 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/protein/SShelper.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/protein/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/protein/Sequencer.py
+-rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/protein/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:39.074665 SBILoops-0.2.6/src/SBILoops/structure/residue/
+-rw-r--r--   0 patrick    (501) staff       (20)    10773 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/residue/Residue.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10725 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/residue/ResidueOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5359 2023-06-05 21:34:52.000000 SBILoops-0.2.6/src/SBILoops/structure/residue/ResidueOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2.6/src/SBILoops/structure/residue/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-12 15:14:38.759518 SBILoops-0.2.6/src/SBILoops.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-12 15:14:38.000000 SBILoops-0.2.6/src/SBILoops.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     4981 2023-06-12 15:14:38.000000 SBILoops-0.2.6/src/SBILoops.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-12 15:14:38.000000 SBILoops-0.2.6/src/SBILoops.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-12 15:14:38.000000 SBILoops-0.2.6/src/SBILoops.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        9 2023-06-12 15:14:38.000000 SBILoops-0.2.6/src/SBILoops.egg-info/top_level.txt
```

### Comparing `SBILoops-0.2.5/PKG-INFO` & `SBILoops-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBILoops
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
 Description-Content-Type: text/markdown
```

### Comparing `SBILoops-0.2.5/README.md` & `SBILoops-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/__init__.py` & `SBILoops-0.2.6/src/SBILoops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import os
 import traceback
 import datetime
 import time
 import logging
 
-__version__ = '0.2.5'
+__version__ = '0.2.6'
 
 
 class Parameters(object):
     '''
     Designed to work through all the {SBI} library.
     It contains several parameters that will control (a) the amount of data
     shown to the user during the execution of {SBI} subroutines and (b) the
```

### Comparing `SBILoops-0.2.5/src/SBILoops/beans/Executable.py` & `SBILoops-0.2.6/src/SBILoops/beans/Executable.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/beans/File.py` & `SBILoops-0.2.6/src/SBILoops/beans/File.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/beans/IndexedNum.py` & `SBILoops-0.2.6/src/SBILoops/beans/IndexedNum.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/beans/Path.py` & `SBILoops-0.2.6/src/SBILoops/beans/Path.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/beans/StorableObject.py` & `SBILoops-0.2.6/src/SBILoops/beans/StorableObject.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/beans/butler.py` & `SBILoops-0.2.6/src/SBILoops/beans/butler.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/beans/singleton.py` & `SBILoops-0.2.6/src/SBILoops/beans/singleton.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/data/Alphabet.py` & `SBILoops-0.2.6/src/SBILoops/data/Alphabet.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/data/AminoAcids.py` & `SBILoops-0.2.6/src/SBILoops/data/AminoAcids.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/data/AtomVariants.py` & `SBILoops-0.2.6/src/SBILoops/data/AtomVariants.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/data/Element.py` & `SBILoops-0.2.6/src/SBILoops/data/Element.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/data/Properties.py` & `SBILoops-0.2.6/src/SBILoops/data/Properties.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/data/SetDict.py` & `SBILoops-0.2.6/src/SBILoops/data/SetDict.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/data/__init__.py` & `SBILoops-0.2.6/src/SBILoops/data/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/CATHlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/CATHlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/DrugBanklink.py` & `SBILoops-0.2.6/src/SBILoops/databases/DrugBanklink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/Enzymelink.py` & `SBILoops-0.2.6/src/SBILoops/databases/Enzymelink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/GOlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/GOlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/PDBTMlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/PDBTMlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/PDBeChemlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/PDBeChemlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/PDBlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/PDBlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/SCOPlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/SCOPlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/TaxIDlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/TaxIDlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/Uniprotlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/__Uniprotlink.py` & `SBILoops-0.2.6/src/SBILoops/databases/__Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/__init__.py` & `SBILoops-0.2.6/src/SBILoops/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/dblink.py` & `SBILoops-0.2.6/src/SBILoops/databases/dblink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/uniprot/connect.py` & `SBILoops-0.2.6/src/SBILoops/databases/uniprot/connect.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/databases/uniprot/uniprot.py` & `SBILoops-0.2.6/src/SBILoops/databases/uniprot/uniprot.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/error/BlastError.py` & `SBILoops-0.2.6/src/SBILoops/error/BlastError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/error/FileError.py` & `SBILoops-0.2.6/src/SBILoops/error/FileError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/error/SeqAliError.py` & `SBILoops-0.2.6/src/SBILoops/error/SeqAliError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/CDhit/CDhit.py` & `SBILoops-0.2.6/src/SBILoops/external/CDhit/CDhit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/CDhit/CDhitExe.py` & `SBILoops-0.2.6/src/SBILoops/external/CDhit/CDhitExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/CDhit/CDhitHomolog.py` & `SBILoops-0.2.6/src/SBILoops/external/CDhit/CDhitHomolog.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/CDhit/CDhitList.py` & `SBILoops-0.2.6/src/SBILoops/external/CDhit/CDhitList.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/DSSP/DSSP.py` & `SBILoops-0.2.6/src/SBILoops/external/DSSP/DSSP.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/DSSP/DSSPExe.py` & `SBILoops-0.2.6/src/SBILoops/external/DSSP/DSSPExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/blast/BlastExe.py` & `SBILoops-0.2.6/src/SBILoops/external/blast/BlastExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/blast/BlastHit.py` & `SBILoops-0.2.6/src/SBILoops/external/blast/BlastHit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/blast/BlastResult.py` & `SBILoops-0.2.6/src/SBILoops/external/blast/BlastResult.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/external/blast/blast_parser.py` & `SBILoops-0.2.6/src/SBILoops/external/blast/blast_parser.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/math/stats.py` & `SBILoops-0.2.6/src/SBILoops/math/stats.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/sequence/Fasta.py` & `SBILoops-0.2.6/src/SBILoops/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/sequence/IndexedSeqAli.py` & `SBILoops-0.2.6/src/SBILoops/sequence/IndexedSeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/sequence/SeqAli.py` & `SBILoops-0.2.6/src/SBILoops/sequence/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/sequence/Sequence.py` & `SBILoops-0.2.6/src/SBILoops/sequence/Sequence.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/sequence/alignment/Needleman_Wunsch.py` & `SBILoops-0.2.6/src/SBILoops/sequence/alignment/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/sequence/alignment/SeqAli.py` & `SBILoops-0.2.6/src/SBILoops/sequence/alignment/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/sequence/alignment/SimilarityMatrix.py` & `SBILoops-0.2.6/src/SBILoops/sequence/alignment/SimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/PDB.py` & `SBILoops-0.2.6/src/SBILoops/structure/PDB.py`

 * *Files 16% similar despite different names*

```diff
@@ -645,12 +645,86 @@
                 data['FASTA'].append(
                     ">{0}\n{1}".format(c.globalID, c.gapped_nucleotide_sequence()))
                 data['IDX'].append(
                     ">{0}\t{1}".format(c.globalID, c.nucleotide_idx()))
 
         return data
 
+    """
+    Gathering the loop similarities between two proteins
+    """
+    def compare_loops(self, PDB2, rho_thresh=10, delta_thresh=5, theta_thresh=5, distance_thresh=0.5):
+        Similarities = []
+        for target in PDB2.chains:
+            target.clean()
+            target.calculate_dssp()
+            target.calculate_archs()
+
+        for query in self.chains:
+            query.clean()
+            query.calculate_dssp()
+            query.calulate_archs()
+            for query_arch in query.archs:
+                for target in PDB2.chains:
+                    for target_arch in target.archs:
+                        Rho = math.sqrt((query_arch.rho - target_arch.rho)**2)
+                        Delta = math.sqrt((query_arch.delta - target_arch.delta)**2)
+                        Theta = math.sqrt((query_arch.theta - target_arch.theta)**2)
+                        Distance = math.sqrt((query_arch.cartesian_distance - target_arch.cartesian_distance)**2)
+                        if Distance <= distance_thresh  and Rho <= rho_thresh and Delta <= delta_thresh and Theta <= theta_thresh:
+                            Similarities.append("QueryProt:"+query.chain+","+query_arch.initial_position+","+query_arch.end_position":TargetProt:"+target.chain+","+target_arch.initial_position+","+target_arch.end_position)
+
+        if len(Similarities) == 0
+            print("No similar loops at the given thresholds were found")
+
+        return Similarities    
+    """
+    Patrick Gohl
+    """
+
+    """ 
+    Splicing a selected loop pair 
+    """
+    def splice(self, PDB2, selection):
+        query_chain_id = selection.split(":")[1].split(",")[0]
+        query_start = selection.split(":")[1].split(",")[1]
+        query_end = selection.split(":")[1].split(",")[2]
+        target_chain_id = selection.split(":")[3].split(",")[0]
+        target_start = selection.split(":")[3].split(",")[1]
+        target_end = selection.split(":")[3].split(",")[2]
+
+        query_chain = self.get_chain_by_id(query_chain_id)
+        NewChain = query_chain.extract('1',int(query_start)-1, backbone=True) 
+        target_chain = PDB2.get_chain_by_id(target_chain_id)
+        extension = target_chain.extract(target_start , int(target_end) -1 , backbone=True)
+        NewChain.join(extension)
+        extension = target_chain.extract(int(query_end) , len(target_chain.protein_sequence) , backbone=True)
+        NewChain.join(extension)
+        NewChain.chain = query_chain_id+"_s"
+        SplicedProtein = PDB()
+        for chain in self.chain_identifiers:
+            if chain != query_chain_id:
+                SplicedProtein.add_chain(self.get_chain_by_id(chain))
+                if (self.get_chain_by_id(chain).chaintype == "P"):
+                    SplicedProtein._has_prot = "TRUE"
+                elif (self.get_chain_by_id(chain).chaintype == "N"):
+                    SplicedProtein._has_nucl = "TRUE"
+            else:
+                SplicedProtein.add_chain(NewChain)
+
+        return SplicedProtein
+
+
+
+    """
+    Patrick Gohl
+    """
+
+
+
+
+
     #
     # OVERRIDE DEFAULT METHODS
     #
     def __len__(self):
         return len(self._chains)
```

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/atom/Atom.py` & `SBILoops-0.2.6/src/SBILoops/structure/atom/Atom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/atom/AtomOfAminoAcid.py` & `SBILoops-0.2.6/src/SBILoops/structure/atom/AtomOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/atom/AtomOfNucleotide.py` & `SBILoops-0.2.6/src/SBILoops/structure/atom/AtomOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/atom/AtomSeries.py` & `SBILoops-0.2.6/src/SBILoops/structure/atom/AtomSeries.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/chain/Chain.py` & `SBILoops-0.2.6/src/SBILoops/structure/chain/Chain.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/chain/ChainFrame.py` & `SBILoops-0.2.6/src/SBILoops/structure/chain/ChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/chain/ChainOfNucleotide.py` & `SBILoops-0.2.6/src/SBILoops/structure/chain/ChainOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/chain/ChainOfProtein.py` & `SBILoops-0.2.6/src/SBILoops/structure/chain/ChainOfProtein.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/chain/ProteinChainFrame.py` & `SBILoops-0.2.6/src/SBILoops/structure/chain/ProteinChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/Complex.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/Complex.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/InnerContacts.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/InnerContacts.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/Contact.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/Contact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/ContactAA.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/ContactAA.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/ContactAH.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/ContactAH.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/contact/ContactAN.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/contact/ContactAN.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/inner/PHInnerContact.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/inner/PHInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/inner/PPInnerContact.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/inner/PPInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/Interface.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/Interface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/PHInterface.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/PHInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/PNInterface.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/PNInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/contacts/interface/PPInterface.py` & `SBILoops-0.2.6/src/SBILoops/structure/contacts/interface/PPInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/geometry/RMSD.py` & `SBILoops-0.2.6/src/SBILoops/structure/geometry/RMSD.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/geometry/basics.py` & `SBILoops-0.2.6/src/SBILoops/structure/geometry/basics.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/BioMolecule.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/BioMolecule.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/DBreference.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/DBreference.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/Experiment.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/Experiment.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/Header.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/Header.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/HeteroAtom.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/HeteroAtom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/MiniRes.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/MiniRes.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/Molecule.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/Molecule.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/SecondaryStructure.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/Site.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/Site.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/header/__init__.py` & `SBILoops-0.2.6/src/SBILoops/structure/header/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/parse_mmCIF.py` & `SBILoops-0.2.6/src/SBILoops/structure/parse_mmCIF.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/parse_pdb.py` & `SBILoops-0.2.6/src/SBILoops/structure/parse_pdb.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/protein/Arch.py` & `SBILoops-0.2.6/src/SBILoops/structure/protein/Arch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/protein/SShelper.py` & `SBILoops-0.2.6/src/SBILoops/structure/protein/SShelper.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/protein/SecondaryStructure.py` & `SBILoops-0.2.6/src/SBILoops/structure/protein/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/protein/Sequencer.py` & `SBILoops-0.2.6/src/SBILoops/structure/protein/Sequencer.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/residue/Residue.py` & `SBILoops-0.2.6/src/SBILoops/structure/residue/Residue.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/residue/ResidueOfAminoAcid.py` & `SBILoops-0.2.6/src/SBILoops/structure/residue/ResidueOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops/structure/residue/ResidueOfNucleotide.py` & `SBILoops-0.2.6/src/SBILoops/structure/residue/ResidueOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.5/src/SBILoops.egg-info/PKG-INFO` & `SBILoops-0.2.6/src/SBILoops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBILoops
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
 Description-Content-Type: text/markdown
```

### Comparing `SBILoops-0.2.5/src/SBILoops.egg-info/SOURCES.txt` & `SBILoops-0.2.6/src/SBILoops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

