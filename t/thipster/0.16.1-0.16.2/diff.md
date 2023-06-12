# Comparing `tmp/thipster-0.16.1.tar.gz` & `tmp/thipster-0.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.16.1.tar", last modified: Mon Jun 12 08:10:12 2023, max compression
+gzip compressed data, was "thipster-0.16.2.tar", last modified: Mon Jun 12 08:15:07 2023, max compression
```

## Comparing `thipster-0.16.1.tar` & `thipster-0.16.2.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.407849 thipster-0.16.1/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-12 08:10:08.000000 thipster-0.16.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 08:10:08.000000 thipster-0.16.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4137 2023-06-12 08:10:12.407849 thipster-0.16.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3501 2023-06-12 08:10:08.000000 thipster-0.16.1/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-12 08:10:08.000000 thipster-0.16.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-12 08:10:08.000000 thipster-0.16.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 08:10:12.407849 thipster-0.16.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-12 08:10:09.000000 thipster-0.16.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.399850 thipster-0.16.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.399850 thipster-0.16.1/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.399850 thipster-0.16.1/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.399850 thipster-0.16.1/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15548 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     6952 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10326 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13708 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    19125 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6275 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20100 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4137 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-12 08:15:03.000000 thipster-0.16.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 08:15:03.000000 thipster-0.16.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-06-12 08:15:07.306557 thipster-0.16.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3501 2023-06-12 08:15:03.000000 thipster-0.16.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-12 08:15:03.000000 thipster-0.16.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-12 08:15:03.000000 thipster-0.16.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 08:15:07.306557 thipster-0.16.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-12 08:15:04.000000 thipster-0.16.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15546 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     6952 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13387 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19129 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6417 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20100 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.16.1/LICENSE` & `thipster-0.16.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/PKG-INFO` & `thipster-0.16.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.1
+Version: 0.16.2
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.16.1/README.md` & `thipster-0.16.2/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/pyproject.toml` & `thipster-0.16.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/setup.py` & `thipster-0.16.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.16.1'
+__version__ = '0.16.2'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.16.1/tests/engine/test_engine.py` & `thipster-0.16.2/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.16.2/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,15 +571,15 @@
 ):
 
     exc_info = __test_parser_raises(mocker, input, DSLSyntaxException)
 
     exp = str(' or '.join(list(map(lambda x: str(x), expected))))\
         if isinstance(expected, list) else str(expected.value)
 
-    assert repr(exc_info.value) == f'(File : \
+    assert str(exc_info.value) == f'(File : \
 {os.getcwd()}/test/test_file.thips, Ln {str(ln)}, Col {str(col)}) :\n\t\
 Syntax error : Expected {exp}, got {str(got.value)}'
 
 
 def test_syntax_error_resource(mocker):
     # MISSING NAME
     input = """bucket :
@@ -632,15 +632,15 @@
 
 
 """
     exc_info = __test_parser_raises(
         mocker, input=input, exception=DSLUnexpectedEOF,
     )
 
