# Comparing `tmp/pymaidol-0.1.2.tar.gz` & `tmp/pymaidol-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymaidol-0.1.2.tar", last modified: Thu May 25 05:41:11 2023, max compression
+gzip compressed data, was "/home/fqj/pymaidol/dist/.tmp-_lmblz5z/pymaidol-0.1.3.tar", last modified: Mon Jun 12 15:40:13 2023, max compression
```

## Comparing `pymaidol-0.1.2.tar` & `pymaidol-0.1.3.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.719943 pymaidol-0.1.2/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2028 2023-05-23 13:11:17.000000 pymaidol-0.1.2/.gitignore
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1080 2023-05-23 13:11:17.000000 pymaidol-0.1.2/LICENSE
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3309 2023-05-25 05:41:11.719943 pymaidol-0.1.2/PKG-INFO
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2905 2023-05-25 05:40:12.000000 pymaidol-0.1.2/README.md
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.707943 pymaidol-0.1.2/docs/
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/docs/zh-cn/
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/docs/zh-cn/AnnotationType/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      379 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/AnnotationType/AnnotationTypeEnum枚举.md
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      907 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/AnnotationType/AnnotationType模块.md
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      731 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/AnnotationType/MultiLineAnnotationTypeEnum枚举.md
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      692 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/AnnotationType/SingleLineAnnotationTypeEnum枚举.md
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1469 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/Position类.md
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      530 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/Pymaidol_API目录.md
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2080 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/TemplateBase类.md
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1359 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/TemplateRenderer类.md
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2957 2023-05-23 13:11:17.000000 pymaidol-0.1.2/docs/zh-cn/语法参考.md
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/examples/
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/examples/first_template/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      714 2023-05-25 05:40:12.000000 pymaidol-0.1.2/examples/first_template/FirstTemplate.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)       79 2023-05-23 13:11:17.000000 pymaidol-0.1.2/examples/first_template/FirstTemplate.pymd
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/examples/template_renderer/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      705 2023-05-25 05:40:12.000000 pymaidol-0.1.2/examples/template_renderer/renderer_demo.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      118 2023-05-25 05:40:12.000000 pymaidol-0.1.2/examples/template_renderer/template.pymd
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.715943 pymaidol-0.1.2/pymaidol/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      663 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/AnnotationType.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3598 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/Errors.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     5719 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/Executor.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3857 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/Nodes.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)    26701 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/Parser.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      930 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/Positions.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3954 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/SyntaxChecker.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2794 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/TemplateBase.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1649 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/TemplateRenderer.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     7475 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/Traversers.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      436 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/__init__.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1365 2023-05-24 08:16:01.000000 pymaidol-0.1.2/pymaidol/__main__.py
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.715943 pymaidol-0.1.2/pymaidol/code_templates/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      548 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/code_templates/SubClassTemplate.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      478 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/code_templates/SubClassTemplate.pymd
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/code_templates/__init__.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1209 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/keywords.py
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.715943 pymaidol-0.1.2/pymaidol.egg-info/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3309 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/PKG-INFO
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1550 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/SOURCES.txt
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        1 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/dependency_links.txt
--rw-rw-r--   0 eterance  (1000) eterance  (1000)       22 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/requires.txt
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        9 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/top_level.txt
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      557 2023-05-24 07:32:43.000000 pymaidol-0.1.2/pyproject.toml
--rw-rw-r--   0 eterance  (1000) eterance  (1000)       38 2023-05-25 05:41:11.719943 pymaidol-0.1.2/setup.cfg
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.715943 pymaidol-0.1.2/tests/
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.719943 pymaidol-0.1.2/tests/harder_demo/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      367 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/CodeLangTemplate.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      892 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/CodeLangTemplate.pymd
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      472 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/codelang.json
--rw-rw-r--   0 eterance  (1000) eterance  (1000)    83313 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1274 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset.pml
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      198 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      718 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset_pml.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      234 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/test_class.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/test_class.pymd
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1188 2023-05-25 05:40:12.000000 pymaidol-0.1.2/tests/test_everything.py
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     2028 2023-06-12 15:35:09.000000 pymaidol-0.1.3/.gitignore
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1080 2023-06-12 15:36:03.000000 pymaidol-0.1.3/LICENSE
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     3343 2023-06-12 15:40:13.000000 pymaidol-0.1.3/PKG-INFO
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     2939 2023-06-12 15:36:04.000000 pymaidol-0.1.3/README.md
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/docs/
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/docs/zh-cn/
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/docs/zh-cn/AnnotationType/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      379 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/AnnotationType/AnnotationTypeEnum枚举.md
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      907 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/AnnotationType/AnnotationType模块.md
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      731 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/AnnotationType/MultiLineAnnotationTypeEnum枚举.md
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      692 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/AnnotationType/SingleLineAnnotationTypeEnum枚举.md
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1469 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/Position类.md
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      530 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/Pymaidol_API目录.md
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     2511 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/TemplateBase类.md
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1359 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/TemplateRenderer类.md
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     2957 2023-06-12 15:36:03.000000 pymaidol-0.1.3/docs/zh-cn/语法参考.md
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/examples/
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/examples/first_template/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      732 2023-06-12 15:36:03.000000 pymaidol-0.1.3/examples/first_template/FirstTemplate.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)       79 2023-06-12 15:36:03.000000 pymaidol-0.1.3/examples/first_template/FirstTemplate.pymd
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/examples/template_renderer/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      733 2023-06-12 15:36:03.000000 pymaidol-0.1.3/examples/template_renderer/renderer_demo.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      118 2023-06-12 15:36:03.000000 pymaidol-0.1.3/examples/template_renderer/template.pymd
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/pymaidol/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      687 2023-06-12 15:36:03.000000 pymaidol-0.1.3/pymaidol/AnnotationType.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     3696 2023-06-12 15:36:03.000000 pymaidol-0.1.3/pymaidol/Errors.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     5868 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/Executor.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     3997 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/Nodes.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)    27231 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/Parser.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      930 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/Positions.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     4034 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/SyntaxChecker.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     3272 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/TemplateBase.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1649 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/TemplateRenderer.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     7638 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/Traversers.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      436 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/__init__.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1400 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/__main__.py
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/pymaidol/code_templates/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      559 2023-06-12 15:36:03.000000 pymaidol-0.1.3/pymaidol/code_templates/SubClassTemplate.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      579 2023-06-12 15:36:03.000000 pymaidol-0.1.3/pymaidol/code_templates/SubClassTemplate.pymd
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:36:03.000000 pymaidol-0.1.3/pymaidol/code_templates/__init__.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1255 2023-06-12 15:36:04.000000 pymaidol-0.1.3/pymaidol/keywords.py
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/pymaidol.egg-info/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     3343 2023-06-12 15:40:12.000000 pymaidol-0.1.3/pymaidol.egg-info/PKG-INFO
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1638 2023-06-12 15:40:13.000000 pymaidol-0.1.3/pymaidol.egg-info/SOURCES.txt
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)        1 2023-06-12 15:40:12.000000 pymaidol-0.1.3/pymaidol.egg-info/dependency_links.txt
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)       22 2023-06-12 15:40:12.000000 pymaidol-0.1.3/pymaidol.egg-info/requires.txt
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)        9 2023-06-12 15:40:12.000000 pymaidol-0.1.3/pymaidol.egg-info/top_level.txt
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      578 2023-06-12 15:39:01.000000 pymaidol-0.1.3/pyproject.toml
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)       38 2023-06-12 15:40:13.000000 pymaidol-0.1.3/setup.cfg
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/tests/
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/tests/din/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      687 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/din/ContextDebugTemplate.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      976 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/din/ContextDebugTemplate.pymd
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      697 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/din/test.py
+drwxrwxr-x   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:40:13.000000 pymaidol-0.1.3/tests/harder_demo/
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      367 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/harder_demo/CodeLangTemplate.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      892 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/harder_demo/CodeLangTemplate.pymd
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      472 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/harder_demo/codelang.json
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)    83313 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1274 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/harder_demo/sparc_sub_dataset.pml
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      198 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/harder_demo/sparc_sub_dataset.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      718 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/harder_demo/sparc_sub_dataset_pml.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)      238 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/test_class.py
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)        0 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/test_class.pymd
+-rw-rw-r--   0 fqj       (1052) fqj       (1052)     1188 2023-06-12 15:36:06.000000 pymaidol-0.1.3/tests/test_everything.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pymaidol-0.1.2/.gitignore` & `pymaidol-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/LICENSE` & `pymaidol-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/PKG-INFO` & `pymaidol-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymaidol
-Version: 0.1.2
+Version: 0.1.3
 Summary: A markup gramma that embed python code into text
 Author: Eterance
 Keywords: Prompt,Markup Language,NLP,AI,GPT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -20,15 +20,15 @@
 ⚠**警告：Pymaidol 目前处于开发阶段，语法和一些对空白符、换行符的处理逻辑尚未确定，以后可能会被修改。强烈不建议在生产环境中使用。**
 
 ## 环境要求与安装
 
 python >= 3.10
 
 ``` bash
-pip install Pymaidol
+pip install Pymaidol -i https://pypi.python.org/simple
 ```
 
 ## 第一个 Pymaidol 模板
 
 ### 创建模板文件
 
 首先，假设你创建了一个名为 `pymaidol_test` 的文件夹。使用编辑器或者 IDE 打开该文件夹作为工作目录。
```

### Comparing `pymaidol-0.1.2/README.md` & `pymaidol-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ⚠**警告：Pymaidol 目前处于开发阶段，语法和一些对空白符、换行符的处理逻辑尚未确定，以后可能会被修改。强烈不建议在生产环境中使用。**
 
 ## 环境要求与安装
 
 python >= 3.10
 
 ``` bash
-pip install Pymaidol
+pip install Pymaidol -i https://pypi.python.org/simple
 ```
 
 ## 第一个 Pymaidol 模板
 
 ### 创建模板文件
 
 首先，假设你创建了一个名为 `pymaidol_test` 的文件夹。使用编辑器或者 IDE 打开该文件夹作为工作目录。
```

### Comparing `pymaidol-0.1.2/docs/zh-cn/AnnotationType/AnnotationType模块.md` & `pymaidol-0.1.3/docs/zh-cn/AnnotationType/AnnotationType模块.md`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/docs/zh-cn/AnnotationType/MultiLineAnnotationTypeEnum枚举.md` & `pymaidol-0.1.3/docs/zh-cn/AnnotationType/MultiLineAnnotationTypeEnum枚举.md`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/docs/zh-cn/AnnotationType/SingleLineAnnotationTypeEnum枚举.md` & `pymaidol-0.1.3/docs/zh-cn/AnnotationType/SingleLineAnnotationTypeEnum枚举.md`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/docs/zh-cn/Position类.md` & `pymaidol-0.1.3/docs/zh-cn/Position类.md`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/docs/zh-cn/Pymaidol_API目录.md` & `pymaidol-0.1.3/docs/zh-cn/Pymaidol_API目录.md`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/docs/zh-cn/TemplateBase类.md` & `pymaidol-0.1.3/docs/zh-cn/TemplateBase类.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ### `TemplateBase(template, template_file_path, supported_annotation_types)` (virtual)
 
 #### 参数
 
 - `template` (str, optional): 模板字符串。默认为 `None`。
 - `template_file_path` (str, optional): 模板文件路径。默认为 `None`。
 - `supported_annotation_types` (list[AnnotationTypeEnum], optional): 支持的注释类型列表。默认为所有注释类型（Python、C的单行与多行注释、HTML注释）。
+- `disable_annotation_types` (list[AnnotationTypeEnum], optional): 禁用的注释类型列表，使这些注释出现在渲染后的文本中。默认为空。禁用的优先级高于支持。例如，如果 `disable_annotation_types` 中包含 `AnnotationTypeEnum.SingleLineAnnotationTypeEnum.Python` （python 单行注释），则 `supported_annotation_types` 中无论是否包含它，都将被视为禁用该注释类型。
 
 当 `template` 与 `template_file_path` 都为 `None` 时，`TemplateBase` 类及其子类将试图读取在与其同一目录下、与其同名的模板文件 `.pymd`。如果两个都不为空，则优先使用 `template`。
 
 ## 属性
 
 ### `rendered`（str，readonly）
```

### Comparing `pymaidol-0.1.2/docs/zh-cn/TemplateRenderer类.md` & `pymaidol-0.1.3/docs/zh-cn/TemplateRenderer类.md`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/docs/zh-cn/语法参考.md` & `pymaidol-0.1.3/docs/zh-cn/语法参考.md`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/examples/first_template/FirstTemplate.py` & `pymaidol-0.1.3/pymaidol/code_templates/SubClassTemplate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,11 @@
-from pymaidol import TemplateBase
-from pymaidol.AnnotationType import FULL_ANNOTATION_TYPE, AnnotationTypeEnum
-
-class FirstTemplate(TemplateBase):
-    def __init__(self, 
-                 package_name:str, 
-                 template: str | None = None, 
-                 template_file_path: str | None = None, 
-                 supported_annotation_types: list[AnnotationTypeEnum] = FULL_ANNOTATION_TYPE) -> None:
-        super().__init__(template, template_file_path, supported_annotation_types)
-        self.package_name = package_name
-        
-def main():
-    template = FirstTemplate("Pymaidol")
-    string = template.Render({"says": "Hello World"})
-    print(string)
-    
-if __name__ == "__main__":
-    main()
+from pymaidol.AnnotationType import FULL_ANNOTATION_TYPE, AnnotationTypeEnum
+from pymaidol.TemplateBase import TemplateBase
+
+class SubClassTemplate(TemplateBase):
+    def __init__(self, 
+                 class_name:str, 
+                 template: str | None = None, 
+                 template_file_path: str | None = None, 
+                 supported_annotation_types: list[AnnotationTypeEnum] = FULL_ANNOTATION_TYPE) -> None:
+        super().__init__(template, template_file_path, supported_annotation_types)
+        self.class_name = class_name
```

### Comparing `pymaidol-0.1.2/examples/template_renderer/renderer_demo.py` & `pymaidol-0.1.3/examples/template_renderer/renderer_demo.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import os
-import sys
-ROOT_DIR = os.path.join(os.path.dirname(__file__), "../../")
-sys.path.append(ROOT_DIR)
-from pymaidol import TemplateRenderer
-from pymaidol.AnnotationType import SingleLineAnnotationTypeEnum
-
-USELESS = "USELESS"
-
-def main():
-    renderer = TemplateRenderer.ReadFromFile("examples\\template_renderer\\template.pymd", [SingleLineAnnotationTypeEnum.C])
-    alpha = 42
-    beta = 3.14
-    print(renderer.Render(
-        {
-            "global_vars": 
-            {
-                "USELESS": USELESS
-            },
-            "local_vars":
-            {
-                "alpha": alpha, 
-                "beta": beta
-            }
-        }
-    ))
-    
-if __name__ == "__main__":
+import os
+import sys
+ROOT_DIR = os.path.join(os.path.dirname(__file__), "../../")
+sys.path.append(ROOT_DIR)
+from pymaidol import TemplateRenderer
+from pymaidol.AnnotationType import SingleLineAnnotationTypeEnum
+
+USELESS = "USELESS"
+
+def main():
+    renderer = TemplateRenderer.ReadFromFile("examples\\template_renderer\\template.pymd", [SingleLineAnnotationTypeEnum.C])
+    alpha = 42
+    beta = 3.14
+    print(renderer.Render(
+        {
+            "global_vars": 
+            {
+                "USELESS": USELESS
+            },
+            "local_vars":
+            {
+                "alpha": alpha, 
+                "beta": beta
+            }
+        }
+    ))
+    
+if __name__ == "__main__":
     main()
