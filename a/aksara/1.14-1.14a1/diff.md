# Comparing `tmp/aksara-1.14.tar.gz` & `tmp/aksara-1.14a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksara-1.14.tar", last modified: Mon Jun 12 00:04:11 2023, max compression
+gzip compressed data, was "aksara-1.14a1.tar", last modified: Wed May  3 06:04:59 2023, max compression
```

## Comparing `aksara-1.14.tar` & `aksara-1.14a1.tar`

### file list

```diff
@@ -1,151 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.498948 aksara-1.14/
--rw-rw-rw-   0        0        0    35184 2023-03-02 06:04:00.000000 aksara-1.14/LICENSE
--rw-rw-rw-   0        0        0      210 2023-06-11 23:12:02.000000 aksara-1.14/MANIFEST.in
--rw-rw-rw-   0        0        0     9402 2023-06-12 00:04:11.499955 aksara-1.14/PKG-INFO
--rw-rw-rw-   0        0        0     9050 2023-06-11 23:12:02.000000 aksara-1.14/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.896674 aksara-1.14/aksara/
--rw-rw-rw-   0        0        0      479 2023-06-11 23:12:02.000000 aksara-1.14/aksara/__init__.py
--rw-rw-rw-   0        0        0      149 2023-06-11 23:12:02.000000 aksara-1.14/aksara/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.954999 aksara-1.14/aksara/_nlp_internal/
--rw-rw-rw-   0        0        0      347 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/analyzer.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.960039 aksara-1.14/aksara/_nlp_internal/bin/
--rw-rw-rw-   0        0        0        0 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/bin/__init__.py
--rw-rw-rw-   0        0        0      146 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/bin/_get_foma_script_path.py
--rw-rw-rw-   0        0        0   672506 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/bin/aksara@v1.2.0.bin
--rw-rw-rw-   0        0        0     8005 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/core.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.963087 aksara-1.14/aksara/_nlp_internal/dependency_parsing/
--rw-rw-rw-   0        0        0       95 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.975914 aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/
--rw-rw-rw-   0        0        0    23012 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/character.json
--rw-rw-rw-   0        0        0      865 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/pos.json
--rw-rw-rw-   0        0        0     1741 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/type.json
--rw-rw-rw-   0        0        0  7577585 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/word.json
--rw-rw-rw-   0        0        0     3810 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/core.py
--rw-rw-rw-   0        0        0     1238 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/model_proxy.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.989687 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/
--rw-rw-rw-   0        0        0      127 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.007006 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/
--rw-rw-rw-   0        0        0       95 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/__init__.py
--rw-rw-rw-   0        0        0     5084 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/alphabet.py
--rw-rw-rw-   0        0        0    22771 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/conllx_data.py
--rw-rw-rw-   0        0        0     1108 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/instance.py
--rw-rw-rw-   0        0        0      748 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/logger.py
--rw-rw-rw-   0        0        0     6085 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/reader.py
--rw-rw-rw-   0        0        0      247 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/utils.py
--rw-rw-rw-   0        0        0     2521 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/writer.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.012066 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io_multi/
--rw-rw-rw-   0        0        0      134 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io_multi/__init__.py
--rw-rw-rw-   0        0        0     1626 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io_multi/lang_id.py
--rw-rw-rw-   0        0        0     7840 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io_multi/multi_vocab.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.013387 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/models/
--rw-rw-rw-   0        0        0       46 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/models/__init__.py
--rw-rw-rw-   0        0        0    16655 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/models/parsing.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.019782 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/
--rw-rw-rw-   0        0        0       66 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/__init__.py
--rw-rw-rw-   0        0        0      437 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/init.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.027960 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/modules/
--rw-rw-rw-   0        0        0      103 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/modules/__init__.py
--rw-rw-rw-   0        0        0     7472 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/modules/attention.py
--rw-rw-rw-   0        0        0     2946 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/modules/linear.py
--rw-rw-rw-   0        0        0     6753 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/modules/variational_rnn.py
--rw-rw-rw-   0        0        0     2882 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.030826 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/tasks/
--rw-rw-rw-   0        0        0       45 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/tasks/__init__.py
--rw-rw-rw-   0        0        0     9680 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/tasks/parser.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.041735 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/
--rw-rw-rw-   0        0        0      162 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/encoder.py
--rw-rw-rw-   0        0        0     7411 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/multi_head_attn.py
--rw-rw-rw-   0        0        0     1311 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/position_ffn.py
--rw-rw-rw-   0        0        0     3839 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/transformer.py
--rw-rw-rw-   0        0        0      817 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/util_class.py
--rw-rw-rw-   0        0        0     4095 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.045178 aksara-1.14/aksara/_nlp_internal/disambiguation/
--rw-rw-rw-   0        0        0        0 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/disambiguation/__init__.py
--rw-rw-rw-   0        0        0     5952 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/disambiguation/hmmdecode.py
--rw-rw-rw-   0        0        0     2744 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/disambiguation/hmmlearn.py
--rw-rw-rw-   0        0        0     1475 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/disambiguator.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.840051 aksara-1.14/aksara/_nlp_internal/etc/
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.060877 aksara-1.14/aksara/_nlp_internal/etc/dataset/
--rw-rw-rw-   0        0        0    72291 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/etc/dataset/informal_gold_standard.conllu
--rw-rw-rw-   0        0        0   540996 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/etc/dataset/preprocessed.txt
--rw-rw-rw-   0        0        0     3435 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/formatter.py
--rw-rw-rw-   0        0        0      144 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/parser.py
--rw-rw-rw-   0        0        0     1330 2023-06-11 23:12:02.000000 aksara-1.14/aksara/_nlp_internal/tokenizer.py
--rw-rw-rw-   0        0        0     3675 2023-06-11 23:12:02.000000 aksara-1.14/aksara/conllu.py
--rw-rw-rw-   0        0        0     9374 2023-06-11 23:12:02.000000 aksara-1.14/aksara/dependency_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.072535 aksara-1.14/aksara/dependency_tree/
--rw-rw-rw-   0        0        0       35 2023-06-11 23:12:02.000000 aksara-1.14/aksara/dependency_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.080124 aksara-1.14/aksara/dependency_tree/drawer/
--rw-rw-rw-   0        0        0      135 2023-06-11 23:12:02.000000 aksara-1.14/aksara/dependency_tree/drawer/__init__.py
--rw-rw-rw-   0        0        0     2357 2023-06-11 23:12:02.000000 aksara-1.14/aksara/dependency_tree/drawer/_drawer_utils.py
--rw-rw-rw-   0        0        0     1325 2023-06-11 23:12:02.000000 aksara-1.14/aksara/dependency_tree/drawer/abstract_drawer.py
--rw-rw-rw-   0        0        0     4293 2023-06-11 23:12:02.000000 aksara-1.14/aksara/dependency_tree/drawer/matplotlib_drawer.py
--rw-rw-rw-   0        0        0     8030 2023-06-11 23:12:02.000000 aksara-1.14/aksara/dependency_tree/drawer/plotly_drawer.py
--rw-rw-rw-   0        0        0     3157 2023-06-11 23:12:02.000000 aksara-1.14/aksara/dependency_tree/tree_drawer.py
--rw-rw-rw-   0        0        0     2801 2023-06-11 23:12:02.000000 aksara-1.14/aksara/lemmatizer.py
--rw-rw-rw-   0        0        0     6233 2023-06-11 23:12:02.000000 aksara-1.14/aksara/morphological_analyzer.py
--rw-rw-rw-   0        0        0     5876 2023-06-11 23:12:02.000000 aksara-1.14/aksara/morphological_feature.py
--rw-rw-rw-   0        0        0     7561 2023-06-11 23:12:02.000000 aksara-1.14/aksara/pos_tagger.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.089804 aksara-1.14/aksara/tokenizers/
--rw-rw-rw-   0        0        0      145 2023-06-11 23:12:02.000000 aksara-1.14/aksara/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     1321 2023-06-11 23:12:02.000000 aksara-1.14/aksara/tokenizers/abstract_tokenizer.py
--rw-rw-rw-   0        0        0     1706 2023-06-11 23:12:02.000000 aksara-1.14/aksara/tokenizers/base_tokenizer.py
--rw-rw-rw-   0        0        0     2257 2023-06-11 23:12:02.000000 aksara-1.14/aksara/tokenizers/multiword_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.093834 aksara-1.14/aksara/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 23:12:02.000000 aksara-1.14/aksara/utils/__init__.py
--rw-rw-rw-   0        0        0     4224 2023-06-11 23:12:02.000000 aksara-1.14/aksara/utils/conllu_io.py
--rw-rw-rw-   0        0        0     2180 2023-06-11 23:12:02.000000 aksara-1.14/aksara/utils/sentence_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.942403 aksara-1.14/aksara.egg-info/
--rw-rw-rw-   0        0        0     9402 2023-06-12 00:04:10.000000 aksara-1.14/aksara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5264 2023-06-12 00:04:10.000000 aksara-1.14/aksara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 00:04:10.000000 aksara-1.14/aksara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      323 2023-06-12 00:04:10.000000 aksara-1.14/aksara.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 00:04:10.000000 aksara-1.14/aksara.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.120122 aksara-1.14/docs/
--rw-rw-rw-   0        0        0      658 2023-05-16 10:13:17.000000 aksara-1.14/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.135661 aksara-1.14/docs/data/
--rw-rw-rw-   0        0        0       56 2023-05-16 10:14:49.000000 aksara-1.14/docs/data/formal_text.txt
--rw-rw-rw-   0        0        0       50 2023-05-16 10:14:49.000000 aksara-1.14/docs/data/informal_text.txt
--rwxrwxrwx   0        0        0      804 2023-05-16 10:13:17.000000 aksara-1.14/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.142920 aksara-1.14/docs/source/
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:10.849723 aksara-1.14/docs/source/_templates/
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.229867 aksara-1.14/docs/source/_templates/autosummary/
--rw-rw-rw-   0        0        0      370 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/_templates/autosummary/attributes.rst
--rw-rw-rw-   0        0        0      459 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/_templates/autosummary/base.rst
--rw-rw-rw-   0        0        0      396 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/_templates/autosummary/class.rst
--rw-rw-rw-   0        0        0      367 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/_templates/autosummary/member.rst
--rw-rw-rw-   0        0        0      367 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/_templates/autosummary/method.rst
--rw-rw-rw-   0        0        0      115 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/_templates/autosummary/minimal_module.rst
--rw-rw-rw-   0        0        0      862 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/_templates/autosummary/module.rst
--rw-rw-rw-   0        0        0     1760 2023-06-11 23:12:02.000000 aksara-1.14/docs/source/conf.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.250034 aksara-1.14/docs/source/contributor_guide/
--rw-rw-rw-   0        0        0     5740 2023-06-11 23:12:02.000000 aksara-1.14/docs/source/contributor_guide/index.rst
--rw-rw-rw-   0        0        0     2050 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.329942 aksara-1.14/docs/source/reference/
--rw-rw-rw-   0        0        0      201 2023-06-11 23:12:02.000000 aksara-1.14/docs/source/reference/conllu.rst
--rw-rw-rw-   0        0        0      937 2023-05-24 03:26:08.000000 aksara-1.14/docs/source/reference/dependency_parsing.rst
--rw-rw-rw-   0        0        0      617 2023-06-11 23:12:02.000000 aksara-1.14/docs/source/reference/index.rst
--rw-rw-rw-   0        0        0      245 2023-05-24 14:29:10.000000 aksara-1.14/docs/source/reference/lemmatization.rst
--rw-rw-rw-   0        0        0      448 2023-05-24 03:26:08.000000 aksara-1.14/docs/source/reference/morphological_feature_analysis.rst
--rw-rw-rw-   0        0        0      244 2023-05-23 08:34:00.000000 aksara-1.14/docs/source/reference/pos_tagging.rst
--rw-rw-rw-   0        0        0      688 2023-05-16 10:13:17.000000 aksara-1.14/docs/source/reference/tokenization.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.360114 aksara-1.14/docs/source/savefig/
--rw-rw-rw-   0        0        0    18837 2023-05-24 03:26:08.000000 aksara-1.14/docs/source/savefig/autotree1.png
--rw-rw-rw-   0        0        0    18611 2023-05-24 03:26:08.000000 aksara-1.14/docs/source/savefig/autotree2.png
--rw-rw-rw-   0        0        0    41366 2023-05-24 03:26:08.000000 aksara-1.14/docs/source/savefig/autotree3.png
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.493422 aksara-1.14/docs/source/user_guide/
--rw-rw-rw-   0        0        0     3567 2023-05-24 03:26:08.000000 aksara-1.14/docs/source/user_guide/analyze_text.rst
--rw-rw-rw-   0        0        0     6058 2023-06-11 23:12:02.000000 aksara-1.14/docs/source/user_guide/draw_dep_tree.rst
--rw-rw-rw-   0        0        0     3726 2023-05-24 03:26:08.000000 aksara-1.14/docs/source/user_guide/get_morph_features.rst
--rw-rw-rw-   0        0        0      430 2023-06-11 23:12:02.000000 aksara-1.14/docs/source/user_guide/index.rst
--rw-rw-rw-   0        0        0     1748 2023-05-24 14:29:10.000000 aksara-1.14/docs/source/user_guide/lemmatization.rst
--rw-rw-rw-   0        0        0     2459 2023-05-24 03:26:08.000000 aksara-1.14/docs/source/user_guide/parse_text.rst
--rw-rw-rw-   0        0        0     2250 2023-06-11 23:12:02.000000 aksara-1.14/docs/source/user_guide/pos_tagging.rst
--rw-rw-rw-   0        0        0     2282 2023-06-11 23:12:02.000000 aksara-1.14/docs/source/user_guide/tokenize_text.rst
--rw-rw-rw-   0        0        0       82 2023-03-31 07:34:16.000000 aksara-1.14/pyproject.toml
--rw-rw-rw-   0        0        0      905 2023-06-12 00:04:11.505421 aksara-1.14/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 00:04:11.493422 aksara-1.14/tests/
--rw-rw-rw-   0        0        0     4052 2023-06-11 23:12:02.000000 aksara-1.14/tests/test_conllu.py
--rw-rw-rw-   0        0        0     2788 2023-06-11 23:12:02.000000 aksara-1.14/tests/test_lemmatization.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.820783 aksara-1.14a1/
+-rw-rw-rw-   0        0        0    35184 2023-03-02 06:04:00.000000 aksara-1.14a1/LICENSE
+-rw-rw-rw-   0        0        0      102 2023-03-31 07:34:16.000000 aksara-1.14a1/MANIFEST.in
+-rw-rw-rw-   0        0        0       77 2023-05-03 06:04:59.820783 aksara-1.14a1/PKG-INFO
+-rw-rw-rw-   0        0        0     6586 2023-03-31 07:35:08.000000 aksara-1.14a1/README.md
+-rw-rw-rw-   0        0        0       82 2023-03-31 07:34:16.000000 aksara-1.14a1/pyproject.toml
+-rw-rw-rw-   0        0        0      644 2023-05-03 06:04:59.822780 aksara-1.14a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.554626 aksara-1.14a1/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.605332 aksara-1.14a1/src/aksara/
+-rw-rw-rw-   0        0        0       12 2023-05-03 06:04:26.000000 aksara-1.14a1/src/aksara/VERSION
+-rw-rw-rw-   0        0        0      297 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/__init__.py
+-rw-rw-rw-   0        0        0     4715 2023-03-06 14:10:13.000000 aksara-1.14a1/src/aksara/analyzer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.645795 aksara-1.14a1/src/aksara/bin/
+-rw-rw-rw-   0        0        0   672506 2023-03-31 07:34:16.000000 aksara-1.14a1/src/aksara/bin/aksara@v1.2.0.bin
+-rw-rw-rw-   0        0        0     3675 2023-04-17 00:11:30.000000 aksara-1.14a1/src/aksara/conllu.py
+-rw-rw-rw-   0        0        0    10114 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/core.py
+-rw-rw-rw-   0        0        0     3944 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/dependency_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.650794 aksara-1.14a1/src/aksara/dependency_tree/
+-rw-rw-rw-   0        0        0       37 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/dependency_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.658262 aksara-1.14a1/src/aksara/dependency_tree/_drawer/
+-rw-rw-rw-   0        0        0      138 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/dependency_tree/_drawer/__init__.py
+-rw-rw-rw-   0        0        0     1554 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/dependency_tree/_drawer/_abstract_drawer.py
+-rw-rw-rw-   0        0        0     2307 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/dependency_tree/_drawer/_drawer_utils.py
+-rw-rw-rw-   0        0        0     2856 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/dependency_tree/_drawer/_matplotlib_drawer.py
+-rw-rw-rw-   0        0        0     6054 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/dependency_tree/_drawer/_plotly_drawer.py
+-rw-rw-rw-   0        0        0     3009 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/dependency_tree/tree_drawer.py
+-rw-rw-rw-   0        0        0     1473 2023-03-02 14:04:12.000000 aksara-1.14a1/src/aksara/disambiguator.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.542626 aksara-1.14a1/src/aksara/etc/
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.683086 aksara-1.14a1/src/aksara/etc/dataset/
+-rw-rw-rw-   0        0        0    72291 2023-03-31 07:34:16.000000 aksara-1.14a1/src/aksara/etc/dataset/informal_gold_standard.conllu
+-rw-rw-rw-   0        0        0   540996 2023-03-31 07:34:16.000000 aksara-1.14a1/src/aksara/etc/dataset/preprocessed.txt
+-rw-rw-rw-   0        0        0     3464 2023-03-06 14:10:13.000000 aksara-1.14a1/src/aksara/formatter.py
+-rw-rw-rw-   0        0        0     3035 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/lemmatizer.py
+-rw-rw-rw-   0        0        0     4191 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/morphological_analyzer.py
+-rw-rw-rw-   0        0        0      146 2023-03-06 14:10:13.000000 aksara-1.14a1/src/aksara/parser.py
+-rw-rw-rw-   0        0        0     8024 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/pos_tagger.py
+-rw-rw-rw-   0        0        0     1394 2023-03-31 19:27:39.000000 aksara-1.14a1/src/aksara/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.690126 aksara-1.14a1/src/aksara/tokenizers/
+-rw-rw-rw-   0        0        0      145 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/tokenizers/abstract_tokenizer.py
+-rw-rw-rw-   0        0        0      900 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/tokenizers/base_tokenizer.py
+-rw-rw-rw-   0        0        0     1557 2023-05-03 06:03:23.000000 aksara-1.14a1/src/aksara/tokenizers/multiword_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.693083 aksara-1.14a1/src/aksara/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:11:30.000000 aksara-1.14a1/src/aksara/utils/__init__.py
+-rw-rw-rw-   0        0        0     2093 2023-04-17 00:11:30.000000 aksara-1.14a1/src/aksara/utils/conllu_io.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.636781 aksara-1.14a1/src/aksara.egg-info/
+-rw-rw-rw-   0        0        0       77 2023-05-03 06:04:59.000000 aksara-1.14a1/src/aksara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3235 2023-05-03 06:04:59.000000 aksara-1.14a1/src/aksara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 06:04:59.000000 aksara-1.14a1/src/aksara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      323 2023-05-03 06:04:59.000000 aksara-1.14a1/src/aksara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2023-05-03 06:04:59.000000 aksara-1.14a1/src/aksara.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.700081 aksara-1.14a1/src/dependency_parsing/
+-rw-rw-rw-   0        0        0       95 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.746396 aksara-1.14a1/src/dependency_parsing/alphabets/
+-rw-rw-rw-   0        0        0    23012 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/alphabets/character.json
+-rw-rw-rw-   0        0        0      865 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/alphabets/pos.json
+-rw-rw-rw-   0        0        0     1741 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/alphabets/type.json
+-rw-rw-rw-   0        0        0  7577585 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/alphabets/word.json
+-rw-rw-rw-   0        0        0     3784 2023-03-13 04:35:34.000000 aksara-1.14a1/src/dependency_parsing/core.py
+-rw-rw-rw-   0        0        0     1252 2023-03-31 07:34:16.000000 aksara-1.14a1/src/dependency_parsing/model_proxy.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.761356 aksara-1.14a1/src/dependency_parsing/neuronlp2/
+-rw-rw-rw-   0        0        0      127 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.774289 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/
+-rw-rw-rw-   0        0        0       95 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/__init__.py
+-rw-rw-rw-   0        0        0     5022 2023-03-13 13:31:17.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/alphabet.py
+-rw-rw-rw-   0        0        0    22771 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/conllx_data.py
+-rw-rw-rw-   0        0        0     1108 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/instance.py
+-rw-rw-rw-   0        0        0      748 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/logger.py
+-rw-rw-rw-   0        0        0     6085 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/reader.py
+-rw-rw-rw-   0        0        0      247 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/utils.py
+-rw-rw-rw-   0        0        0     2521 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.781302 aksara-1.14a1/src/dependency_parsing/neuronlp2/io_multi/
+-rw-rw-rw-   0        0        0      134 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io_multi/__init__.py
+-rw-rw-rw-   0        0        0     1626 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io_multi/lang_id.py
+-rw-rw-rw-   0        0        0     7840 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/io_multi/multi_vocab.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.785303 aksara-1.14a1/src/dependency_parsing/neuronlp2/models/
+-rw-rw-rw-   0        0        0       46 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/models/__init__.py
+-rw-rw-rw-   0        0        0    16628 2023-03-02 06:58:52.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/models/parsing.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.789304 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/
+-rw-rw-rw-   0        0        0       66 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/init.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.795308 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/modules/
+-rw-rw-rw-   0        0        0      103 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0     7472 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/modules/attention.py
+-rw-rw-rw-   0        0        0     2946 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/modules/linear.py
+-rw-rw-rw-   0        0        0     6753 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/modules/variational_rnn.py
+-rw-rw-rw-   0        0        0     2882 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.798327 aksara-1.14a1/src/dependency_parsing/neuronlp2/tasks/
+-rw-rw-rw-   0        0        0       45 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/tasks/__init__.py
+-rw-rw-rw-   0        0        0     9680 2023-03-21 03:53:30.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/tasks/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.809200 aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/
+-rw-rw-rw-   0        0        0      162 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/encoder.py
+-rw-rw-rw-   0        0        0     7411 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/multi_head_attn.py
+-rw-rw-rw-   0        0        0     1311 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/position_ffn.py
+-rw-rw-rw-   0        0        0     3839 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/transformer.py
+-rw-rw-rw-   0        0        0      817 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/util_class.py
+-rw-rw-rw-   0        0        0     4095 2023-03-02 06:04:00.000000 aksara-1.14a1/src/dependency_parsing/neuronlp2/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.815199 aksara-1.14a1/src/disambiguation/
+-rw-rw-rw-   0        0        0        0 2023-03-02 06:04:00.000000 aksara-1.14a1/src/disambiguation/__init__.py
+-rw-rw-rw-   0        0        0     5956 2023-03-06 14:10:13.000000 aksara-1.14a1/src/disambiguation/hmmdecode.py
+-rw-rw-rw-   0        0        0     2785 2023-03-31 07:34:16.000000 aksara-1.14a1/src/disambiguation/hmmlearn.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:04:59.818770 aksara-1.14a1/tests/
+-rw-rw-rw-   0        0        0     4024 2023-04-17 00:11:30.000000 aksara-1.14a1/tests/test_conllu.py
+-rw-rw-rw-   0        0        0     2794 2023-05-03 06:03:23.000000 aksara-1.14a1/tests/test_lemmatization.py
```

### Comparing `aksara-1.14/LICENSE` & `aksara-1.14a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/analyzer.py` & `aksara-1.14a1/src/aksara/analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/python3
 
