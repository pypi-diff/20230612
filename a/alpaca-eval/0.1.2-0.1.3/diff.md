# Comparing `tmp/alpaca_eval-0.1.2.tar.gz` & `tmp/alpaca_eval-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.1.2.tar", last modified: Thu Jun  8 19:04:08 2023, max compression
+gzip compressed data, was "alpaca_eval-0.1.3.tar", last modified: Sun Jun 11 23:01:49 2023, max compression
```

## Comparing `alpaca_eval-0.1.2.tar` & `alpaca_eval-0.1.3.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.548826 alpaca_eval-0.1.2/
--rw-r--r--   0 xuechenli   (501) staff       (20)    11409 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/LICENSE
--rw-r--r--   0 xuechenli   (501) staff       (20)      187 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/MANIFEST.in
--rw-r--r--   0 xuechenli   (501) staff       (20)    64291 2023-06-08 19:04:08.548657 alpaca_eval-0.1.2/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)    63472 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/README.md
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.527830 alpaca_eval-0.1.2/example/
--rw-r--r--   0 xuechenli   (501) staff       (20)   517613 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/example/outputs.json
--rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-08 19:04:08.548866 alpaca_eval-0.1.2/setup.cfg
--rw-r--r--   0 xuechenli   (501) staff       (20)     2121 2023-06-08 19:03:04.000000 alpaca_eval-0.1.2/setup.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.522109 alpaca_eval-0.1.2/src/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.530988 alpaca_eval-0.1.2/src/alpaca_eval/
--rw-r--r--   0 xuechenli   (501) staff       (20)       22 2023-06-08 19:03:26.000000 alpaca_eval-0.1.2/src/alpaca_eval/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    20821 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.532604 alpaca_eval-0.1.2/src/alpaca_eval/annotators/
--rw-r--r--   0 xuechenli   (501) staff       (20)       33 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    31305 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3939 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     5218 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/constants.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.533859 alpaca_eval-0.1.2/src/alpaca_eval/decoders/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1913 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4730 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2835 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3905 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4697 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11804 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/openai.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.534034 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 xuechenli   (501) staff       (20)     9670 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.534401 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1204 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      270 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.536911 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1650 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6045 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.537309 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      362 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.537736 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1048 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      324 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.538138 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1116 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      325 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.538520 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1137 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      317 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.538839 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 xuechenli   (501) staff       (20)      259 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1087 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.538996 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 xuechenli   (501) staff       (20)      303 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.539162 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      314 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.539585 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1298 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      452 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.539803 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      322 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.539973 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      317 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.540304 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      319 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1051 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.540749 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1054 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      367 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.541230 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1017 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      341 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.523858 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.541764 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1739 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 xuechenli   (501) staff       (20)     1744 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 xuechenli   (501) staff       (20)      351 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.541930 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 xuechenli   (501) staff       (20)     2577 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/main.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1313 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.526550 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.542286 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      382 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      152 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.542490 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 xuechenli   (501) staff       (20)      433 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.542737 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 xuechenli   (501) staff       (20)      456 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.542921 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 xuechenli   (501) staff       (20)      196 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.543229 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 xuechenli   (501) staff       (20)      184 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)       34 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.543391 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 xuechenli   (501) staff       (20)      188 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/cohere/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.543556 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 xuechenli   (501) staff       (20)      405 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.543748 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 xuechenli   (501) staff       (20)      401 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.544107 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      100 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      178 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.544315 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.544510 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.544677 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.545038 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      425 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      195 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.545350 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      407 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.545498 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      449 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.545831 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      436 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)       42 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.546158 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      458 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)       51 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.546319 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 xuechenli   (501) staff       (20)      438 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.546505 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 xuechenli   (501) staff       (20)      211 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.546820 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 xuechenli   (501) staff       (20)      211 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)       34 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.547230 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      387 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.547673 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      383 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.548101 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      394 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)    22484 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/plotting.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      283 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/types.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    15488 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.532243 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/
--rw-r--r--   0 xuechenli   (501) staff       (20)    64291 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     5723 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       54 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      418 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.576854 alpaca_eval-0.1.3/
+-rw-r--r--   0 rtaori     (501) staff       (20)    11409 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/LICENSE
+-rw-r--r--   0 rtaori     (501) staff       (20)      187 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/MANIFEST.in
+-rw-r--r--   0 rtaori     (501) staff       (20)    64419 2023-06-11 23:01:49.576688 alpaca_eval-0.1.3/PKG-INFO
+-rw-r--r--   0 rtaori     (501) staff       (20)    63598 2023-06-11 22:46:48.000000 alpaca_eval-0.1.3/README.md
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.559123 alpaca_eval-0.1.3/example/
+-rw-r--r--   0 rtaori     (501) staff       (20)   517613 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/example/outputs.json
+-rw-r--r--   0 rtaori     (501) staff       (20)       38 2023-06-11 23:01:49.576893 alpaca_eval-0.1.3/setup.cfg
+-rw-r--r--   0 rtaori     (501) staff       (20)     2123 2023-06-11 22:46:22.000000 alpaca_eval-0.1.3/setup.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.555032 alpaca_eval-0.1.3/src/
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.561843 alpaca_eval-0.1.3/src/alpaca_eval/
+-rw-r--r--   0 rtaori     (501) staff       (20)       22 2023-06-11 22:58:03.000000 alpaca_eval-0.1.3/src/alpaca_eval/__init__.py
+-rw-r--r--   0 rtaori     (501) staff       (20)    20821 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.563197 alpaca_eval-0.1.3/src/alpaca_eval/annotators/
+-rw-r--r--   0 rtaori     (501) staff       (20)       33 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 rtaori     (501) staff       (20)    31305 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     3939 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     5218 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/constants.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.564312 alpaca_eval-0.1.3/src/alpaca_eval/decoders/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1913 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     4730 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     2835 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     3905 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     4697 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 rtaori     (501) staff       (20)    11804 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/decoders/openai.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.564494 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 rtaori     (501) staff       (20)     9670 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.564813 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1204 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      270 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.567347 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1650 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     5869 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     2475 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     3721 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     3423 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     6849 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     6797 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     6700 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     6045 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)     1016 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     3969 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     5932 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     5370 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.567677 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)     7373 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      362 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.567971 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1048 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      324 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.568278 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1116 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      325 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.568584 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1137 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      317 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.568933 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 rtaori     (501) staff       (20)      259 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)     1087 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569140 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 rtaori     (501) staff       (20)      303 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569320 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      314 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569624 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1298 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      452 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569774 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      322 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.569931 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      317 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.570250 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      319 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)     1051 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.570563 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1054 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      367 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.570884 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1017 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      341 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.556446 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.571338 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1739 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 rtaori     (501) staff       (20)     1744 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 rtaori     (501) staff       (20)      351 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.571494 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 rtaori     (501) staff       (20)     2577 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 rtaori     (501) staff       (20)    21692 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/main.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     1313 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.558209 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.571817 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      382 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      152 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.571964 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 rtaori     (501) staff       (20)      433 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572117 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 rtaori     (501) staff       (20)      456 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572266 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 rtaori     (501) staff       (20)      196 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572528 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 rtaori     (501) staff       (20)      184 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       34 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572673 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 rtaori     (501) staff       (20)      188 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/cohere/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572811 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 rtaori     (501) staff       (20)      405 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.572951 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 rtaori     (501) staff       (20)      401 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573228 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      100 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      178 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573391 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573528 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573657 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.573968 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      425 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      195 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.574255 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      407 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.574385 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      449 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.574705 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      436 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       42 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.574978 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      458 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       51 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.575108 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 rtaori     (501) staff       (20)      438 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.575256 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 rtaori     (501) staff       (20)      211 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.575554 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 rtaori     (501) staff       (20)      211 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       34 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.575856 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      387 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.576158 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      383 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.576418 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      394 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)    22484 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/plotting.py
+-rw-r--r--   0 rtaori     (501) staff       (20)      283 2023-06-08 16:33:22.000000 alpaca_eval-0.1.3/src/alpaca_eval/types.py
+-rw-r--r--   0 rtaori     (501) staff       (20)    15488 2023-06-11 22:44:32.000000 alpaca_eval-0.1.3/src/alpaca_eval/utils.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-11 23:01:49.562847 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/
+-rw-r--r--   0 rtaori     (501) staff       (20)    64419 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 rtaori     (501) staff       (20)     5723 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)        1 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)       54 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      418 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)       12 2023-06-11 23:01:49.000000 alpaca_eval-0.1.3/src/alpaca_eval.egg-info/top_level.txt
```

### Comparing `alpaca_eval-0.1.2/LICENSE` & `alpaca_eval-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/PKG-INFO` & `alpaca_eval-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.1.2
+Version: 0.1.3
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: analysis
 Provides-Extra: dev
 Provides-Extra: local
 Provides-Extra: api
 Provides-Extra: all
 License-File: LICENSE
 
 # <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/yKbbQga9WE)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
 Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
 AlpacaEval provides the following:
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.1.2 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.1.3 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.9 Description-Content-Type: text/markdown
+Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Provides-Extra: analysis Provides-Extra: dev Provides-Extra: local Provides-
 Extra: api Provides-Extra: all License-File: LICENSE # [https://
 raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png]
 AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-
 green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data
 License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-
 red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [!
-[Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://
-www.python.org/downloads/release/python-390/) Evaluation of instruction-
-following models (e.g., ChatGPT) typically requires human interactions. This is
-time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based
-automatic evaluation that is fast, cheap, replicable, and validated against 20K
-human annotations. It is particularly useful for model development. Although we
+[Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://
+www.python.org/downloads/release/python-3100/) [![discord](https://
+img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https:/
+/discord.gg/yKbbQga9WE) Evaluation of instruction-following models (e.g.,
+ChatGPT) typically requires human interactions. This is time-consuming,
+expensive, and hard to replicate. AlpacaEval in an LLM-based automatic
+evaluation that is fast, cheap, replicable, and validated against 20K human
+annotations. It is particularly useful for model development. Although we
 improved over prior automatic evaluation pipelines, there are still fundamental
 [limitations](#limitations). AlpacaEval provides the following: - [**Automatic
 evaluator**](#evaluators): an automatic evaluator that has high agreement with
 humans (validated on 20K annotations). We evaluate a model by measuring the
 fraction of times an powerful LLM (e.g. GPT 4 or Claude) prefers the outputs
 from that model over outputs from a reference model. Our evaluators enable
 caching and output randomization by default. - [**Leaderboard**](https://tatsu-
```

### Comparing `alpaca_eval-0.1.2/README.md` & `alpaca_eval-0.1.3/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,36 @@
+Metadata-Version: 2.1
+Name: alpaca-eval
+Version: 0.1.3
+Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
+Author: The Alpaca Team
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: analysis
+Provides-Extra: dev
+Provides-Extra: local
+Provides-Extra: api
+Provides-Extra: all
+License-File: LICENSE
+
 # <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/yKbbQga9WE)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
 Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
 AlpacaEval provides the following:
```

#### html2text {}

```diff
@@ -1,30 +1,42 @@
-# [https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/
-AlpacaFarm_small.png] AlpacaEval : An Automatic Evaluator for Instruction-
-following Language Models [![Code License](https://img.shields.io/badge/
-Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/
-blob/main/LICENSE) [![Data License](https://img.shields.io/badge/
-Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/
-alpaca_farm/blob/main/DATA_LICENSE) [![Python 3.9+](https://img.shields.io/
-badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-
-390/) Evaluation of instruction-following models (e.g., ChatGPT) typically
-requires human interactions. This is time-consuming, expensive, and hard to
-replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
-replicable, and validated against 20K human annotations. It is particularly
-useful for model development. Although we improved over prior automatic
-evaluation pipelines, there are still fundamental [limitations](#limitations).
-AlpacaEval provides the following: - [**Automatic evaluator**](#evaluators): an
-automatic evaluator that has high agreement with humans (validated on 20K
-annotations). We evaluate a model by measuring the fraction of times an
-powerful LLM (e.g. GPT 4 or Claude) prefers the outputs from that model over
-outputs from a reference model. Our evaluators enable caching and output
-randomization by default. - [**Leaderboard**](https://tatsu-lab.github.io/
-alpaca_eval/): a leaderboard of common models on the AlpacaEval evaluation set.
-- [**Toolkit for building automatic evaluators**](#analysis): a simple
-interface for building advanced automatic evaluators (e.g. with caching,
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.1.3 Summary: AlpacaEval : An
+Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Education Classifier: Intended Audience :: Science/Research Classifier: License
+:: OSI Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.10 Description-Content-Type: text/markdown
+Provides-Extra: analysis Provides-Extra: dev Provides-Extra: local Provides-
+Extra: api Provides-Extra: all License-File: LICENSE # [https://
+raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png]
+AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
+[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-
+green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data
+License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-
+red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [!
+[Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://
+www.python.org/downloads/release/python-3100/) [![discord](https://
+img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https:/
+/discord.gg/yKbbQga9WE) Evaluation of instruction-following models (e.g.,
+ChatGPT) typically requires human interactions. This is time-consuming,
+expensive, and hard to replicate. AlpacaEval in an LLM-based automatic
+evaluation that is fast, cheap, replicable, and validated against 20K human
+annotations. It is particularly useful for model development. Although we
+improved over prior automatic evaluation pipelines, there are still fundamental
+[limitations](#limitations). AlpacaEval provides the following: - [**Automatic
+evaluator**](#evaluators): an automatic evaluator that has high agreement with
+humans (validated on 20K annotations). We evaluate a model by measuring the
+fraction of times an powerful LLM (e.g. GPT 4 or Claude) prefers the outputs
+from that model over outputs from a reference model. Our evaluators enable
+caching and output randomization by default. - [**Leaderboard**](https://tatsu-
+lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
+evaluation set. - [**Toolkit for building automatic evaluators**](#analysis): a
+simple interface for building advanced automatic evaluators (e.g. with caching,
 batching, or multi-annotators) and analyzing them (quality, price, speed,
 statistical power, bias, variance etc). - [**Human evaluation data**](#data-
 release): 20K human preferences between a given and reference model on the
 [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
 set. 2.5K of these are cross-annotations (4 humans annotating the same 650
 examples). - [**AlpacaEval dataset**](#data-release): a simplification of
 [AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
```

### Comparing `alpaca_eval-0.1.2/example/outputs.json` & `alpaca_eval-0.1.3/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/setup.py` & `alpaca_eval-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,24 +38,24 @@
     extras_require={
         "analysis": PACKAGES_ANALYSIS,
         "dev": PACKAGES_DEV,
         "local": PACKAGES_LOCAL,
         "api": PACKAGES_ALL_API,
         "all": PACKAGES_ALL,
     },
-    python_requires=">=3.9",
+    python_requires=">=3.10",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     entry_points={
         "console_scripts": [
             "alpaca_eval=alpaca_eval.main:main",
         ],
     },
```

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/analyze.py` & `alpaca_eval-0.1.3/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.1.3/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.1.3/src/alpaca_eval/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/constants.py` & `alpaca_eval-0.1.3/src/alpaca_eval/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.1.3/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.1.3/src/alpaca_eval/decoders/anthropic.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.1.3/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.1.3/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.1.3/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.1.3/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.1.3/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.1.3/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/main.py` & `alpaca_eval-0.1.3/src/alpaca_eval/main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/metrics.py` & `alpaca_eval-0.1.3/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/plotting.py` & `alpaca_eval-0.1.3/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval/utils.py` & `alpaca_eval-0.1.3/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,13 @@
-Metadata-Version: 2.1
-Name: alpaca-eval
-Version: 0.1.2
-Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
-Author: The Alpaca Team
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: analysis
-Provides-Extra: dev
-Provides-Extra: local
-Provides-Extra: api
-Provides-Extra: all
-License-File: LICENSE
-
 # <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/yKbbQga9WE)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
 Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
 AlpacaEval provides the following:
```

#### html2text {}

```diff
@@ -1,40 +1,32 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.1.2 Summary: AlpacaEval : An
-Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Education Classifier: Intended Audience :: Science/Research Classifier: License
-:: OSI Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.9 Description-Content-Type: text/markdown
-Provides-Extra: analysis Provides-Extra: dev Provides-Extra: local Provides-
-Extra: api Provides-Extra: all License-File: LICENSE # [https://
-raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png]
-AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
-[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-
-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data
-License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-
-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [!
-[Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://
-www.python.org/downloads/release/python-390/) Evaluation of instruction-
-following models (e.g., ChatGPT) typically requires human interactions. This is
-time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based
-automatic evaluation that is fast, cheap, replicable, and validated against 20K
-human annotations. It is particularly useful for model development. Although we
-improved over prior automatic evaluation pipelines, there are still fundamental
-[limitations](#limitations). AlpacaEval provides the following: - [**Automatic
-evaluator**](#evaluators): an automatic evaluator that has high agreement with
-humans (validated on 20K annotations). We evaluate a model by measuring the
-fraction of times an powerful LLM (e.g. GPT 4 or Claude) prefers the outputs
-from that model over outputs from a reference model. Our evaluators enable
-caching and output randomization by default. - [**Leaderboard**](https://tatsu-
-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
-evaluation set. - [**Toolkit for building automatic evaluators**](#analysis): a
-simple interface for building advanced automatic evaluators (e.g. with caching,
+# [https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/
+AlpacaFarm_small.png] AlpacaEval : An Automatic Evaluator for Instruction-
+following Language Models [![Code License](https://img.shields.io/badge/
+Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/
+blob/main/LICENSE) [![Data License](https://img.shields.io/badge/
+Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/
+alpaca_farm/blob/main/DATA_LICENSE) [![Python 3.10+](https://img.shields.io/
+badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-
+3100/) [![discord](https://img.shields.io/badge/discord-server-
+blue?logo=discord&logoColor=white)](https://discord.gg/yKbbQga9WE) Evaluation
+of instruction-following models (e.g., ChatGPT) typically requires human
+interactions. This is time-consuming, expensive, and hard to replicate.
+AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
+replicable, and validated against 20K human annotations. It is particularly
+useful for model development. Although we improved over prior automatic
+evaluation pipelines, there are still fundamental [limitations](#limitations).
+AlpacaEval provides the following: - [**Automatic evaluator**](#evaluators): an
+automatic evaluator that has high agreement with humans (validated on 20K
+annotations). We evaluate a model by measuring the fraction of times an
+powerful LLM (e.g. GPT 4 or Claude) prefers the outputs from that model over
+outputs from a reference model. Our evaluators enable caching and output
+randomization by default. - [**Leaderboard**](https://tatsu-lab.github.io/
+alpaca_eval/): a leaderboard of common models on the AlpacaEval evaluation set.
+- [**Toolkit for building automatic evaluators**](#analysis): a simple
+interface for building advanced automatic evaluators (e.g. with caching,
 batching, or multi-annotators) and analyzing them (quality, price, speed,
 statistical power, bias, variance etc). - [**Human evaluation data**](#data-
 release): 20K human preferences between a given and reference model on the
 [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
 set. 2.5K of these are cross-annotations (4 humans annotating the same 650
 examples). - [**AlpacaEval dataset**](#data-release): a simplification of
 [AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
```

### Comparing `alpaca_eval-0.1.2/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.1.3/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