```

### Comparing `pymaidol-0.1.2/pymaidol/AnnotationType.py` & `pymaidol-0.1.3/pymaidol/AnnotationType.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from enum import Enum
-
-
-class AnnotationTypeEnum(Enum):
-    pass
-
-class SingleLineAnnotationTypeEnum(AnnotationTypeEnum):    
-    Python:str = "#"
-    C:str = "//"
-    
-class MultiLineAnnotationTypeEnum(AnnotationTypeEnum):
-    PythonSingleQuotation:str = "'''"    
-    PythonDoubleQuotation:str = '"""'
-    C:str = "/*"
-    Html:str = "<!--"
-    
-FULL_ANNOTATION_TYPE:list[AnnotationTypeEnum] = [
-    SingleLineAnnotationTypeEnum.Python,
-    SingleLineAnnotationTypeEnum.C,
-    MultiLineAnnotationTypeEnum.PythonSingleQuotation,
-    MultiLineAnnotationTypeEnum.PythonDoubleQuotation,
-    MultiLineAnnotationTypeEnum.C,
-    MultiLineAnnotationTypeEnum.Html
-]
+from enum import Enum
+
+
+class AnnotationTypeEnum(Enum):
+    pass
+
+class SingleLineAnnotationTypeEnum(AnnotationTypeEnum):    
+    Python:str = "#"
+    C:str = "//"
+    
+class MultiLineAnnotationTypeEnum(AnnotationTypeEnum):
+    PythonSingleQuotation:str = "'''"    
+    PythonDoubleQuotation:str = '"""'
+    C:str = "/*"
+    Html:str = "<!--"
+    
+FULL_ANNOTATION_TYPE:list[AnnotationTypeEnum] = [
+    SingleLineAnnotationTypeEnum.Python,
+    SingleLineAnnotationTypeEnum.C,
+    MultiLineAnnotationTypeEnum.PythonSingleQuotation,
+    MultiLineAnnotationTypeEnum.PythonDoubleQuotation,
+    MultiLineAnnotationTypeEnum.C,
+    MultiLineAnnotationTypeEnum.Html
+]
```

### Comparing `pymaidol-0.1.2/pymaidol/Executor.py` & `pymaidol-0.1.3/pymaidol/Executor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,124 @@
-
-from collections.abc import Iterable
-from enum import Enum
-from typing import Any
-
-from pymaidol.Errors import (LackingConditionError, NameException, PythonExecutionError,
-                    TypeException, WrongForStatement)
-from pymaidol.Nodes import (AnnotationNode, BaseNode, BodyComponent, BranchRole,
-                   BreakNode, CodeBlockNode, ComponentOrRole, ContinueNode,
-                   ElifNode, ElseNode, EmptyNode, ForNode, IfNode,
-                   InvisibleRole, LoopRole, NonTerminalNode, ShowBlockNode,
-                   TerminalNode, TextNode, VisibleRole, WhileNode)
-
-
-class ControlResultEnum(Enum):
-    Default = "Default"
-    Break = "Break"
-    Continue = "Continue"
-
-
-class Executor:
-    def __init__(self, root:BaseNode) -> None:
-        self._root = root
-        self._prompt = ""
-    
-    @property
-    def root(self):
-        return self._root
-        
-    def Execute(self, global_var:dict[str, Any], local_var:dict[str, Any]) -> str:
-        self._recursive_traverse(self._root, global_var, local_var)
-        return self._prompt
-        
-    def _recursive_traverse(self, node:BaseNode, global_var:dict[str, Any], local_var:dict[str, Any]) -> ControlResultEnum:
-        if isinstance(node, NonTerminalNode):
-            if isinstance(node, (IfNode, ElifNode)):
-                try:
-                    result = eval(node.condition, global_var, local_var)
-                    if result:
-                        for child in node.children:
-                            result = self._recursive_traverse(child, global_var, local_var)
-                            if result == ControlResultEnum.Break or result == ControlResultEnum.Continue:
-                                return result
-                        return ControlResultEnum.Default
-                    else:
-                        if node.next_branch is not None:
-                            return self._recursive_traverse(node.next_branch, global_var, local_var)
-                        else:
-                            return ControlResultEnum.Default
-                except Exception as ex:
-                    raise PythonExecutionError(node.start, ex)
-            
-            elif isinstance(node, ElseNode):
-                for child in node.children:
-                    result = self._recursive_traverse(child, global_var, local_var)
-                    if result == ControlResultEnum.Break or result == ControlResultEnum.Continue:
-                        return result
-                return ControlResultEnum.Default
-                
-            elif isinstance(node, ForNode):
-                # 提取变量名和可枚举对象
-                strings = node.condition.split(" in ")
-                assert len(strings) == 2, WrongForStatement(node.start)
-                variables_string = strings[0].strip()
-                try:
-                    enumerate_object = eval(strings[1].strip(), global_var, local_var)
-                except NameError as ne:
-                    raise NameException(node.start, str(ne))
-                assert isinstance(enumerate_object, Iterable), TypeException(node.start, f"{strings[1].strip()} ({type(enumerate_object)}) is not iterable")
-                
-                try:
-                    for element in enumerate_object:
-                        exec(f"{variables_string} = {element}", global_var, local_var)
-                        for child in node.children:
-                            result = self._recursive_traverse(child, global_var, local_var)
-                            if result == ControlResultEnum.Break:
-                                return ControlResultEnum.Default
-                            elif result == ControlResultEnum.Continue:
-                                break
-                    return ControlResultEnum.Default
-                except Exception as ex:
-                    raise PythonExecutionError(node.start, ex)
-                
-            elif isinstance(node, WhileNode):
-                try:
-                    while (result := eval(node.condition, global_var, local_var)):
-                        for child in node.children:
-                            result = self._recursive_traverse(child, global_var, local_var)
-                            if result == ControlResultEnum.Break:
-                                return ControlResultEnum.Default
-                            elif result == ControlResultEnum.Continue:
-                                break
-                    return ControlResultEnum.Default
-                except Exception as ex:
-                    raise PythonExecutionError(node.start, ex)
-            
-            else:
-                for child in node.children:
-                    self._recursive_traverse(child, global_var, local_var)
-                return ControlResultEnum.Default
-        else:
-            if type(node) == TextNode:
-                self._prompt = f"{self._prompt}{node.content}"
-                
-            elif type(node) == ShowBlockNode:
-                try:
-                    self._prompt = f"{self._prompt}{eval(node.body, global_var, local_var)}"
-                except Exception as ex:
-                    raise PythonExecutionError(node.start, ex)
-                
-            elif type(node) == CodeBlockNode:
-                try:
-                    exec(node.body, global_var, local_var)
-                except Exception as ex:
-                    raise PythonExecutionError(node.start, ex)
-                
-            elif type(node) == BreakNode:
-                return ControlResultEnum.Break
-            
-            elif type(node) == ContinueNode:
-                return ControlResultEnum.Continue
-            
+
+from collections.abc import Iterable
+from enum import Enum
+from typing import Any
+
+from pymaidol.Errors import (LackingConditionError, NameException, PythonExecutionError,
+                    TypeException, WrongForStatement)
+from pymaidol.Nodes import (AnnotationNode, BaseNode, BodyComponent, BranchRole,
+                   BreakNode, CodeBlockNode, ComponentOrRole, ContinueNode,
+                   ElifNode, ElseNode, EmptyNode, ForNode, IfNode,
+                   InvisibleRole, LoopRole, NonTerminalNode, ShowBlockNode,
+                   TerminalNode, TextNode, VisibleRole, WhileNode)
+
+
+class ControlResultEnum(Enum):
+    Default = "Default"
+    Break = "Break"
+    Continue = "Continue"
+
+
+class Executor:
+    def __init__(self, root:BaseNode) -> None:
+        self._root = root
+        self._prompt = ""
+    
+    @property
+    def root(self):
+        return self._root
+        
+    def Execute(self, global_var:dict[str, Any], local_var:dict[str, Any]) -> str:
+        self._prompt = ""
+        self._recursive_traverse(self._root, global_var, local_var)
+        return self._prompt
+        
+    def _recursive_traverse(self, node:BaseNode, global_var:dict[str, Any], local_var:dict[str, Any]) -> ControlResultEnum:
+        if isinstance(node, NonTerminalNode):
+            if isinstance(node, (IfNode, ElifNode)):
+                try:
+                    result = eval(node.condition, global_var, local_var)
+                    if result:
+                        for child in node.children:
+                            result = self._recursive_traverse(child, global_var, local_var)
+                            if result == ControlResultEnum.Break or result == ControlResultEnum.Continue:
+                                return result
+                        return ControlResultEnum.Default
+                    else:
+                        if node.next_branch is not None:
+                            return self._recursive_traverse(node.next_branch, global_var, local_var)
+                        else:
+                            return ControlResultEnum.Default
+                except Exception as ex:
+                    raise PythonExecutionError(node.start, ex)
+            
+            elif isinstance(node, ElseNode):
+                for child in node.children:
+                    result = self._recursive_traverse(child, global_var, local_var)
+                    if result == ControlResultEnum.Break or result == ControlResultEnum.Continue:
+                        return result
+                return ControlResultEnum.Default
+                
+            elif isinstance(node, ForNode):
+                # 提取变量名和可枚举对象
+                strings = node.condition.split(" in ")
+                assert len(strings) == 2, WrongForStatement(node.start)
+                variables_string = strings[0].strip()
+                try:
+                    enumerate_object = eval(strings[1].strip(), global_var, local_var)
+                except NameError as ne:
+                    raise NameException(node.start, str(ne))
+                assert isinstance(enumerate_object, Iterable), TypeException(node.start, f"{strings[1].strip()} ({type(enumerate_object)}) is not iterable")
+                
+                try:
+                    for element in enumerate_object:
+                        exec(f"{variables_string} = {element}", global_var, local_var)
+                        for child in node.children:
+                            result = self._recursive_traverse(child, global_var, local_var)
+                            if result == ControlResultEnum.Break:
+                                return ControlResultEnum.Default
+                            elif result == ControlResultEnum.Continue:
+                                break
+                    return ControlResultEnum.Default
+                except Exception as ex:
+                    raise PythonExecutionError(node.start, ex)
+                
+            elif isinstance(node, WhileNode):
+                try:
+                    while (result := eval(node.condition, global_var, local_var)):
+                        for child in node.children:
+                            result = self._recursive_traverse(child, global_var, local_var)
+                            if result == ControlResultEnum.Break:
+                                return ControlResultEnum.Default
+                            elif result == ControlResultEnum.Continue:
+                                break
+                    return ControlResultEnum.Default
+                except Exception as ex:
+                    raise PythonExecutionError(node.start, ex)
+            
+            else:
+                for child in node.children:
+                    self._recursive_traverse(child, global_var, local_var)
+                return ControlResultEnum.Default
+        else:
+            if type(node) == TextNode:
+                self._prompt = f"{self._prompt}{node.content}"
+                
+            elif type(node) == ShowBlockNode:
+                try:
+                    self._prompt = f"{self._prompt}{eval(node.body, global_var, local_var)}"
+                except Exception as ex:
+                    raise PythonExecutionError(node.start, ex)
+                
+            elif type(node) == CodeBlockNode:
+                try:
+                    exec(node.body, global_var, local_var)
+                except Exception as ex:
+                    raise PythonExecutionError(node.start, ex)
+                
+            elif type(node) == BreakNode:
+                return ControlResultEnum.Break
+            
+            elif type(node) == ContinueNode:
+                return ControlResultEnum.Continue
+            
         return ControlResultEnum.Default
