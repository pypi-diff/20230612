# Comparing `tmp/thipster-0.16.0.tar.gz` & `tmp/thipster-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.16.0.tar", last modified: Thu Jun  8 15:18:49 2023, max compression
+gzip compressed data, was "thipster-0.16.1.tar", last modified: Mon Jun 12 08:10:12 2023, max compression
```

## Comparing `thipster-0.16.0.tar` & `thipster-0.16.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.810503 thipster-0.16.0/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-08 15:18:45.000000 thipster-0.16.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-08 15:18:45.000000 thipster-0.16.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-08 15:18:49.810503 thipster-0.16.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3390 2023-06-08 15:18:45.000000 thipster-0.16.0/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-08 15:18:45.000000 thipster-0.16.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-08 15:18:45.000000 thipster-0.16.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 15:18:49.810503 thipster-0.16.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-08 15:18:46.000000 thipster-0.16.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15548 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     6952 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.806502 thipster-0.16.0/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.806502 thipster-0.16.0/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.806502 thipster-0.16.0/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.810503 thipster-0.16.0/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10326 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13708 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    19125 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2254 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6275 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.810503 thipster-0.16.0/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.810503 thipster-0.16.0/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20189 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.806502 thipster-0.16.0/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.407849 thipster-0.16.1/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-12 08:10:08.000000 thipster-0.16.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 08:10:08.000000 thipster-0.16.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-06-12 08:10:12.407849 thipster-0.16.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3501 2023-06-12 08:10:08.000000 thipster-0.16.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-12 08:10:08.000000 thipster-0.16.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-12 08:10:08.000000 thipster-0.16.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 08:10:12.407849 thipster-0.16.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-12 08:10:09.000000 thipster-0.16.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.399850 thipster-0.16.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.399850 thipster-0.16.1/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.399850 thipster-0.16.1/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.399850 thipster-0.16.1/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15548 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     6952 2023-06-12 08:10:08.000000 thipster-0.16.1/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13708 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19125 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20100 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-06-12 08:10:08.000000 thipster-0.16.1/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:10:12.403849 thipster-0.16.1/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 08:10:12.000000 thipster-0.16.1/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.16.0/LICENSE` & `thipster-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/PKG-INFO` & `thipster-0.16.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.0
+Version: 0.16.1
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: google
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 
@@ -37,14 +38,20 @@
 
 To use THipster, you can simply install the package with pip:
 
 ```console
 pip install thipster
 ```
 
