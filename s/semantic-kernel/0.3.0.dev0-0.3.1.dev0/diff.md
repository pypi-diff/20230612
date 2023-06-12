# Comparing `tmp/semantic_kernel-0.3.0.dev0.tar.gz` & `tmp/semantic_kernel-0.3.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.3.0.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.3.1.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.3.0.dev0.tar` & `semantic_kernel-0.3.1.dev0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.955726 semantic_kernel-0.3.0.dev0/pip/README.md
--rw-r--r--   0        0        0      907 2023-06-05 21:39:22.282927 semantic_kernel-0.3.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     1227 2023-05-08 23:38:10.959435 semantic_kernel-0.3.0.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0      719 2023-05-25 17:48:21.153018 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0      709 2023-05-25 17:48:21.153502 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-30 18:57:02.985239 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-30 18:57:02.985587 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     4980 2023-05-25 17:48:21.154076 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.960592 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.030156 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.032300 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.034473 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     7130 2023-05-25 17:48:21.154688 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     5296 2023-05-25 17:48:21.155487 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.041646 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      679 2023-05-25 17:48:21.156192 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      182 2023-05-18 17:32:52.334054 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    15118 2023-06-05 21:39:19.137459 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     3568 2023-05-18 17:32:52.335005 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0    10783 2023-06-05 21:39:19.137785 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/weaviate_memory_store.py
--rw-r--r--   0        0        0      691 2023-05-19 18:06:11.089827 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.044314 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3164 2023-05-15 18:12:57.045974 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     7504 2023-05-25 23:34:34.714729 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    27735 2023-05-19 23:02:13.063161 semantic_kernel-0.3.0.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.3.0.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-30 18:57:02.996159 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3090 2023-05-08 23:38:10.963328 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.063945 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-13 23:12:46.175270 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6050 2023-06-05 17:09:41.373093 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1196 2023-04-30 18:57:02.998063 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.047968 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.064609 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    15915 2023-05-08 23:26:29.698891 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      158 2023-05-08 23:38:10.963774 semantic_kernel-0.3.0.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0     7287 2023-05-25 17:48:21.156811 semantic_kernel-0.3.0.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0      396 2023-05-08 23:26:29.700122 semantic_kernel-0.3.0.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0      932 2023-05-19 23:02:13.065230 semantic_kernel-0.3.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      694 2023-06-05 21:39:19.138269 semantic_kernel-0.3.0.dev0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4269 2023-04-30 18:57:02.999997 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-13 23:12:46.186028 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.3.0.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.3.0.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     6467 2023-05-15 18:12:57.049895 semantic_kernel-0.3.0.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.3.0.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-14 00:51:57.213683 semantic_kernel-0.3.0.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.3.0.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.3.0.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 semantic_kernel-0.3.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.955726 semantic_kernel-0.3.1.dev0/pip/README.md
+-rw-r--r--   0        0        0      927 2023-06-12 17:06:53.335469 semantic_kernel-0.3.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1227 2023-05-08 23:38:10.959435 semantic_kernel-0.3.1.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.153018 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.338448 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1235 2023-06-12 17:06:53.340338 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1405 2023-06-12 17:06:53.340916 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.341797 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.960592 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.030156 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.032300 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.034473 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     8467 2023-06-12 17:06:53.342528 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5504 2023-06-12 17:06:53.343178 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.041646 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.344173 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.334054 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    15268 2023-06-08 17:22:29.422161 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4402 2023-06-08 17:22:29.423786 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.345249 semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      691 2023-05-19 18:06:11.089827 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.044314 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3164 2023-05-15 18:12:57.045974 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7502 2023-06-08 17:22:29.425604 semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    27810 2023-06-12 17:06:53.346838 semantic_kernel-0.3.1.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.3.1.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.427355 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3708 2023-06-08 17:22:29.428125 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.063945 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1272 2023-06-08 17:22:29.429766 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6295 2023-06-08 17:22:29.430728 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1298 2023-06-08 17:22:29.431397 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.047968 semantic_kernel-0.3.1.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.064609 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    15915 2023-05-08 23:26:29.698891 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      158 2023-05-08 23:38:10.963774 semantic_kernel-0.3.1.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0     7287 2023-05-25 17:48:21.156811 semantic_kernel-0.3.1.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0      396 2023-05-08 23:26:29.700122 semantic_kernel-0.3.1.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0      932 2023-05-19 23:02:13.065230 semantic_kernel-0.3.1.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-06-05 21:39:19.138269 semantic_kernel-0.3.1.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.347832 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.350203 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.3.1.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.3.1.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     6467 2023-05-15 18:12:57.049895 semantic_kernel-0.3.1.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.3.1.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     1643 2023-06-08 17:22:29.433328 semantic_kernel-0.3.1.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.3.1.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.3.1.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 semantic_kernel-0.3.1.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.3.0.dev0/pip/README.md` & `semantic_kernel-0.3.1.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/pyproject.toml` & `semantic_kernel-0.3.1.dev0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.3.0.dev"
+version = "0.3.1.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.2"
 openai = "^0.27.0"
 aiofiles = "^23.1.0"