```

### Comparing `pymaidol-0.1.2/pymaidol/Nodes.py` & `pymaidol-0.1.3/pymaidol/Nodes.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-from abc import ABC
-from typing import Optional
-
-from pymaidol.AnnotationType import AnnotationTypeEnum
-from pymaidol.Positions import Position
-
-
-class ComponentOrRole(ABC):
-    '''
-    通过继承该类，实现的抽象子类可以用作其他结点类的组件类被继承。\n
-    可以往实例结点中添加成员变量，或者赋予实例结点某种身份。
-    '''
-    pass
-
-class VisibleRole(ComponentOrRole, ABC):
-    pass
-
-class InvisibleRole(ComponentOrRole, ABC):
-    pass
-
-class BodyComponent(ComponentOrRole, ABC):
-    def __init__(self) -> None:
-        self.body:str = ""
-        
-
-class BranchRole(ComponentOrRole, ABC):
-    def __init__(self) -> None: 
-        self.previous_branch:Optional[BranchRole] = None
-        self.next_branch:Optional[BranchRole] = None
-        
-class LoopRole(ComponentOrRole, ABC):
-    pass
-
-class BaseNode(ABC): 
-    def __init__(
-        self,
-        start_position:Position,
-        father:Optional['NonTerminalNode'] = None,
-        add_father_children:bool=False,
-        *args,
-        **kwargs) -> None:
-        
-        self.content = ""
-        self.start:Position = start_position        
-        self.end:Position = Position.Default()
-        self.father = father
-        if self.father is not None and add_father_children:
-            self.father.children.append(self)
-        
-    def __str__(self) -> str:
-        return self.content
-    
-    @property
-    def PositionString(self):
-        return f"Start: {self.start}, End: {self.end}"
-    
-    def __repr__(self) -> str:
-        return f'{self.PositionString}; {type(self)}, {[self.content]}'
-    
-    def append_content(self, string:str):
-        self.content = f"{self.content}{string}"
-    
-    @classmethod
-    def FromInstance(cls, baseNode:'BaseNode'):
-        new_one = cls(baseNode.start)
-        new_one.content = baseNode.content
-        new_one.end = baseNode.end
-        new_one.father = baseNode.father
-        return new_one
-    
-class TerminalNode(BaseNode, ABC):
-    pass
-    
-class NonTerminalNode(BaseNode, InvisibleRole, BodyComponent, ABC):
-    def __init__(
-        self,
-        *args,
-        **kwargs) -> None: 
-        super().__init__(*args, **kwargs)
-        self.children:list[BaseNode] = []
-        self.condition:Optional[str] = None    
-    
-    def append_content(self, string:str):
-        self.content = f"{self.content}{string}"
-    
-    @classmethod
-    def FromInstance(cls, baseNode:'BaseNode'):
-        new_one = super().FromInstance(baseNode)
-        if isinstance(baseNode, NonTerminalNode):
-            new_one.children = baseNode.children
-            new_one.condition = baseNode.condition
-            new_one.body = baseNode.body
-        return new_one
-
-class TextNode(TerminalNode, VisibleRole):
-    pass
-
-class AnnotationNode(TerminalNode, InvisibleRole, BodyComponent):
-    def __init__(
-        self,
-        annotation_type:AnnotationTypeEnum,
-        *args,
-        **kwargs) -> None: 
-        super().__init__(*args, **kwargs)
-        self.type:AnnotationTypeEnum = annotation_type
-    
-    def __repr__(self) -> str:
-        return f'{self.PositionString}; {self.type}, {[self.content]}'
-
-# content 是不包括圆括号的表达式
-class ShowBlockNode(TerminalNode, VisibleRole, BodyComponent):
-    pass
-
-# content 是不包括花括号的python代码体
-class CodeBlockNode(TerminalNode, InvisibleRole, BodyComponent):
-    pass
-
-class IfNode(NonTerminalNode, BranchRole):
-    pass
-
-class ElifNode(NonTerminalNode, BranchRole):
-    pass
-
-# self.condition 无意义
-class ElseNode(NonTerminalNode, BranchRole):
-    pass
-
-class ForNode(NonTerminalNode, LoopRole):
-    pass
-
-class WhileNode(NonTerminalNode, LoopRole):
-    pass
-
-class BreakNode(TerminalNode, InvisibleRole):
-    pass
-
-class ContinueNode(TerminalNode, InvisibleRole):
-    pass
-
-class EmptyNode(NonTerminalNode):
+from abc import ABC
+from typing import Optional
+
+from pymaidol.AnnotationType import AnnotationTypeEnum
+from pymaidol.Positions import Position
+
+
+class ComponentOrRole(ABC):
+    '''
+    通过继承该类，实现的抽象子类可以用作其他结点类的组件类被继承。\n
+    可以往实例结点中添加成员变量，或者赋予实例结点某种身份。
+    '''
+    pass
+
+class VisibleRole(ComponentOrRole, ABC):
+    pass
+
+class InvisibleRole(ComponentOrRole, ABC):
+    pass
+
+class BodyComponent(ComponentOrRole, ABC):
+    def __init__(self) -> None:
+        self.body:str = ""
+        
+
+class BranchRole(ComponentOrRole, ABC):
+    def __init__(self) -> None: 
+        self.previous_branch:Optional[BranchRole] = None
+        self.next_branch:Optional[BranchRole] = None
+        
+class LoopRole(ComponentOrRole, ABC):
+    pass
+
+class BaseNode(ABC): 
+    def __init__(
+        self,
+        start_position:Position,
+        father:Optional['NonTerminalNode'] = None,
+        add_father_children:bool=False,
+        *args,
+        **kwargs) -> None:
+        
+        self.content = ""
+        self.start:Position = start_position        
+        self.end:Position = Position.Default()
+        self.father = father
+        if self.father is not None and add_father_children:
+            self.father.children.append(self)
+        
+    def __str__(self) -> str:
+        return self.content
+    
+    @property
+    def PositionString(self):
+        return f"Start: {self.start}, End: {self.end}"
+    
+    def __repr__(self) -> str:
+        return f'{self.PositionString}; {type(self)}, {[self.content]}'
+    
+    def append_content(self, string:str):
+        self.content = f"{self.content}{string}"
+    
+    @classmethod
+    def FromInstance(cls, baseNode:'BaseNode'):
+        new_one = cls(baseNode.start)
+        new_one.content = baseNode.content
+        new_one.end = baseNode.end
+        new_one.father = baseNode.father
+        return new_one
+    
+class TerminalNode(BaseNode, ABC):
+    pass
+    
+class NonTerminalNode(BaseNode, InvisibleRole, BodyComponent, ABC):
+    def __init__(
+        self,
+        *args,
+        **kwargs) -> None: 
+        super().__init__(*args, **kwargs)
+        self.children:list[BaseNode] = []
+        self.condition:Optional[str] = None    
+    
+    def append_content(self, string:str):
+        self.content = f"{self.content}{string}"
+    
+    @classmethod
+    def FromInstance(cls, baseNode:'BaseNode'):
+        new_one = super().FromInstance(baseNode)
+        if isinstance(baseNode, NonTerminalNode):
+            new_one.children = baseNode.children
+            new_one.condition = baseNode.condition
+            new_one.body = baseNode.body
+        return new_one
+
+class TextNode(TerminalNode, VisibleRole):
+    pass
+
+class AnnotationNode(TerminalNode, InvisibleRole, BodyComponent):
+    def __init__(
+        self,
+        annotation_type:AnnotationTypeEnum,
+        *args,
+        **kwargs) -> None: 
+        super().__init__(*args, **kwargs)
+        self.type:AnnotationTypeEnum = annotation_type
+    
+    def __repr__(self) -> str:
+        return f'{self.PositionString}; {self.type}, {[self.content]}'
+
+# content 是不包括圆括号的表达式
+class ShowBlockNode(TerminalNode, VisibleRole, BodyComponent):
+    pass
+
+# content 是不包括花括号的python代码体
+class CodeBlockNode(TerminalNode, InvisibleRole, BodyComponent):
+    pass
+
+class IfNode(NonTerminalNode, BranchRole):
+    pass
+
+class ElifNode(NonTerminalNode, BranchRole):
+    pass
+
+# self.condition 无意义
+class ElseNode(NonTerminalNode, BranchRole):
+    pass
+
+class ForNode(NonTerminalNode, LoopRole):
+    pass
+
+class WhileNode(NonTerminalNode, LoopRole):
+    pass
+
+class BreakNode(TerminalNode, InvisibleRole):
+    pass
+
+class ContinueNode(TerminalNode, InvisibleRole):
+    pass
+
+class EmptyNode(NonTerminalNode):
     pass