+If you want to install the google dependencies aswell use
+
+```console
+pip install thipster[google]
+```
+
 The list of available versions can be found on [PyPI](https://pypi.org/project/thipster/).
 
 ## Usage
 
 You can use THipster in two ways:
 - By leveraging the [THipster CLI](https://github.com/THipster/THipster-cli)
 - By directly using the [THipster Python package](https://pypi.org/project/thipster/) in your own code
@@ -85,15 +92,15 @@
 If you have questions, concerns, bug reports, etc, please file an issue in this repository's [Issue tracker](https://github.com/THipster/THipster/issues).
 
 ## Getting involved
 
 To install the project for development, you can use the following command:
 
 ```console
-pip install -r requirements.txt && pip install -e .[dev,test,doc]
+pip install -r requirements.txt && pip install -e .[dev,test,doc,google]
 pre-commit install && pre-commit run --all-files
 ```
 
 For more information on how to help out, please check the [CONTRIBUTING](https://github.com/THipster/THipster/blob/main/CONTRIBUTING.md) file.
 
 ## Open source licensing info
 1. [LICENSE](https://github.com/THipster/THipster/blob/main/LICENSE)
```

### Comparing `thipster-0.16.0/README.md` & `thipster-0.16.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 
 To use THipster, you can simply install the package with pip:
 
 ```console
 pip install thipster
 ```
 
+If you want to install the google dependencies aswell use
+
+```console
+pip install thipster[google]
+```
+
 The list of available versions can be found on [PyPI](https://pypi.org/project/thipster/).
 
 ## Usage
 
 You can use THipster in two ways:
 - By leveraging the [THipster CLI](https://github.com/THipster/THipster-cli)
 - By directly using the [THipster Python package](https://pypi.org/project/thipster/) in your own code
@@ -71,15 +77,15 @@
 If you have questions, concerns, bug reports, etc, please file an issue in this repository's [Issue tracker](https://github.com/THipster/THipster/issues).
 
 ## Getting involved
 
 To install the project for development, you can use the following command:
 
 ```console
-pip install -r requirements.txt && pip install -e .[dev,test,doc]
+pip install -r requirements.txt && pip install -e .[dev,test,doc,google]
 pre-commit install && pre-commit run --all-files
 ```
 
 For more information on how to help out, please check the [CONTRIBUTING](https://github.com/THipster/THipster/blob/main/CONTRIBUTING.md) file.
 
 ## Open source licensing info
 1. [LICENSE](https://github.com/THipster/THipster/blob/main/LICENSE)
```

### Comparing `thipster-0.16.0/pyproject.toml` & `thipster-0.16.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/setup.py` & `thipster-0.16.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.16.0'
+__version__ = '0.16.1'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
 
@@ -43,9 +43,14 @@
             'dagger.io',
             'pre-commit',
         ],
         'doc': [
             'sphinx',
             'myst-parser',
         ],
+
+        'google': [
+            'cdktf-cdktf-provider-google==7.0.9',
+            'google-auth==2.19.1',
+        ],
     },
 )
```

### Comparing `thipster-0.16.0/tests/engine/test_engine.py` & `thipster-0.16.1/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.16.1/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/parser/dsl_parser/test_ast.py` & `thipster-0.16.1/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.16.1/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/parser/dsl_parser/test_token.py` & `thipster-0.16.1/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.16.1/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/parser/test_ParserFactory.py` & `thipster-0.16.1/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/parser/test_YAMLParser.py` & `thipster-0.16.1/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/parser/test_parsedfile.py` & `thipster-0.16.1/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/tests/test_e2e.py` & `thipster-0.16.1/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/auth/google.py` & `thipster-0.16.1/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/engine/engine.py` & `thipster-0.16.1/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/engine/i_parser.py` & `thipster-0.16.1/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/engine/i_repository.py` & `thipster-0.16.1/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/engine/i_terraform.py` & `thipster-0.16.1/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/engine/parsed_file.py` & `thipster-0.16.1/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/engine/resource_model.py` & `thipster-0.16.1/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/helpers.py` & `thipster-0.16.1/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/dsl_parser/ast.py` & `thipster-0.16.1/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.16.1/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.16.1/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/dsl_parser/lexer.py` & `thipster-0.16.1/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.16.1/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/dsl_parser/parser.py` & `thipster-0.16.1/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/dsl_parser/token.py` & `thipster-0.16.1/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.16.1/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/parser/parser_factory.py` & `thipster-0.16.1/thipster/parser/parser_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,20 @@
                 files += self.__getfiles(f'{path}/{content}')
 
         if os.path.isfile(path):
             return [path]
 
         return files
 
-    def __noParser(self):
-        raise Exception()
+    def __noParser(self, pathExtension):
+        class noParser():
+            def run(path):
+                raise Exception(f'{pathExtension} files can\'t be parsed')
+
+        return noParser
 
     def run(self, path: str) -> ParsedFile:
         """Run the ParserFactory
 
         Parameters
         ----------
         path: str
@@ -86,8 +90,10 @@
 
         return res
 
     def __getParser(self, path) -> I_Parser:
 
         _, pathExtension = os.path.splitext(path)
 
-        return ParserFactory.__parsers.get(pathExtension, self.__noParser)
+        return ParserFactory.__parsers.get(
+            pathExtension, self.__noParser(pathExtension),
+        )
```

### Comparing `thipster-0.16.0/thipster/parser/yaml_parser.py` & `thipster-0.16.1/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/repository/github.py` & `thipster-0.16.1/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/repository/json.py` & `thipster-0.16.1/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster/terraform/cdk.py` & `thipster-0.16.1/thipster/terraform/cdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from thipster.engine import I_Auth, I_Terraform
 from thipster.helpers import create_logger as Logger
 
 
 class CDK(I_Terraform):
     _models = []
     _parent_resources_stack = []
-    _imported_packages = []
 
     _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
     _logger = Logger(__name__)
 
     def apply(self, plan_file_path: str | None = None):
         """Applies generated Terraform plan
@@ -57,14 +56,15 @@
             associated models
         _auth : I_Auth
             authenticator to use
         """
         CDK._created_resources = {}
         CDK._models = models
         CDK._parent_resources_stack = []
+
         # Init CDK
         app = App()
 
         f_position = file.resources[0].position
         file_name = f_position.fileName if f_position else 'thipster_infrastructure'
 
         CDK._logger.debug('Creating tf code for file %s', file_name)
@@ -139,19 +139,18 @@
         """Install a package if it wasn't already installed by thipster
 
         Parameters
         ----------
         package : str
             package to install
         """
-        if package not in CDK._imported_packages:
+        if package not in sys.modules:
             subprocess.check_call(
                 [sys.executable, '-m', 'pip', 'install', '-qqq', package],
             )
-            CDK._imported_packages.append(package)
 
     def _import(package_name: str, module_name: str, class_name: str) -> type:
         """Import a class from any package
 
         Parameters
         ----------
         package_name : str
```

### Comparing `thipster-0.16.0/thipster/terraform/exceptions.py` & `thipster-0.16.1/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.0/thipster.egg-info/PKG-INFO` & `thipster-0.16.1/thipster.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.0
+Version: 0.16.1
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: google
 License-File: LICENSE
 
 # THipster
 
 THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 
@@ -37,14 +38,20 @@
 
 To use THipster, you can simply install the package with pip:
 
 ```console
 pip install thipster
 ```
 
+If you want to install the google dependencies aswell use
+
+```console
+pip install thipster[google]
+```
+
 The list of available versions can be found on [PyPI](https://pypi.org/project/thipster/).
 
 ## Usage
 
 You can use THipster in two ways:
 - By leveraging the [THipster CLI](https://github.com/THipster/THipster-cli)
 - By directly using the [THipster Python package](https://pypi.org/project/thipster/) in your own code
@@ -85,15 +92,15 @@
 If you have questions, concerns, bug reports, etc, please file an issue in this repository's [Issue tracker](https://github.com/THipster/THipster/issues).
 
 ## Getting involved
 
 To install the project for development, you can use the following command:
 
 ```console
-pip install -r requirements.txt && pip install -e .[dev,test,doc]
+pip install -r requirements.txt && pip install -e .[dev,test,doc,google]
 pre-commit install && pre-commit run --all-files
 ```
 
 For more information on how to help out, please check the [CONTRIBUTING](https://github.com/THipster/THipster/blob/main/CONTRIBUTING.md) file.
 
 ## Open source licensing info
 1. [LICENSE](https://github.com/THipster/THipster/blob/main/LICENSE)
```

### Comparing `thipster-0.16.0/thipster.egg-info/SOURCES.txt` & `thipster-0.16.1/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