+python-dotenv = "1.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.21.0"
-black = {version = "^23.3.0", allow-prereleases = true}
+pre-commit = "2.21.0"
+black = {version = "23.3.0", allow-prereleases = true}
 ipykernel = "^6.21.1"
 pytest = "7.2.0"
-ruff = "^0.0.257"
-pytest-asyncio = "^0.21.0"
+ruff = "0.0.257"
+pytest-asyncio = "0.21.0"
 
 
 [tool.poetry.group.hugging_face.dependencies]
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "2.0.0"
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
     from semantic_kernel.semantic_functions.prompt_template_config import (
         PromptTemplateConfig,
     )
 
 
 @dataclass
-class ChatRequestSettings:
+class CompleteRequestSettings:
     temperature: float = 0.0
     top_p: float = 1.0
     presence_penalty: float = 0.0
     frequency_penalty: float = 0.0
     max_tokens: int = 256
+    stop_sequences: List[str] = field(default_factory=list)
+    number_of_responses: int = 1
+    logprobs: int = 0
 
     def update_from_completion_config(
         self, completion_config: "PromptTemplateConfig.CompletionConfig"
     ):
         self.temperature = completion_config.temperature
         self.top_p = completion_config.top_p
         self.presence_penalty = completion_config.presence_penalty
         self.frequency_penalty = completion_config.frequency_penalty
         self.max_tokens = completion_config.max_tokens
+        self.stop_sequences = completion_config.stop_sequences
+        self.number_of_responses = completion_config.number_of_responses
 
     @staticmethod
     def from_completion_config(
         completion_config: "PromptTemplateConfig.CompletionConfig",
-    ) -> "ChatRequestSettings":
-        settings = ChatRequestSettings()
+    ) -> "CompleteRequestSettings":
+        settings = CompleteRequestSettings()
         settings.update_from_completion_config(completion_config)
         return settings
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, List
+from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from semantic_kernel.semantic_functions.prompt_template_config import (
         PromptTemplateConfig,
     )
 
 
 @dataclass
-class CompleteRequestSettings:
+class ChatRequestSettings:
     temperature: float = 0.0
     top_p: float = 1.0
     presence_penalty: float = 0.0
     frequency_penalty: float = 0.0
-    max_tokens: int = 256
-    stop_sequences: List[str] = field(default_factory=list)
     number_of_responses: int = 1
-    logprobs: int = 0
+    max_tokens: int = 256
 
     def update_from_completion_config(
         self, completion_config: "PromptTemplateConfig.CompletionConfig"
     ):
         self.temperature = completion_config.temperature
         self.top_p = completion_config.top_p
         self.presence_penalty = completion_config.presence_penalty
         self.frequency_penalty = completion_config.frequency_penalty
+        self.number_of_responses = completion_config.number_of_responses
         self.max_tokens = completion_config.max_tokens
-        self.stop_sequences = completion_config.stop_sequences
 
     @staticmethod
     def from_completion_config(
         completion_config: "PromptTemplateConfig.CompletionConfig",
-    ) -> "CompleteRequestSettings":
-        settings = CompleteRequestSettings()
+    ) -> "ChatRequestSettings":
+        settings = ChatRequestSettings()
         settings.update_from_completion_config(completion_config)
         return settings
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
-from typing import Any, List, Optional, Tuple
+from typing import Any, List, Optional, Tuple, Union
 
 import openai
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.chat_completion_client_base import (
     ChatCompletionClientBase,
 )
@@ -57,36 +57,45 @@
         self._api_version = api_version
         self._endpoint = endpoint
         self._log = log if log is not None else NullLogger()
         self._messages = []
 
     async def complete_chat_async(
         self, messages: List[Tuple[str, str]], request_settings: ChatRequestSettings
-    ) -> str:
+    ) -> Union[str, List[str]]:
         # TODO: tracking on token counts/etc.
         response = await self._send_chat_request(messages, request_settings, False)
 
-        return response.choices[0].message.content
+        if len(response.choices) == 1:
+            return response.choices[0].message.content
+        else:
+            return [choice.message.content for choice in response.choices]
 
     async def complete_chat_stream_async(
         self, messages: List[Tuple[str, str]], request_settings: ChatRequestSettings
     ):
         response = await self._send_chat_request(messages, request_settings, True)
+
+        # parse the completion text(s) and yield them
         async for chunk in response:
-            if "role" in chunk.choices[0].delta:
-                yield chunk.choices[0].delta.role + ": "
-            if "content" in chunk.choices[0].delta:
-                yield chunk.choices[0].delta.content
+            text, index = _parse_choices(chunk)
+            # if multiple responses are requested, keep track of them
+            if request_settings.number_of_responses > 1:
+                completions = [""] * request_settings.number_of_responses
+                completions[index] = text
+                yield completions
+            # if only one response is requested, yield it
+            else:
+                yield text
 
     async def complete_async(
         self, prompt: str, request_settings: CompleteRequestSettings
-    ) -> str:
+    ) -> Union[str, List[str]]:
         """
-        Completes the given prompt. Returns a single string completion.
-        Cannot return multiple completions. Cannot return logprobs.
+        Completes the given prompt.
 
         Arguments:
             prompt {str} -- The prompt to complete.
             request_settings {CompleteRequestSettings} -- The request settings.
 
         Returns:
             str -- The completed text.
@@ -94,46 +103,59 @@
         prompt_to_message = [("user", prompt)]
         chat_settings = ChatRequestSettings(
             temperature=request_settings.temperature,
             top_p=request_settings.top_p,
             presence_penalty=request_settings.presence_penalty,
             frequency_penalty=request_settings.frequency_penalty,
             max_tokens=request_settings.max_tokens,
+            number_of_responses=request_settings.number_of_responses,
         )
         response = await self._send_chat_request(
             prompt_to_message, chat_settings, False
         )
 
-        return response.choices[0].message.content
+        if len(response.choices) == 1:
+            return response.choices[0].message.content
+        else:
+            return [choice.message.content for choice in response.choices]
 
     async def complete_stream_async(
         self, prompt: str, request_settings: CompleteRequestSettings
     ):
         prompt_to_message = [("user", prompt)]
         chat_settings = ChatRequestSettings(
             temperature=request_settings.temperature,
             top_p=request_settings.top_p,
             presence_penalty=request_settings.presence_penalty,
             frequency_penalty=request_settings.frequency_penalty,
             max_tokens=request_settings.max_tokens,
+            number_of_responses=request_settings.number_of_responses,
         )
         response = await self._send_chat_request(prompt_to_message, chat_settings, True)
 
+        # parse the completion text(s) and yield them
         async for chunk in response:
-            if "content" in chunk.choices[0].delta:
-                yield chunk.choices[0].delta.content
+            text, index = _parse_choices(chunk)
+            # if multiple responses are requested, keep track of them
+            if request_settings.number_of_responses > 1:
+                completions = [""] * request_settings.number_of_responses
+                completions[index] = text
+                yield completions
+            # if only one response is requested, yield it
+            else:
+                yield text
 
     async def _send_chat_request(
         self,
         messages: List[Tuple[str, str]],
         request_settings: ChatRequestSettings,
         stream: bool,
     ):
         """
-        Completes the given user message. Returns a single string completion.
+        Completes the given user message with an asynchronous stream.
 
         Arguments:
             user_message {str} -- The message (from a user) to respond to.
             request_settings {ChatRequestSettings} -- The request settings.
 
         Returns:
             str -- The completed text.
@@ -180,19 +202,31 @@
                 organization=self._org_id,
                 messages=formatted_messages,
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 presence_penalty=request_settings.presence_penalty,
                 frequency_penalty=request_settings.frequency_penalty,
                 max_tokens=request_settings.max_tokens,
+                n=request_settings.number_of_responses,
                 stream=stream,
             )
         except Exception as ex:
             raise AIException(
                 AIException.ErrorCodes.ServiceError,
                 "OpenAI service failed to complete the chat",
                 ex,
             )
 
         # TODO: tracking on token counts/etc.
 
         return response
+
+
+def _parse_choices(chunk):
+    message = ""
+    if "role" in chunk.choices[0].delta:
+        message += chunk.choices[0].delta.role + ": "
+    if "content" in chunk.choices[0].delta:
+        message += chunk.choices[0].delta.content
+
+    index = chunk.choices[0].index
+    return message, index
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
-from typing import Any, Optional
+from typing import Any, List, Optional, Union
 
 import openai
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.complete_request_settings import (
     CompleteRequestSettings,
 )
@@ -52,27 +52,38 @@
         self._api_version = api_version
         self._endpoint = endpoint
         self._org_id = org_id
         self._log = log if log is not None else NullLogger()
 
     async def complete_async(
         self, prompt: str, request_settings: CompleteRequestSettings
-    ) -> str:
+    ) -> Union[str, List[str]]:
         # TODO: tracking on token counts/etc.
         response = await self._send_completion_request(prompt, request_settings, False)
-        return response.choices[0].text
+
+        if len(response.choices) == 1:
+            return response.choices[0].text
+        else:
+            return [choice.text for choice in response.choices]
 
     # TODO: complete w/ multiple...
 
     async def complete_stream_async(
         self, prompt: str, request_settings: CompleteRequestSettings
     ):
         response = await self._send_completion_request(prompt, request_settings, True)