```

### Comparing `pymaidol-0.1.2/pymaidol/Parser.py` & `pymaidol-0.1.3/pymaidol/Parser.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,531 +1,531 @@
-from enum import Enum
-from typing import Optional, Union
-
-from pymaidol.AnnotationType import (AnnotationTypeEnum, FULL_ANNOTATION_TYPE,
-                                MultiLineAnnotationTypeEnum,
-                                SingleLineAnnotationTypeEnum)
-from pymaidol.Errors import (MultiLineAnnotationFormatError, UnexpectedTokenError,
-                    UnknownEmbedIdentifierError)
-from pymaidol.keywords import (KeywordsEnum, NonTerminalKeywords, TerminalKeywords,
-                      TranslateKeywords2Type)
-from pymaidol.Nodes import (AnnotationNode, BaseNode, BodyComponent, CodeBlockNode,
-                   EmptyNode, NonTerminalNode, ShowBlockNode, TerminalNode,
-                   TextNode, VisibleRole)
-from pymaidol.Positions import Position
-from pymaidol.Traversers import PreOrderTraverser
-
-
-class Parser:
-    def __init__(
-        self, 
-        template:str, 
-        root_node:Optional[NonTerminalNode]=None, 
-        start:Position = Position.Default(), 
-        end:Optional[Position] = None
-        ) -> None:
-        # 指的是当前未被消费的字符的位置。如果当前字符被消费，则应该立即步进1.
-        self._current_position:Position = start
-        # end 的行号和行内字符序号不重要
-        self._end:Position = end if end is not None else Position(0, 0, len(template)-1)
-        self.root = root_node if root_node else EmptyNode(0, 0, 0)
-        self._current_node:BaseNode = TextNode(self._current_position, father=self.root)
-        self._last_line_final_char_index = -1
-        self.template:str = template
-        self.__used = False
-        # 用于记录当前行是否有可见字符。注意：“当前行”的定义是当前 node 的 start 所在行，而不是当前字符所在行。
-        self._is_line_of_current_start_has_visible_content = False
-        
-        self.clean_trailing_whitespaces:bool = True
-        self.supported_annotation_types:'list[AnnotationTypeEnum]' = FULL_ANNOTATION_TYPE
-    
-    @property
-    def _current_char(self):
-        return self.template[self._current_position.total]
-    
-    def _peek_several(self, char_count):
-        end = self._current_position.total + char_count
-        return self.template[self._current_position.total:end]
-    
-    @property
-    def _remains(self):
-        return self.template[self._current_position.total+1:]
-    
-    @property
-    def _remains_include_current_char(self):
-        return self.template[self._current_position.total:]
-    
-    def _detect_annotation(self):
-        """
-        检测注释类型。如果当前字符不是注释，则返回None，否则返回注释类型（注释的开始符）和注释的结束符。
-        Args:
-            support_annotation_types (list[AnnotationType], optional): 支持被检测的注释类型。默认为所有注释类型。
-        """
-        supported_annotation_types = self.supported_annotation_types
-        if SingleLineAnnotationTypeEnum.Python in supported_annotation_types:
-            if self._remains_include_current_char.startswith(SingleLineAnnotationTypeEnum.Python.value):
-                return SingleLineAnnotationTypeEnum.Python, '\n'
-        if SingleLineAnnotationTypeEnum.C in supported_annotation_types:
-            if self._remains_include_current_char.startswith(SingleLineAnnotationTypeEnum.C.value):
-                return SingleLineAnnotationTypeEnum.C, '\n'
-        if MultiLineAnnotationTypeEnum.PythonDoubleQuotation in supported_annotation_types:
-            if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.PythonDoubleQuotation.value):
-                return MultiLineAnnotationTypeEnum.PythonDoubleQuotation, '"""'
-        if MultiLineAnnotationTypeEnum.PythonSingleQuotation in supported_annotation_types:
-            if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.PythonSingleQuotation.value):
-                return MultiLineAnnotationTypeEnum.PythonSingleQuotation, "'''"
-        if MultiLineAnnotationTypeEnum.C in supported_annotation_types:
-            if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.C.value):
-                return MultiLineAnnotationTypeEnum.C, '*/'
-        if MultiLineAnnotationTypeEnum.Html in supported_annotation_types:
-            if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.Html.value):
-                return MultiLineAnnotationTypeEnum.Html, '-->'
-        return None
-    
-    def _process_annotation(self, start_sign:AnnotationTypeEnum, end_sign:str):
-        self._end_current_node_at_last_char()
-        self._create_new_node_at_current_char(AnnotationNode, annotation_type=start_sign)
-        assert isinstance(self._current_node, AnnotationNode)
-        # 消费开始符
-        self._current_node.append_content(start_sign.value)
-        self._consume_current_char_index(len(start_sign.value))
-        # 匹配注释体
-        self._current_node.body, _, _ = self._consume_and_pair("", end_sign)
-        # 多行注释时，检查注释结束符后面是否有除了空白字符以外的字符
-        # 有则报错
-        if isinstance(start_sign, MultiLineAnnotationTypeEnum):
-            whitespace_peek, after_whitespace_peek = self._peek_while([' ', '\t'])
-            if not after_whitespace_peek.startswith('\n'):
-                raise MultiLineAnnotationFormatError(self._current_position)
-            else:
-                # 空白和换行符也算在多行注释里
-                self._current_node.append_content(f"{whitespace_peek}\n")
-                self._consume_current_char_index(len(whitespace_peek) + 1)
-        # 清除前导空白符（如果这一行前面没有其他东西，也就是有缩进）
-        if len(self.root.children) > 0 \
-            and self.root.children[-1].start.line_index == self._current_node.start.line_index \
-            and self.root.children[-1].content.strip() == "":
-            #self._current_node.content = f"{self._root.children[-1].content}{self._current_node.content}"
-            self._current_node.start = self.root.children[-1].start
-            self.root.children.pop()
-        # 如果上一个结点结束行和当前注释结点的起始相同（也就是注释不是开始于单独一行），则在上一个结点最后面加一个回车
-        if len(self.root.children) > 0 and self.root.children[-1].end.line_index == self._current_node.start.line_index:
-            self.root.children[-1].append_content('\n')
-        # 结束
-        self._end_current_node_at_last_char()
-        self._create_new_node_at_current_char()
-    
-    def _end_current_node_at_last_char(self):
-        end_line = self._current_position.line_index if self._current_position.char_index != 0 else self._current_position.line_index - 1
-        end = self._current_position.char_index - 1 if self._current_position.char_index != 0 else self._last_line_final_char_index
-        total_end = self._current_position.total - 1
-        self._current_node.end = Position(end_line, end, total_end)
-        if self._current_node.content != "":
-            self.root.children.append(self._current_node)
-            if isinstance(self._current_node, VisibleRole):
-                self._is_line_of_current_start_has_visible_content = True
-    
-    def _end_current_part_at_this_char(self):
-        end_line = self._current_position.line_index
-        end = self._current_position.char_index
-        total_end = self._current_position.total
-        self._current_node.end = Position(end_line, end, total_end)
-        if self._current_node.content != "":
-            self.root.children.append(self._current_node)
-            if isinstance(self._current_node, VisibleRole):
-                self._is_line_of_current_start_has_visible_content = True
-    
-    def _create_new_node_at_current_char(self, type:type[BaseNode]=TextNode, **kwargs):
-        self._current_node = type(
-            start_position=self._current_position,
-            father=self.root,
-            **kwargs)
-    
-    def _consume_current_char_index(self, steps:int=1):
-        """
-        如果当前字符被消耗了（追加到 self._current_part.content 中），
-        那么就要调用本函数更新 self._current_line_index 和 current_total_index。
-        会自动处理换行逻辑。
-        """
-        if steps < 1:
-            raise ValueError("steps must be greater than 0")
-        for _ in range(steps):
-            if self._current_char == '\n':
-                self._last_line_final_char_index = self._current_position.char_index # 本行的长度，包括 \n
-                self._current_position = Position(
-                    self._current_position.line_index + 1, 
-                    0, 
-                    self._current_position.total + 1
-                )
-            else:
-                self._current_position = Position(
-                    self._current_position.line_index, 
-                    self._current_position.char_index + 1, 
-                    self._current_position.total + 1
-                )
-    
-    def _consume_and_pair(
-        self, 
-        pair_left:str, 
-        pair_right:str, 
-        is_include_right:bool=True,
-        suppress_unpaired_error:bool = False
-        ):
-        """
-
-        Args:
-            pair_left (str):
-            pair_right (str):
-        """
-        # TODO: 处理左右长度不相等的情况
-        # 持续消费，直到匹配到右侧
-        content_start = self._current_position
-        content_end = content_start
-        pair_step = len(pair_right)
-        content_inside = ""
-        pair_finder = PairFinder(pair_left, pair_right)
-        while(self._current_position.total < len(self.template)):
-            pair_result = pair_finder.IsPair(self._peek_several(pair_step))
-            if pair_result:
-                if is_include_right:                    
-                    self._current_node.content = f"{self._current_node.content}{self._peek_several(pair_step)}"
-                    self._consume_current_char_index(pair_step)
-                break
-            content_inside = f"{content_inside}{self._current_char}"
-            self._current_node.content = f"{self._current_node.content}{self._current_char}"
-            content_end = self._current_position
-            self._consume_current_char_index()
-        if pair_finder.unpaired_left_count > 0 and not suppress_unpaired_error:
-            # TODO: 报错未匹配的起始位置
-            raise Exception(f"Unpaired left {pair_finder.unpaired_left_count} in template {self.template}")
-        return content_inside, content_start, content_end
-    
-    def _new_node_foresee_and_pair(
-            self, 
-            foresee_consume_count:int, 
-            pair_left:str, 
-            pair_right:str, 
-            node_type:type[NonTerminalNode|AnnotationNode], 
-            is_include_right:bool=True,
-            is_clean_whitespace:bool=True):
-        
-        self._end_current_node_at_last_char()
-        self._create_new_node_at_current_char(node_type)
-        assert isinstance(self._current_node, BodyComponent)
-        # 消费当前的 @ 和前瞻的词语
-        # 一次吃多个字符
-        self._current_node.content = f"{self._current_node.content}{self._peek_several(foresee_consume_count)}"
-        self._consume_current_char_index(foresee_consume_count)
-        # 匹配
-        self._current_node.body, _, _ = self._consume_and_pair(pair_left, pair_right, is_include_right)
-        # 结束
-        if is_clean_whitespace == True:
-            self._try_discard_continuous_whitespaces_with_linefeed()
-        self._end_current_node_at_last_char()
-        self._create_new_node_at_current_char()
-        
-    def _add_and_consume_continuous_char(
-        self, 
-        char_list:list[str], 
-        add_into_current_part:bool=True
-        ):
-        while (self._current_char in char_list):
-            if add_into_current_part:
-                self._current_node.content = f"{self._current_node.content}{self._current_char}"
-            self._consume_current_char_index()
-            
-    def _peek_until(
-        self, 
-        until_char_list:list[str]=[' ', '\t', '\n', '\r', '(', ')', '{', '}', '[', ']', '"', "'", '`', '@', '#', '$', '%', '^', '&', '*', '-', '+', '=', '|', '\\', '/', '?', '<', '>', ',', '.', ';', ':', '!'],
-        include_current_chat:bool=False
-        ):
-        start = self._current_position.total if include_current_chat else self._current_position.total+1
-        remaining:str = self.template[start:]
-        _index = 0
-        _peeked = ""
-        while (_index < len(remaining)):
-            if remaining[_index] in until_char_list:
-                break
-            _peeked = f"{_peeked}{remaining[_index]}"
-            _index += 1
-        after_peek = remaining[_index:]
-        return _peeked, after_peek
-    
-    def _peek_while(
-        self, 
-        char_list:list[str],
-        include_current_chat:bool=True
-        ):
-        start = self._current_position.total if include_current_chat else self._current_position.total+1
-        remaining:str = self.template[start:]
-        _index = 0
-        _peeked = ""
-        while (_index < len(remaining)):
-            if remaining[_index] not in char_list:
-                break
-            _peeked = f"{_peeked}{remaining[_index]}"
-            _index += 1
-        after_peek = remaining[_index:]
-        return _peeked, after_peek
-    
-    def _peek_while_from_tail(
-        self, 
-        string:str,
-        char_list:list[str],
-        ):
-        _index = len(string)-1
-        _peeked = ""
-        while (_index >= 0):
-            if string[_index] not in char_list:
-                break
-            _peeked = f"{string[_index]}{_peeked}"
-            _index -= 1
-        after_peek = string[:_index+1]
-        return _peeked, after_peek
-        
-    def _non_terminal_keyword_check_type(self):
-        """
-        检查剩余的字符串是否以 char_list 中的任意一个开头
-        """
-        _peek, _ = self._peek_until([' ', '\t', '\n', '\r', '(', ')', '{', '}', '[', ']', '"', "'", '`', '@', '#', '$', '%', '^', '&', '*', '-', '+', '=', '|', '\\', '/', '?', '<', '>', ',', '.', ';', ':', '!'])
-        for keyword_type in NonTerminalKeywords:
-            if _peek == keyword_type.value:
-                return keyword_type
-        return None
-    
-    def _terminal_keyword_check_type(self):
-        """
-        检查剩余的字符串是否以 char_list 中的任意一个开头
-        """
-        _peek, _ = self._peek_until([';'])
-        for keyword_type in TerminalKeywords:
-            if _peek == keyword_type.value:
-                return keyword_type
-        return None
-    
-    def _is_continuous_whitespaces_until_linefeed(self):
-        whitespace_peek, after_whitespace_peek = self._peek_while([' ', '\t'])
-        if after_whitespace_peek.startswith('\n'):
-            return True
-        else:
-            return False
-    
-    def _try_discard_continuous_whitespaces_with_linefeed(self):
-        """试图清除从当前位置开始的连续的空白符，直到遇到换行符为止。如果该行有内容，则不会清除任何空白符。
-        """
-        whitespace_peek, after_whitespace_peek = self._peek_while([' ', '\t'])
-        if after_whitespace_peek.startswith('\n'):
-            # 抛弃左大括号后跟的掉空白符以及第一个换行符，也就是等于将body的第一行放到左大括号后面
-            self._consume_current_char_index(len(whitespace_peek)+1)
-    
-    def _is_leading_continuous_whitespaces(self):
-        if len(self.root.children) > 0 \
-            and isinstance(self.root.children[-1], TextNode) \
-            and self.root.children[-1].content.strip() == "" \
-            and self.root.children[-1].start.line_index == self._current_node.start.line_index \
-            and self.root.children[-1].start.char_index == 0 \
-            :
-            return True
-        else:
-            return False
-        
-    def _try_discard_leading_continuous_whitespaces(self):
-        # 清除当前 node 的行首前导空白符
-        # 上一个 text 结点是当前结点的前导空白符的判断标准：
-        # 1. 上一个结点是 TextNode，并且全是空白符
-        # 2. 上一个结点的 start 位置和当前结点的 start 位置在同一行
-        # 3. 上一个结点是从行首开始计数的（start.char_index == 0）
-        if len(self.root.children) > 0 \
-            and isinstance(self.root.children[-1], TextNode) \
-            and self.root.children[-1].content.strip() == "" \
-            and self.root.children[-1].start.line_index == self._current_node.start.line_index \
-            and self.root.children[-1].start.char_index == 0 \
-            :
-            self._is_line_of_current_start_has_visible_content = False
-            self._current_node.start = self.root.children[-1].start
-            self.root.children.pop()
-        
-    def _non_terminal_node_parse(self, keyword_type:KeywordsEnum):
-        self._end_current_node_at_last_char()
-        self._create_new_node_at_current_char(TranslateKeywords2Type(keyword_type))
-        assert isinstance(self._current_node, NonTerminalNode)
-        # 消费@关键词
-        self._current_node.content = f"{self._current_node.content}{self._current_char}{keyword_type.value}"
-        self._consume_current_char_index(len(keyword_type.value)+1)
-        
-        peek, after_peek = self._peek_while([' ', '\t'], True)
-        # 以左圆括号开头，说明有条件
-        if after_peek.startswith('('):
-            # 关键词与左圆括号之间的空白符，和左圆括号全部消费
-            self._current_node.append_content(f"{peek}(")
-            self._consume_current_char_index(len(peek)+1)
-            # 消费后，当前的字符应该是左圆括号后的条件表达式的第一个字符
-            self._current_node.condition, _, _ = self._consume_and_pair('(', ')', is_include_right=False)
-            # 消费右圆括号  
-            self._current_node.append_content(f")")      
-            self._consume_current_char_index()
-        
-        peek, after_peek = self._peek_while([' ', '\t', '\n', '\r'], True)
-        # 以左大括号开头，说明有 body
-        if after_peek.startswith('{'):
-            # 关键词与左大括号之间的空白符、换行符，和左大括号全部消费            
-            self._current_node.append_content(peek + "{")
-            self._consume_current_char_index(len(peek)+1)
-            # 抛弃左大括号后跟的掉空白符以及第一个换行符，也就是等于将body的第一行放到左大括号后面
-            # 消费后，当前的字符应该是左大括号后的body的第一个字符
-            self._try_discard_continuous_whitespaces_with_linefeed()
-            self._current_node.body, body_start, body_end = self._consume_and_pair('{', '}', is_include_right=False)
-            # 如果右括号单独一行，清除右大括号前的空白符，遇到换行符停止（不清除换行符）
-            is_right_brace_start_of_new_line = False
-            whitespace, after_whitespace_peek = self._peek_while_from_tail(self._current_node.body, [' ', '\t'])
-            if after_whitespace_peek.endswith('\n'):
-                is_right_brace_start_of_new_line = True
-                self._current_node.body = after_whitespace_peek
-                body_end = Position(body_end.line_index, body_end.char_index-len(whitespace), body_end.total-len(whitespace))
-            # 右大括号
-            self._current_node.append_content("}")
-            self._consume_current_char_index()
-            
-            # 处理子结点
-            sub_parser = Parser(self.template, self._current_node, body_start, body_end)
-            sub_parser.clean_trailing_whitespaces = False
-            sub_parser.Parse()
-            
-            # 如果子结点都是不可见，并且本分支结点单独一行；           
-            # 或者如果右括号单独一行, 清除右大括号后的空白符，遇到第一个换行符停止（清除换行符）
-            if (self._is_children_have_visible_content(self._current_node) == False\
-                and self._current_node.start.line_index == self._current_position.line_index)\
-                or is_right_brace_start_of_new_line == True:
-                self._try_discard_continuous_whitespaces_with_linefeed()
-            
-            self._end_current_node_at_last_char()
-            self._create_new_node_at_current_char()
-        else:
-            raise UnexpectedTokenError(self._current_position, ['{'], after_peek[0])
-        
-    def _is_children_have_visible_content(self, node:NonTerminalNode):
-        for child in node.children:
-            if isinstance(child, VisibleRole):
-                return True
-            elif isinstance(child, NonTerminalNode) and self._is_children_have_visible_content(child):
-                return True
-        return False
-    
-    def _terminal_keyword_process(self, keyword_type:KeywordsEnum):
-        self._end_current_node_at_last_char()
-        self._create_new_node_at_current_char(TranslateKeywords2Type(keyword_type))
-        assert isinstance(self._current_node, TerminalNode)
-        # 消费@关键词
-        # self._current_char is '@'
-        self._current_node.content = f"{self._current_node.content}{keyword_type.value}"
-        self._consume_current_char_index(len(keyword_type.value)+1)
-        # 消费掉分号
-        self._consume_current_char_index()
-        # 如果这一行只有终结符关键字，清除前导后随空白符和换行
-        if self._is_leading_continuous_whitespaces()\
-            and self._is_continuous_whitespaces_until_linefeed():
-            
-            self._try_discard_leading_continuous_whitespaces()
-            self._try_discard_continuous_whitespaces_with_linefeed()
-        
-        self._end_current_node_at_last_char()
-        self._create_new_node_at_current_char()
-    
-    def Parse(self):
-        if self.__used == True:
-            raise Exception("Parser can only be used once.")
-        while(self._current_position.total <= self._end.total):
-            if self._current_char == '\n':
-                # 每一个Text的换行都要新建一个 part
-                self._current_node.content = f"{self._current_node.content}{self._current_char}"
-                self._consume_current_char_index()
-                self._end_current_node_at_last_char()
-                self._create_new_node_at_current_char()
-                self._is_line_of_current_start_has_visible_content = False
-            
-            # 注释处理
-            elif (_detect_result := self._detect_annotation()) is not None:
-                start_type, end_sign = _detect_result
-                self._process_annotation(start_type, end_sign)
-            
-            # 可能的嵌入符号
-            elif self._current_char == '@':
-                # 前瞻也是@，那么就是转义为 @
-                if self._remains.startswith('@'):
-                    # 第一个 @ 不追加到 self._current_part.content 中，直接消费掉
-                    self._consume_current_char_index()
-                    # 直接追加第二个 @ 到 self._current_part.content 中，之后就不会触发嵌入符号的逻辑了
-                    self._current_node.content = f"{self._current_node.content}{self._current_char}"
-                    self._consume_current_char_index()
-                    
-                # 前瞻是 {，那么新建 part，匹配到 } 为止
-                elif self._remains.startswith('{'):
-                    self._new_node_foresee_and_pair(2, '{', '}', CodeBlockNode)
-                
-                # 前瞻是 (，那么新建 part，匹配到 ) 为止
-                elif self._remains.startswith('('):
-                    self._new_node_foresee_and_pair(2, '(', ')', ShowBlockNode, is_clean_whitespace=False)
-                                    
-                elif (keyword_type := self._non_terminal_keyword_check_type()) is not None:
-                    self._non_terminal_node_parse(keyword_type)
-                
-                elif (keyword_type := self._terminal_keyword_check_type()) is not None:
-                    # 处理主体
-                    self._terminal_keyword_process(keyword_type)
-                
-                # 未知的嵌入符号
-                else:
-                    _peek_identifier, _ = self._peek_until([' ', '\t', '\n', '\r', '(', ')', '{', '}', '[', ']', '"', "'", '`', '@', '#', '$', '%', '^', '&', '*', '-', '+', '=', '|', '\\', '/', '?', '<', '>', ',', '.', ';', ':', '!'])
-                    raise UnknownEmbedIdentifierError(self._current_position, _peek_identifier)
-                
-            # 纯文本
-            else:
-                self._current_node.content = f"{self._current_node.content}{self._current_char}"
-                self._consume_current_char_index()
-        
-        # 结束最后一个 part
-        self._end_current_node_at_last_char()
-        self.__used = True
-        self._post_process()
-        return self.root
-    
-    def _post_process(self):
-        if self.clean_trailing_whitespaces == True:
-            traverser = PreOrderTraverser(self.root)
-            traverser.entered_TextNode += self._delete_trailing_whitespaces
-            traverser.traverse()
-            traverser.entered_TextNode -= self._delete_trailing_whitespaces
-            
-    def _delete_trailing_whitespaces(self, sender:PreOrderTraverser, text_node:TextNode):
-        cleaned = ""
-        index = len(text_node.content) - 1
-        kill_whitespace = False
-        while index >= 0:
-            if text_node.content[index] == '\n':
-                cleaned = f"{text_node.content[index]}{cleaned}"
-                kill_whitespace = True
-            elif kill_whitespace == True and text_node.content[index] in [' ', '\t']:
-                pass
-            else:
-                cleaned = f"{text_node.content[index]}{cleaned}"
-                kill_whitespace = False
-            index -= 1
-        text_node.content = cleaned
-
-class PairFinder():
-    def __init__(self, left:str, right:str) -> None:
-        self.unpaired_left_count = 0
-        self.__left = left
-        self.__right = right
-    
-    def IsPair(self, target:str):
-        if target == self.__left:
-            self.unpaired_left_count += 1
-            return False
-        elif target == self.__right:
-            if self.unpaired_left_count == 0:
-                return True
-            else:
-                self.unpaired_left_count -= 1
-                return False
-        else:
+from enum import Enum
+from typing import Optional, Union
+
+from pymaidol.AnnotationType import (AnnotationTypeEnum, FULL_ANNOTATION_TYPE,
+                                MultiLineAnnotationTypeEnum,
+                                SingleLineAnnotationTypeEnum)
+from pymaidol.Errors import (MultiLineAnnotationFormatError, UnexpectedTokenError,
+                    UnknownEmbedIdentifierError)
+from pymaidol.keywords import (KeywordsEnum, NonTerminalKeywords, TerminalKeywords,
+                      TranslateKeywords2Type)
+from pymaidol.Nodes import (AnnotationNode, BaseNode, BodyComponent, CodeBlockNode,
+                   EmptyNode, NonTerminalNode, ShowBlockNode, TerminalNode,
+                   TextNode, VisibleRole)
+from pymaidol.Positions import Position
+from pymaidol.Traversers import PreOrderTraverser
+
+
+class Parser:
+    def __init__(
+        self, 
+        template:str, 
+        root_node:Optional[NonTerminalNode]=None, 
+        start:Position = Position.Default(), 
+        end:Optional[Position] = None
+        ) -> None:
+        # 指的是当前未被消费的字符的位置。如果当前字符被消费，则应该立即步进1.
+        self._current_position:Position = start
+        # end 的行号和行内字符序号不重要
+        self._end:Position = end if end is not None else Position(0, 0, len(template)-1)
+        self.root = root_node if root_node else EmptyNode(0, 0, 0)
+        self._current_node:BaseNode = TextNode(self._current_position, father=self.root)
+        self._last_line_final_char_index = -1
+        self.template:str = template
+        self.__used = False
+        # 用于记录当前行是否有可见字符。注意：“当前行”的定义是当前 node 的 start 所在行，而不是当前字符所在行。
+        self._is_line_of_current_start_has_visible_content = False
+        
+        self.clean_trailing_whitespaces:bool = True
+        self.supported_annotation_types:'list[AnnotationTypeEnum]' = FULL_ANNOTATION_TYPE
+    
+    @property
+    def _current_char(self):
+        return self.template[self._current_position.total]
+    
+    def _peek_several(self, char_count):
+        end = self._current_position.total + char_count
+        return self.template[self._current_position.total:end]
+    
+    @property
+    def _remains(self):
+        return self.template[self._current_position.total+1:]
+    
+    @property
+    def _remains_include_current_char(self):
+        return self.template[self._current_position.total:]
+    
+    def _detect_annotation(self):
+        """
+        检测注释类型。如果当前字符不是注释，则返回None，否则返回注释类型（注释的开始符）和注释的结束符。
+        Args:
+            support_annotation_types (list[AnnotationType], optional): 支持被检测的注释类型。默认为所有注释类型。
+        """
+        supported_annotation_types = self.supported_annotation_types
+        if SingleLineAnnotationTypeEnum.Python in supported_annotation_types:
+            if self._remains_include_current_char.startswith(SingleLineAnnotationTypeEnum.Python.value):
+                return SingleLineAnnotationTypeEnum.Python, '\n'
+        if SingleLineAnnotationTypeEnum.C in supported_annotation_types:
+            if self._remains_include_current_char.startswith(SingleLineAnnotationTypeEnum.C.value):
+                return SingleLineAnnotationTypeEnum.C, '\n'
+        if MultiLineAnnotationTypeEnum.PythonDoubleQuotation in supported_annotation_types:
+            if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.PythonDoubleQuotation.value):
+                return MultiLineAnnotationTypeEnum.PythonDoubleQuotation, '"""'
+        if MultiLineAnnotationTypeEnum.PythonSingleQuotation in supported_annotation_types:
+            if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.PythonSingleQuotation.value):
+                return MultiLineAnnotationTypeEnum.PythonSingleQuotation, "'''"
+        if MultiLineAnnotationTypeEnum.C in supported_annotation_types:
+            if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.C.value):
+                return MultiLineAnnotationTypeEnum.C, '*/'
+        if MultiLineAnnotationTypeEnum.Html in supported_annotation_types:
+            if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.Html.value):
+                return MultiLineAnnotationTypeEnum.Html, '-->'
+        return None
+    
+    def _process_annotation(self, start_sign:AnnotationTypeEnum, end_sign:str):
+        self._end_current_node_at_last_char()
+        self._create_new_node_at_current_char(AnnotationNode, annotation_type=start_sign)
+        assert isinstance(self._current_node, AnnotationNode)
+        # 消费开始符
+        self._current_node.append_content(start_sign.value)
+        self._consume_current_char_index(len(start_sign.value))
+        # 匹配注释体
+        self._current_node.body, _, _ = self._consume_and_pair("", end_sign)
+        # 多行注释时，检查注释结束符后面是否有除了空白字符以外的字符
+        # 有则报错
+        if isinstance(start_sign, MultiLineAnnotationTypeEnum):
+            whitespace_peek, after_whitespace_peek = self._peek_while([' ', '\t'])
+            if not after_whitespace_peek.startswith('\n'):
+                raise MultiLineAnnotationFormatError(self._current_position)
+            else:
+                # 空白和换行符也算在多行注释里
+                self._current_node.append_content(f"{whitespace_peek}\n")
+                self._consume_current_char_index(len(whitespace_peek) + 1)
+        # 清除前导空白符（如果这一行前面没有其他东西，也就是有缩进）
+        if len(self.root.children) > 0 \
+            and self.root.children[-1].start.line_index == self._current_node.start.line_index \
+            and self.root.children[-1].content.strip() == "":
+            #self._current_node.content = f"{self._root.children[-1].content}{self._current_node.content}"
+            self._current_node.start = self.root.children[-1].start
+            self.root.children.pop()
+        # 如果上一个结点结束行和当前注释结点的起始相同（也就是注释不是开始于单独一行），则在上一个结点最后面加一个回车
+        if len(self.root.children) > 0 and self.root.children[-1].end.line_index == self._current_node.start.line_index:
+            self.root.children[-1].append_content('\n')
+        # 结束
+        self._end_current_node_at_last_char()
+        self._create_new_node_at_current_char()
+    
+    def _end_current_node_at_last_char(self):
+        end_line = self._current_position.line_index if self._current_position.char_index != 0 else self._current_position.line_index - 1
+        end = self._current_position.char_index - 1 if self._current_position.char_index != 0 else self._last_line_final_char_index
+        total_end = self._current_position.total - 1
+        self._current_node.end = Position(end_line, end, total_end)
+        if self._current_node.content != "":
+            self.root.children.append(self._current_node)
+            if isinstance(self._current_node, VisibleRole):
+                self._is_line_of_current_start_has_visible_content = True
+    
+    def _end_current_part_at_this_char(self):
+        end_line = self._current_position.line_index
+        end = self._current_position.char_index
+        total_end = self._current_position.total
+        self._current_node.end = Position(end_line, end, total_end)
+        if self._current_node.content != "":
+            self.root.children.append(self._current_node)
+            if isinstance(self._current_node, VisibleRole):
+                self._is_line_of_current_start_has_visible_content = True
+    
+    def _create_new_node_at_current_char(self, type:type[BaseNode]=TextNode, **kwargs):
+        self._current_node = type(
+            start_position=self._current_position,
+            father=self.root,
+            **kwargs)
+    
+    def _consume_current_char_index(self, steps:int=1):
+        """
+        如果当前字符被消耗了（追加到 self._current_part.content 中），
+        那么就要调用本函数更新 self._current_line_index 和 current_total_index。
+        会自动处理换行逻辑。
+        """
+        if steps < 1:
+            raise ValueError("steps must be greater than 0")
+        for _ in range(steps):
+            if self._current_char == '\n':
+                self._last_line_final_char_index = self._current_position.char_index # 本行的长度，包括 \n
+                self._current_position = Position(
+                    self._current_position.line_index + 1, 
+                    0, 
+                    self._current_position.total + 1
+                )
+            else:
+                self._current_position = Position(
+                    self._current_position.line_index, 
+                    self._current_position.char_index + 1, 
+                    self._current_position.total + 1
+                )
+    
+    def _consume_and_pair(
+        self, 
+        pair_left:str, 
+        pair_right:str, 
+        is_include_right:bool=True,
+        suppress_unpaired_error:bool = False
+        ):
+        """
+
+        Args:
+            pair_left (str):
+            pair_right (str):
+        """
+        # TODO: 处理左右长度不相等的情况
+        # 持续消费，直到匹配到右侧
+        content_start = self._current_position
+        content_end = content_start
+        pair_step = len(pair_right)
+        content_inside = ""
+        pair_finder = PairFinder(pair_left, pair_right)
+        while(self._current_position.total < len(self.template)):
+            pair_result = pair_finder.IsPair(self._peek_several(pair_step))
+            if pair_result:
+                if is_include_right:                    
+                    self._current_node.content = f"{self._current_node.content}{self._peek_several(pair_step)}"
+                    self._consume_current_char_index(pair_step)
+                break
+            content_inside = f"{content_inside}{self._current_char}"
+            self._current_node.content = f"{self._current_node.content}{self._current_char}"
+            content_end = self._current_position
+            self._consume_current_char_index()
+        if pair_finder.unpaired_left_count > 0 and not suppress_unpaired_error:
+            # TODO: 报错未匹配的起始位置
+            raise Exception(f"Unpaired left {pair_finder.unpaired_left_count} in template {self.template}")
+        return content_inside, content_start, content_end
+    
+    def _new_node_foresee_and_pair(
+            self, 
+            foresee_consume_count:int, 
+            pair_left:str, 
+            pair_right:str, 
+            node_type:type[NonTerminalNode|AnnotationNode], 
+            is_include_right:bool=True,
+            is_clean_whitespace:bool=True):
+        
+        self._end_current_node_at_last_char()
+        self._create_new_node_at_current_char(node_type)
+        assert isinstance(self._current_node, BodyComponent)
+        # 消费当前的 @ 和前瞻的词语
+        # 一次吃多个字符
+        self._current_node.content = f"{self._current_node.content}{self._peek_several(foresee_consume_count)}"
+        self._consume_current_char_index(foresee_consume_count)
+        # 匹配
+        self._current_node.body, _, _ = self._consume_and_pair(pair_left, pair_right, is_include_right)
+        # 结束
+        if is_clean_whitespace == True:
+            self._try_discard_continuous_whitespaces_with_linefeed()
+        self._end_current_node_at_last_char()
+        self._create_new_node_at_current_char()
+        
+    def _add_and_consume_continuous_char(
+        self, 
+        char_list:list[str], 
+        add_into_current_part:bool=True
+        ):
+        while (self._current_char in char_list):
+            if add_into_current_part:
+                self._current_node.content = f"{self._current_node.content}{self._current_char}"
+            self._consume_current_char_index()
+            
+    def _peek_until(
+        self, 
+        until_char_list:list[str]=[' ', '\t', '\n', '\r', '(', ')', '{', '}', '[', ']', '"', "'", '`', '@', '#', '$', '%', '^', '&', '*', '-', '+', '=', '|', '\\', '/', '?', '<', '>', ',', '.', ';', ':', '!'],
+        include_current_chat:bool=False
+        ):
+        start = self._current_position.total if include_current_chat else self._current_position.total+1
+        remaining:str = self.template[start:]
+        _index = 0
+        _peeked = ""
+        while (_index < len(remaining)):
+            if remaining[_index] in until_char_list:
+                break
+            _peeked = f"{_peeked}{remaining[_index]}"
+            _index += 1
+        after_peek = remaining[_index:]
+        return _peeked, after_peek
+    
+    def _peek_while(
+        self, 
+        char_list:list[str],
+        include_current_chat:bool=True
+        ):
+        start = self._current_position.total if include_current_chat else self._current_position.total+1
+        remaining:str = self.template[start:]
+        _index = 0
+        _peeked = ""
+        while (_index < len(remaining)):
+            if remaining[_index] not in char_list:
+                break
+            _peeked = f"{_peeked}{remaining[_index]}"
+            _index += 1
+        after_peek = remaining[_index:]
+        return _peeked, after_peek
+    
+    def _peek_while_from_tail(
+        self, 
+        string:str,
+        char_list:list[str],
+        ):
+        _index = len(string)-1
+        _peeked = ""
+        while (_index >= 0):
+            if string[_index] not in char_list:
+                break
+            _peeked = f"{string[_index]}{_peeked}"
+            _index -= 1
+        after_peek = string[:_index+1]
+        return _peeked, after_peek
+        
+    def _non_terminal_keyword_check_type(self):
+        """
+        检查剩余的字符串是否以 char_list 中的任意一个开头
+        """
+        _peek, _ = self._peek_until([' ', '\t', '\n', '\r', '(', ')', '{', '}', '[', ']', '"', "'", '`', '@', '#', '$', '%', '^', '&', '*', '-', '+', '=', '|', '\\', '/', '?', '<', '>', ',', '.', ';', ':', '!'])
+        for keyword_type in NonTerminalKeywords:
+            if _peek == keyword_type.value:
+                return keyword_type
+        return None
+    
+    def _terminal_keyword_check_type(self):
+        """
+        检查剩余的字符串是否以 char_list 中的任意一个开头
+        """
+        _peek, _ = self._peek_until([';'])
+        for keyword_type in TerminalKeywords:
+            if _peek == keyword_type.value:
+                return keyword_type
+        return None
+    
+    def _is_continuous_whitespaces_until_linefeed(self):
+        whitespace_peek, after_whitespace_peek = self._peek_while([' ', '\t'])
+        if after_whitespace_peek.startswith('\n'):
+            return True
+        else:
+            return False
+    
+    def _try_discard_continuous_whitespaces_with_linefeed(self):
+        """试图清除从当前位置开始的连续的空白符，直到遇到换行符为止。如果该行有内容，则不会清除任何空白符。
+        """
+        whitespace_peek, after_whitespace_peek = self._peek_while([' ', '\t'])
+        if after_whitespace_peek.startswith('\n'):
+            # 抛弃左大括号后跟的掉空白符以及第一个换行符，也就是等于将body的第一行放到左大括号后面
+            self._consume_current_char_index(len(whitespace_peek)+1)
+    
+    def _is_leading_continuous_whitespaces(self):
+        if len(self.root.children) > 0 \
+            and isinstance(self.root.children[-1], TextNode) \
+            and self.root.children[-1].content.strip() == "" \
+            and self.root.children[-1].start.line_index == self._current_node.start.line_index \
+            and self.root.children[-1].start.char_index == 0 \
+            :
+            return True
+        else:
+            return False
+        
+    def _try_discard_leading_continuous_whitespaces(self):
+        # 清除当前 node 的行首前导空白符
+        # 上一个 text 结点是当前结点的前导空白符的判断标准：
+        # 1. 上一个结点是 TextNode，并且全是空白符
+        # 2. 上一个结点的 start 位置和当前结点的 start 位置在同一行
+        # 3. 上一个结点是从行首开始计数的（start.char_index == 0）
+        if len(self.root.children) > 0 \
+            and isinstance(self.root.children[-1], TextNode) \
+            and self.root.children[-1].content.strip() == "" \
+            and self.root.children[-1].start.line_index == self._current_node.start.line_index \
+            and self.root.children[-1].start.char_index == 0 \
+            :
+            self._is_line_of_current_start_has_visible_content = False
+            self._current_node.start = self.root.children[-1].start
+            self.root.children.pop()
+        
+    def _non_terminal_node_parse(self, keyword_type:KeywordsEnum):
+        self._end_current_node_at_last_char()
+        self._create_new_node_at_current_char(TranslateKeywords2Type(keyword_type))
+        assert isinstance(self._current_node, NonTerminalNode)
+        # 消费@关键词
+        self._current_node.content = f"{self._current_node.content}{self._current_char}{keyword_type.value}"
+        self._consume_current_char_index(len(keyword_type.value)+1)
+        
+        peek, after_peek = self._peek_while([' ', '\t'], True)
+        # 以左圆括号开头，说明有条件
+        if after_peek.startswith('('):
+            # 关键词与左圆括号之间的空白符，和左圆括号全部消费
+            self._current_node.append_content(f"{peek}(")
+            self._consume_current_char_index(len(peek)+1)
+            # 消费后，当前的字符应该是左圆括号后的条件表达式的第一个字符
+            self._current_node.condition, _, _ = self._consume_and_pair('(', ')', is_include_right=False)
+            # 消费右圆括号  
+            self._current_node.append_content(f")")      
+            self._consume_current_char_index()
+        
+        peek, after_peek = self._peek_while([' ', '\t', '\n', '\r'], True)
+        # 以左大括号开头，说明有 body
+        if after_peek.startswith('{'):
+            # 关键词与左大括号之间的空白符、换行符，和左大括号全部消费            
+            self._current_node.append_content(peek + "{")
+            self._consume_current_char_index(len(peek)+1)
+            # 抛弃左大括号后跟的掉空白符以及第一个换行符，也就是等于将body的第一行放到左大括号后面
+            # 消费后，当前的字符应该是左大括号后的body的第一个字符
+            self._try_discard_continuous_whitespaces_with_linefeed()
+            self._current_node.body, body_start, body_end = self._consume_and_pair('{', '}', is_include_right=False)
+            # 如果右括号单独一行，清除右大括号前的空白符，遇到换行符停止（不清除换行符）
+            is_right_brace_start_of_new_line = False
+            whitespace, after_whitespace_peek = self._peek_while_from_tail(self._current_node.body, [' ', '\t'])
+            if after_whitespace_peek.endswith('\n'):
+                is_right_brace_start_of_new_line = True
+                self._current_node.body = after_whitespace_peek
+                body_end = Position(body_end.line_index, body_end.char_index-len(whitespace), body_end.total-len(whitespace))
+            # 右大括号
+            self._current_node.append_content("}")
+            self._consume_current_char_index()
+            
+            # 处理子结点
+            sub_parser = Parser(self.template, self._current_node, body_start, body_end)
+            sub_parser.clean_trailing_whitespaces = False
+            sub_parser.Parse()
+            
+            # 如果子结点都是不可见，并且本分支结点单独一行；           
+            # 或者如果右括号单独一行, 清除右大括号后的空白符，遇到第一个换行符停止（清除换行符）
+            if (self._is_children_have_visible_content(self._current_node) == False\
+                and self._current_node.start.line_index == self._current_position.line_index)\
+                or is_right_brace_start_of_new_line == True:
+                self._try_discard_continuous_whitespaces_with_linefeed()
+            
+            self._end_current_node_at_last_char()
+            self._create_new_node_at_current_char()
+        else:
+            raise UnexpectedTokenError(self._current_position, ['{'], after_peek[0])
+        
+    def _is_children_have_visible_content(self, node:NonTerminalNode):
+        for child in node.children:
+            if isinstance(child, VisibleRole):
+                return True
+            elif isinstance(child, NonTerminalNode) and self._is_children_have_visible_content(child):
+                return True
+        return False
+    
+    def _terminal_keyword_process(self, keyword_type:KeywordsEnum):
+        self._end_current_node_at_last_char()
+        self._create_new_node_at_current_char(TranslateKeywords2Type(keyword_type))
+        assert isinstance(self._current_node, TerminalNode)
+        # 消费@关键词
+        # self._current_char is '@'
+        self._current_node.content = f"{self._current_node.content}{keyword_type.value}"
+        self._consume_current_char_index(len(keyword_type.value)+1)
+        # 消费掉分号
+        self._consume_current_char_index()
+        # 如果这一行只有终结符关键字，清除前导后随空白符和换行
+        if self._is_leading_continuous_whitespaces()\
+            and self._is_continuous_whitespaces_until_linefeed():
+            
+            self._try_discard_leading_continuous_whitespaces()
+            self._try_discard_continuous_whitespaces_with_linefeed()
+        
+        self._end_current_node_at_last_char()
+        self._create_new_node_at_current_char()
+    
+    def Parse(self):
+        if self.__used == True:
+            raise Exception("Parser can only be used once.")
+        while(self._current_position.total <= self._end.total):
+            if self._current_char == '\n':
+                # 每一个Text的换行都要新建一个 part
+                self._current_node.content = f"{self._current_node.content}{self._current_char}"
+                self._consume_current_char_index()
+                self._end_current_node_at_last_char()
+                self._create_new_node_at_current_char()
+                self._is_line_of_current_start_has_visible_content = False
+            
+            # 注释处理
+            elif (_detect_result := self._detect_annotation()) is not None:
+                start_type, end_sign = _detect_result
+                self._process_annotation(start_type, end_sign)
+            
+            # 可能的嵌入符号
+            elif self._current_char == '@':
+                # 前瞻也是@，那么就是转义为 @
+                if self._remains.startswith('@'):
+                    # 第一个 @ 不追加到 self._current_part.content 中，直接消费掉
+                    self._consume_current_char_index()
+                    # 直接追加第二个 @ 到 self._current_part.content 中，之后就不会触发嵌入符号的逻辑了
+                    self._current_node.content = f"{self._current_node.content}{self._current_char}"
+                    self._consume_current_char_index()
+                    
+                # 前瞻是 {，那么新建 part，匹配到 } 为止
+                elif self._remains.startswith('{'):
+                    self._new_node_foresee_and_pair(2, '{', '}', CodeBlockNode)
+                
+                # 前瞻是 (，那么新建 part，匹配到 ) 为止
+                elif self._remains.startswith('('):
+                    self._new_node_foresee_and_pair(2, '(', ')', ShowBlockNode, is_clean_whitespace=False)
+                                    
+                elif (keyword_type := self._non_terminal_keyword_check_type()) is not None:
+                    self._non_terminal_node_parse(keyword_type)
+                
+                elif (keyword_type := self._terminal_keyword_check_type()) is not None:
+                    # 处理主体
+                    self._terminal_keyword_process(keyword_type)
+                
+                # 未知的嵌入符号
+                else:
+                    _peek_identifier, _ = self._peek_until([' ', '\t', '\n', '\r', '(', ')', '{', '}', '[', ']', '"', "'", '`', '@', '#', '$', '%', '^', '&', '*', '-', '+', '=', '|', '\\', '/', '?', '<', '>', ',', '.', ';', ':', '!'])
+                    raise UnknownEmbedIdentifierError(self._current_position, _peek_identifier)
+                
+            # 纯文本
+            else:
+                self._current_node.content = f"{self._current_node.content}{self._current_char}"
+                self._consume_current_char_index()
+        
+        # 结束最后一个 part
+        self._end_current_node_at_last_char()
+        self.__used = True
+        self._post_process()
+        return self.root
+    
+    def _post_process(self):
+        if self.clean_trailing_whitespaces == True:
+            traverser = PreOrderTraverser(self.root)
+            traverser.entered_TextNode += self._delete_trailing_whitespaces
+            traverser.traverse()
+            traverser.entered_TextNode -= self._delete_trailing_whitespaces
+            
+    def _delete_trailing_whitespaces(self, sender:PreOrderTraverser, text_node:TextNode):
+        cleaned = ""
+        index = len(text_node.content) - 1
+        kill_whitespace = False
+        while index >= 0:
+            if text_node.content[index] == '\n':
+                cleaned = f"{text_node.content[index]}{cleaned}"
+                kill_whitespace = True
+            elif kill_whitespace == True and text_node.content[index] in [' ', '\t']:
+                pass
+            else:
+                cleaned = f"{text_node.content[index]}{cleaned}"
+                kill_whitespace = False
+            index -= 1
+        text_node.content = cleaned
+
+class PairFinder():
+    def __init__(self, left:str, right:str) -> None:
+        self.unpaired_left_count = 0
+        self.__left = left
+        self.__right = right
+    
+    def IsPair(self, target:str):
+        if target == self.__left:
+            self.unpaired_left_count += 1
+            return False
+        elif target == self.__right:
+            if self.unpaired_left_count == 0:
+                return True
+            else:
+                self.unpaired_left_count -= 1
+                return False
+        else:
             return False