+import stat
+from sys import platform
 from tempfile import NamedTemporaryFile
 
 import os
 import re
 import subprocess
 
-from sys import platform
-import stat
 
 # BIN_FILE = "bin/umabi@v1.0.3.bin"
 
 
 class BaseAnalyzer:
 
     def __init__(self, bin_file):
@@ -32,37 +32,36 @@
         out = subprocess.check_output(['foma', '-q', '-f', temp_file.name])
 
         if platform == "win32":
             # temp file in windows is default to READ_ONLY
             # os.unlink will raise error on READ_ONLY file
             os.chmod(temp_file.name, stat.S_IWRITE)
             os.unlink(temp_file.name)
-
         return repr(out)[2:-1]
 
     def analyze(self, word):
         # Get lemma from Foma
         analysis = self.__get_analysis(word)
-        analysis = analysis[:-2] # Remove most right \n
-        
-        if("@informal" == analysis[:9]):
+        analysis = analysis[:-2]  # Remove most right \n
+
+        if "@informal" == analysis[:9]:
             analysis = analysis[9:]
 
         if analysis == '???':
-            if("@informal" == word[:9]):
+            if "@informal" == word[:9]:
                 word = word[9:]
             analysis = self.__analyze_unknown(word)
 
         analysis = list(set(analysis.split("\\n")))
         return "\\n".join(analysis)
 
     def __trim_analysis(self, analysis):
         # Remove the clitics