+
         async for chunk in response:
-            yield chunk.choices[0].text
+            if request_settings.number_of_responses > 1:
+                for choice in chunk.choices:
+                    completions = [""] * request_settings.number_of_responses
+                    completions[choice.index] = choice.text
+                    yield completions
+            else:
+                yield chunk.choices[0].text
 
     async def _send_completion_request(
         self, prompt: str, request_settings: CompleteRequestSettings, stream: bool
     ):
         """
         Completes the given prompt. Returns a single string completion.
         Cannot return multiple completions. Cannot return logprobs.
@@ -92,21 +103,14 @@
         if request_settings.max_tokens < 1:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
                 "The max tokens must be greater than 0, "
                 f"but was {request_settings.max_tokens}",
             )
 
-        if request_settings.number_of_responses != 1:
-            raise AIException(
-                AIException.ErrorCodes.InvalidRequest,
-                "complete_async only supports a single completion, "
-                f"but {request_settings.number_of_responses} were requested",
-            )
-
         if request_settings.logprobs != 0:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
                 "complete_async does not support logprobs, "
                 f"but logprobs={request_settings.logprobs} was requested",
             )
 
@@ -127,14 +131,15 @@
                 prompt=prompt,
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 presence_penalty=request_settings.presence_penalty,
                 frequency_penalty=request_settings.frequency_penalty,
                 max_tokens=request_settings.max_tokens,
                 stream=stream,
+                n=request_settings.number_of_responses,
                 stop=(
                     request_settings.stop_sequences
                     if request_settings.stop_sequences is not None
                     and len(request_settings.stop_sequences) > 0
                     else None
                 ),
             )
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,32 +154,35 @@
         Returns:
             List[str] -- The unique database key of the record.
         """
         collection = await self.get_collection_async(collection_name)
         if collection is None:
             raise Exception(f"Collection '{collection_name}' does not exist")
 
-        # TODO: timestamp
+        record._key = record._id
         metadata = {
             "timestamp": record._timestamp or "",
             "is_reference": record._is_reference,
             "external_source_name": record._external_source_name or "",
             "description": record._description or "",
+            "additional_metadata": record._additional_metadata or "",
+            "id": record._id or "",
         }
 
         collection.add(
             metadatas=metadata,
             # by providing embeddings, we can skip the chroma's embedding function call
             embeddings=record.embedding.tolist(),
             documents=record._text,
-            ids=record._id,
+            ids=record._key,
         )
+
         if self._persist_directory is not None:
             self._client.persist()
-        return record._id
+        return record._key
 
     async def upsert_batch_async(
         self, collection_name: str, records: List[MemoryRecord]
     ) -> List[str]:
         """Upserts a batch of records.
 
         Arguments:
@@ -233,15 +236,15 @@
         query_includes = (
             ["embeddings", "metadatas", "documents"]
             if with_embeddings
             else ["metadatas", "documents"]
         )
 
         value = collection.get(ids=keys, include=query_includes)
-        record = query_results_to_records(value)
+        record = query_results_to_records(value, with_embeddings)
         return record
 
     async def remove_async(self, collection_name: str, key: str) -> None:
         """Removes a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the record from.