```

### Comparing `pymaidol-0.1.2/pymaidol/Positions.py` & `pymaidol-0.1.3/pymaidol/Positions.py`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/pymaidol/SyntaxChecker.py` & `pymaidol-0.1.3/pymaidol/SyntaxChecker.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from pymaidol.Errors import BranchError, ElseExtraConditionError, LackingConditionError
-from pymaidol.Nodes import (BaseNode, BranchRole, ElifNode, ElseNode, ForNode, IfNode,
-                   TextNode, WhileNode)
-from pymaidol.Traversers import PreOrderTraverser
-
-
-class SyntaxChecker():
-    def __init__(self) -> None:
-        pass
-    
-    def Check(self, root:BaseNode):        
-        traverser = PreOrderTraverser(root)
-        traverser.entered_IfNode += self._construct_if_branches
-        traverser.entered_ForNode += self._loop_node_condition_check
-        traverser.entered_WhileNode += self._loop_node_condition_check
-        traverser.entered_BranchRole += self._wrong_branch_check
-        
-        traverser.traverse()
-        
-        traverser.entered_IfNode -= self._construct_if_branches
-        traverser.entered_ForNode -= self._loop_node_condition_check
-        traverser.entered_WhileNode -= self._loop_node_condition_check
-        traverser.entered_BranchRole -= self._wrong_branch_check
-        
-        return root
-    
-    def _construct_if_branches(self, sender:PreOrderTraverser, node:IfNode):
-        # 不知道为什么没有在初始化时拥有属性，因此在这里定义
-        node.previous_branch = None
-        node.next_branch = None
-        if node.condition is None:
-            raise LackingConditionError(node.start)
-        father = node.father
-        assert father is not None
-        index = father.children.index(node)
-        index += 1
-        previous = node
-        possible_gapping_whitespace_index:list[int] = []
-        # 检查后续连续的 elif 和 else 结点，将它们构造成以 if 结点为头结点的链表
-        while index < len(father.children):
-            current = father.children[index]
-            if isinstance(current, (ElifNode, ElseNode)):                
-                current.previous_branch = None
-                current.next_branch = None
-                if isinstance(current, ElifNode) and current.condition is None:
-                    raise LackingConditionError(current.start)
-                if isinstance(current, ElseNode) and current.condition is not None:
-                    raise ElseExtraConditionError(current.start)
-                # 设置链表
-                previous.next_branch = current
-                current.previous_branch = previous
-                previous = current                
-                # 本分支结点不再能从父结点进入，只能从上一个分支结点进入                
-                father.children.pop(index)
-                # 倒序删除间隔的空白符
-                for i in reversed(possible_gapping_whitespace_index):                   
-                    father.children.pop(i)
-                index -= len(possible_gapping_whitespace_index)
-                possible_gapping_whitespace_index.clear()
-                # else 后面不会再有分支结点，直接退出
-                if isinstance(current, ElseNode):                    
-                    break
-            elif isinstance(current, TextNode):                
-                if current.content.strip() == '':
-                    # 虽然中间插了文本结点，但是全是空白符，可以忽略
-                    possible_gapping_whitespace_index.append(index)
-                    index += 1
-                else:
-                    break
-            else:
-                break
-    
-    def _loop_node_condition_check(self, sender:PreOrderTraverser, node:ForNode|WhileNode):
-        if node.condition is None:
-            raise LackingConditionError(node.start)
-    
-    def _wrong_branch_check(self, sender:PreOrderTraverser, node:BranchRole):
-        # 所有的 elif 和 else 结点都被从父结点中移除了，只能从 if 进入
-        # 如果触发这个方法，说明有游离的 elif 或 else 结点
-        if isinstance(node, (ElifNode, ElseNode)):
+from pymaidol.Errors import BranchError, ElseExtraConditionError, LackingConditionError
+from pymaidol.Nodes import (BaseNode, BranchRole, ElifNode, ElseNode, ForNode, IfNode,
+                   TextNode, WhileNode)
+from pymaidol.Traversers import PreOrderTraverser
+
+
+class SyntaxChecker():
+    def __init__(self) -> None:
+        pass
+    
+    def Check(self, root:BaseNode):        
+        traverser = PreOrderTraverser(root)
+        traverser.entered_IfNode += self._construct_if_branches
+        traverser.entered_ForNode += self._loop_node_condition_check
+        traverser.entered_WhileNode += self._loop_node_condition_check
+        traverser.entered_BranchRole += self._wrong_branch_check
+        
+        traverser.traverse()
+        
+        traverser.entered_IfNode -= self._construct_if_branches
+        traverser.entered_ForNode -= self._loop_node_condition_check
+        traverser.entered_WhileNode -= self._loop_node_condition_check
+        traverser.entered_BranchRole -= self._wrong_branch_check
+        
+        return root
+    
+    def _construct_if_branches(self, sender:PreOrderTraverser, node:IfNode):
+        # 不知道为什么没有在初始化时拥有属性，因此在这里定义
+        node.previous_branch = None
+        node.next_branch = None
+        if node.condition is None:
+            raise LackingConditionError(node.start)
+        father = node.father
+        assert father is not None
+        index = father.children.index(node)
+        index += 1
+        previous = node
+        possible_gapping_whitespace_index:list[int] = []
+        # 检查后续连续的 elif 和 else 结点，将它们构造成以 if 结点为头结点的链表
+        while index < len(father.children):
+            current = father.children[index]
+            if isinstance(current, (ElifNode, ElseNode)):                
+                current.previous_branch = None
+                current.next_branch = None
+                if isinstance(current, ElifNode) and current.condition is None:
+                    raise LackingConditionError(current.start)
+                if isinstance(current, ElseNode) and current.condition is not None:
+                    raise ElseExtraConditionError(current.start)
+                # 设置链表
+                previous.next_branch = current
+                current.previous_branch = previous
+                previous = current                
+                # 本分支结点不再能从父结点进入，只能从上一个分支结点进入                
+                father.children.pop(index)
+                # 倒序删除间隔的空白符
+                for i in reversed(possible_gapping_whitespace_index):                   
+                    father.children.pop(i)
+                index -= len(possible_gapping_whitespace_index)
+                possible_gapping_whitespace_index.clear()
+                # else 后面不会再有分支结点，直接退出
+                if isinstance(current, ElseNode):                    
+                    break
+            elif isinstance(current, TextNode):                
+                if current.content.strip() == '':
+                    # 虽然中间插了文本结点，但是全是空白符，可以忽略
+                    possible_gapping_whitespace_index.append(index)
+                    index += 1
+                else:
+                    break
+            else:
+                break
+    
+    def _loop_node_condition_check(self, sender:PreOrderTraverser, node:ForNode|WhileNode):
+        if node.condition is None:
+            raise LackingConditionError(node.start)
+    
+    def _wrong_branch_check(self, sender:PreOrderTraverser, node:BranchRole):
+        # 所有的 elif 和 else 结点都被从父结点中移除了，只能从 if 进入
+        # 如果触发这个方法，说明有游离的 elif 或 else 结点
+        if isinstance(node, (ElifNode, ElseNode)):
             raise BranchError(node.start)
```

