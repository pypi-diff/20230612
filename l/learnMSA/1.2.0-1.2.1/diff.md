# Comparing `tmp/learnMSA-1.2.0.tar.gz` & `tmp/learnMSA-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learnMSA-1.2.0.tar", last modified: Fri Jun  9 07:25:13 2023, max compression
+gzip compressed data, was "learnMSA-1.2.1.tar", last modified: Mon Jun 12 09:05:53 2023, max compression
```

## Comparing `learnMSA-1.2.0.tar` & `learnMSA-1.2.1.tar`

### file list

```diff
@@ -1,292 +1,292 @@
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:13.445426 learnMSA-1.2.0/
--rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-09 07:25:13.445060 learnMSA-1.2.0/PKG-INFO
--rw-r--r--   0 jovyan   (17731) root         (0)     3721 2023-06-07 06:46:13.000000 learnMSA-1.2.0/README.md
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.036971 learnMSA-1.2.0/learnMSA/
--rw-r--r--   0 jovyan   (17731) root         (0)       33 2023-01-12 09:31:05.000000 learnMSA-1.2.0/learnMSA/__init__.py
--rw-r--r--   0 jovyan   (17731) root         (0)       21 2023-06-09 07:21:50.000000 learnMSA-1.2.0/learnMSA/_version.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.109855 learnMSA-1.2.0/learnMSA/msa_hmm/
--rw-r--r--   0 jovyan   (17731) root         (0)    34665 2023-06-08 09:14:32.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Align.py
--rw-r--r--   0 jovyan   (17731) root         (0)     6483 2023-06-09 07:19:53.000000 learnMSA-1.2.0/learnMSA/msa_hmm/AlignInsertions.py
--rw-r--r--   0 jovyan   (17731) root         (0)    34673 2023-06-08 08:57:24.000000 learnMSA-1.2.0/learnMSA/msa_hmm/AlignmentModel.py
--rw-r--r--   0 jovyan   (17731) root         (0)    25907 2023-04-17 07:14:46.000000 learnMSA-1.2.0/learnMSA/msa_hmm/AncProbsLayer.py
--rw-r--r--   0 jovyan   (17731) root         (0)     4510 2023-06-01 14:05:27.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Configuration.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7999 2023-02-27 14:23:42.000000 learnMSA-1.2.0/learnMSA/msa_hmm/DirichletMixture.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7519 2023-05-08 08:03:16.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Emitter.py
--rw-r--r--   0 jovyan   (17731) root         (0)    11353 2023-06-01 11:47:09.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Fasta.py
--rw-r--r--   0 jovyan   (17731) root         (0)     6065 2023-04-18 09:17:14.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Initializers.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7824 2023-05-08 09:04:58.000000 learnMSA-1.2.0/learnMSA/msa_hmm/MsaHmmCell.py
--rw-r--r--   0 jovyan   (17731) root         (0)     5645 2023-05-08 08:54:55.000000 learnMSA-1.2.0/learnMSA/msa_hmm/MsaHmmLayer.py
--rw-r--r--   0 jovyan   (17731) root         (0)     9183 2023-04-06 07:04:35.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Priors.py
--rw-r--r--   0 jovyan   (17731) root         (0)     9857 2023-04-18 10:52:29.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Training.py
--rw-r--r--   0 jovyan   (17731) root         (0)    29732 2023-06-01 16:57:53.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Transitioner.py
--rw-r--r--   0 jovyan   (17731) root         (0)     1119 2023-01-12 09:37:48.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Utility.py
--rw-r--r--   0 jovyan   (17731) root         (0)    13807 2023-04-18 10:55:32.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Visualize.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7809 2023-05-08 08:18:25.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Viterbi.py
--rw-r--r--   0 jovyan   (17731) root         (0)      897 2023-06-01 11:39:37.000000 learnMSA-1.2.0/learnMSA/msa_hmm/__init__.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:58.836651 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.680225 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    53002 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1434 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.784145 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   518353 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.865836 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      818 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:00.320068 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:00.405339 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    35917 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1627 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:00.543252 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    68449 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:00.898145 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    67114 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.110649 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1745 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.361744 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1997 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.405701 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3913 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1598 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.432407 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4441 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.477464 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3106 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.796052 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:02.222098 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   130517 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:02.393442 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    68173 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1641 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:02.523027 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   132961 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:02.766075 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   131626 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:03.329836 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     9557 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:03.658701 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:03.816790 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    11725 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.610927 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    20065 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1617 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.725954 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    18730 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1415 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.791122 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     2249 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.842058 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3005 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.931241 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4417 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.993482 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     5449 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:05.430069 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4114 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:05.685703 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   260305 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:05.764712 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.290222 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      812 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.485418 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    19789 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1610 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.585254 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    36193 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1624 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.641727 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    34858 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1425 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.744603 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3761 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.979308 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     6029 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.208000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     5929 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.271910 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     8473 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.375790 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     7138 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:58.851374 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.509855 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.563267 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.962507 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.022213 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.297885 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.524785 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.695837 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.735006 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.426033 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.483204 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.715189 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1601 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      792 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.787561 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1709 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.859043 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1673 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      794 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.936643 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1853 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      800 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:10.379364 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1437 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:10.930956 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:11.550495 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     2453 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:11.639468 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1541 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:11.861770 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:11.909572 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:12.543145 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1685 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:12.634104 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:12.841160 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1781 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:12.932645 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1733 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:13.174985 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:13.442221 learnMSA-1.2.0/learnMSA/run/
--rw-r--r--   0 jovyan   (17731) root         (0)       41 2022-08-17 06:53:42.000000 learnMSA-1.2.0/learnMSA/run/__init__.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7910 2023-06-08 09:43:01.000000 learnMSA-1.2.0/learnMSA/run/console.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.045022 learnMSA-1.2.0/learnMSA.egg-info/
--rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/PKG-INFO
--rw-r--r--   0 jovyan   (17731) root         (0)    15625 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan   (17731) root         (0)        1 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       51 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/entry_points.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       45 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/requires.txt
--rw-r--r--   0 jovyan   (17731) root         (0)        9 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/top_level.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       80 2022-08-09 12:49:25.000000 learnMSA-1.2.0/pyproject.toml
--rw-r--r--   0 jovyan   (17731) root         (0)       38 2023-06-09 07:25:13.445801 learnMSA-1.2.0/setup.cfg
--rw-r--r--   0 jovyan   (17731) root         (0)     1015 2023-02-01 15:12:42.000000 learnMSA-1.2.0/setup.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.722967 learnMSA-1.2.1/
+-rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-12 09:05:53.722683 learnMSA-1.2.1/PKG-INFO
+-rw-r--r--   0 jovyan   (17731) root         (0)     3721 2023-06-07 06:46:13.000000 learnMSA-1.2.1/README.md
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.395357 learnMSA-1.2.1/learnMSA/
+-rw-r--r--   0 jovyan   (17731) root         (0)       33 2023-01-12 09:31:05.000000 learnMSA-1.2.1/learnMSA/__init__.py
+-rw-r--r--   0 jovyan   (17731) root         (0)       21 2023-06-12 09:05:35.000000 learnMSA-1.2.1/learnMSA/_version.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.424632 learnMSA-1.2.1/learnMSA/msa_hmm/
+-rw-r--r--   0 jovyan   (17731) root         (0)    34665 2023-06-08 09:14:32.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Align.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     6542 2023-06-12 08:50:18.000000 learnMSA-1.2.1/learnMSA/msa_hmm/AlignInsertions.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    34673 2023-06-08 08:57:24.000000 learnMSA-1.2.1/learnMSA/msa_hmm/AlignmentModel.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    25907 2023-04-17 07:14:46.000000 learnMSA-1.2.1/learnMSA/msa_hmm/AncProbsLayer.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     4510 2023-06-01 14:05:27.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Configuration.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7999 2023-02-27 14:23:42.000000 learnMSA-1.2.1/learnMSA/msa_hmm/DirichletMixture.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7519 2023-05-08 08:03:16.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Emitter.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    11353 2023-06-01 11:47:09.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Fasta.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     6065 2023-04-18 09:17:14.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Initializers.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7824 2023-05-08 09:04:58.000000 learnMSA-1.2.1/learnMSA/msa_hmm/MsaHmmCell.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     5645 2023-05-08 08:54:55.000000 learnMSA-1.2.1/learnMSA/msa_hmm/MsaHmmLayer.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     9183 2023-04-06 07:04:35.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Priors.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     9857 2023-04-18 10:52:29.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Training.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    29732 2023-06-01 16:57:53.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Transitioner.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     1119 2023-01-12 09:37:48.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Utility.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    13807 2023-04-18 10:55:32.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Visualize.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7809 2023-05-08 08:18:25.000000 learnMSA-1.2.1/learnMSA/msa_hmm/Viterbi.py
+-rw-r--r--   0 jovyan   (17731) root         (0)      897 2023-06-01 11:39:37.000000 learnMSA-1.2.1/learnMSA/msa_hmm/__init__.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.378872 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.429165 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    53002 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1434 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.434409 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   518353 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.439226 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      818 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.443721 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.448240 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    35917 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1627 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.452743 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    68449 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.457561 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    67114 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.461828 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1745 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.466682 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1997 2023-01-12 09:32:03.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.472780 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3913 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1598 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.478917 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4441 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.483565 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3106 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.487907 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.492314 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   130517 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.496705 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    68173 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1641 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.501073 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   132961 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.505485 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   131626 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.509633 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     9557 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.513836 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.517994 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    11725 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.522210 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    20065 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1617 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.526490 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    18730 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1415 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.530593 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     2249 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.534848 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3005 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.539225 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4417 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.543619 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     5449 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.548213 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4114 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.553182 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   260305 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.559078 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.563504 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      812 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.567825 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    19789 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1610 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.572183 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    36193 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1624 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.576496 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    34858 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1425 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.580737 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3761 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.585023 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     6029 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.589316 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     5929 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.593572 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     8473 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.597805 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     7138 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.390781 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.602477 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.607186 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.611948 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.616869 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.621980 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.626631 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.631334 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.636173 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.640794 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.645723 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.650531 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1601 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      792 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.655387 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1709 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.660027 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1673 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      794 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.664697 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1853 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      800 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.669442 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1437 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.674386 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.679378 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     2453 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.684613 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1541 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.689579 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.694449 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.699429 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1685 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.704327 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.709152 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1781 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.713977 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1733 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.718796 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.721398 learnMSA-1.2.1/learnMSA/run/
+-rw-r--r--   0 jovyan   (17731) root         (0)       41 2022-08-17 06:53:42.000000 learnMSA-1.2.1/learnMSA/run/__init__.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7910 2023-06-08 09:43:01.000000 learnMSA-1.2.1/learnMSA/run/console.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-12 09:05:53.402385 learnMSA-1.2.1/learnMSA.egg-info/
+-rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-12 09:05:53.000000 learnMSA-1.2.1/learnMSA.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan   (17731) root         (0)    15625 2023-06-12 09:05:53.000000 learnMSA-1.2.1/learnMSA.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)        1 2023-06-12 09:05:53.000000 learnMSA-1.2.1/learnMSA.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       51 2023-06-12 09:05:53.000000 learnMSA-1.2.1/learnMSA.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       45 2023-06-12 09:05:53.000000 learnMSA-1.2.1/learnMSA.egg-info/requires.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)        9 2023-06-12 09:05:53.000000 learnMSA-1.2.1/learnMSA.egg-info/top_level.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       80 2022-08-09 12:49:25.000000 learnMSA-1.2.1/pyproject.toml
+-rw-r--r--   0 jovyan   (17731) root         (0)       38 2023-06-12 09:05:53.723233 learnMSA-1.2.1/setup.cfg
+-rw-r--r--   0 jovyan   (17731) root         (0)     1015 2023-02-01 15:12:42.000000 learnMSA-1.2.1/setup.py
```

### Comparing `learnMSA-1.2.0/README.md` & `learnMSA-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Align.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Align.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/AlignInsertions.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/AlignInsertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import learnMSA.msa_hmm.Fasta as fasta
 import learnMSA.msa_hmm.AlignmentModel as alignment_model
 import subprocess
 from shutil import which
 import sys
 
 
