# Comparing `tmp/agixt-1.2.4.tar.gz` & `tmp/agixt-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.4.tar", last modified: Sun Jun 11 19:07:29 2023, max compression
+gzip compressed data, was "agixt-1.2.5.tar", last modified: Mon Jun 12 03:39:16 2023, max compression
```

## Comparing `agixt-1.2.4.tar` & `agixt-1.2.5.tar`

### file list

```diff
@@ -1,199 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.769282 agixt-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-11 19:07:16.000000 agixt-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 19:07:16.000000 agixt-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 19:07:29.769282 agixt-1.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt/WORKSPACE/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/WORKSPACE/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.745283 agixt-1.2.4/agixt/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt/agents/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/agents/gpt4free/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Smart Chat.json
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Smart Instruct.json
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Task.json
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Test_Commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Write a Poem.json
--rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.753283 agixt-1.2.4/agixt/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/agixt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/briantts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/dalle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/gtts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/macostts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/microsoft_365.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/searxng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/sendgrid_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/web_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Chat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Create New Command.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Custom Input.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Get Task List.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Prioritize.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Score Response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Task Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Tell Me How.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Title a Poem.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Validation.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/WebSearch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Write a Poem.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/gpt-3.5-turbo/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/gpt-3.5-turbo/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/gpt-4/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/starchat/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/starchat/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/vicuna/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/vicuna/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/runpod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/docs/1-Getting started/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/1-Getting started/Quick Start.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/1-Getting started/Support.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.761283 agixt-1.2.4/docs/2-Concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/0-Core Concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Prompts.md
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Providers.md
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Smart Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Smart Instruct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Smart Task.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Tasks.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.761283 agixt-1.2.4/docs/3-Providers/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Anthropic Claude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Azure OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/ChatGPT.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/FastChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/GPT4ALL-GPU.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/GPT4ALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/GPT4Free.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Google Bard.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Google Palm.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Hugging Face Transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/HuggingChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Kobold.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Microsoft Bing.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Oobabooga Text Generation Web UI.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/llamacpp API.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/llamacpp.md
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT-gradient-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT-gradient-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT.png
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT_Original_PSD.psd
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXTwhiteborder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Docker-desktop-win-setting-streamlit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Smart Instruct.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Smart Instruct.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Smart Tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Smart Tasks.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Untitled Diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 19:07:16.000000 agixt-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-11 19:07:16.000000 agixt-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:07:29.769282 agixt-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-11 19:07:16.000000 agixt-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/streamlit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/streamlit/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/Main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/streamlit/auth_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/Cfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/Redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/Users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/streamlit/auth_libs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/pages/Login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/pages/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/pages/Register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.769282 agixt-1.2.4/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/verify_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.769282 agixt-1.2.4/streamlit/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/pages/0-Agent_Settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/pages/1-Prompt_Templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/pages/2-Chain_Management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/pages/3-Interact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.769282 agixt-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-11 19:07:16.000000 agixt-1.2.4/tests/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-11 19:07:16.000000 agixt-1.2.4/tests/test-commands.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-06-11 19:07:16.000000 agixt-1.2.4/tests/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 03:39:03.000000 agixt-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 03:39:03.000000 agixt-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 03:39:16.415971 agixt-1.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.391970 agixt-1.2.5/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.395970 agixt-1.2.5/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.387970 agixt-1.2.5/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.395970 agixt-1.2.5/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.395970 agixt-1.2.5/agixt/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Smart Chat.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Smart Instruct.json
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Task.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Test_Commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/chains/Write a Poem.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.395970 agixt-1.2.5/agixt/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/agixt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/briantts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/gtts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/macostts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/microsoft_365.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/searxng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/extensions/web_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Chat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Create New Command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Custom Input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Get Task List.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Prioritize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Score Response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Task Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Validation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/WebSearch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/Write a Poem.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/gpt-3.5-turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/gpt-3.5-turbo/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/gpt-4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/starchat/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/starchat/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.399971 agixt-1.2.5/agixt/prompts/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/prompts/vicuna/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.403971 agixt-1.2.5/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 03:39:03.000000 agixt-1.2.5/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.391970 agixt-1.2.5/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 03:39:16.000000 agixt-1.2.5/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.403971 agixt-1.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.403971 agixt-1.2.5/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/1-Getting started/Screenshots.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.407971 agixt-1.2.5/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Smart Task.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/2-Concepts/Tasks.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.407971 agixt-1.2.5/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.411971 agixt-1.2.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 03:39:03.000000 agixt-1.2.5/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 03:39:03.000000 agixt-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 03:39:03.000000 agixt-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:39:16.415971 agixt-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-12 03:39:03.000000 agixt-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.411971 agixt-1.2.5/streamlit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.411971 agixt-1.2.5/streamlit/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/Main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.411971 agixt-1.2.5/streamlit/auth_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/Cfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/Redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/Users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/streamlit/auth_libs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/pages/Login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/pages/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/auth_libs/pages/Register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/components/verify_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/streamlit/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/pages/0-Agent_Settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/pages/1-Prompt_Templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/pages/2-Chain_Management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-12 03:39:03.000000 agixt-1.2.5/streamlit/pages/3-Interact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:39:16.415971 agixt-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-12 03:39:03.000000 agixt-1.2.5/tests/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-12 03:39:03.000000 agixt-1.2.5/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-06-12 03:39:03.000000 agixt-1.2.5/tests/tests.ipynb
```

### Comparing `agixt-1.2.4/LICENSE` & `agixt-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/PKG-INFO` & `agixt-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.4
+Version: 1.2.5
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AGiXT
 [![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
-![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
-
-[![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
-[![GitHub](https://img.shields.io/badge/GitHub-NextJS_Front_End-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
-
+![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html) [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
 [![Logo](images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
```

### Comparing `agixt-1.2.4/agixt/Agent.py` & `agixt-1.2.5/agixt/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     "embedder": "default",
 }
 
 
 def get_agent_file_paths(agent_name):
     base_path = os.path.join(os.getcwd(), "agents")
     folder_path = os.path.normpath(os.path.join(base_path, agent_name))
-    config_path = os.path.normpath(os.path.join(base_path, "config.json"))
-    history_path = os.path.normpath(os.path.join(base_path, "history.yaml"))
+    config_path = os.path.normpath(os.path.join(folder_path, "config.json"))
+    history_path = os.path.normpath(os.path.join(folder_path, "history.yaml"))
     if not config_path.startswith(base_path) or not folder_path.startswith(base_path):
         raise ValueError("Invalid path, agent name must not contain slashes.")
     if not os.path.exists(folder_path):
         os.mkdir(folder_path)
     return config_path, history_path, folder_path
```

### Comparing `agixt-1.2.4/agixt/Chain.py` & `agixt-1.2.5/agixt/Chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,19 +246,21 @@
                     prompt_name = ""
                 args = self.get_step_content(
                     chain_name=chain_name,
                     prompt_content=step["prompt"],
                     user_input=user_input,
                     agent_name=agent_name,
                 )
+                print(f"ARGS: {args}")
                 if prompt_type == "Command":
                     return await Extensions(
                         agent_config=agent.agent.agent_config
                     ).execute_command(
-                        command_name=args["command_name"], command_args=args
+                        command_name=args["command_name"],
+                        command_args=args["command_args"],
                     )
                 elif prompt_type == "Prompt":
                     result = await agent.run(
                         user_input=user_input,
                         prompt=prompt_name,
                         chain_name=chain_name,
                         step_number=step_number,
```

### Comparing `agixt-1.2.4/agixt/Embedding.py` & `agixt-1.2.5/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/Extensions.py` & `agixt-1.2.5/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/Interactions.py` & `agixt-1.2.5/agixt/Interactions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/Memories.py` & `agixt-1.2.5/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/Prompts.py` & `agixt-1.2.5/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/app.py` & `agixt-1.2.5/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/chains/Smart Chat.json` & `agixt-1.2.5/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/chains/Smart Instruct.json` & `agixt-1.2.5/agixt/chains/Smart Instruct.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/chains/Task.json` & `agixt-1.2.5/agixt/chains/Task.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/chains/Test_Commands.json` & `agixt-1.2.5/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/chains/Write a Poem.json` & `agixt-1.2.5/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/example.ipynb` & `agixt-1.2.5/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/agixt_agent.py` & `agixt-1.2.5/agixt/extensions/agixt_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from Extensions import Extensions
 from Agent import get_agents
 from Chain import Chain
 from Interactions import Interactions
 import json
 import os
 from typing import List, Optional
+from transformers import BlipProcessor, BlipForConditionalGeneration
+import torch
+from PIL import Image
+import requests
 
 
 class agixt_agent(Extensions):
     def __init__(self, **kwargs):
         agents = get_agents()
         self.chains = Chain().get_chains()
         self.commands = {
@@ -17,14 +21,15 @@
             "Perform Automated Testing": self.perform_automated_testing,
             "Run CI-CD Pipeline": self.run_ci_cd_pipeline,
             "Improve Code": self.improve_code,
             "Write Tests": self.write_tests,
             "Create a new command": self.create_command,
             "Execute Task List": self.execute_task_list,
             "Prompt AI Agent": self.prompt_agent,
+            "Describe Image": self.describe_image,
         }
         if agents != None:
             for agent in agents:
                 if "name" in agent:
                     name = f" AI Agent {agent['name']}"
                     self.commands.update(
                         {
@@ -130,39 +135,40 @@
     async def instruct(self, user_input: str, agent: str = "AGiXT") -> str:
         response = await Interactions(agent_name=agent).run(
             user_input=user_input, prompt="instruct", websearch=True, websearch_depth=8
         )
         return response
 
     async def prompt_agent(
-        agent: str,
-        user_input: str,
-        prompt_name: int,
-        prompt_args: dict,
+        self,
+        agent: str = "gpt4free",
+        user_input: str = "",
+        prompt_name: str = "",
+        prompt_args: dict = {},
         websearch: bool = False,
         websearch_depth: int = 3,
         context_results: int = 5,
         shots: int = 1,
     ) -> str:
         response = await Interactions(agent_name=agent).run(
             user_input=user_input,
             prompt=prompt_name,
-            prompt_args=prompt_args,
             websearch=websearch,
             websearch_depth=websearch_depth,
             context_results=context_results,
+            **prompt_args,
         )
         if shots > 1:
             responses = [response]
             for shot in range(shots - 1):
                 response = await Interactions(agent_name=agent).run(
                     user_input=user_input,
                     prompt=prompt_name,
-                    prompt_args=prompt_args,
                     context_results=context_results,
+                    **prompt_args,
                 )
                 responses.append(response)
             # Join responses by "Response # <shot number>:" and return
             return "\n".join(
                 [
                     f"Response {shot + 1}:\n{response}"
                     for shot, response in enumerate(responses)
@@ -196,7 +202,32 @@
                     },
                     websearch=websearch,
                     websearch_depth=websearch_depth,
                     context_results=context_results,
                 )
                 responses.append(response)
         return "\n".join(responses)
+
+    async def describe_image(self, image_url):
+        """
+        Describe an image using FuseCap.
+        """
+        if image_url:
+            processor = BlipProcessor.from_pretrained("noamrot/FuseCap")
+            model = BlipForConditionalGeneration.from_pretrained("noamrot/FuseCap")
+
+            # Define the device to run the model on (CPU or GPU)
+
+            device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+            model.to(device)
+            raw_image = Image.open(requests.get(image_url, stream=True).raw).convert(
+                "RGB"
+            )
+
+            # Generate a caption for the image using FuseCap
+            text = "a picture of "
+            inputs = processor(raw_image, text, return_tensors="pt").to(device)
+            out = model.generate(**inputs, num_beams=3)
+            caption = processor.decode(out[0], skip_special_tokens=True)
+
+            # Return the caption
+            return caption
```

### Comparing `agixt-1.2.4/agixt/extensions/briantts.py` & `agixt-1.2.5/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/dalle.py` & `agixt-1.2.5/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/discord.py` & `agixt-1.2.5/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/elevenlabs.py` & `agixt-1.2.5/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/file_system.py` & `agixt-1.2.5/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/github.py` & `agixt-1.2.5/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/google.py` & `agixt-1.2.5/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/gtts.py` & `agixt-1.2.5/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/huggingface.py` & `agixt-1.2.5/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/macostts.py` & `agixt-1.2.5/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/microsoft_365.py` & `agixt-1.2.5/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/searxng.py` & `agixt-1.2.5/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/sendgrid_email.py` & `agixt-1.2.5/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/twitter.py` & `agixt-1.2.5/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/extensions/web_playwright.py` & `agixt-1.2.5/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/Create New Command.txt` & `agixt-1.2.5/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/Execution.txt` & `agixt-1.2.5/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/Instruction.txt` & `agixt-1.2.5/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.5/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.5/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/Task Execution.txt` & `agixt-1.2.5/agixt/prompts/Task Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.5/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.5/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.5/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/instruct.txt` & `agixt-1.2.5/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.5/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.5/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/__init__.py` & `agixt-1.2.5/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/azure.py` & `agixt-1.2.5/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/bing.py` & `agixt-1.2.5/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/chatgpt.py` & `agixt-1.2.5/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/claude.py` & `agixt-1.2.5/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/fastchat.py` & `agixt-1.2.5/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/gpt4all.py` & `agixt-1.2.5/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/gpt4free.py` & `agixt-1.2.5/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/gpugpt4all.py` & `agixt-1.2.5/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/huggingchat.py` & `agixt-1.2.5/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/huggingface.py` & `agixt-1.2.5/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/kobold.py` & `agixt-1.2.5/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/llamacpp.py` & `agixt-1.2.5/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/llamacppapi.py` & `agixt-1.2.5/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/oobabooga.py` & `agixt-1.2.5/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/openai.py` & `agixt-1.2.5/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/palm.py` & `agixt-1.2.5/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/runpod.py` & `agixt-1.2.5/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt/provider/transformer.py` & `agixt-1.2.5/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/agixt.egg-info/PKG-INFO` & `agixt-1.2.5/agixt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.4
+Version: 1.2.5
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AGiXT
 [![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
-![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
-
-[![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
-[![GitHub](https://img.shields.io/badge/GitHub-NextJS_Front_End-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
-
+![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html) [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
 [![Logo](images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
```

### Comparing `agixt-1.2.4/agixt.egg-info/SOURCES.txt` & `agixt-1.2.5/agixt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 agixt/provider/openai.py
 agixt/provider/palm.py
 agixt/provider/runpod.py
 agixt/provider/transformer.py
 docs/.gitignore
 docs/README.md
 docs/1-Getting started/Quick Start.md
+docs/1-Getting started/Screenshots.md
 docs/1-Getting started/Support.md
 docs/2-Concepts/0-Core Concepts.md
 docs/2-Concepts/Agents.md
 docs/2-Concepts/Chains.md
 docs/2-Concepts/Chat.md
 docs/2-Concepts/Commands.md
 docs/2-Concepts/Instructions.md
```

### Comparing `agixt-1.2.4/docs/1-Getting started/Quick Start.md` & `agixt-1.2.5/docs/1-Getting started/Quick Start.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/1-Getting started/Support.md` & `agixt-1.2.5/docs/1-Getting started/Support.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/0-Core Concepts.md` & `agixt-1.2.5/docs/2-Concepts/0-Core Concepts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Agents.md` & `agixt-1.2.5/docs/2-Concepts/Agents.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Chains.md` & `agixt-1.2.5/docs/2-Concepts/Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Chat.md` & `agixt-1.2.5/docs/2-Concepts/Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Commands.md` & `agixt-1.2.5/docs/2-Concepts/Commands.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Instructions.md` & `agixt-1.2.5/docs/2-Concepts/Instructions.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Prompts.md` & `agixt-1.2.5/docs/2-Concepts/Prompts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Smart Chat.md` & `agixt-1.2.5/docs/2-Concepts/Smart Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Smart Instruct.md` & `agixt-1.2.5/docs/2-Concepts/Smart Instruct.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/2-Concepts/Smart Task.md` & `agixt-1.2.5/docs/2-Concepts/Smart Task.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/Anthropic Claude.md` & `agixt-1.2.5/docs/3-Providers/Anthropic Claude.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/Azure OpenAI.md` & `agixt-1.2.5/docs/3-Providers/Azure OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/ChatGPT.md` & `agixt-1.2.5/docs/3-Providers/ChatGPT.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/FastChat.md` & `agixt-1.2.5/docs/3-Providers/FastChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/GPT4ALL-GPU.md` & `agixt-1.2.5/docs/3-Providers/GPT4ALL-GPU.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/GPT4ALL.md` & `agixt-1.2.5/docs/3-Providers/GPT4ALL.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/GPT4Free.md` & `agixt-1.2.5/docs/3-Providers/GPT4Free.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/Google Bard.md` & `agixt-1.2.5/docs/3-Providers/Google Bard.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/Hugging Face Transformers.md` & `agixt-1.2.5/docs/3-Providers/Hugging Face Transformers.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/HuggingChat.md` & `agixt-1.2.5/docs/3-Providers/HuggingChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/Microsoft Bing.md` & `agixt-1.2.5/docs/3-Providers/Microsoft Bing.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/Oobabooga Text Generation Web UI.md` & `agixt-1.2.5/docs/3-Providers/Oobabooga Text Generation Web UI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/OpenAI.md` & `agixt-1.2.5/docs/3-Providers/OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/llamacpp API.md` & `agixt-1.2.5/docs/3-Providers/llamacpp API.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/3-Providers/llamacpp.md` & `agixt-1.2.5/docs/3-Providers/llamacpp.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/README.md` & `agixt-1.2.5/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # AGiXT
 [![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
-![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
-
-[![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
-[![GitHub](https://img.shields.io/badge/GitHub-NextJS_Front_End-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
-
+![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html) [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
 [![Logo](images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
```

### Comparing `agixt-1.2.4/docs/images/AGiXT-gradient-flat.svg` & `agixt-1.2.5/docs/images/AGiXT-gradient-flat.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/AGiXT-gradient-light.svg` & `agixt-1.2.5/docs/images/AGiXT-gradient-light.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/AGiXT.png` & `agixt-1.2.5/docs/images/AGiXT.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/AGiXT.svg` & `agixt-1.2.5/docs/images/AGiXT.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/AGiXT_Original_PSD.psd` & `agixt-1.2.5/docs/images/AGiXT_Original_PSD.psd`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/AGiXTwhiteborder.svg` & `agixt-1.2.5/docs/images/AGiXTwhiteborder.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/Docker-desktop-win-setting-streamlit.png` & `agixt-1.2.5/docs/images/Docker-desktop-win-setting-streamlit.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/Smart Instruct.drawio` & `agixt-1.2.5/docs/images/Smart Instruct.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/Smart Instruct.drawio.svg` & `agixt-1.2.5/docs/images/Smart Instruct.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/Smart Tasks.drawio` & `agixt-1.2.5/docs/images/Smart Tasks.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/Smart Tasks.drawio.svg` & `agixt-1.2.5/docs/images/Smart Tasks.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/docs/images/Untitled Diagram.drawio` & `agixt-1.2.5/docs/images/Untitled Diagram.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/setup.py` & `agixt-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/ApiClient.py` & `agixt-1.2.5/streamlit/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/Main.py` & `agixt-1.2.5/streamlit/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/auth_libs/Cfig.py` & `agixt-1.2.5/streamlit/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/auth_libs/Redirect.py` & `agixt-1.2.5/streamlit/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/auth_libs/Users.py` & `agixt-1.2.5/streamlit/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/auth_libs/pages/Login.py` & `agixt-1.2.5/streamlit/auth_libs/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/auth_libs/pages/Profile.py` & `agixt-1.2.5/streamlit/auth_libs/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/auth_libs/pages/Register.py` & `agixt-1.2.5/streamlit/auth_libs/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/components/chain.py` & `agixt-1.2.5/streamlit/components/chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/components/docs.py` & `agixt-1.2.5/streamlit/components/docs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/components/history.py` & `agixt-1.2.5/streamlit/components/history.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/components/learning.py` & `agixt-1.2.5/streamlit/components/learning.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/components/selectors.py` & `agixt-1.2.5/streamlit/components/selectors.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/components/verify_backend.py` & `agixt-1.2.5/streamlit/components/verify_backend.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/pages/0-Agent_Settings.py` & `agixt-1.2.5/streamlit/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/pages/1-Prompt_Templates.py` & `agixt-1.2.5/streamlit/pages/1-Prompt_Templates.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/pages/2-Chain_Management.py` & `agixt-1.2.5/streamlit/pages/2-Chain_Management.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/streamlit/pages/3-Interact.py` & `agixt-1.2.5/streamlit/pages/3-Interact.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/tests/ApiClient.py` & `agixt-1.2.5/tests/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/tests/test-commands.ipynb` & `agixt-1.2.5/tests/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.4/tests/tests.ipynb` & `agixt-1.2.5/tests/tests.ipynb`

 * *Files identical despite different names*