-        temp = analysis.split("+_")[-1] # Remove proclitic
-        temp = temp.split("_+")[0] # Remove enclitic
+        temp = analysis.split("+_")[-1]  # Remove proclitic
+        temp = temp.split("_+")[0]  # Remove enclitic
         return temp.split("+")
 
     def __get_postag(self, text):
         return self.__trim_analysis(text)[1]
 
     def __get_lemma(self, text):
         return self.__trim_analysis(text)[0]
@@ -102,15 +101,16 @@
 
         return new_analysis
 
     def __analyze_unknown(self, surface):
         # Regex pattern
         redup_pattern = re.compile(r'([a-z]+)(\-)([a-z]+)')
         proper_noun_pattern = re.compile(r'[A-Z]+[a-z]*')
-        sym_pattern = re.compile(r'[^\w“”,.?!()—":\'(\-\-)\-]|[\w\-\.]+@([\w\-]+\.)+[\w\-]{2,4}|:[\S](?=\s|$)|:-[\S](?=\s|$)')
+        sym_pattern = re.compile(
+            r'[^\w“”,.?!()—":\'(\-\-)\-]|[\w\-\.]+@([\w\-]+\.)+[\w\-]{2,4}|:[\S](?=\s|$)|:-[\S](?=\s|$)')
         punct_pattern = re.compile(r'[“”,.?!()—":\'(\-\-)\-]')
 
         # Word list
         proper_noun_lst = ['of', 'the', "n't", "'s", "'m"]
 
         # Check every pattern
         analysis = "???"
@@ -143,8 +143,8 @@
             tags.append("Foreign=Yes")
 
         # Add first plus sign
         tags = "+".join(sorted(tags))
         if tags:
             tags = "+" + tags
 