-def find_long_insertions_and_write_slice(fasta_file, lens, starts, name, directory, t = 20, k=2, verbose=True):
+def find_long_insertions_and_write_slice(fasta_file, lens, starts, name, directory, t = 20, k=2, max_insertions_len=500, verbose=True):
         """
         Finds insertions that have at least length t. If there are at least k of these sequences, writes them to file.
         Args: 
             fasta_file: Fasta file containing the complete sequences.
             lens, starts: Arrays of length n where n is the number of sequences in fasta_file. Indicate how long insertions are and where they start respectively.
             name: Identifier for the location of the slice (e.g. left_flank or match_5).
         """
@@ -28,15 +28,15 @@
                     aa_seq = fasta_file.aminoacid_seq_str(which[j])
                     segment = aa_seq[start[j] : start[j] + lengths[j]]
                     only_non_standard_aa = True
                     for aa in fasta.alphabet[:20]:
                         if aa in segment:
                             only_non_standard_aa = False
                             break
-                    if only_non_standard_aa:
+                    if only_non_standard_aa or lengths[j] > max_insertions_len:
                         to_delete.append(j)
                     else:
                         slice_file.write(">"+fasta_file.seq_ids[which[j]]+"\n")
                         slice_file.write(segment+"\n")
             which = np.delete(which, to_delete)
             return (which, filename)
```

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/AlignmentModel.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/AlignmentModel.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/AncProbsLayer.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/AncProbsLayer.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Configuration.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Configuration.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/DirichletMixture.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/DirichletMixture.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Emitter.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Emitter.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Fasta.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Fasta.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Initializers.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Initializers.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/MsaHmmCell.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/MsaHmmCell.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/MsaHmmLayer.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/MsaHmmLayer.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Priors.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Priors.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Training.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Training.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Transitioner.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Transitioner.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Utility.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Utility.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Visualize.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Visualize.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/Viterbi.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/Viterbi.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/__init__.py` & `learnMSA-1.2.1/learnMSA/msa_hmm/__init__.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index` & `learnMSA-1.2.1/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA/run/console.py` & `learnMSA-1.2.1/learnMSA/run/console.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/learnMSA.egg-info/SOURCES.txt` & `learnMSA-1.2.1/learnMSA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.0/setup.py` & `learnMSA-1.2.1/setup.py`

 * *Files identical despite different names*