-    assert repr(exc_info.value) == 'Unexpected EOF'
+    assert str(exc_info.value) == 'Unexpected EOF'
 
 
 def test_syntax_error_amount(mocker):
     # MISSING COLON
     input = """
 bucket my-bucket: amount 3
 \tregion: euw
```

### Comparing `thipster-0.16.1/tests/parser/dsl_parser/test_ast.py` & `thipster-0.16.2/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.16.2/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/tests/parser/dsl_parser/test_token.py` & `thipster-0.16.2/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.16.2/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/tests/parser/test_ParserFactory.py` & `thipster-0.16.2/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/tests/parser/test_YAMLParser.py` & `thipster-0.16.2/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/tests/parser/test_parsedfile.py` & `thipster-0.16.2/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/tests/test_e2e.py` & `thipster-0.16.2/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/auth/google.py` & `thipster-0.16.2/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/engine/engine.py` & `thipster-0.16.2/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/engine/i_parser.py` & `thipster-0.16.2/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/engine/i_repository.py` & `thipster-0.16.2/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/engine/i_terraform.py` & `thipster-0.16.2/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/engine/parsed_file.py` & `thipster-0.16.2/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/engine/resource_model.py` & `thipster-0.16.2/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/helpers.py` & `thipster-0.16.2/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/parser/dsl_parser/ast.py` & `thipster-0.16.2/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.16.2/thipster/parser/dsl_parser/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,84 @@
+from thipster.engine import THipsterException
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
-class DSLParserBaseException(Exception):
-    def __init__(self, message, *args: object) -> None:
+class DSLParserBaseException(THipsterException):
+    def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
-        self.__message = message
-
-    @property
-    def message(self):
-        return self.__message
-
 
 class DSLParserPathNotFound(DSLParserBaseException):
     def __init__(self, file, *args: object) -> None:
-        super().__init__(f'Path not found : {file}', *args)
+        super().__init__(*args)
+        self.file = file
+
+    @property
+    def message(self) -> str:
+        return f'Path not found : {self.file}'
 
 
-class DSLSyntaxException(Exception):
+class DSLSyntaxException(DSLParserBaseException):
     def __init__(self, token: Token, expected: TT | list[TT], *args: object) -> None:
         super().__init__(*args)
-        self.__tok = token
-        self.__exp = expected
-
-    def __repr__(self) -> str:
-
-        if type(self.__exp) is TT:
-            return f"""{str(self.__tok.position)} :\n\tSyntax error : Expected \
-{str(self.__exp.value)}, got {str(self.__tok.tokenType)}"""
-        else:
-            return f"""{str(self.__tok.position)} :\n\tSyntax error : Expected \
-{str(' or '.join(list(map(lambda x : str(x), self.__exp))))}, got {
-    str(self.__tok.tokenType)}"""
+        self.token = token
+        self.expected = expected
 
     @property
-    def tok(self):
-        return self.__tok
+    def message(self) -> str:
+        if type(self.expected) is TT:
+            return f"""{str(self.token.position)} :\n\tSyntax error : Expected \
+{str(self.expected.value)}, got {str(self.token.tokenType)}"""
+        else:
+            return f"""{str(self.token.position)} :\n\tSyntax error : Expected \
+{str(' or '.join(list(map(lambda x : str(x), self.expected))))}, got {
+    str(self.token.tokenType)}"""
 
 
-class DSLConditionException(Exception):
+class DSLConditionException(DSLParserBaseException):
     def __init__(self, token: Token, *args: object) -> None:
         super().__init__(*args)
-        self.__tok = token
+        self.token = token
 
-    def __repr__(self) -> str:
-        return f"""{str(self.__tok.position)} :\n\tBad condition"""
+    @property
+    def message(self) -> str:
+        return f"""{str(self.token.position)} :\n\tBad condition"""
 
 
-class DSLUnexpectedEOF(Exception):
+class DSLUnexpectedEOF(DSLParserBaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
-    def __repr__(self) -> str:
+    @property
+    def message(self) -> str:
         return 'Unexpected EOF'
 
 
 class DSLParserNoEndingQuotes(DSLParserBaseException):
     def __init__(self, position, *args: object) -> None:
-        super().__init__(
-            f'Invalid syntax, missing ending quotes at : {position}', *args,
-        )
+        super().__init__(*args)
+        self.position = position
+
+    @property
+    def message(self) -> str:
+        return f'Invalid syntax, missing ending quotes at : {self.position}'
+
+
+class DSLParserVariableAlreadyUsed(DSLParserBaseException):
+    def __init__(self, var: str, *args: object) -> None:
+        super().__init__(*args)
+        self.variable = var
+
+    @property
+    def message(self) -> str:
+        return f'Variable already used : {self.variable}',
+
+
+class DSLParserVariableNotDeclared(DSLParserBaseException):
+    def __init__(self, var: str, *args: object) -> None:
+        super().__init__(*args)
+        self.variable = var
+
+    @property
+    def message(self) -> str:
+        return f'Variable not declared : {self.variable}',
```

### Comparing `thipster-0.16.1/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.16.2/thipster/parser/dsl_parser/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 import thipster.engine.parsed_file as pf
 import thipster.parser.dsl_parser.ast as ast
 
-from .exceptions import DSLParserBaseException
+from .exceptions import (
+    DSLParserVariableAlreadyUsed,
+    DSLParserVariableNotDeclared,
+)
 from .token import TOKENTYPES as TT
 from .token_parser import DSLSyntaxException
 
 
-class DSLParserVariableAlreadyUsed(DSLParserBaseException):
-    def __init__(self, var: str, *args: object) -> None:
-        super().__init__(f'Variable already used : {var}', *args)
-
-
-class DSLParserVariableNotDeclared(DSLParserBaseException):
-    def __init__(self, var: str, *args: object) -> None:
-        super().__init__(f'Variable already used : {var}', *args)
-
-
 class Interpreter():
     """Interpreter class for the DSL Parser
 
     Implements a visitor design pattern on the AST nodes
     """
 
     def __init__(self) -> None:
```

### Comparing `thipster-0.16.1/thipster/parser/dsl_parser/lexer.py` & `thipster-0.16.2/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.16.2/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/parser/dsl_parser/parser.py` & `thipster-0.16.2/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/parser/dsl_parser/token.py` & `thipster-0.16.2/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.16.2/thipster/parser/dsl_parser/token_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         # [if_ctrl], "\n" (liste | dict)
         try:
             ifCtrl = self.__get_if_ctrl()
             self.__get_whitespaces()
             nl = self.__get_newline()
             properties = self.__get_properties(indent+1)
         except DSLSyntaxException as e:
-            if e.tok.tokenType == TT.TAB:
+            if e.token.tokenType == TT.TAB:
                 raise DSLSyntaxException(
                     token=nl,
                     expected=TT.STRING,
                 )
 
             raise e
 
@@ -474,15 +474,15 @@
 
                     self.__get_whitespaces()
                     expr2 = self.__get_arith_expr()
                     self.__get_whitespaces()
                     return ast.CompExprNode(expr1, op, expr2)
 
         except DSLSyntaxException as e:
-            raise DSLConditionException(e.tok)
+            raise DSLConditionException(e.token)
 
     def __get_arith_expr(self) -> ast.ArithExprNode:
         terms = []
         op = []
         terms.append(self.__get_term())
         self.__get_whitespaces()
```

### Comparing `thipster-0.16.1/thipster/parser/parser_factory.py` & `thipster-0.16.2/thipster/parser/parser_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 
 from thipster.engine import I_Parser
+from thipster.engine import THipsterException
 from thipster.engine.parsed_file import ParsedFile
 from .dsl_parser import DSLParser
 from .yaml_parser import YAMLParser
 
 
-class ParserPathNotFound(Exception):
+class ParserPathNotFound(THipsterException):
     def __init__(self, path, *args: object) -> None:
         super().__init__(*args)
 
-        self.__message = f'Path not found : {path}'
+        self.__path = path
 
     @property
-    def message(self):
-        return self.__message
+    def message(self) -> str:
+        return f'Path not found : {self.__path}'
 
 
 class ParserFactory(I_Parser):
 
     __parsers = {
         '.yaml': YAMLParser,
         '.yml': YAMLParser,
```

### Comparing `thipster-0.16.1/thipster/parser/yaml_parser.py` & `thipster-0.16.2/thipster/parser/yaml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import os
 
 import yaml
 from jinja2 import Environment, FileSystemLoader
+from thipster.engine import THipsterException
 
 import thipster.engine.parsed_file as pf
 from thipster.engine import I_Parser
 
 
-class YAMLParserBaseException(Exception):
-    def __init__(self, message, *args: object) -> None:
+class YAMLParserBaseException(THipsterException):
+    def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
-        self.__message = message
-
-    @property
-    def message(self):
-        return self.__message
-
 
 class YAMLParserPathNotFound(YAMLParserBaseException):
-    def __init__(file, *args: object) -> None:
-        super().__init__(f'Path not found : {file}', *args)
+    def __init__(self, file, *args: object) -> None:
+        super().__init__(*args)
+        self.file = file
+
+    @property
+    def message(self) -> str:
+        return f'Path not found : {self.file}',
 
 
 class YAMLParserNoName(YAMLParserBaseException):
-    def __init__(resource, *args: object) -> None:
-        super().__init__(f'No name for resource : {resource}', *args)
+    def __init__(self, resource, *args: object) -> None:
+        super().__init__(*args)
+        self.resource = resource
+
+    @property
+    def message(self) -> str:
+        return f'No name for resource : {self.resource}'
 
 
 class YAMLParser(I_Parser):
 
     def __getfiles(path: str) -> list[str]:
         """Recursively get all files names in the requested directory and its\
               sudirectories