-        return tags
+        return tags
```

### Comparing `aksara-1.14/aksara/_nlp_internal/bin/aksara@v1.2.0.bin` & `aksara-1.14a1/src/aksara/bin/aksara@v1.2.0.bin`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/character.json` & `aksara-1.14a1/src/dependency_parsing/alphabets/character.json`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/pos.json` & `aksara-1.14a1/src/dependency_parsing/alphabets/pos.json`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/type.json` & `aksara-1.14a1/src/dependency_parsing/alphabets/type.json`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/alphabets/word.json` & `aksara-1.14a1/src/dependency_parsing/alphabets/word.json`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/core.py` & `aksara-1.14a1/src/dependency_parsing/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,77 @@
-
 import os
 import json
 import torch
 
-from .neuronlp2.io import  conllx_data
-from .neuronlp2.io_multi import  get_word_index_with_spec
-from .neuronlp2.models import BiRecurrentConvBiAffine
-from .model_proxy import ModelProxy
+from dependency_parsing.neuronlp2.io import conllx_data
+from dependency_parsing.neuronlp2.io_multi import get_word_index_with_spec
+from dependency_parsing.neuronlp2.models import BiRecurrentConvBiAffine
+from dependency_parsing.model_proxy import ModelProxy
 
 ROOT_CHAR = "_ROOT_CHAR"
 ROOT_POS = "_ROOT_POS"
 ROOT = "_ROOT"
 
-class DependencyParser: 
+
+class DependencyParser:
     def __init__(self, model_name='FR_GSD-ID_CSUI'):
-        current_dir = os.path.dirname(__file__)
+        current_dir, _ = os.path.split(os.path.realpath(__file__))
         alphabet_path = os.path.join(current_dir, "alphabets")
-        self.word_alphabet, self.char_alphabet, self.pos_alphabet, self.type_alphabet, _ = conllx_data.create_alphabets(alphabet_path,
+        self.word_alphabet, self.char_alphabet, self.pos_alphabet, self.type_alphabet, _ = conllx_data.create_alphabets(
+            alphabet_path,
             None, data_paths=[None, None], max_vocabulary_size=50000, embedd_dict=None)
-        
+
         model_dir = os.path.join(current_dir, ".pretrained_model")
-        if not os.path.isdir(model_dir): 
+        if not os.path.isdir(model_dir):
             os.makedirs(model_dir)
-        
+
         def load_model_arguments_from_json():
-            file_handle = open(arg_path, 'r')
-            arguments = json.load(file_handle)
-            file_handle.close()
+            arguments = json.load(open(arg_path, 'r'))
             return arguments['args'], arguments['kwargs']
-        
+
         self.model_path = os.path.join(model_dir, model_name)
         self.model_path += '.pt'
         arg_path = self.model_path + '.arg.json'
-        
+
         if not os.path.exists(self.model_path) or not os.path.exists(arg_path):
             ModelProxy.download_model(model_name)
 
         args, kwargs = load_model_arguments_from_json()
         self.model = BiRecurrentConvBiAffine(use_gpu=False, *args, **kwargs)
-        
+
         self.model.load_state_dict(torch.load(self.model_path))
-    
+
     def parse_rows(self, rows):
         modified_rows = rows.copy()
         heads_pred, types_pred = self.predict(rows)
-        
+
         i = 1
         for row in modified_rows:
-            if (row[0].isnumeric()):
+            if row[0].isnumeric():
                 row[6] = str(heads_pred[i])
                 row[7] = self.type_alphabet.get_instance(types_pred[i])
                 i += 1
         return modified_rows
 
     def predict(self, rows):
         self.model.cpu()
         self.model.eval()
 
         words, chars, postags = self.convert_to_tensor(rows)
         mask = torch.tensor([[1 for i in range(words.shape[1])]])
-        length = torch.tensor([words.shape[1]]) 
+        length = torch.tensor([words.shape[1]])
 
         temp_heads_pred, temp_types_pred = self.model.decode_mst(words, chars, postags, mask=mask, length=length,
-                                        leading_symbolic=conllx_data.NUM_SYMBOLIC_TAGS)
+                                                                 leading_symbolic=conllx_data.NUM_SYMBOLIC_TAGS)
 
         heads_pred = temp_heads_pred[0, :]
         types_pred = temp_types_pred[0, :]
-        
+
         return heads_pred, types_pred
-    
+
     def convert_to_tensor(self, rows):
         words = []
         chars = []
         postags = []
         max_char_len = 0
 
         for row in rows:
@@ -83,20 +82,18 @@
         temp_char = [self.char_alphabet.get_index(ROOT_CHAR)]
         for padding in range(max_char_len - 1):
             temp_char.append(1)
         chars.append(temp_char)
         postags.append(self.pos_alphabet.get_index(ROOT_POS))
 
         for row in rows:
-            if(row[0].isnumeric()):
+            if row[0].isnumeric():
                 words.append(get_word_index_with_spec(self.word_alphabet, row[1], 'id'))
                 temp_char = []
                 for char in row[1]:
                     temp_char.append(self.char_alphabet.get_index(char))
                 for padding in range(max_char_len - len(row[1])):
                     temp_char.append(1)
                 chars.append(temp_char)
                 postags.append(self.pos_alphabet.get_index(row[3]))
-        
-        return torch.tensor([words]), torch.tensor([chars]), torch.tensor([postags])
-
 
+        return torch.tensor([words]), torch.tensor([chars]), torch.tensor([postags])
```

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/model_proxy.py` & `aksara-1.14a1/src/dependency_parsing/model_proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import os
 from statistics import mode
 import gdown
 import zipfile
 
+
 class ModelProxy:
     file_id = {
         "FR_GSD-ID_CSUI": "1tg3qNum3Q97-ogBJbXeSqwEdV38kN1hu",
         "IT_ISDT-ID_CSUI": "1K4-mwq9CwHjoIHfGksUUVghP35oyUB8b",
         "SL_SSJ-ID_CSUI": "1jzIJMUWbuueMOWHklQthQAzHVKw4tacT",
         "EN_GUM-ID_CSUI": "1PmzgzT4F5_gBUtMPE8ZEJNGJOTjkc9tj",
         "FR_GSD-ID_GSD": "1bpJsiPwRI09PwA8FdH1L7n1BPw4WbLGw",
         "IT_ISDT-ID_GSD": "1n8VE-LiKkdsUvyNvREK0IEVoNIZ0mn5b",
         "SL_SSJ-ID_GSD": "1IoAYZdKkKCHR4-azXQsg2gQrAX-vtPuR",
         "EN_GUM-ID_GSD": "1JXwgsMwkhfRtvNx9q6hGH-izyA8f-mph",
     }
 
     def download_model(model_name):
-        if (model_name not in ModelProxy.file_id):
+        if model_name not in ModelProxy.file_id:
             print(model_name)
             raise NotImplementedError
 
-        url="https://drive.google.com/uc?id={}".format(ModelProxy.file_id[model_name])
-        curdir_path = os.path.dirname(__file__)
+        url = "https://drive.google.com/uc?id={}".format(ModelProxy.file_id[model_name])
+        curdir_path, _ = os.path.split(os.path.realpath(__file__))
         output_dir = os.path.join(curdir_path, ".pretrained_model")
         output_file = os.path.join(output_dir, "{}.zip".format(model_name))
         gdown.download(url, output_file, quiet=True)
-        
-        with zipfile.ZipFile(output_file,"r") as zip_ref:
+
+        with zipfile.ZipFile(output_file, "r") as zip_ref:
             zip_ref.extractall(output_dir)
```

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/alphabet.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/io/alphabet.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,13 +129,10 @@
         """
         Load model architecture and weights from the give directory. This allow we use old models even the structure
         changes.
         :param input_directory: Directory to save model and weights
         :return:
         """
         loading_name = name if name else self.__name
-
-        with open(os.path.join(input_directory, loading_name + ".json")) as model_file_handle:
-            self.__from_json(json.load(model_file_handle))
-
+        self.__from_json(json.load(open(os.path.join(input_directory, loading_name + ".json"))))
         self.next_index = len(self.instances) + self.offset
         self.keep_growing = False
```

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/conllx_data.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/io/conllx_data.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/instance.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/io/instance.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/logger.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/io/logger.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/reader.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/io/reader.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io/writer.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/io/writer.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io_multi/lang_id.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/io_multi/lang_id.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/io_multi/multi_vocab.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/io_multi/multi_vocab.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/models/parsing.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/models/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from enum import Enum
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Variable
 from ..nn import VarMaskedFastLSTM
 from ..nn import BiAAttention, BiLinear
-from dependency_parsing.neuronlp2.tasks import parser
+from ..tasks import parser
 from ..transformer import TransformerEncoder
 
 class PriorOrder(Enum):
     DEPTH = 0
     INSIDE_OUT = 1
     LEFT2RIGTH = 2
```

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/modules/attention.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/modules/attention.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/modules/linear.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/modules/variational_rnn.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/modules/variational_rnn.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/nn/utils.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/nn/utils.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/tasks/parser.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/tasks/parser.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/encoder.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/multi_head_attn.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/position_ffn.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/position_ffn.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/transformer.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/transformer/util_class.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/transformer/util_class.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/dependency_parsing/neuronlp2/utils.py` & `aksara-1.14a1/src/dependency_parsing/neuronlp2/utils.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/disambiguation/hmmdecode.py` & `aksara-1.14a1/src/disambiguation/hmmdecode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import math
-import os, sys
+import os
+import sys
+
 from .hmmlearn import HMMLearn
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 parent_dir_path = os.path.abspath(os.path.join(dir_path, os.pardir))
 sys.path.insert(0, parent_dir_path)
 
 
@@ -89,24 +91,24 @@
                 prev_best = max(prev_viterbi.keys(), key=lambda prevtag: prev_viterbi[prevtag])
                 tag = tags[index][0]
                 cur_viterbi[tag] = prev_viterbi[prev_best]
                 cur_backpointer[tag] = prev_best
             else:
                 for tag in tags[index]:
                     prev_best = max(prev_viterbi.keys(),
-                                    key=lambda prev_tag: \
+                                    key=lambda prev_tag:
                                         self.__calculate_viterbi_value(
                                             prev_viterbi[prev_tag],
                                             self.hmm.get_transition_prob(tag, prev_tag),
                                             self.hmm.get_emission_prob(sentence[index], tag)))
 
-                    cur_viterbi[tag] = self.__calculate_viterbi_value\
-                        (prev_viterbi[prev_best],
-                         self.hmm.get_transition_prob(tag, prev_best),
-                         self.hmm.get_emission_prob(sentence[index], tag))
+                    cur_viterbi[tag] = self.__calculate_viterbi_value(
+                        prev_viterbi[prev_best],
+                        self.hmm.get_transition_prob(tag, prev_best),
+                        self.hmm.get_emission_prob(sentence[index], tag))
                     cur_backpointer[tag] = prev_best
 
             viterbi.append(cur_viterbi)
             backpointer.append(cur_backpointer)
 
         prev_viterbi = viterbi[-1]
         prev_best = max(prev_viterbi.keys(),
```