@@ -314,15 +317,15 @@
 
         similarity_score = chroma_compute_similarity_scores(embedding, embedding_array)
 
         # Convert query results into memory records
         record_list = [
             (record, distance)
             for record, distance in zip(
-                query_results_to_records(query_results),
+                query_results_to_records(query_results, with_embeddings),
                 similarity_score,
             )
         ]
 
         sorted_results = sorted(
             record_list,
             key=lambda x: x[1],
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,48 +18,71 @@
                 snake_str += "_"
             if i != len(camel_str) - 1 and camel_str[i + 1].islower():
                 snake_str += "_"
         snake_str += char.lower()
     return snake_str
 
 
-def query_results_to_records(results: "QueryResult") -> List[MemoryRecord]:
+def query_results_to_records(
+    results: "QueryResult", with_embedding: bool
+) -> List[MemoryRecord]:
     # if results has only one record, it will be a list instead of a nested list
     # this is to make sure that results is always a nested list
     # {'ids': ['test_id1'], 'embeddings': [[...]], 'documents': ['sample text1'], 'metadatas': [{...}]}
     # => {'ids': [['test_id1']], 'embeddings': [[[...]]], 'documents': [['sample text1']], 'metadatas': [[{...}]]}
     try:
         if isinstance(results["ids"][0], str):
             for k, v in results.items():
                 results[k] = [v]
     except IndexError:
         return []
 
-    memory_records = [
-        (
-            MemoryRecord(
-                is_reference=metadata["is_reference"],
-                external_source_name=metadata["external_source_name"],
-                id=id,
-                description=metadata["description"],
-                text=document,
-                # TODO: get_async say embedding is optional but Record constructor requires it
-                embedding=embedding,
-                # TODO: what is key for?
-                key=None,
-                timestamp=metadata["timestamp"],
+    if with_embedding:
+        memory_records = [
+            (
+                MemoryRecord(
+                    is_reference=metadata["is_reference"],
+                    external_source_name=metadata["external_source_name"],
+                    id=metadata["id"],
+                    description=metadata["description"],
+                    text=document,
+                    embedding=embedding,
+                    additional_metadata=metadata["additional_metadata"],
+                    key=id,
+                    timestamp=metadata["timestamp"],
+                )
             )
-        )
-        for id, document, embedding, metadata in zip(
-            results["ids"][0],
-            results["documents"][0],
-            results["embeddings"][0],
-            results["metadatas"][0],
-        )
-    ]
+            for id, document, embedding, metadata in zip(
+                results["ids"][0],
+                results["documents"][0],
+                results["embeddings"][0],
+                results["metadatas"][0],
+            )
+        ]
+    else:
+        memory_records = [
+            (
+                MemoryRecord(
+                    is_reference=metadata["is_reference"],
+                    external_source_name=metadata["external_source_name"],
+                    id=metadata["id"],
+                    description=metadata["description"],
+                    text=document,
+                    embedding=None,
+                    additional_metadata=metadata["additional_metadata"],
+                    key=id,
+                    timestamp=metadata["timestamp"],
+                )
+            )
+            for id, document, metadata in zip(
+                results["ids"][0],
+                results["documents"][0],
+                results["metadatas"][0],
+            )
+        ]
     return memory_records
 
 
 def chroma_compute_similarity_scores(
     embedding: ndarray, embedding_array: ndarray, logger=None
 ) -> ndarray:
     """Computes the cosine similarity scores between a query embedding and a group of embeddings.
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/weaviate_memory_store.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,19 @@
             "dataType": ["text"],
         },
         {
             "name": "text",
             "description": "The text of the record.",
             "dataType": ["text"],
         },
+        {
+            "name": "additionalMetadata",
+            "description": "Optional custom metadata of the record.",
+            "dataType": ["string"],
+        },
     ],
 }
 
 ALL_PROPERTIES = [property["name"] for property in SCHEMA["properties"]]
 
 
 @dataclass
@@ -77,14 +82,15 @@
             "_key": "key",
             "_timestamp": "timestamp",
             "_is_reference": "isReference",
             "_external_source_name": "externalSourceName",
             "_id": "skId",
             "_description": "description",
             "_text": "text",
+            "_additional_metadata": "additionalMetadata",
             "_embedding": "vector",
         }
 
         WEAVIATE_TO_SK_MAPPING = {v: k for k, v in SK_TO_WEAVIATE_MAPPING.items()}
 
         @classmethod
         def sk_to_weaviate(cls, sk_dict):
@@ -129,39 +135,46 @@
                 return weaviate.Client(url=self.config.url)
         else:
             raise ValueError("Weaviate config must have either url or use_embed set")
 
     async def create_collection_async(self, collection_name: str) -> None:
         schema = SCHEMA.copy()
         schema["class"] = collection_name
-        await asyncio.to_thread(self.client.schema.create_class, schema)
+        await asyncio.get_running_loop().run_in_executor(
+            None, self.client.schema.create_class, schema
+        )
 
     async def get_collections_async(self) -> List[str]:
-        schemas = await asyncio.to_thread(self.client.schema.get)
+        schemas = await asyncio.get_running_loop().run_in_executor(
+            None, self.client.schema.get
+        )
         return [schema["class"] for schema in schemas["classes"]]
 
     async def delete_collection_async(self, collection_name: str) -> bool:
-        await asyncio.to_thread(self.client.schema.delete_class, collection_name)
+        await asyncio.get_running_loop().run_in_executor(
+            None, self.client.schema.delete_class, collection_name
+        )
 
     async def does_collection_exist_async(self, collection_name: str) -> bool:
         collections = await self.get_collections_async()
         return collection_name in collections
 
     async def upsert_async(self, collection_name: str, record: MemoryRecord) -> str:
         weaviate_record = self.FieldMapper.sk_to_weaviate(vars(record))
 
         vector = weaviate_record.pop("vector", None)
         weaviate_id = weaviate.util.generate_uuid5(weaviate_record, collection_name)
 
-        return await asyncio.to_thread(
+        return await asyncio.get_running_loop().run_in_executor(
+            None,
             self.client.data_object.create,
-            data_object=weaviate_record,
-            uuid=weaviate_id,
-            vector=vector,
-            class_name=collection_name,
+            weaviate_record,
+            collection_name,
+            weaviate_id,
+            vector,
         )
 
     async def upsert_batch_async(
         self, collection_name: str, records: List[MemoryRecord]
     ) -> List[str]:
         def _upsert_batch_inner():
             results = []
@@ -178,29 +191,33 @@
                         vector=vector,
                         class_name=collection_name,
                     )
                     results.append(weaviate_id)
 
             return results
 
-        return await asyncio.to_thread(_upsert_batch_inner)
+        return await asyncio.get_running_loop().run_in_executor(
+            None, _upsert_batch_inner
+        )
 
     async def get_async(
         self, collection_name: str, key: str, with_embedding: bool
     ) -> MemoryRecord:
         # Call the batched version with a single key
         results = await self.get_batch_async(collection_name, [key], with_embedding)
         return results[0] if results else None
 
     async def get_batch_async(
         self, collection_name: str, keys: List[str], with_embedding: bool
     ) -> List[MemoryRecord]:
         queries = self._build_multi_get_query(collection_name, keys, with_embedding)
 
-        results = await asyncio.to_thread(self.client.query.multi_get(queries).do)
+        results = await asyncio.get_running_loop().run_in_executor(
+            None, self.client.query.multi_get(queries).do
+        )
 
         get_dict = results.get("data", {}).get("Get", {})
 
         memory_records = [
             self._convert_weaviate_doc_to_memory_record(doc)
             for docs in get_dict.values()
             for doc in docs
@@ -250,18 +267,16 @@
         for key in keys:
             where = {
                 "path": ["key"],
                 "operator": "Equal",
                 "valueString": key,
             }
 
-            await asyncio.to_thread(
-                self.client.batch.delete_objects,
-                class_name=collection_name,
-                where=where,
+            await asyncio.get_running_loop().run_in_executor(
+                None, self.client.batch.delete_objects, collection_name, where
             )
 
     async def get_nearest_matches_async(
         self,
         collection_name: str,
         embedding: np.ndarray,
         limit: int,
@@ -280,15 +295,15 @@
         query = (
             self.client.query.get(collection_name, ALL_PROPERTIES)
             .with_near_vector(nearVector)
             .with_additional(additional)
             .with_limit(limit)
         )
 
-        results = await asyncio.to_thread(query.do)
+        results = await asyncio.get_running_loop().run_in_executor(None, query.do)
 
         get_dict = results.get("data", {}).get("Get", {})
 
         memory_records_and_scores = [
             (
                 self._convert_weaviate_doc_to_memory_record(doc),
                 item["_additional"]["certainty"],
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,16 +192,16 @@
              SKContext["input"] = "3"
              {{time.days_ago $input}} => Sunday, 7 May, 2023
         """
         d = datetime.date.today() - datetime.timedelta(days=int(days))
         return d.strftime("%A, %d %B, %Y")
 
     @sk_function(
-        description="""Get the date of the last day matching the supplied week day name in English. 
-        Example: Che giorno era 'Martedi' scorso -> dateMatchingLastDayName 'Tuesday' => Tuesday, 
+        description="""Get the date of the last day matching the supplied week day name in English.
+        Example: Che giorno era 'Martedi' scorso -> dateMatchingLastDayName 'Tuesday' => Tuesday,
         16 May, 2023"""
     )
     def date_matching_last_day_name(self, day_name: str) -> str:
         """
         Get the date of the last day matching the supplied day name
 
         params:
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,14 +689,15 @@
         skill_name: Optional[str] = None,
         description: Optional[str] = None,
         max_tokens: int = 256,
         temperature: float = 0.0,
         top_p: float = 1.0,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
+        number_of_responses: int = 1,
         stop_sequences: Optional[List[str]] = None,
     ) -> "SKFunctionBase":
         function_name = (
             function_name
             if function_name is not None
             else f"f_{str(uuid4()).replace('-', '_')}"
         )
@@ -710,14 +711,15 @@
             type="completion",
             completion=PromptTemplateConfig.CompletionConfig(
                 temperature,
                 top_p,
                 presence_penalty,
                 frequency_penalty,
                 max_tokens,
+                number_of_responses,
                 stop_sequences if stop_sequences is not None else [],
             ),
         )
 
         validate_function_name(function_name)
         if skill_name is not None:
             validate_skill_name(skill_name)
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 
 class MemoryQueryResult:
     is_reference: bool
     external_source_name: Optional[str]
     id: str
     description: Optional[str]
     text: Optional[str]
+    additional_metadata: Optional[str]
     relevance: float
     embedding: Optional[ndarray]
 
     def __init__(
         self,
         is_reference: bool,
         external_source_name: Optional[str],
         id: str,
         description: Optional[str],
         text: Optional[str],
+        additional_metadata: Optional[str],
         embedding: Optional[ndarray],
         relevance: float,
     ) -> None:
         """Initialize a new instance of MemoryQueryResult.
 
         Arguments:
             is_reference {bool} -- Whether the record is a reference record.
@@ -41,14 +43,15 @@
             None -- None.
         """
         self.is_reference = is_reference
         self.external_source_name = external_source_name
         self.id = id
         self.description = description
         self.text = text
+        self.additional_metadata = additional_metadata
         self.relevance = relevance
         self.embedding = embedding
 
     @staticmethod
     def from_memory_record(
         record: MemoryRecord,
         relevance: float,
@@ -64,10 +67,11 @@
         """
         return MemoryQueryResult(
             is_reference=record._is_reference,
             external_source_name=record._external_source_name,
             id=record._id,
             description=record._description,
             text=record._text,
+            additional_metadata=record._additional_metadata,
             embedding=record._embedding,
             relevance=relevance,
         )
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_record.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,96 +9,109 @@
     _key: str
     _timestamp: str
     _is_reference: bool
     _external_source_name: Optional[str]
     _id: str
     _description: Optional[str]
     _text: Optional[str]
+    _additional_metadata: Optional[str]
     _embedding: ndarray
 
     def __init__(
         self,
         is_reference: bool,
         external_source_name: Optional[str],
         id: str,
         description: Optional[str],
         text: Optional[str],
-        embedding: ndarray,
+        additional_metadata: Optional[str],
+        embedding: Optional[ndarray],
         key: Optional[str] = None,
         timestamp: Optional[str] = None,
     ) -> None:
         """Initialize a new instance of MemoryRecord.
 
         Arguments:
             is_reference {bool} -- Whether the record is a reference record.
             external_source_name {Optional[str]} -- The name of the external source.
             id {str} -- A unique for the record.
             description {Optional[str]} -- The description of the record.
             text {Optional[str]} -- The text of the record.
+            additional_metadata {Optional[str]} -- Custom metadata for the record.
             embedding {ndarray} -- The embedding of the record.
 
         Returns:
             None -- None.
         """
         self._key = key
         self._timestamp = timestamp
         self._is_reference = is_reference
         self._external_source_name = external_source_name
         self._id = id
         self._description = description
         self._text = text
+        self._additional_metadata = additional_metadata
         self._embedding = embedding
 
     @property
     def embedding(self) -> ndarray:
         return self._embedding
 
     @staticmethod
     def reference_record(
         external_id: str,
         source_name: str,
         description: Optional[str],
+        additional_metadata: Optional[str],
         embedding: ndarray,
     ) -> "MemoryRecord":
         """Create a reference record.
 
         Arguments:
             external_id {str} -- The external id of the record.
             source_name {str} -- The name of the external source.
             description {Optional[str]} -- The description of the record.
+            additional_metadata {Optional[str]} -- Custom metadata for the record.
             embedding {ndarray} -- The embedding of the record.
 
         Returns:
             MemoryRecord -- The reference record.
         """
         return MemoryRecord(
             is_reference=True,
             external_source_name=source_name,
             id=external_id,
             description=description,
             text=None,
+            additional_metadata=additional_metadata,
             embedding=embedding,
         )
 
     @staticmethod
     def local_record(
-        id: str, text: str, description: Optional[str], embedding: ndarray
+        id: str,
+        text: str,
+        description: Optional[str],
+        additional_metadata: Optional[str],
+        embedding: ndarray,
     ) -> "MemoryRecord":
         """Create a local record.
 
         Arguments:
             id {str} -- A unique for the record.
             text {str} -- The text of the record.
             description {Optional[str]} -- The description of the record.
+            additional_metadata {Optional[str]} -- Custom metadata for the record.
             embedding {ndarray} -- The embedding of the record.
 
         Returns:
             MemoryRecord -- The local record.
         """
         return MemoryRecord(
             is_reference=False,
             external_source_name=None,
             id=id,
             description=description,
             text=text,
+            additional_metadata=additional_metadata,
             embedding=embedding,
         )
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/null_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,31 @@
 
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 
 
 class NullMemory(SemanticTextMemoryBase):
     async def save_information_async(
-        self, collection: str, text: str, id: str, description: Optional[str] = None
+        self,
+        collection: str,
+        text: str,
+        id: str,
+        description: Optional[str] = None,
+        additional_metadata: Optional[str] = None,
     ) -> None:
         return None
 
     async def save_reference_async(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
         description: Optional[str] = None,
+        additional_metadata: Optional[str] = None,
     ) -> None:
         return None
 
     async def get_async(
         self, collection: str, query: str
     ) -> Optional[MemoryQueryResult]:
         return None
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
     async def save_information_async(
         self,
         collection: str,
         text: str,
         id: str,
         description: Optional[str] = None,
+        additional_metadata: Optional[str] = None,
     ) -> None:
         """Save information to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the information to.
             text {str} -- The text to save.
             id {str} -- The id of the information.
@@ -53,26 +54,31 @@
         if not await self._storage.does_collection_exist_async(
             collection_name=collection
         ):
             await self._storage.create_collection_async(collection_name=collection)
 
         embedding = await self._embeddings_generator.generate_embeddings_async([text])
         data = MemoryRecord.local_record(
-            id=id, text=text, description=description, embedding=embedding
+            id=id,
+            text=text,
+            description=description,
+            additional_metadata=additional_metadata,
+            embedding=embedding,
         )
 
         await self._storage.upsert_async(collection_name=collection, record=data)
 
     async def save_reference_async(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
         description: Optional[str] = None,
+        additional_metadata: Optional[str] = None,
     ) -> None:
         """Save a reference to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the reference to.
             text {str} -- The text to save.
             external_id {str} -- The external id of the reference.
@@ -89,14 +95,15 @@
             await self._storage.create_collection_async(collection_name=collection)
 
         embedding = await self._embeddings_generator.generate_embeddings_async([text])
         data = MemoryRecord.reference_record(
             external_id=external_id,
             source_name=external_source_name,
             description=description,
+            additional_metadata=additional_metadata,
             embedding=embedding,
         )
 
         await self._storage.upsert_async(collection_name=collection, record=data)
 
     async def get_async(
         self,
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,28 @@
     @abstractmethod
     async def save_information_async(
         self,
         collection: str,
         text: str,
         id: str,
         description: Optional[str] = None,
+        additional_metadata: Optional[str] = None,
         # TODO: ctoken?
     ) -> None:
         pass
 
     @abstractmethod
     async def save_reference_async(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
         description: Optional[str] = None,
+        additional_metadata: Optional[str] = None,
     ) -> None:
         pass
 
     @abstractmethod
     async def get_async(
         self,
         collection: str,
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     @dataclass
     class CompletionConfig:
         temperature: float = 0.0
         top_p: float = 1.0
         presence_penalty: float = 0.0
         frequency_penalty: float = 0.0
         max_tokens: int = 256
+        number_of_responses: int = 1
         stop_sequences: List[str] = field(default_factory=list)
 
     @dataclass
     class InputParameter:
         name: str = ""
         description: str = ""
         default_value: str = ""
@@ -47,14 +48,17 @@
         config.completion = PromptTemplateConfig.CompletionConfig()
         completion_dict = data["completion"]
         config.completion.temperature = completion_dict.get("temperature")
         config.completion.top_p = completion_dict.get("top_p")
         config.completion.presence_penalty = completion_dict.get("presence_penalty")
         config.completion.frequency_penalty = completion_dict.get("frequency_penalty")
         config.completion.max_tokens = completion_dict.get("max_tokens")
+        config.completion.number_of_responses = completion_dict.get(
+            "number_of_responses"
+        )
         config.completion.stop_sequences = completion_dict.get("stop_sequences", [])
         config.default_services = data.get("default_services", [])
 
         # Some skills may not have input parameters defined
         config.input = PromptTemplateConfig.InputConfig()
         config.input.parameters = []
         if data.get("input") is not None:
@@ -98,17 +102,19 @@
     @staticmethod
     def from_completion_parameters(
         temperature: float = 0.0,
         top_p: float = 1.0,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         max_tokens: int = 256,
+        number_of_responses: int = 1,
         stop_sequences: List[str] = [],
     ) -> "PromptTemplateConfig":
         config = PromptTemplateConfig()
         config.completion.temperature = temperature
         config.completion.top_p = top_p
         config.completion.presence_penalty = presence_penalty
         config.completion.frequency_penalty = frequency_penalty
         config.completion.max_tokens = max_tokens
+        config.completion.number_of_responses = number_of_responses
         config.completion.stop_sequences = stop_sequences
         return config
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,8 +39,21 @@
                 f"There are 2 functions with the same name: {function_name}."
                 f"One is native and the other semantic.",
             )
 
         return as_sf
 
     def is_native(self, skill_name: str, function_name: str) -> bool:
-        return not self.is_semantic(skill_name, function_name)
+        as_sf = self._semantic_functions.get(skill_name, [])
+        as_sf = any(f.name == function_name for f in as_sf)
+
+        as_nf = self._native_functions.get(skill_name, [])
+        as_nf = any(f.name == function_name for f in as_nf)
+
+        if as_sf and as_nf:
+            raise KernelException(
+                KernelException.ErrorCodes.AmbiguousImplementation,
+                f"There are 2 functions with the same name: {function_name}."
+                f"One is native and the other semantic.",
+            )
+
+        return as_nf
```

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.3.1.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.0.dev0/PKG-INFO` & `semantic_kernel-0.3.1.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.3.0.dev0
+Version: 0.3.1.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
+Requires-Dist: python-dotenv (==1.0.0)
 Description-Content-Type: text/markdown
 
 # About Semantic Kernel
 
 **Semantic Kernel (SK)** is a lightweight SDK enabling integration of AI Large
 Language Models (LLMs) with conventional programming languages. The SK
 extensible programming model combines natural language **semantic functions**,
```

