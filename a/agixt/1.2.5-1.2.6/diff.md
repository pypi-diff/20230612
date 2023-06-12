# Comparing `tmp/agixt-1.2.5.tar.gz` & `tmp/agixt-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.5.tar", last modified: Mon Jun 12 03:39:16 2023, max compression
+gzip compressed data, was "agixt-1.2.6.tar", last modified: Mon Jun 12 04:26:37 2023, max compression
```

## Comparing `agixt-1.2.5.tar` & `agixt-1.2.6.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 03:39:03.000000 agixt-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 03:39:03.000000 agixt-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 03:39:16.415971 agixt-1.2.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.391970 agixt-1.2.5/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.395970 agixt-1.2.5/agixt/WORKSPACE/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/WORKSPACE/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.387970 agixt-1.2.5/agixt/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.395970 agixt-1.2.5/agixt/agents/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/agents/gpt4free/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.395970 agixt-1.2.5/agixt/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Smart Chat.json
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Smart Instruct.json
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Task.json
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Test_Commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Write a Poem.json
--rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.395970 agixt-1.2.5/agixt/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/agixt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/briantts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/dalle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/gtts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/macostts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/microsoft_365.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/searxng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/sendgrid_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/web_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Chat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Create New Command.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Custom Input.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Get Task List.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Prioritize.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Score Response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Task Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Tell Me How.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Title a Poem.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Validation.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/WebSearch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Write a Poem.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/gpt-3.5-turbo/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/gpt-3.5-turbo/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/gpt-4/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/starchat/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/starchat/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/vicuna/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/vicuna/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.403971 agixt-1.2.5/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/runpod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.391970 agixt-1.2.5/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.403971 agixt-1.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.403971 agixt-1.2.5/docs/1-Getting started/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/1-Getting started/Quick Start.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/1-Getting started/Screenshots.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/1-Getting started/Support.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.407971 agixt-1.2.5/docs/2-Concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/0-Core Concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Prompts.md
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Providers.md
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Smart Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Smart Instruct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Smart Task.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Tasks.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.407971 agixt-1.2.5/docs/3-Providers/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Anthropic Claude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Azure OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/ChatGPT.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/FastChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/GPT4ALL-GPU.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/GPT4ALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/GPT4Free.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Google Bard.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Google Palm.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Hugging Face Transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/HuggingChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Kobold.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Microsoft Bing.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Oobabooga Text Generation Web UI.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/llamacpp API.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/llamacpp.md
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.411971 agixt-1.2.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT-gradient-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT-gradient-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT.png
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT_Original_PSD.psd
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXTwhiteborder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Docker-desktop-win-setting-streamlit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Smart Instruct.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Smart Instruct.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Smart Tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Smart Tasks.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Untitled Diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 03:39:03.000000 agixt-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 03:39:03.000000 agixt-1.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:39:16.415971 agixt-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-12 03:39:03.000000 agixt-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.411971 agixt-1.2.5/streamlit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.411971 agixt-1.2.5/streamlit/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/Main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.411971 agixt-1.2.5/streamlit/auth_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/Cfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/Redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/Users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/streamlit/auth_libs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/pages/Login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/pages/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/pages/Register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/verify_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/streamlit/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/pages/0-Agent_Settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/pages/1-Prompt_Templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/pages/2-Chain_Management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/pages/3-Interact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-12 03:39:03.000000 agixt-1.2.5/tests/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-12 03:39:03.000000 agixt-1.2.5/tests/test-commands.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-06-12 03:39:03.000000 agixt-1.2.5/tests/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.787020 agixt-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 04:26:23.000000 agixt-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 04:26:23.000000 agixt-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 04:26:37.787020 agixt-1.2.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.759019 agixt-1.2.6/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.763019 agixt-1.2.6/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.755019 agixt-1.2.6/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.763019 agixt-1.2.6/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.763019 agixt-1.2.6/agixt/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Smart Chat.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Smart Instruct.json
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Task.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Test_Commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Write a Poem.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.763019 agixt-1.2.6/agixt/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/agixt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/briantts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/gtts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/macostts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/microsoft_365.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/searxng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/web_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Chat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Create New Command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Custom Input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Get Task List.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Prioritize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Score Response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Task Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Validation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/WebSearch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Write a Poem.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/gpt-3.5-turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/gpt-3.5-turbo/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/gpt-4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/starchat/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/starchat/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/vicuna/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.775020 agixt-1.2.6/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.759019 agixt-1.2.6/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.775020 agixt-1.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.775020 agixt-1.2.6/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/1-Getting started/Screenshots.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.775020 agixt-1.2.6/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Smart Task.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Tasks.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.779019 agixt-1.2.6/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 04:26:23.000000 agixt-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 04:26:23.000000 agixt-1.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 04:26:37.787020 agixt-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-12 04:26:23.000000 agixt-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/Main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/auth_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/Cfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/Redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/Users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/auth_libs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/pages/Login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/pages/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/pages/Register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/verify_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.787020 agixt-1.2.6/streamlit/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/pages/0-Agent_Settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/pages/1-Prompt_Templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/pages/2-Chain_Management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/pages/3-Interact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.787020 agixt-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-12 04:26:23.000000 agixt-1.2.6/tests/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-12 04:26:23.000000 agixt-1.2.6/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-06-12 04:26:23.000000 agixt-1.2.6/tests/tests.ipynb
```

### Comparing `agixt-1.2.5/LICENSE` & `agixt-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/PKG-INFO` & `agixt-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.5
+Version: 1.2.6
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.5/agixt/Agent.py` & `agixt-1.2.6/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/Chain.py` & `agixt-1.2.6/agixt/Chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,14 @@
         return responses
 
     def get_step_response(self, chain_name, step_number="all"):
         file_path = get_chain_responses_file_path(chain_name=chain_name)
         try:
             with open(file_path, "r") as f:
                 responses = json.load(f)