### Comparing `aksara-1.14/aksara/_nlp_internal/disambiguation/hmmlearn.py` & `aksara-1.14a1/src/disambiguation/hmmlearn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-import os
 import nltk
+import os
 
 
 class HMMLearn:
-
     N = 0
     TAGS = [
         'NOUN', 'PRON', 'VERB',
         'NUM', 'ADJ', 'ADP',
         'CCONJ', 'SCONJ', 'X',
         'AUX', 'DET', 'ADV',
         'PART', 'INTJ', 'PUNCT',
         'SYM', 'PROPN',
     ]
 
     def __init__(self, train_file=os.path.join("etc", "dataset", "preprocessed.txt"), trigram=False):
         self.trigram = trigram
         word_tags = []
 
-        train_file = os.path.join(
-            os.path.dirname(__file__),
-            '..',
-            train_file)
+        # fix path
+        aksara_path = os.path.join(os.path.dirname(__file__), "..", "aksara")
+        train_file = os.path.join(aksara_path, train_file)
 
         train = open(train_file, "r+", encoding="utf-8").readlines()
         for sentence in train:
             word_tags.append(("START", "START"))
             pairs = sentence.split(" ")
             pairs = pairs[:-1]  # ignore newline
             for pair in pairs:
@@ -61,15 +59,15 @@
         # for key, val in sorted(self.fd.items(), key=lambda x: x[1], reverse=True):
         #     print(key, val)
 
         if not trigram:
             self.cfd_tags = nltk.ConditionalFreqDist(nltk.bigrams(tags))
             # print(self.cfd_tags.keys())
         else:
-            trigrams = [((x,y),z) for x,y,z in nltk.trigrams(tags)]
+            trigrams = [((x, y), z) for x, y, z in nltk.trigrams(tags)]
             self.cfd_tags = nltk.ConditionalFreqDist(trigrams)
 
     def get_emission_prob(self, word, tag, smoothing=True):
         num = self.cfd_word_tags[tag][word]
         denom = sum(list(self.cfd_word_tags[tag].values()))
         if smoothing:
             return (num + 1) / (denom + self.N)
```

### Comparing `aksara-1.14/aksara/_nlp_internal/disambiguator.py` & `aksara-1.14a1/src/aksara/disambiguator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 
-from .disambiguation.hmmlearn import HMMLearn
-from .disambiguation.hmmdecode import HMMDecode
+from disambiguation.hmmlearn import HMMLearn
+from disambiguation.hmmdecode import HMMDecode
 
 
 class Disambiguator:
 
     def __init__(self):
         self.__hmmlearn = HMMLearn(trigram=True)
         self.__hmmdecode = HMMDecode(hmm=self.__hmmlearn, log=True)
```

### Comparing `aksara-1.14/aksara/_nlp_internal/etc/dataset/informal_gold_standard.conllu` & `aksara-1.14a1/src/aksara/etc/dataset/informal_gold_standard.conllu`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/etc/dataset/preprocessed.txt` & `aksara-1.14a1/src/aksara/etc/dataset/preprocessed.txt`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/_nlp_internal/formatter.py` & `aksara-1.14a1/src/aksara/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,20 @@
                 misc += "+"
                 misc += "".join(suff)
             misc += "_" + cand[1]
 
             for key, value in kwargs.items():
                 if key == 'space_after' and value:
                     misc += "|SpaceAfter=No"
-            if misc == "": misc = "_"
+            if misc == "":
+                misc = "_"
             appended_misc += misc + "/"
 
-            feats_string = "|".join("=".join(element) for element in feats_list if element[0] not in ["Prepref", "Pref", "Stem", "Suff"])
+            feats_string = "|".join(
+                "=".join(element) for element in feats_list if element[0] not in ["Prepref", "Pref", "Stem", "Suff"])
             if feats_string == "":
                 feats_string = "_"
             if len(candidates) > 1:
                 feats_string = ambiguous_features_template.format(cand[1], feats_string)
             appended_features += feats_string + "/"
         else:
             misc = "Morf="
@@ -72,15 +74,14 @@
             if cand[1] != 'X':
                 misc += "<" + cand[1] + ">"
             else:
                 misc += "<X>"
             misc += "_" + cand[1]
             appended_misc += misc + "/"
 
-    
     if appended_features == "" or appended_features == "/":
         appended_features = "_/"
 
     appended_lemma = appended_lemma[:-1]
     appended_tags = appended_tags[:-1]
     appended_features = appended_features[:-1]
     appended_misc = appended_misc[:-1]
```

### Comparing `aksara-1.14/aksara/_nlp_internal/tokenizer.py` & `aksara-1.14a1/src/aksara/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/python3
 
 import re
 
 
 class BaseTokenizer:
     _whitespace_pattern = r"\s+"
-    _tokenize_pattern = r'([0-9]+\-an|[+-]?[0-9]*[,.]?[0-9]+|[A-Z][a-z]\.|(?:[A-Z]+\.)(?:[A-Za-z]+\.){1,}|[\w\-\.]+@([\w\-]+\.)+[\w\-]{2,4}|(?P<punct>[^\w\s+])(?P=punct)+|@[\w.]+|:[\S](?=\s|$)|:-[\S](?=\s|$)|\w+(?=n\'t)|n\'t|\w+(?=\'[m|s]\s)|\'[m|s]\s|[^\w\s+]|(?:[\w-]{0,}))'
+    _tokenize_pattern = r'([0-9]+\-an|[+-]?[0-9]*[,.]?[0-9]+|[A-Z][a-z]\.|(?:[A-Z]+\.)(?:[A-Za-z]+\.){1,}|[\w\-\.]+@(' \
+                        r'[\w\-]+\.)+[\w\-]{2,4}|(?P<punct>[^\w\s+])(?P=punct)+|@[\w.]+|:[\S](?=\s|$)|:-[\S](' \
+                        r'?=\s|$)|\w+(?=n\'t)|n\'t|\w+(?=\'[m|s]\s)|\'[m|s]\s|[^\w\s+]|(?:[\w-]{0,}))'
 
     def __init__(self):
         self.regex = re.compile(self._tokenize_pattern)
         self.whitespace_regex = re.compile(self._whitespace_pattern)
 
     def tokenize(self, sent):
         stripped_sent = self.whitespace_regex.sub(" ", sent).strip()
@@ -29,8 +31,8 @@
             if token == '':
                 is_whitespace = True
             else:
                 flag[i] = not is_whitespace
                 i += 1
                 is_whitespace = False
 
