# Comparing `tmp/thipster-0.16.3.tar.gz` & `tmp/thipster-0.16.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.16.3.tar", last modified: Mon Jun 12 08:37:40 2023, max compression
+gzip compressed data, was "thipster-0.16.4.tar", last modified: Mon Jun 12 08:42:39 2023, max compression
```

## Comparing `thipster-0.16.3.tar` & `thipster-0.16.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.292230 thipster-0.16.3/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-12 08:37:36.000000 thipster-0.16.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 08:37:36.000000 thipster-0.16.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4094 2023-06-12 08:37:40.292230 thipster-0.16.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3458 2023-06-12 08:37:36.000000 thipster-0.16.3/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-12 08:37:36.000000 thipster-0.16.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-12 08:37:36.000000 thipster-0.16.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 08:37:40.292230 thipster-0.16.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-12 08:37:37.000000 thipster-0.16.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.284230 thipster-0.16.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.284230 thipster-0.16.3/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3214 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.284230 thipster-0.16.3/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     6924 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5070 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.292230 thipster-0.16.3/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10326 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13387 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    19129 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6417 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.292230 thipster-0.16.3/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.292230 thipster-0.16.3/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20100 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4094 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1688 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.701296 thipster-0.16.4/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-12 08:42:36.000000 thipster-0.16.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 08:42:36.000000 thipster-0.16.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-12 08:42:39.701296 thipster-0.16.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-12 08:42:36.000000 thipster-0.16.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-12 08:42:36.000000 thipster-0.16.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-12 08:42:36.000000 thipster-0.16.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 08:42:39.701296 thipster-0.16.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-06-12 08:42:37.000000 thipster-0.16.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15546 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     6924 2023-06-12 08:42:36.000000 thipster-0.16.4/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.693296 thipster-0.16.4/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.697296 thipster-0.16.4/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.697296 thipster-0.16.4/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.697296 thipster-0.16.4/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.701296 thipster-0.16.4/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13387 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19129 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6417 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.701296 thipster-0.16.4/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.701296 thipster-0.16.4/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20100 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-12 08:42:36.000000 thipster-0.16.4/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:42:39.697296 thipster-0.16.4/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 08:42:39.000000 thipster-0.16.4/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.16.3/LICENSE` & `thipster-0.16.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/PKG-INFO` & `thipster-0.16.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.3
+Version: 0.16.4
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.16.3/README.md` & `thipster-0.16.4/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/pyproject.toml` & `thipster-0.16.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/setup.py` & `thipster-0.16.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.16.3'
+__version__ = '0.16.4'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
 
@@ -45,12 +45,12 @@
         ],
         'doc': [
             'sphinx',
             'myst-parser',
         ],
 
         'google': [
-            'cdktf-cdktf-provider-google==7.0.9',
+            'cdktf-cdktf-provider-google==7.0.10',
             'google-auth==2.19.1',
         ],
     },
 )
```

### Comparing `thipster-0.16.3/tests/engine/test_engine.py` & `thipster-0.16.4/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.16.4/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/parser/dsl_parser/test_ast.py` & `thipster-0.16.4/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.16.4/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/parser/dsl_parser/test_token.py` & `thipster-0.16.4/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.16.4/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/parser/test_ParserFactory.py` & `thipster-0.16.4/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/parser/test_YAMLParser.py` & `thipster-0.16.4/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/parser/test_parsedfile.py` & `thipster-0.16.4/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/tests/test_e2e.py` & `thipster-0.16.4/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/auth/google.py` & `thipster-0.16.4/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/engine/engine.py` & `thipster-0.16.4/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/engine/i_parser.py` & `thipster-0.16.4/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/engine/i_repository.py` & `thipster-0.16.4/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/engine/i_terraform.py` & `thipster-0.16.4/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/engine/parsed_file.py` & `thipster-0.16.4/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/engine/resource_model.py` & `thipster-0.16.4/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/helpers.py` & `thipster-0.16.4/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/dsl_parser/ast.py` & `thipster-0.16.4/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.16.4/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.16.4/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/dsl_parser/lexer.py` & `thipster-0.16.4/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.16.4/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/dsl_parser/parser.py` & `thipster-0.16.4/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/dsl_parser/token.py` & `thipster-0.16.4/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.16.4/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/parser_factory.py` & `thipster-0.16.4/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/parser/yaml_parser.py` & `thipster-0.16.4/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/repository/github.py` & `thipster-0.16.4/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/repository/json.py` & `thipster-0.16.4/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/terraform/cdk.py` & `thipster-0.16.4/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster/terraform/exceptions.py` & `thipster-0.16.4/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.3/thipster.egg-info/PKG-INFO` & `thipster-0.16.4/thipster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.3
+Version: 0.16.4
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.16.3/thipster.egg-info/SOURCES.txt` & `thipster-0.16.4/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