```

### Comparing `thipster-0.16.1/thipster/repository/github.py` & `thipster-0.16.2/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/repository/json.py` & `thipster-0.16.2/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/terraform/cdk.py` & `thipster-0.16.2/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.1/thipster/terraform/exceptions.py` & `thipster-0.16.2/thipster/terraform/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-class CDKException(Exception):
-    @property
-    def message(self):
-        return str(self)
+from thipster.engine import THipsterException
+
+
+class CDKException(THipsterException):
+    pass
 
 
 class CDKInvalidAttribute(CDKException):
     def __init__(self, attr: str, modelType: str, **args: object) -> None:
         super().__init__(*args)
         self.__attr = attr
         self.__modelType = modelType
 
-    def __str__(self) -> str:
+    @property
+    def message(self) -> str:
         return f'{self.__attr} in {self.__modelType} but not useful'
 
 
 class CDKMissingAttribute(CDKException):
-    pass
+    @property
+    def message(self) -> str:
+        return 'Missing an attribute'
 
 
 class CDKMissingAttributeInDependency(CDKMissingAttribute):
     pass
 
 
 class CDKDependencyNotDeclared(CDKException):
     def __init__(self, depType: str, depName: str, **args: object) -> None:
         super().__init__(*args)
         self.__name = depName
         self.__type = depType
 