-        return flag[1:] + [False]
+        return flag[1:] + [False]
```

### Comparing `aksara-1.14/aksara/conllu.py` & `aksara-1.14a1/src/aksara/conllu.py`

 * *Files identical despite different names*

### Comparing `aksara-1.14/aksara/dependency_parser.py` & `aksara-1.14a1/src/aksara/pos_tagger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,263 +1,236 @@
-"""
-Module for aksara dependency parsing feature
-"""
-
-from typing import List, Literal
-
-import aksara._nlp_internal.dependency_parsing.core as dep_parser_core
-from .conllu import ConlluData
-from ._nlp_internal import _get_foma_script_path
-from ._nlp_internal.core import analyze_sentence
-from ._nlp_internal.analyzer import BaseAnalyzer
-from .utils.conllu_io import write_conllu
-from .utils.sentence_util import _get_sentence_list
-
-
-class DependencyParser:
-    """
-    Class to perform dependency parsing
-    """
-
-    __all_models = [
-        "FR_GSD-ID_CSUI",
-        "FR_GSD-ID_GSD",
-        "IT_ISDT-ID_CSUI",
-        "IT_ISDT-ID_GSD",
-        "EN_GUM-ID_CSUI",
-        "EN_GUM-ID_GSD"
-    ]
-
-
-    def __init__(self):
-        self.default_analyzer = BaseAnalyzer(_get_foma_script_path())
-
-    def parse(
-            self, input_src: str,
-            input_mode: Literal['f', 's'] = 's',
-            is_informal: bool = False,
-            sep_regex: str = None,
-            model: str = "FR_GSD-ID_CSUI"
-    ) -> List[List[ConlluData]]:
-        """ performs dependency parsing on the text (multiple sentences)
-
-        If `input_mode` is set to 's', text is provided as string
-        in `input_src`. Alternatively, if `input_mode` is set to 'f',
-        the path to a file containing the text is provided in `input_src`
+"""This file contains various POS tagging functions"""
 
-        Parameters
+import os
+from warnings import warn
+from typing import List, Tuple, Literal
+from aksara.core import analyze_sentence, split_sentence, sentences_from_file
+from aksara.analyzer import BaseAnalyzer
+from dependency_parsing.core import DependencyParser
+
+
+class POSTagger:
+    __all_input_modes = ["f", "s"]
+
+    def __init__(self) -> None:
+        self.analyzer = self.__get_default_analyzer()
+        self.dependency_parser = self.__get_default_dependency_parser()
+
+    def __get_sentences_string(self, input_str, input_mode, sep_regex) -> str:
+        sentences = []
+        if input_mode == "s":
+            sentences = split_sentence(input_str, sep_regex)
+        elif input_mode == "f":
+            sentences = sentences_from_file(input_str, sep_regex)
+        else:
+            raise ValueError(
+                f"input_mode must be one of {self.__all_input_modes}, but {input_mode} was given"
+            )
+        sentences_string = ""
+        for i in sentences:
+            sentences_string += i + " "
+
+        return sentences_string
+
+    def tag(
+        self,
+        input_src: str,
+        input_mode: Literal["s", "f"] = "s",
+        is_informal: bool = False,
+        sep_regex: str = None,
+    ) -> List[List[Tuple[str, str]]]:
+        sentences_string = self.__get_sentences_string(input_src, input_mode, sep_regex)
+
+        return self._pos_tag_multi_sentences(sentences_string, is_informal, sep_regex)
+
+    def tag_to_file(
+        self,
+        input_src: str,
+        write_path: str,
+        input_mode: Literal["s", "f"] = "s",
+        write_mode: Literal["x", "a", "w"] = "w",
+        is_informal: bool = False,
+        sep_regex: str = None,
+    ) -> str:
+        sentences_string = self.__get_sentences_string(input_src, input_mode, sep_regex)
+
+        self._pos_tag_then_save_to_file(
+            sentences_string, write_path, sep_regex, write_mode, is_informal
+        )
+
+        return write_path
+
+    def _pos_tag_one_word(self, word: str, is_informal: bool = False) -> str:
+        stripped_word = word.strip()
+
+        if stripped_word == "":
+            return ""
+
+        # check space
+        if stripped_word.find(" ") != -1:
+            warn(f'expected a single word input but "{word}" was given')
+            return "X"
+
+        analyzed_word = analyze_sentence(
+            stripped_word,
+            self.analyzer,
+            self.dependency_parser,
+            v1=False,
+            lemma=False,
+            postag=True,
+            informal=is_informal,
+        )
+
+        # check if tokenizer recognize stripped_word as a multi word
+        if len(analyzed_word.split("\n")) > 1:
+            warn(f'expected a single word input but "{word}" was given')
+            return "X"
+        _, _, tag = analyzed_word.split("\t")
+        return tag
+
+    def _pos_tag_one_sentence(
+        self, sentence: str, is_informal: bool = False
+    ) -> list[tuple[str, str]]:
+        """
+        performs pos tagging on the text that will be considered as a sentence,
+        then returns a list of tuple containing each word with its corresponding
+        POS tag as the result
+
+        parameters
         ----------
-        input_src : str
-            text that will be parsed if `input_mode` is set to 's' or
-            file path to a file containing the text if `input_mode`
-            is set to 'f'
-
-        input_mode : {'f', 's'}, optional
-            specifies the source of the input, default is 's'
-
-        is_informal : bool, optional
-            tells aksara to treat text as informal one, default is False
-
-        sep_regex : str, optional
-            regex rule that specifies the end of sentence, default is None
-
-        model : str, optional
-            the model to use for dependency parsing,
-            default is "FR_GSD-ID_CSUI"
-
-        Returns
-        -------
-        result : list of list of ConlluData
-            list of result of dependency parsing of each sentence
-            in form of list of ConlluData class for each word
+        sentece: str
+            the sentence that will be analyzed
+
+        is_informal: bool
+            tell aksara to treat text as informal one, default to False
 
-        Raises
+        return
         ------
-        FileNotFoundError
-            if `input_mode` is set to 'f' but file in `input_src` doesn't exist
-        ValueError
-            if `input_mode` is not in ['f', 's']
-
-        Examples
-        --------
-        >>> from aksara import DependencyParser
-        >>> parser = DependencyParser()
-        >>> text = "Apa yang kamu inginkan? Saya ingin makan."
-        >>> result = parser.parse(text)
-        >>> for sentence in result: #doctest: +NORMALIZE_WHITESPACE
-        ...     for conllu_word in sentence:
-        ...         print(conllu_word)
-        1   Apa     apa     PRON    _       _       0       root    _       _
-        2   yang    yang    SCONJ   _       _       4       mark    _       _
-        3   kamu    kamu    PRON    _       Number=Sing|Person=2|PronType=Prs       4       nsubj   _       _
-        4   inginkan        ingin   VERB    _       Voice=Act       1       acl     _       _
-        5   ?       ?       PUNCT   _       _       4       punct   _       _
-        1   Saya    saya    PRON    _       Number=Sing|Person=1|PronType=Prs       2       nsubj   _       _
-        2   ingin   ingin   VERB    _       _       0       root    _       _
-        3   makan   makan   VERB    _       _       2       xcomp   _       _
-        4   .       .       PUNCT   _       _       3       punct   _       _
+        ReturnType: list[tuple[str, str]]
+            will return list of tuple containing each word with its corresponding POS tag
         """
 
-        sentence_list = _get_sentence_list(input_src, input_mode, sep_regex)
+        sentence = str(sentence).strip()
 
-        if len(sentence_list) == 0:
+        if sentence == "":
             return []
 
+        temp_result = analyze_sentence(
+            text=sentence,
+            analyzer=self.analyzer,
+            dependency_parser=self.dependency_parser,
+            v1=False,
+            lemma=False,
+            postag=True,
+            informal=is_informal,
+        )
+
         result = []
 
-        for sentence in sentence_list:
-            sentence_result = self._parse_one_sentence(
-                sentence, is_informal, model
-            )
-            result.append(sentence_result)
+        for line in temp_result.split("\n"):
+            _, word, postag = line.split("\t")
+            result.append((word, postag))
 
         return result
 
-    def parse_to_file(
-            self, input_src: str,
-            write_path: str,
-            input_mode: Literal['f', 's'] = 's',
-            write_mode: Literal['a', 'w', 'x'] = 'x',
-            is_informal: bool = False,
-            sep_regex: str = None,
-            sep_column: str = '\t',
-            model: str = "FR_GSD-ID_CSUI"
-    ) -> str:
-        """ performs dependency parsing on the text (multiple sentences)
-        and save the result in the CoNLL-U format in a file specified
-        by `write_path`
-
-        If `input_mode` is set to 's', text is provided as string
-        in `input_src`. Alternatively, if `input_mode` is set to 'f',
-        the path to a file containing the text is provided in `input_src`
-
-        Parameters
-        ----------
-        input_src : str
-            text that will be parsed if `input_mode` is set to 's' or
-            file path to a file containing the text if `input_mode`
-            is set to 'f'
+    def _pos_tag_multi_sentences(
+        self, sentences: str, is_informal: bool = False, sep_regex: str = None
+    ) -> List[List[Tuple[str, str]]]:
+        sentences = sentences.strip()
 
-        write_path : str
-            path to the file where the result will be saved to
+        if sentences == "":
+            return []
 
-        input_mode : {'f', 's'}, optional
-            specifies the source of the input, default is 's'
+        result: List[List[Tuple[str, str]]] = []
 
-        write_mode : {'x', 'a', 'w'}, optional
-            mode while writing on the file specified by `write_path`, default is 'x' ::
+        sentence_list = split_sentence(sentences, sep_regex)
+        for sentence in sentence_list:
+            analyzed_sentence = self._pos_tag_one_sentence(sentence, is_informal)
 
-                'x': create the specified file, throws error FileExistsError if already exists
-                'a': append the pos tagging result at the end of the file,
-                     create the specified file if not exists
-                'w': overwrite the current file content with the pos tagging result,
-                     create the specified file if not exists
+            result.append(analyzed_sentence)
 
-            NOTE::
+        return result
 
-                - 'a' write_mode will add '\\n\\n' before the pos tagging result.
-                - If you plan to use 'a' write_mode in a file that already has dependency
-                  parsing result on CoNLL-U format, the sent_id between the old (already in
-                  the file) and new dependency parsing result will not be in sequence.
+    def _pos_tag_then_save_to_file(
+        self,
+        text: str,
+        file_path: str,
+        sep_regex: str = None,
+        write_mode: Literal["x", "a", "w"] = "w",
+        is_informal: bool = False,
+    ) -> bool:
+        """
+        performs pos tagging on the text, then save the result in the file specified by file_path
 
-        is_informal : bool, optional
-            tell aksara to treat text as informal one, default is False
+        parameters
+        ----------
+        text: str
+            the text that will be analyzed
 
-        sep_regex : str, optional
-            regex rule that specifies the end of sentence, default is None
+        file_path: str
+            path to the file where the pos tagging result will be saved to
 
-        sep_column : str, optional
-            regex rule that specifies gap between columns in CoNLL-U format,
-            default is '\t'
+        sep_regex: str
+            regex rule that specify end of sentence
 
-        model : str, optional
-            the model to use for dependency parsing,
-            default is "FR_GSD-ID_CSUI"
+        write_mode: str, ['x', 'a', 'w'], default to 'w'
+            mode while writing on the file specified by file_path
+
+            'x': create the specified file, throws error FileExistsError if already exists
+            'a': append the pos tagging result at the end of the file,
+                    create the specified file if not exists
+            'w': overwrite the current file content with the pos tagging result,
+                    create the specified file if not exists
+
+            NOTE:
+            - if write_mode not in ['x', 'a', 'w'] will throws ValueError
+            - 'a' write_mode will add '\n\n' before the pos tagging result.
+            - If you plan to use 'a' write_mode in a file that already has
+                pos taging result on connlu format, the sent_id between
+                the old (already in the file) and new pos tag result will not ne in sequence.
 
-        Returns
-        -------
-        str
-            absolute path of output file if succesful, null otherwise
+        is_informal: bool
+            tell aksara to treat text as informal one, default to False
 
-        Raises
+        return
         ------
-        FileExistError
-            if `write_mode` is set to 'x' but file already exists
-        ValueError
-            if `write_mode` not in ['x', 'a', 'w'],
-            also if `input_mode` not in ['f', 's']
-
+        ReturnType: bool
+            will return true if succesfully pos tag and save the result on the given file_path
         """
 