### Comparing `pymaidol-0.1.2/pymaidol/TemplateBase.py` & `pymaidol-0.1.3/pymaidol/TemplateBase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,78 @@
-
-import inspect
-from abc import ABC, abstractmethod
-from typing import Any, Optional, final
-
-from pymaidol.Executor import Executor
-from pymaidol.Parser import Parser
-from pymaidol.SyntaxChecker import SyntaxChecker
-from pymaidol.TemplateRenderer import TemplateRenderer
-from pymaidol.AnnotationType import FULL_ANNOTATION_TYPE, AnnotationTypeEnum
-
-
-class TemplateBase(ABC):
-    @abstractmethod
-    def __init__(self, 
-                 template:Optional[str]=None, 
-                 template_file_path:Optional[str]=None,
-                 supported_annotation_types:'list[AnnotationTypeEnum]' = FULL_ANNOTATION_TYPE) -> None:
-        self.supported_annotation_types = supported_annotation_types
-        self.HotReload(template, template_file_path)
-        self._rendered:Optional[str] = None    
-    
-    @property
-    def template(self): 
-        return self._renderer.template
-    
-    @property
-    def rendered(self): 
-        '''
-        模板设计文件渲染后的结果。如果初始化或热重载以来没有渲染过，则为None。
-        '''
-        return self._rendered    
-    
-    @final
-    def HotReload(self, template:Optional[str]=None, template_file_path:Optional[str]=None):
-        """ 热重载模板设计文件。如果不指定模板设计文件路径，则使用初始化时指定的模板设计文件路径或者检测到的模板设计文件路径。
-
-        Args:
-            template_file_path (Optional[str], optional): 模板设计文件路径. Defaults to None.
-        """
-        if template is not None:
-            pass
-        elif template_file_path is not None:
-            template = self._ReadTemplate(template_file_path)
-        else:
-            # 获取类的文件路径
-            # https://stackoverflow.com/a/697395
-            template_file_path = inspect.getfile(self.__class__)[:-3] + ".pymd"
-            template = self._ReadTemplate(template_file_path)        
-        self._renderer = TemplateRenderer(template, self.supported_annotation_types)
-    
-    @final
-    def _ReadTemplate(self, template_file_path)->str:
-        try: 
-            with open(template_file_path, "r", encoding='utf-8') as f:
-                return f.read()
-        except FileNotFoundError as fex:
-            fex.strerror = f"No such template design file"
-            raise fex
-    
-    @final
-    def Render(self, inject_kwargs:Optional[dict[str, Any]] = None) -> str:
-        global_vars:dict[str, Any] = {}
-        local_vars = {"self": self}
-        if inject_kwargs is not None:
-            global_vars.update(inject_kwargs)
-        result = self._renderer.Render(local_vars, global_vars)
-        self._rendered = result
-        return result
-    
-    @final
-    def TranslateToPython(self) -> str:
-        return self._renderer.TranslateToPython()
+import copy
+import inspect
+from abc import ABC, abstractmethod
+from typing import Any, Optional, final
+
+from pymaidol.Executor import Executor
+from pymaidol.Parser import Parser
+from pymaidol.SyntaxChecker import SyntaxChecker
+from pymaidol.TemplateRenderer import TemplateRenderer
+from pymaidol.AnnotationType import FULL_ANNOTATION_TYPE, AnnotationTypeEnum
+
+
+class TemplateBase(ABC):
+    @abstractmethod
+    def __init__(self, 
+                 template:Optional[str]=None, 
+                 template_file_path:Optional[str]=None,
+                 supported_annotation_types:'list[AnnotationTypeEnum]' = FULL_ANNOTATION_TYPE,
+                 disable_annotation_types:'list[AnnotationTypeEnum]' = []) -> None:
+        self.supported_annotation_types = copy.deepcopy(supported_annotation_types) 
+        for annotation_type in disable_annotation_types:
+            for supported_annotation_type in self.supported_annotation_types:
+                if annotation_type.value == supported_annotation_type.value:
+                    self.supported_annotation_types.remove(supported_annotation_type)
+        self.HotReload(template, template_file_path)
+        self._rendered:Optional[str] = None    
+    
+    @property
+    def template(self): 
+        return self._renderer.template
+    
+    @property
+    def rendered(self): 
+        '''
+        模板设计文件渲染后的结果。如果初始化或热重载以来没有渲染过，则为None。
+        '''
+        return self._rendered    
+    
+    @final
+    def HotReload(self, template:Optional[str]=None, template_file_path:Optional[str]=None):
+        """ 热重载模板设计文件。如果不指定模板设计文件路径，则使用初始化时指定的模板设计文件路径或者检测到的模板设计文件路径。
+
+        Args:
+            template_file_path (Optional[str], optional): 模板设计文件路径. Defaults to None.
+        """
+        if template is not None:
+            pass
+        elif template_file_path is not None:
+            template = self._ReadTemplate(template_file_path)
+        else:
+            # 获取类的文件路径
+            # https://stackoverflow.com/a/697395
+            template_file_path = inspect.getfile(self.__class__)[:-3] + ".pymd"
+            template = self._ReadTemplate(template_file_path)        
+        self._renderer = TemplateRenderer(template, self.supported_annotation_types)
+    
+    @final
+    def _ReadTemplate(self, template_file_path)->str:
+        try: 
+            with open(template_file_path, "r", encoding='utf-8') as f:
+                return f.read()
+        except FileNotFoundError as fex:
+            fex.strerror = f"No such template design file"
+            raise fex
+    
+    @final
+    def Render(self, inject_kwargs:Optional[dict[str, Any]] = None) -> str:
+        global_vars:dict[str, Any] = {}
+        local_vars = {"self": self}
+        if inject_kwargs is not None:
+            global_vars.update(inject_kwargs)
+        result = self._renderer.Render(local_vars, global_vars)
+        self._rendered = result
+        return result
+    
+    @final
+    def TranslateToPython(self) -> str:
+        return self._renderer.TranslateToPython()
```

### Comparing `pymaidol-0.1.2/pymaidol/TemplateRenderer.py` & `pymaidol-0.1.3/pymaidol/TemplateRenderer.py`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/pymaidol/Traversers.py` & `pymaidol-0.1.3/pymaidol/Traversers.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-from abc import ABC, abstractmethod
-
-from pythondelegate.event_handler import EventHandler
-
-from pymaidol.Nodes import (AnnotationNode, BaseNode, BodyComponent, BranchRole,
-                    BreakNode, CodeBlockNode, ComponentOrRole, ContinueNode,
-                    ElifNode, ElseNode, EmptyNode, ForNode, IfNode,
-                    InvisibleRole, LoopRole, NonTerminalNode, ShowBlockNode,
-                    TerminalNode, TextNode, VisibleRole, WhileNode)
-
-
-class TraverserBase(ABC):
-    def __init__(self, tree_root:BaseNode, is_trigger_father_class_event:bool=True):
-        """ The base class of all traversers. It provides a series of events that can be triggered when traversing the tree. The event is triggered when the node is entered. The event is triggered in the order of the inheritance chain of the node class. 
-        
-        Args:
-            tree_root (BaseNode): The root node of the tree to be traversed.
-            is_trigger_father_class_event (bool, optional): Whether to trigger the event of the parent class. Defaults to True. For example, if current node is a TextNode and this parameter is False, then the event of TerminalNode will not be triggered. Defaults to True.
-        """
-        self.entered_BaseNode = EventHandler[BaseNode]()
-        self.entered_TerminalNode = EventHandler[TerminalNode]()
-        self.entered_NonTerminalNode = EventHandler[NonTerminalNode]()
-        self.entered_TextNode = EventHandler[TextNode]()
-        self.entered_AnnotationNode = EventHandler[AnnotationNode]()
-        self.entered_ShowBlockNode = EventHandler[ShowBlockNode]()
-        self.entered_CodeBlockNode = EventHandler[CodeBlockNode]()
-        self.entered_IfNode = EventHandler[IfNode]()
-        self.entered_ElifNode = EventHandler[ElifNode]()
-        self.entered_ElseNode = EventHandler[ElseNode]()
-        self.entered_ForNode = EventHandler[ForNode]()
-        self.entered_WhileNode = EventHandler[WhileNode]()
-        self.entered_BreakNode = EventHandler[BreakNode]()
-        self.entered_ContinueNode = EventHandler[ContinueNode]()
-        self.entered_EmptyNode = EventHandler[EmptyNode]()
-        
-        self.entered_BranchRole = EventHandler[BranchRole]()
-        self.entered_ComponentOrRole = EventHandler[ComponentOrRole]()
-        self.entered_VisibleRole = EventHandler[VisibleRole]()
-        self.entered_InvisibleRole = EventHandler[InvisibleRole]()
-        self.entered_BodyComponent = EventHandler[BodyComponent]()
-        self.entered_LoopRole = EventHandler[LoopRole]()
-        
-        self.tree_root = tree_root
-        self.is_trigger_father_class_event = is_trigger_father_class_event
-        
-    def _entered_event_invoke(self, node:BaseNode):
-        if node is None:
-            return
-        # TerminalNode
-        if type(node) == TextNode: 
-            self.entered_TextNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == AnnotationNode: 
-            self.entered_AnnotationNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == ShowBlockNode: 
-            self.entered_ShowBlockNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == CodeBlockNode: 
-            self.entered_CodeBlockNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == BreakNode: 
-            self.entered_BreakNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == ContinueNode: 
-            self.entered_ContinueNode(self, node)
-            if self.is_trigger_father_class_event: return
-            
-        # NonTerminalNode
-        if type(node) == IfNode: 
-            self.entered_IfNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == ElifNode: 
-            self.entered_ElifNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == ElseNode: 
-            self.entered_ElseNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == ForNode: 
-            self.entered_ForNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == WhileNode: 
-            self.entered_WhileNode(self, node)     
-            if self.is_trigger_father_class_event: return   
-        if type(node) == EmptyNode: 
-            self.entered_EmptyNode(self, node)
-            if self.is_trigger_father_class_event: return
-        
-        # VirtualNode
-        if type(node) == TerminalNode: 
-            self.entered_TerminalNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == NonTerminalNode: 
-            self.entered_NonTerminalNode(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == BaseNode:
-            self.entered_BaseNode(self, node)
-            if self.is_trigger_father_class_event: return
-            
-        # ComponentNode
-        if type(node) == LoopRole: 
-            self.entered_LoopRole(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == BranchRole: 
-            self.entered_BranchRole(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == BodyComponent: 
-            self.entered_BodyComponent(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == InvisibleRole: 
-            self.entered_InvisibleRole(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == VisibleRole: 
-            self.entered_VisibleRole(self, node)
-            if self.is_trigger_father_class_event: return
-        if type(node) == ComponentOrRole: 
-            self.entered_ComponentOrRole(self, node)
-            if self.is_trigger_father_class_event: return
-    
-    def traverse(self):
-        self._recursive_traverse(self.tree_root)
-    
-    @abstractmethod
-    def _recursive_traverse(self, node:BaseNode):
-        pass
-
-
-class PreOrderTraverser(TraverserBase):
-    """
-        先序（先根）遍历语法树。
-    """
-    # Override
-    def _recursive_traverse(self, node:BaseNode):
-        self._entered_event_invoke(node)
-        if isinstance(node, NonTerminalNode):
-            index = 0
-            # 由于在遍历过程中可能会修改children，所以不能使用for循环
-            while index < len(node.children):
-                current_node = node.children[index]
-                self._recursive_traverse(current_node)
-                try:
-                    index = node.children.index(current_node)
-                except:
-                    pass
-                index += 1
-        
-class InOrderTraverser(TraverserBase):
-    """
-        中序（后根）遍历语法树。
-    """
-    # Override
-    def _recursive_traverse(self, node:BaseNode):        
-        if isinstance(node, NonTerminalNode):
-            index = 0
-            # 由于在遍历过程中可能会修改children，所以不能使用for循环
-            while index < len(node.children):
-                current_node = node.children[index]
-                self._recursive_traverse(current_node)
-                try:
-                    index = node.children.index(current_node)
-                except:
-                    pass
-                index += 1
+from abc import ABC, abstractmethod
+
+from pythondelegate.event_handler import EventHandler
+
+from pymaidol.Nodes import (AnnotationNode, BaseNode, BodyComponent, BranchRole,
+                    BreakNode, CodeBlockNode, ComponentOrRole, ContinueNode,
+                    ElifNode, ElseNode, EmptyNode, ForNode, IfNode,
+                    InvisibleRole, LoopRole, NonTerminalNode, ShowBlockNode,
+                    TerminalNode, TextNode, VisibleRole, WhileNode)
+
+
+class TraverserBase(ABC):
+    def __init__(self, tree_root:BaseNode, is_trigger_father_class_event:bool=True):
+        """ The base class of all traversers. It provides a series of events that can be triggered when traversing the tree. The event is triggered when the node is entered. The event is triggered in the order of the inheritance chain of the node class. 
+        
+        Args:
+            tree_root (BaseNode): The root node of the tree to be traversed.
+            is_trigger_father_class_event (bool, optional): Whether to trigger the event of the parent class. Defaults to True. For example, if current node is a TextNode and this parameter is False, then the event of TerminalNode will not be triggered. Defaults to True.
+        """
+        self.entered_BaseNode = EventHandler[BaseNode]()
+        self.entered_TerminalNode = EventHandler[TerminalNode]()
+        self.entered_NonTerminalNode = EventHandler[NonTerminalNode]()
+        self.entered_TextNode = EventHandler[TextNode]()
+        self.entered_AnnotationNode = EventHandler[AnnotationNode]()
+        self.entered_ShowBlockNode = EventHandler[ShowBlockNode]()
+        self.entered_CodeBlockNode = EventHandler[CodeBlockNode]()
+        self.entered_IfNode = EventHandler[IfNode]()
+        self.entered_ElifNode = EventHandler[ElifNode]()
+        self.entered_ElseNode = EventHandler[ElseNode]()
+        self.entered_ForNode = EventHandler[ForNode]()
+        self.entered_WhileNode = EventHandler[WhileNode]()
+        self.entered_BreakNode = EventHandler[BreakNode]()
+        self.entered_ContinueNode = EventHandler[ContinueNode]()
+        self.entered_EmptyNode = EventHandler[EmptyNode]()
+        
+        self.entered_BranchRole = EventHandler[BranchRole]()
+        self.entered_ComponentOrRole = EventHandler[ComponentOrRole]()
+        self.entered_VisibleRole = EventHandler[VisibleRole]()
+        self.entered_InvisibleRole = EventHandler[InvisibleRole]()
+        self.entered_BodyComponent = EventHandler[BodyComponent]()
+        self.entered_LoopRole = EventHandler[LoopRole]()
+        
+        self.tree_root = tree_root
+        self.is_trigger_father_class_event = is_trigger_father_class_event
+        
+    def _entered_event_invoke(self, node:BaseNode):
+        if node is None:
+            return
+        # TerminalNode
+        if type(node) == TextNode: 
+            self.entered_TextNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == AnnotationNode: 
+            self.entered_AnnotationNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == ShowBlockNode: 
+            self.entered_ShowBlockNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == CodeBlockNode: 
+            self.entered_CodeBlockNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == BreakNode: 
+            self.entered_BreakNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == ContinueNode: 
+            self.entered_ContinueNode(self, node)
+            if self.is_trigger_father_class_event: return
+            
+        # NonTerminalNode
+        if type(node) == IfNode: 
+            self.entered_IfNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == ElifNode: 
+            self.entered_ElifNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == ElseNode: 
+            self.entered_ElseNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == ForNode: 
+            self.entered_ForNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == WhileNode: 
+            self.entered_WhileNode(self, node)     
+            if self.is_trigger_father_class_event: return   
+        if type(node) == EmptyNode: 
+            self.entered_EmptyNode(self, node)
+            if self.is_trigger_father_class_event: return
+        
+        # VirtualNode
+        if type(node) == TerminalNode: 
+            self.entered_TerminalNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == NonTerminalNode: 
+            self.entered_NonTerminalNode(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == BaseNode:
+            self.entered_BaseNode(self, node)
+            if self.is_trigger_father_class_event: return
+            
+        # ComponentNode
+        if type(node) == LoopRole: 
+            self.entered_LoopRole(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == BranchRole: 
+            self.entered_BranchRole(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == BodyComponent: 
+            self.entered_BodyComponent(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == InvisibleRole: 
+            self.entered_InvisibleRole(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == VisibleRole: 
+            self.entered_VisibleRole(self, node)
+            if self.is_trigger_father_class_event: return
+        if type(node) == ComponentOrRole: 
+            self.entered_ComponentOrRole(self, node)
+            if self.is_trigger_father_class_event: return
+    
+    def traverse(self):
+        self._recursive_traverse(self.tree_root)
+    
+    @abstractmethod
+    def _recursive_traverse(self, node:BaseNode):
+        pass
+
+
+class PreOrderTraverser(TraverserBase):
+    """
+        先序（先根）遍历语法树。
+    """
+    # Override
+    def _recursive_traverse(self, node:BaseNode):
+        self._entered_event_invoke(node)
+        if isinstance(node, NonTerminalNode):
+            index = 0
+            # 由于在遍历过程中可能会修改children，所以不能使用for循环
+            while index < len(node.children):
+                current_node = node.children[index]
+                self._recursive_traverse(current_node)
+                try:
+                    index = node.children.index(current_node)
+                except:
+                    pass
+                index += 1
+        
+class InOrderTraverser(TraverserBase):
+    """
+        中序（后根）遍历语法树。
+    """
+    # Override
+    def _recursive_traverse(self, node:BaseNode):        
+        if isinstance(node, NonTerminalNode):
+            index = 0
+            # 由于在遍历过程中可能会修改children，所以不能使用for循环
+            while index < len(node.children):
+                current_node = node.children[index]
+                self._recursive_traverse(current_node)
+                try:
+                    index = node.children.index(current_node)
+                except:
+                    pass
+                index += 1
         self._entered_event_invoke(node)
```