-    def __str__(self) -> str:
+    @property
+    def message(self) -> str:
         return f'{self.__type} {self.__name} not declared \
 (be sure to declare it before using it)'
 
 
 class CDKCyclicDependencies(CDKException):
     def __init__(self, stack: list[str], **args: object) -> None:
         super().__init__(*args)
         self.__stack = stack
 
-    def __str__(self) -> str:
+    @property
+    def message(self) -> str:
         return ','.join(self.__stack)
```

### Comparing `thipster-0.16.1/thipster.egg-info/PKG-INFO` & `thipster-0.16.2/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.1
+Version: 0.16.2
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.16.1/thipster.egg-info/SOURCES.txt` & `thipster-0.16.2/thipster.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 thipster.egg-info/dependency_links.txt
 thipster.egg-info/requires.txt
 thipster.egg-info/top_level.txt
 thipster/auth/__init__.py
 thipster/auth/google.py
 thipster/engine/__init__.py
 thipster/engine/engine.py
+thipster/engine/exceptions.py
 thipster/engine/i_auth.py
 thipster/engine/i_parser.py
 thipster/engine/i_repository.py
 thipster/engine/i_terraform.py
 thipster/engine/parsed_file.py
 thipster/engine/resource_model.py
 thipster/parser/__init__.py
```