-        result = self.parse(
-            input_src, input_mode=input_mode, is_informal=is_informal,
-            sep_regex=sep_regex, model=model
-        )
-
-        sentence_list = _get_sentence_list(
-            input_src,
-            input_mode=input_mode,
-            sep_regex=sep_regex
-        )
-
-        return write_conllu(sentence_list, result, write_path,
-                            write_mode=write_mode, separator=sep_column)
-
-    # pylint: disable-msg=too-many-locals
-    def _parse_one_sentence(
-            self, sentence: str,
-            is_informal: bool = False,
-            model: str = "FR_GSD-ID_CSUI"
-    ) -> List[ConlluData]:
-        """ performs dependency parsing on one sentence
+        all_write_modes = ["x", "a", "w"]
 
-        Parameters
-        ----------
-        is_informal : bool, optional
-            tells aksara to treat text as informal one, default is False
+        if write_mode not in all_write_modes:
+            raise ValueError(f"write_mode must be in {all_write_modes}")
 
+        sentence_list = split_sentence(text, sep_regex)
 
-        model : str, optional
-            the model to use for dependency parsing,
-            default is "FR_GSD-ID_CSUI"
-
-        Returns
-        -------
-        result: list of ConlluData
-            list of ConlluData class for each word
-        """
+        result_list: List[List[Tuple[str, str]]] = self._pos_tag_multi_sentences(
+            text, sep_regex=sep_regex, is_informal=is_informal
+        )
 
-        sentence = sentence.strip()
+        header_format = "# sent_id = {}\n# text = {}"
 
-        if sentence == "":
-            return []
+        with open(file_path, write_mode, encoding="utf-8") as output_file:
+            if write_mode == "a" and len(result_list) != 0:
+                output_file.writelines("\n\n")
 
-        default_dependency_parser = self.__get_default_dependency_parser(model)
+            for i, token_with_tag in enumerate(result_list):
+                output_file.writelines(
+                    header_format.format(str(i + 1), sentence_list[i])
+                )
 
-        analyzed_sentence = analyze_sentence(
-            sentence,
-            self.default_analyzer,
-            default_dependency_parser,
-            v1=False,
-            lemma=False,
-            postag=False,
-            informal=is_informal
-        )
+                for idx, (token, tag) in enumerate(token_with_tag):
+                    output_file.writelines(f"\n{idx + 1}\t{token}\t{tag}")
 
-        result = []
-        for row in analyzed_sentence.split("\n"):
-            idx, form, lemma, upos, xpos, feat, head_id, deprel, _, _ = row.split("\t")
-            conllu_data = ConlluData(
-                idx, form, lemma, upos, xpos, feat, head_id, deprel
-            )
-            result.append(conllu_data)
+                if i < len(result_list) - 1:  # don't add \n at the end of the file
+                    output_file.writelines("\n\n")
 
-        return result
+        return True
 
-    def __get_default_dependency_parser(self, model) -> dep_parser_core.DependencyParser:
-        """ returns a dependency parser instance with the specified model
-        """
+    def __get_default_analyzer(self) -> BaseAnalyzer:
+        bin_path = os.path.join(os.path.dirname(__file__), "bin", "aksara@v1.2.0.bin")
 
-        if model not in self.__all_models:
-            raise ValueError(f"model must be one of {self.__all_models}, but {model} was given")
+        return BaseAnalyzer(bin_path)
 
-        return dep_parser_core.DependencyParser(model)
+    def __get_default_dependency_parser(self) -> DependencyParser:
+        return DependencyParser()
```

### Comparing `aksara-1.14/aksara/dependency_tree/drawer/_drawer_utils.py` & `aksara-1.14a1/src/aksara/dependency_tree/_drawer/_drawer_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,19 +52,15 @@
         offset = int(conllu_row.get_id()) - my_idx
         parent_idx = int(conllu_row.get_head_id())
         edge_list.append([my_idx, parent_idx - offset])
 
     return edge_list
 
 def is_in_ipython() -> bool:
-    try:
-        get_ipython()
-        return True
-    except NameError:
-        return False
+    return hasattr(__builtins__, '__IPYTHON__')
 
 def create_igraph_layout(
         graph: igraph.Graph,
         root: int,
         scale_x: float,
         scale_y: float
     ) -> igraph.Layout:
```

### Comparing `aksara-1.14/aksara/dependency_tree/drawer/abstract_drawer.py` & `aksara-1.14a1/src/aksara/dependency_tree/_drawer/_abstract_drawer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABCMeta, abstractmethod
 from typing import List
 from aksara.conllu import ConlluData
 
 class AbstractDrawer(metaclass=ABCMeta):
     """
-    Abstract class for all drawers.
+    Abstract drawer class.
     Subclass must implement `draw` and `save_image` method
     
     """
 
     @abstractmethod
     def draw(self, conllu_datas: List[List[ConlluData]], *args, **kwargs):
         """
@@ -17,16 +17,16 @@
         Parameters
         ----------
         conllu_datas: list of list of ConlluData
             conllu_datas that will be drawn
         
         See Also
         --------
-        :class:`drawer.MatplotlibDrawer`: Matplotlib drawer instance
-        :class:`drawer.PlotlyDrawer`: Plotly drawer instance
+        aksara.dependency_tree._drawer.MatplotlibDrawer: Matplotlib drawer instance
+        aksara.dependency_tree._drawer.PlotlyDrawer: Plotly drawer instance
         """
 
         raise NotImplementedError("`draw` method is not implemented")
 
     @abstractmethod
     def save_image(self, conllu_datas: List[List[ConlluData]], output_path: str, *args, **kwargs):
         """
@@ -35,10 +35,15 @@
         Parameters
         ----------
         conllu_datas: list of list of ConlluData
             conllu_datas that will be drawn and saved
         
         output_path: str
             file path at which the image will be saved
+        
+        See Also
+        --------
+        aksara.dependency_tree._drawer.MatplotlibDrawer: Matplotlib drawer instance
+        aksara.dependency_tree._drawer.PlotlyDrawer: Plotly drawer instance
         """
 
         raise NotImplementedError("`save_image` method is not implemented")
```

### Comparing `aksara-1.14/aksara/dependency_tree/tree_drawer.py` & `aksara-1.14a1/src/aksara/dependency_tree/tree_drawer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from typing import List, Type, Any
 from aksara.conllu import ConlluData
-from .drawer import MatplotlibDrawer, AbstractDrawer, PlotlyDrawer
+from ._drawer import MatplotlibDrawer, AbstractDrawer, PlotlyDrawer
 
 class TreeDrawer:
     """
     Draw dependency tree with specific drawer (e.g. Matplotlib, Plotly, etc)
+
+    Attributes
+    ----------
+    name_to_drawer: dict
+        mapping drawer name with its instance
     
-    See Also
-    --------
-    :class:`aksara.dependency_tree.drawer.MatplotlibDrawer`: drawer for `drawer_name='matploltlib'`
-    :class:`aksara.dependency_tree.drawer.PlotlyDrawer`: drawer for `drawer_name='plotly'`
+    Methods
+    -------
+    draw(conllu_datas)
+        Draw dependency tree based on `conllu_datas`
     
+    save_image(conllu_datas, ouput_path)
+        Save dependency tree image
+
     """
 
     name_to_drawer = {
         'matplotlib' : MatplotlibDrawer(),
         'plotly': PlotlyDrawer()
     }
 
-    def __init__(self, drawer_name: str = 'matplotlib') -> None:
-        self.set_drawer(drawer_name)
+    def __init__(self, drawer: str = 'matplotlib') -> None:
+        self.set_drawer(drawer)
 
     def draw(
         self,
         conllu_datas: List[List[ConlluData]],
         *args,
         **kwargs
     ) -> Any:
@@ -32,69 +40,64 @@
 
         Parameters
         ----------
         conllu_datas: list of list of ConlluData
             conllu_datas that will be drawn
         
         *args: tuple
-            will be passed to its drawer instance
+            will be passed to its drawer
         
         **kwargs
-            will be passed to its drawer instance
+            will be passed to its drawer
 
         Returns
         -------
         Any
             See drawer return value
 
         See Also
         --------
-        :class:`aksara.dependency_tree.drawer.MatplotlibDrawer`: 
-            drawer instance for `drawer_name='matploltlib'`
-        :class:`aksara.dependency_tree.drawer.PlotlyDrawer`: 
-            drawer instance for `drawer_name='plotly'` 
+        aksara.dependency_tree._drawer.MatplotlibDrawer: Matplotlib drawer instance
+        aksara.dependency_tree._drawer.PlotlyDrawer: Plotly drawer instance
         """
 
         return self.__drawer.draw(conllu_datas, *args, **kwargs)
 
     def save_image(
         self,
         conllu_datas: List[List[ConlluData]],
         output_path: str,
         *args,
         **kwargs
     ) -> None:
         """