-            print(responses)
             if step_number == "all":
                 return responses
             else:
                 return responses.get(str(step_number))
         except:
             return ""
 
@@ -246,21 +245,20 @@
                     prompt_name = ""
                 args = self.get_step_content(
                     chain_name=chain_name,
                     prompt_content=step["prompt"],
                     user_input=user_input,
                     agent_name=agent_name,
                 )
-                print(f"ARGS: {args}")
                 if prompt_type == "Command":
                     return await Extensions(
                         agent_config=agent.agent.agent_config
                     ).execute_command(
                         command_name=args["command_name"],
-                        command_args=args["command_args"],
+                        command_args=args,
                     )
                 elif prompt_type == "Prompt":
                     result = await agent.run(
                         user_input=user_input,
                         prompt=prompt_name,
                         chain_name=chain_name,
                         step_number=step_number,
```

### Comparing `agixt-1.2.5/agixt/Embedding.py` & `agixt-1.2.6/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/Extensions.py` & `agixt-1.2.6/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/Interactions.py` & `agixt-1.2.6/agixt/Interactions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/Memories.py` & `agixt-1.2.6/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/Prompts.py` & `agixt-1.2.6/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/app.py` & `agixt-1.2.6/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/chains/Smart Chat.json` & `agixt-1.2.6/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/chains/Smart Instruct.json` & `agixt-1.2.6/agixt/chains/Smart Instruct.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/chains/Task.json` & `agixt-1.2.6/agixt/chains/Task.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/chains/Test_Commands.json` & `agixt-1.2.6/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/chains/Write a Poem.json` & `agixt-1.2.6/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/example.ipynb` & `agixt-1.2.6/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/agixt_agent.py` & `agixt-1.2.6/agixt/extensions/agixt_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,12 +222,12 @@
             raw_image = Image.open(requests.get(image_url, stream=True).raw).convert(
                 "RGB"
             )
 
             # Generate a caption for the image using FuseCap
             text = "a picture of "
             inputs = processor(raw_image, text, return_tensors="pt").to(device)
-            out = model.generate(**inputs, num_beams=3)
+            out = model.generate(max_length=20, temperature=0.7, **inputs, num_beams=3)
             caption = processor.decode(out[0], skip_special_tokens=True)
 
             # Return the caption
             return caption
```

### Comparing `agixt-1.2.5/agixt/extensions/briantts.py` & `agixt-1.2.6/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/dalle.py` & `agixt-1.2.6/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/discord.py` & `agixt-1.2.6/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/elevenlabs.py` & `agixt-1.2.6/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/file_system.py` & `agixt-1.2.6/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/github.py` & `agixt-1.2.6/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/google.py` & `agixt-1.2.6/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/gtts.py` & `agixt-1.2.6/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/huggingface.py` & `agixt-1.2.6/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/macostts.py` & `agixt-1.2.6/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/microsoft_365.py` & `agixt-1.2.6/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/searxng.py` & `agixt-1.2.6/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/sendgrid_email.py` & `agixt-1.2.6/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/twitter.py` & `agixt-1.2.6/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/extensions/web_playwright.py` & `agixt-1.2.6/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/Create New Command.txt` & `agixt-1.2.6/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/Execution.txt` & `agixt-1.2.6/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/Instruction.txt` & `agixt-1.2.6/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.6/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.6/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/Task Execution.txt` & `agixt-1.2.6/agixt/prompts/Task Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.6/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.6/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.6/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/instruct.txt` & `agixt-1.2.6/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.6/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.6/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/__init__.py` & `agixt-1.2.6/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/azure.py` & `agixt-1.2.6/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/bing.py` & `agixt-1.2.6/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/chatgpt.py` & `agixt-1.2.6/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/claude.py` & `agixt-1.2.6/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/fastchat.py` & `agixt-1.2.6/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/gpt4all.py` & `agixt-1.2.6/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/gpt4free.py` & `agixt-1.2.6/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/gpugpt4all.py` & `agixt-1.2.6/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/huggingchat.py` & `agixt-1.2.6/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/huggingface.py` & `agixt-1.2.6/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/kobold.py` & `agixt-1.2.6/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/llamacpp.py` & `agixt-1.2.6/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/llamacppapi.py` & `agixt-1.2.6/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/oobabooga.py` & `agixt-1.2.6/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/openai.py` & `agixt-1.2.6/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/palm.py` & `agixt-1.2.6/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/runpod.py` & `agixt-1.2.6/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt/provider/transformer.py` & `agixt-1.2.6/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/agixt.egg-info/PKG-INFO` & `agixt-1.2.6/agixt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.5
+Version: 1.2.6
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.5/agixt.egg-info/SOURCES.txt` & `agixt-1.2.6/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/1-Getting started/Quick Start.md` & `agixt-1.2.6/docs/1-Getting started/Quick Start.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/1-Getting started/Screenshots.md` & `agixt-1.2.6/docs/1-Getting started/Screenshots.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/1-Getting started/Support.md` & `agixt-1.2.6/docs/1-Getting started/Support.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/0-Core Concepts.md` & `agixt-1.2.6/docs/2-Concepts/0-Core Concepts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Agents.md` & `agixt-1.2.6/docs/2-Concepts/Agents.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Chains.md` & `agixt-1.2.6/docs/2-Concepts/Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Chat.md` & `agixt-1.2.6/docs/2-Concepts/Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Commands.md` & `agixt-1.2.6/docs/2-Concepts/Commands.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Instructions.md` & `agixt-1.2.6/docs/2-Concepts/Instructions.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Prompts.md` & `agixt-1.2.6/docs/2-Concepts/Prompts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Smart Chat.md` & `agixt-1.2.6/docs/2-Concepts/Smart Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Smart Instruct.md` & `agixt-1.2.6/docs/2-Concepts/Smart Instruct.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/2-Concepts/Smart Task.md` & `agixt-1.2.6/docs/2-Concepts/Smart Task.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/Anthropic Claude.md` & `agixt-1.2.6/docs/3-Providers/Anthropic Claude.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/Azure OpenAI.md` & `agixt-1.2.6/docs/3-Providers/Azure OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/ChatGPT.md` & `agixt-1.2.6/docs/3-Providers/ChatGPT.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/FastChat.md` & `agixt-1.2.6/docs/3-Providers/FastChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/GPT4ALL-GPU.md` & `agixt-1.2.6/docs/3-Providers/GPT4ALL-GPU.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/GPT4ALL.md` & `agixt-1.2.6/docs/3-Providers/GPT4ALL.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/GPT4Free.md` & `agixt-1.2.6/docs/3-Providers/GPT4Free.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/Google Bard.md` & `agixt-1.2.6/docs/3-Providers/Google Bard.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/Hugging Face Transformers.md` & `agixt-1.2.6/docs/3-Providers/Hugging Face Transformers.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/HuggingChat.md` & `agixt-1.2.6/docs/3-Providers/HuggingChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/Microsoft Bing.md` & `agixt-1.2.6/docs/3-Providers/Microsoft Bing.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/Oobabooga Text Generation Web UI.md` & `agixt-1.2.6/docs/3-Providers/Oobabooga Text Generation Web UI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/OpenAI.md` & `agixt-1.2.6/docs/3-Providers/OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/llamacpp API.md` & `agixt-1.2.6/docs/3-Providers/llamacpp API.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/3-Providers/llamacpp.md` & `agixt-1.2.6/docs/3-Providers/llamacpp.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/README.md` & `agixt-1.2.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/AGiXT-gradient-flat.svg` & `agixt-1.2.6/docs/images/AGiXT-gradient-flat.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/AGiXT-gradient-light.svg` & `agixt-1.2.6/docs/images/AGiXT-gradient-light.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/AGiXT.png` & `agixt-1.2.6/docs/images/AGiXT.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/AGiXT.svg` & `agixt-1.2.6/docs/images/AGiXT.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/AGiXT_Original_PSD.psd` & `agixt-1.2.6/docs/images/AGiXT_Original_PSD.psd`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/AGiXTwhiteborder.svg` & `agixt-1.2.6/docs/images/AGiXTwhiteborder.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/Docker-desktop-win-setting-streamlit.png` & `agixt-1.2.6/docs/images/Docker-desktop-win-setting-streamlit.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/Smart Instruct.drawio` & `agixt-1.2.6/docs/images/Smart Instruct.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/Smart Instruct.drawio.svg` & `agixt-1.2.6/docs/images/Smart Instruct.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/Smart Tasks.drawio` & `agixt-1.2.6/docs/images/Smart Tasks.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/Smart Tasks.drawio.svg` & `agixt-1.2.6/docs/images/Smart Tasks.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/docs/images/Untitled Diagram.drawio` & `agixt-1.2.6/docs/images/Untitled Diagram.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/setup.py` & `agixt-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/ApiClient.py` & `agixt-1.2.6/streamlit/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/Main.py` & `agixt-1.2.6/streamlit/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/auth_libs/Cfig.py` & `agixt-1.2.6/streamlit/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/auth_libs/Redirect.py` & `agixt-1.2.6/streamlit/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/auth_libs/Users.py` & `agixt-1.2.6/streamlit/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/auth_libs/pages/Login.py` & `agixt-1.2.6/streamlit/auth_libs/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/auth_libs/pages/Profile.py` & `agixt-1.2.6/streamlit/auth_libs/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/auth_libs/pages/Register.py` & `agixt-1.2.6/streamlit/auth_libs/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/components/chain.py` & `agixt-1.2.6/streamlit/components/chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/components/docs.py` & `agixt-1.2.6/streamlit/components/docs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/components/history.py` & `agixt-1.2.6/streamlit/components/history.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/components/learning.py` & `agixt-1.2.6/streamlit/components/learning.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/components/selectors.py` & `agixt-1.2.6/streamlit/components/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     )
 
     if prompt_name:
         prompt_args = ApiClient.get_prompt_args(prompt_name)
         args = build_args(args=prompt_args, prompt=prompt, step_number=step_number)
         new_prompt = {
             "prompt_name": prompt_name,
-            "prompt_args": args,
+            **args,
         }
         return new_prompt
 
 
 def command_selection(prompt: dict = {}, step_number: int = 0):
     agent_commands = cached_get_extensions()
     available_commands = [cmd[0] for cmd in agent_commands]
@@ -51,15 +51,15 @@
     )
 
     if command_name:
         command_args = ApiClient.get_command_args(command_name=command_name)
         args = build_args(args=command_args, prompt=prompt, step_number=step_number)
         new_prompt = {
             "command_name": command_name,
-            "command_args": args,
+            **args,
         }
         return new_prompt
 
 
 def chain_selection(prompt: dict = {}, step_number: int = 0):
     available_chains = ApiClient.get_chains()
     chain_name = st.selectbox(
```

### Comparing `agixt-1.2.5/streamlit/components/verify_backend.py` & `agixt-1.2.6/streamlit/components/verify_backend.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/pages/0-Agent_Settings.py` & `agixt-1.2.6/streamlit/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/pages/1-Prompt_Templates.py` & `agixt-1.2.6/streamlit/pages/1-Prompt_Templates.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/pages/2-Chain_Management.py` & `agixt-1.2.6/streamlit/pages/2-Chain_Management.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/streamlit/pages/3-Interact.py` & `agixt-1.2.6/streamlit/pages/3-Interact.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/tests/ApiClient.py` & `agixt-1.2.6/tests/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/tests/test-commands.ipynb` & `agixt-1.2.6/tests/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.5/tests/tests.ipynb` & `agixt-1.2.6/tests/tests.ipynb`

 * *Files identical despite different names*