### Comparing `pymaidol-0.1.2/pymaidol/__main__.py` & `pymaidol-0.1.3/pymaidol/__main__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import argparse
-import os
-from pymaidol.code_templates.SubClassTemplate import SubClassTemplate
-
-
-parser = argparse.ArgumentParser()
-parser.add_argument('-n', '--name', type=str, help="the class name of the pymaidol files")
-parser.add_argument('-d', '--dir', type=str, help="the directory of the pymaidol files", default="")
-args = parser.parse_args()
-path = args.dir
-if path is not None and path.strip() != "":
-    os.makedirs(path.strip(), exist_ok=True)
-template_file_path =  os.path.join(path, f'{args.name}.pymd')
-code_file_path =  os.path.join(path, f'{args.name}.py')
-# designer file
-if os.path.exists(template_file_path):
-    message = f'Fail: file "{template_file_path}" already exist'
-    print(f'\033[0;31;49m{message}\033[0m')
-else:
-    with open(template_file_path, 'w', encoding='utf-8') as f:
-        f.write("")
-        f.close()
-    message = f'Success: file "{template_file_path}" created'
-    print(f'\033[0;32;49m{message}\033[0m')
-# py file
-if os.path.exists(code_file_path):
-    message = f'Fail: file "{code_file_path}" already exist'
-    print(f'\033[0;31;49m{message}\033[0m')
-else:
-    template = SubClassTemplate(args.name)
-    with open(code_file_path, 'w', encoding='utf-8') as f:
-        f.write(template.Render())
-        f.close()
-    message = f'Success: file "{code_file_path}" created'
-    print(f'\033[0;32;49m{message}\033[0m')
+import argparse
+import os
+from pymaidol.code_templates.SubClassTemplate import SubClassTemplate
+
+
+parser = argparse.ArgumentParser()
+parser.add_argument('-n', '--name', type=str, help="the class name of the pymaidol files")
+parser.add_argument('-d', '--dir', type=str, help="the directory of the pymaidol files", default="")
+args = parser.parse_args()
+path = args.dir
+if path is not None and path.strip() != "":
+    os.makedirs(path.strip(), exist_ok=True)
+template_file_path =  os.path.join(path, f'{args.name}.pymd')
+code_file_path =  os.path.join(path, f'{args.name}.py')
+# designer file
+if os.path.exists(template_file_path):
+    message = f'Fail: file "{template_file_path}" already exist'
+    print(f'\033[0;31;49m{message}\033[0m')
+else:
+    with open(template_file_path, 'w', encoding='utf-8') as f:
+        f.write("")
+        f.close()
+    message = f'Success: file "{template_file_path}" created'
+    print(f'\033[0;32;49m{message}\033[0m')
+# py file
+if os.path.exists(code_file_path):
+    message = f'Fail: file "{code_file_path}" already exist'
+    print(f'\033[0;31;49m{message}\033[0m')
+else:
+    template = SubClassTemplate(args.name)
+    with open(code_file_path, 'w', encoding='utf-8') as f:
+        f.write(template.Render())
+        f.close()
+    message = f'Success: file "{code_file_path}" created'
+    print(f'\033[0;32;49m{message}\033[0m')
```

### Comparing `pymaidol-0.1.2/pymaidol.egg-info/PKG-INFO` & `pymaidol-0.1.3/pymaidol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymaidol
-Version: 0.1.2
+Version: 0.1.3
 Summary: A markup gramma that embed python code into text
 Author: Eterance
 Keywords: Prompt,Markup Language,NLP,AI,GPT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -20,15 +20,15 @@
 ⚠**警告：Pymaidol 目前处于开发阶段，语法和一些对空白符、换行符的处理逻辑尚未确定，以后可能会被修改。强烈不建议在生产环境中使用。**
 
 ## 环境要求与安装
 
 python >= 3.10
 
 ``` bash
-pip install Pymaidol
+pip install Pymaidol -i https://pypi.python.org/simple
 ```
 
 ## 第一个 Pymaidol 模板
 
 ### 创建模板文件
 
 首先，假设你创建了一个名为 `pymaidol_test` 的文件夹。使用编辑器或者 IDE 打开该文件夹作为工作目录。