-        Save dependency tree
+        Draw dependency tree
 
         Parameters
         ----------
         conllu_datas: list of list of ConlluData
             conllu_datas that will be drawn and saved
         
         output_path: str
             file path at which the dependency tree image will be saved
         
         *args: tuple
-            will be passed to its drawer instance
+            will be passed to its drawer
         
         **kwargs
-            will be passed to its drawer instance
+            will be passed to its drawer
 
         Returns
         -------
         None
 
         See Also
         --------
-        :class:`aksara.dependency_tree.drawer.MatplotlibDrawer`: 
-            drawer instance for `drawer_name='matploltlib'`
-        :class:`aksara.dependency_tree.drawer.PlotlyDrawer`: 
-            drawer instance for `drawer_name='plotly'`
-
+        aksara.dependency_tree._drawer.MatplotlibDrawer: Matplotlib drawer instance
+        aksara.dependency_tree._drawer.PlotlyDrawer: Plotly drawer instance
         """
 
         self.__drawer.save_image(conllu_datas, output_path, *args, **kwargs)
 
     def get_drawer(self) -> Type[AbstractDrawer]:
         """drawer instance getter
         """
```

### Comparing `aksara-1.14/aksara/lemmatizer.py` & `aksara-1.14a1/src/aksara/lemmatizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,56 @@
+import os
+
 from typing import Union
-from ._nlp_internal import _get_foma_script_path
-from ._nlp_internal.core import analyze_sentence
-from ._nlp_internal.analyzer import BaseAnalyzer
-from ._nlp_internal.dependency_parsing.core import DependencyParser
+from aksara.core import analyze_sentence
+from aksara.analyzer import BaseAnalyzer
+from dependency_parsing.core import DependencyParser
 
 
 class Lemmatizer:
-    """
-    Class to perform lemmatization task
-    """
-
     def __init__(self):
-        self.default_analyzer = BaseAnalyzer(_get_foma_script_path())
-        self.default_dependency_parser = DependencyParser()
+        self.default_analyzer = self.__get_default_analyzer()
+        self.default_dependency_parser = self.__get_default_dependency_parser()
 
-    def lemmatize(self, word_input: str, is_informal: bool = False) -> Union[str, list[str]]:
+    def lemmatize(self, word_input: str, is_informal: bool = False) -> Union[str, list]:
         """
+
         performs lemmatization on a word,
+
         then returns a string containing its corresponding
+
         lemma as the result or a list if the word contains
+
         certain affixes
 
+
+
         parameters
         ----------
+
         input: str
+
             the word that will be analyzed
 
+
+
         is_informal: bool
+
             tell aksara to treat text as informal , default to False
 
-        returns
-        -------
-        str or list of str
+
+
+        return
+        ------
+
+        ReturnType: str | list
+
             will return string containing each word's lemma or
             list if the word contains certain affixes
+
         """
         word_input = word_input.strip()
 
         if word_input == "":
             return ""
 
         lemmatized_result = self.lemmatize_batch([word_input], is_informal)
@@ -49,31 +62,47 @@
 
         return result
 
     def lemmatize_batch(
         self, list_word: list, is_informal: bool = False
     ) -> list[tuple[str, str]]:
         """
+
         performs lemmatization on the sentence list,
+
         then returns a list containing each word paired with its
+
         corresponding lemma as the result
 
+
+
         parameters
         ----------
+
         input: list
+
             the list of words (sentence) that will be analyzed
 
+
+
         is_informal: bool
+
             tell aksara to treat text as informal , default to False
 
-        returns
-        -------
-        list of tuple
+
+
+        return
+        ------
+
+        ReturnType: list
+
             will return list containing each word paired with its
+
             corresponding lemma as the result
+
         """
 
         if list_word == []:
             return []
 
         input_text = " ".join(list_word)
 
@@ -90,7 +119,14 @@
         result = []
 
         for line in temp_result.split("\n"):
             _, word, lemma = line.split("\t")
             result.append((word, lemma))
 
         return result
+
+    def __get_default_analyzer(self) -> BaseAnalyzer:
+        bin_path = os.path.join(os.path.dirname(__file__), "bin", "aksara@v1.2.0.bin")
+        return BaseAnalyzer(bin_path)
+
+    def __get_default_dependency_parser(self) -> DependencyParser:
+        return DependencyParser()
```

### Comparing `aksara-1.14/aksara/tokenizers/multiword_tokenizer.py` & `aksara-1.14a1/src/aksara/tokenizers/multiword_tokenizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,58 @@
 from typing import List
-from .._nlp_internal import _get_foma_script_path
-from .._nlp_internal.dependency_parsing.core import DependencyParser
-from .._nlp_internal.core import analyze_sentence
-from .._nlp_internal.analyzer import BaseAnalyzer
+import os
+
+from dependency_parsing.core import DependencyParser
+from ..core import analyze_sentence
+from ..analyzer import BaseAnalyzer
 
 from .abstract_tokenizer import AbstractTokenizer
 
 # pylint: disable=R0903
 class MultiwordTokenizer(AbstractTokenizer):
-    """
-    Class to perform tokenization (multiword token will be splitted)
+    """Class to perform tokenization (multiword token will be splitted)
+    
     """
 
     def __init__(self) -> None:
-        self.__base_analyzer = BaseAnalyzer(_get_foma_script_path())
+        __bin_path = os.path.join(os.path.dirname(__file__), "..", "bin", "aksara@v1.2.0.bin")
+        self.__base_analyzer = BaseAnalyzer(__bin_path)
         self.__dependency_parser = DependencyParser()
 
-    def tokenize(self, text: str, ssplit: bool=True, **kwargs) -> List[str]:
-        """tokenize `text`
+    def tokenize(self, text: str, *args, **kwargs) -> List[str]:
+        """
+        tokenize `text`
 
         Parameters
         ----------
 
         text: str
             text that will be tokenized
-
-        ssplit: bool, default=True
-            Tell tokenizer to split sentences (ssplit=False, assume the text as one sentence)        
-
+        
         Returns
         -------
-        list of list of str
-            List of all tokens in each sentences
-        
-        Examples
-        --------
-        >>> from aksara import MultiwordTokenizer
-        >>> tokenizer = MultiwordTokenizer()
-        >>> text = "Biarlah saja seperti itu"   # 'Biarlah' is a multiword token ('Biar' + 'lah')
-        >>> tokenizer.tokenize(text)
-        [['Biar', 'lah', 'saja', 'seperti', 'itu']]
-        
+        list of str
+            list of all token in text
         """
 
-        stripped_text = text.strip()
+        stripped_sentence = text.strip()
 
-        if len(stripped_text) == 0:
+        if stripped_sentence == "":
             return []
 
-        all_tokens = []
-
-        for stripped_sentence in self._preprocess_text(stripped_text, ssplit):
-            analyzed_result = analyze_sentence(
-                stripped_sentence,
-                self.__base_analyzer,
-                self.__dependency_parser,
-                informal=True,
-                v1=False,
-                postag=True,
-                lemma=False
-            )
-
-            result: List[str] = []
-            for conllu_row in analyzed_result.split("\n"):
-                idx, form, _ = conllu_row.split("\t")
-                if "-" not in idx:
-                    result.append(form)
-
-            all_tokens.append(result)
+        analyzed_result = analyze_sentence(
+            stripped_sentence,
+            self.__base_analyzer,
+            self.__dependency_parser,
+            informal=True,
+            v1=False,
+            postag=True,
+            lemma=False
+        )
+
+        result: List[str] = []
+        for conllu_row in analyzed_result.split("\n"):
+            idx, form, _ = conllu_row.split("\t")
+            if "-" not in idx:
+                result.append(form)
 
-        return all_tokens
+        return result
```

### Comparing `aksara-1.14/tests/test_conllu.py` & `aksara-1.14a1/tests/test_conllu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from aksara.conllu import ConlluData
 
+
 class ConlluTest(unittest.TestCase):
-    """Test Conllu Data"""
 
     def setUp(self) -> None:
         self.connlu_data = ConlluData(idx='1', form="berjalan", lemma="jalan",
                                       upos="VERB", xpos='_', feat='Voice=Act',
                                       head_id='0', deprel='root')
 
         return super().setUp()
@@ -82,8 +82,8 @@
 
     def test_conllu_is_not_equal_with_non_conllu(self):
         self.assertNotEqual(self.connlu_data, "")
 
     def test_multiword_token(self):
         multi_word_conllu = ConlluData(idx='1-2', head_id='0')
 
-        self.assertEqual(multi_word_conllu.get_id(), '1-2')
+        self.assertEqual(multi_word_conllu.get_id(), '1-2')
```

### Comparing `aksara-1.14/tests/test_lemmatization.py` & `aksara-1.14a1/tests/test_lemmatization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
-from aksara.lemmatizer import Lemmatizer
+from src.aksara.lemmatizer import Lemmatizer
+
 
 class LemmatizationTest(unittest.TestCase):
     """This class contains unit testcases for the lemmatization feature"""
 
     def setUp(self) -> None:
         self.lemmatizer = Lemmatizer()
         return super().setUp()
```

