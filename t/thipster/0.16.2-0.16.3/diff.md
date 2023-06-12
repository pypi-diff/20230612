# Comparing `tmp/thipster-0.16.2.tar.gz` & `tmp/thipster-0.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.16.2.tar", last modified: Mon Jun 12 08:15:07 2023, max compression
+gzip compressed data, was "thipster-0.16.3.tar", last modified: Mon Jun 12 08:37:40 2023, max compression
```

## Comparing `thipster-0.16.2.tar` & `thipster-0.16.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-12 08:15:03.000000 thipster-0.16.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 08:15:03.000000 thipster-0.16.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4137 2023-06-12 08:15:07.306557 thipster-0.16.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3501 2023-06-12 08:15:03.000000 thipster-0.16.2/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-12 08:15:03.000000 thipster-0.16.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-12 08:15:03.000000 thipster-0.16.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 08:15:07.306557 thipster-0.16.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-12 08:15:04.000000 thipster-0.16.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     6952 2023-06-12 08:15:03.000000 thipster-0.16.2/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10326 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13387 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    19129 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6417 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.306557 thipster-0.16.2/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20100 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-12 08:15:03.000000 thipster-0.16.2/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:15:07.302557 thipster-0.16.2/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4137 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1688 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 08:15:07.000000 thipster-0.16.2/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.292230 thipster-0.16.3/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-12 08:37:36.000000 thipster-0.16.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 08:37:36.000000 thipster-0.16.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-12 08:37:40.292230 thipster-0.16.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-12 08:37:36.000000 thipster-0.16.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-12 08:37:36.000000 thipster-0.16.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-12 08:37:36.000000 thipster-0.16.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 08:37:40.292230 thipster-0.16.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-12 08:37:37.000000 thipster-0.16.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.284230 thipster-0.16.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.284230 thipster-0.16.3/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.284230 thipster-0.16.3/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15546 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     6924 2023-06-12 08:37:36.000000 thipster-0.16.3/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.292230 thipster-0.16.3/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13387 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19129 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6417 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.292230 thipster-0.16.3/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.292230 thipster-0.16.3/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20100 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-12 08:37:36.000000 thipster-0.16.3/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:37:40.288230 thipster-0.16.3/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 08:37:40.000000 thipster-0.16.3/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.16.2/LICENSE` & `thipster-0.16.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/PKG-INFO` & `thipster-0.16.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.2
+Version: 0.16.3
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -55,27 +55,26 @@
 You can use THipster in two ways:
 - By leveraging the [THipster CLI](https://github.com/THipster/THipster-cli)
 - By directly using the [THipster Python package](https://pypi.org/project/thipster/) in your own code
 
 Main feature:
 - Generate Terraform files from a YAML+JINJA or THIPS file:
 ```python
-from thipster.engine.Engine import Engine as ThipsterEngine
-from thipster.repository.GithubRepo import GithubRepo
-from thipster.parser.ParserFactory import ParserFactory
-from thipster.auth.Google import GoogleAuth
-from thipster.terraform.CDK import CDK
+from thipster import Engine as ThipsterEngine
+from thipster.auth import Google
+from thipster.parser import ParserFactory
+from thipster.repository import GithubRepo
+from thipster.terraform import Terraform
 
 # create new THipster engine
-engine = ThipsterEngine(ParserFactory(), GithubRepo('THipster/models'), GoogleAuth, CDK())
+engine = ThipsterEngine(ParserFactory(), GithubRepo('THipster/models'), Google, Terraform())
 
 # generate Terraform files and plan from a YAML+JINJA file
-
-list_dir, tf_plan = engine.run('path/to/file/or/directory')
-print(tf_plan)
+terraform_plan = engine.run('path/to/file/or/directory')
+print(terraform_plan)
 ```
 
 ## How to test the software
 
 To run the tests, you can use the following command:
 
 ```console
```

### Comparing `thipster-0.16.2/README.md` & `thipster-0.16.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,27 +40,26 @@
 You can use THipster in two ways:
 - By leveraging the [THipster CLI](https://github.com/THipster/THipster-cli)
 - By directly using the [THipster Python package](https://pypi.org/project/thipster/) in your own code
 
 Main feature:
 - Generate Terraform files from a YAML+JINJA or THIPS file:
 ```python
-from thipster.engine.Engine import Engine as ThipsterEngine
-from thipster.repository.GithubRepo import GithubRepo
-from thipster.parser.ParserFactory import ParserFactory
-from thipster.auth.Google import GoogleAuth
-from thipster.terraform.CDK import CDK
+from thipster import Engine as ThipsterEngine
+from thipster.auth import Google
+from thipster.parser import ParserFactory
+from thipster.repository import GithubRepo
+from thipster.terraform import Terraform
 
 # create new THipster engine
-engine = ThipsterEngine(ParserFactory(), GithubRepo('THipster/models'), GoogleAuth, CDK())
+engine = ThipsterEngine(ParserFactory(), GithubRepo('THipster/models'), Google, Terraform())
 
 # generate Terraform files and plan from a YAML+JINJA file
-
-list_dir, tf_plan = engine.run('path/to/file/or/directory')
-print(tf_plan)
+terraform_plan = engine.run('path/to/file/or/directory')
+print(terraform_plan)
 ```
 
 ## How to test the software
 
 To run the tests, you can use the following command:
 
 ```console
```

### Comparing `thipster-0.16.2/pyproject.toml` & `thipster-0.16.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/setup.py` & `thipster-0.16.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.16.2'
+__version__ = '0.16.3'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.16.2/tests/engine/test_engine.py` & `thipster-0.16.3/tests/engine/test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     repository = MockRepository()
     auth = MockAuth()
     terraform = MockTerraform()
 
     engine = eng.Engine(parser, repository, auth, terraform)
     res = engine.run('test.file')
 
-    assert res == (None, None)
+    assert res is None
 
 
 def test_parser_failure(mocker):
     def parserFail(self, filename: str):
         raise MockException('Parser failure')
 
     mocker.patch(
```

### Comparing `thipster-0.16.2/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.16.3/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/tests/parser/dsl_parser/test_ast.py` & `thipster-0.16.3/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.16.3/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/tests/parser/dsl_parser/test_token.py` & `thipster-0.16.3/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.16.3/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/tests/parser/test_ParserFactory.py` & `thipster-0.16.3/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/tests/parser/test_YAMLParser.py` & `thipster-0.16.3/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/tests/parser/test_parsedfile.py` & `thipster-0.16.3/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/tests/test_e2e.py` & `thipster-0.16.3/tests/test_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,25 +66,23 @@
     engine = Engine(
         ParserFactory(),
         LocalRepo(local_repo),
         MockAuth,
         Terraform(),
     )
     try:
-        output = engine.run(path_input)
+        engine.run(path_input)
     except Exception as e:
         raise e
     finally:
         __destroy_dir()
 
         if os.path.exists('cdktf.out'):
             shutil.rmtree('cdktf.out')
 
-    return output
-
 
 def get_output():
     with open('thipster.tf.json') as f:
         file_contents = json.load(f)
         f.close()
     return file_contents
```

### Comparing `thipster-0.16.2/thipster/auth/google.py` & `thipster-0.16.3/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/engine/engine.py` & `thipster-0.16.3/thipster/engine/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,19 +106,19 @@
         # Parse file or directory
         parsed_file = self._parse_files(path)
 
         # Get needed models
         models = self._get_models(parsed_file)
 
         # Generate Terraform files
-        dirs = self._generate_tf_files(parsed_file, models)
+        self._generate_tf_files(parsed_file, models)
 
         self.__terraform.init()
 
-        return dirs, self.__terraform.plan()
+        return self.__terraform.plan()
 
     def _parse_files(self, path: str) -> pf.ParsedFile:
         """Parse the input file or directory
 
         Parameters
         ----------
         path : str
@@ -167,17 +167,15 @@
             The dictionary of models
 
         Returns
         -------
         list[str]
             A list of directories containing the Terraform json files
         """
-        dirs = self.__terraform.generate(file, models, self.__auth)
-
-        return dirs
+        self.__terraform.generate(file, models, self.__auth)
 
     def _init_terraform(self) -> None:
         """Initialize Terraform
         """
         self.__terraform.init()
 
     def _plan_terraform(self) -> str:
```

### Comparing `thipster-0.16.2/thipster/engine/i_parser.py` & `thipster-0.16.3/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/engine/i_repository.py` & `thipster-0.16.3/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/engine/i_terraform.py` & `thipster-0.16.3/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/engine/parsed_file.py` & `thipster-0.16.3/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/engine/resource_model.py` & `thipster-0.16.3/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/helpers.py` & `thipster-0.16.3/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/dsl_parser/ast.py` & `thipster-0.16.3/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.16.3/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.16.3/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/dsl_parser/lexer.py` & `thipster-0.16.3/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.16.3/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/dsl_parser/parser.py` & `thipster-0.16.3/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/dsl_parser/token.py` & `thipster-0.16.3/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.16.3/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/parser_factory.py` & `thipster-0.16.3/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/parser/yaml_parser.py` & `thipster-0.16.3/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/repository/github.py` & `thipster-0.16.3/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/repository/json.py` & `thipster-0.16.3/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/terraform/cdk.py` & `thipster-0.16.3/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster/terraform/exceptions.py` & `thipster-0.16.3/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.2/thipster.egg-info/PKG-INFO` & `thipster-0.16.3/thipster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.2
+Version: 0.16.3
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -55,27 +55,26 @@
 You can use THipster in two ways:
 - By leveraging the [THipster CLI](https://github.com/THipster/THipster-cli)
 - By directly using the [THipster Python package](https://pypi.org/project/thipster/) in your own code
 
 Main feature:
 - Generate Terraform files from a YAML+JINJA or THIPS file:
 ```python
-from thipster.engine.Engine import Engine as ThipsterEngine
-from thipster.repository.GithubRepo import GithubRepo
-from thipster.parser.ParserFactory import ParserFactory
-from thipster.auth.Google import GoogleAuth
-from thipster.terraform.CDK import CDK
+from thipster import Engine as ThipsterEngine
+from thipster.auth import Google
+from thipster.parser import ParserFactory
+from thipster.repository import GithubRepo
+from thipster.terraform import Terraform
 
 # create new THipster engine
-engine = ThipsterEngine(ParserFactory(), GithubRepo('THipster/models'), GoogleAuth, CDK())
+engine = ThipsterEngine(ParserFactory(), GithubRepo('THipster/models'), Google, Terraform())
 
 # generate Terraform files and plan from a YAML+JINJA file
-
-list_dir, tf_plan = engine.run('path/to/file/or/directory')
-print(tf_plan)
+terraform_plan = engine.run('path/to/file/or/directory')
+print(terraform_plan)
 ```
 
 ## How to test the software
 
 To run the tests, you can use the following command:
 
 ```console
```

### Comparing `thipster-0.16.2/thipster.egg-info/SOURCES.txt` & `thipster-0.16.3/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