```

### Comparing `pymaidol-0.1.2/pymaidol.egg-info/SOURCES.txt` & `pymaidol-0.1.3/pymaidol.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 pymaidol.egg-info/top_level.txt
 pymaidol/code_templates/SubClassTemplate.py
 pymaidol/code_templates/SubClassTemplate.pymd
 pymaidol/code_templates/__init__.py
 tests/test_class.py
 tests/test_class.pymd
 tests/test_everything.py
+tests/din/ContextDebugTemplate.py
+tests/din/ContextDebugTemplate.pymd
+tests/din/test.py
 tests/harder_demo/CodeLangTemplate.py
 tests/harder_demo/CodeLangTemplate.pymd
 tests/harder_demo/codelang.json
 tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json
 tests/harder_demo/sparc_sub_dataset.pml
 tests/harder_demo/sparc_sub_dataset.py
 tests/harder_demo/sparc_sub_dataset_pml.py
```

### Comparing `pymaidol-0.1.2/tests/harder_demo/CodeLangTemplate.pymd` & `pymaidol-0.1.3/tests/harder_demo/CodeLangTemplate.pymd`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json` & `pymaidol-0.1.3/tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset.pml` & `pymaidol-0.1.3/tests/harder_demo/sparc_sub_dataset.pml`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset_pml.py` & `pymaidol-0.1.3/tests/harder_demo/sparc_sub_dataset_pml.py`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.2/tests/test_everything.py` & `pymaidol-0.1.3/tests/test_everything.py`

 * *Files identical despite different names*

