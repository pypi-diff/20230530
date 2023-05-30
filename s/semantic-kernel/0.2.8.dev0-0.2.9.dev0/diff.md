# Comparing `tmp/semantic_kernel-0.2.8.dev0.tar.gz` & `tmp/semantic_kernel-0.2.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.8.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.9.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.8.dev0.tar` & `semantic_kernel-0.2.9.dev0.tar`

### file list

```diff
@@ -1,93 +1,91 @@
--rw-r--r--   0        0        0     1186 2023-05-09 16:56:59.338396 semantic_kernel-0.2.8.dev0/pip/README.md
--rw-r--r--   0        0        0      771 2023-05-15 18:37:29.801042 semantic_kernel-0.2.8.dev0/pyproject.toml
--rw-r--r--   0        0        0     1227 2023-05-09 16:56:59.344375 semantic_kernel-0.2.8.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-29 00:21:18.081250 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0      506 2023-04-29 00:21:18.081609 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-29 00:21:18.081920 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-29 00:21:18.082190 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-29 00:21:18.082773 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 23:48:28.652652 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     3837 2023-05-09 16:56:59.345779 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-09 16:56:59.347133 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-29 00:21:18.084928 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-12 22:12:56.286732 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-12 22:12:56.289589 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-12 22:12:56.291500 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     5502 2023-05-12 22:12:56.293123 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4746 2023-05-12 22:12:56.294808 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2723 2023-05-12 22:12:56.296394 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      497 2023-04-30 23:48:28.654940 semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      711 2023-05-14 22:39:43.859053 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2510 2023-05-14 22:39:43.859324 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2072 2023-04-14 03:36:09.239029 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-26 22:16:44.328276 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3164 2023-05-12 22:12:56.299298 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 03:36:09.239829 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-14 03:36:09.240512 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5849 2023-04-29 00:21:18.088108 semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    22020 2023-05-09 16:56:59.349187 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2099 2023-05-09 16:56:59.349735 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0     1626 2023-04-29 00:21:18.089839 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-14 03:36:09.245082 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-14 03:36:09.245483 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     3822 2023-04-29 00:21:18.090797 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-14 03:36:09.246857 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1483 2023-05-09 16:56:59.350243 semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-14 03:36:09.247903 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-30 23:48:28.656559 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3090 2023-05-09 16:56:59.350763 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2004 2023-05-09 16:56:59.351286 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-14 03:36:09.249612 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6045 2023-05-02 00:49:03.451205 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1196 2023-04-30 23:48:28.662481 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-12 22:12:56.301028 semantic_kernel-0.2.8.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-20 17:10:26.995186 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 03:36:09.253302 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-14 03:36:09.253662 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-14 03:36:09.254004 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 03:36:09.254344 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    15915 2023-05-09 16:56:59.351884 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 23:48:28.668178 semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      158 2023-05-09 16:56:59.352379 semantic_kernel-0.2.8.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0     7275 2023-05-09 16:56:59.352682 semantic_kernel-0.2.8.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0      396 2023-05-09 16:56:59.352963 semantic_kernel-0.2.8.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0      919 2023-04-14 03:36:09.255908 semantic_kernel-0.2.8.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-14 03:36:09.256522 semantic_kernel-0.2.8.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-14 03:36:09.256949 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 03:36:09.257319 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-14 03:36:09.257703 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4269 2023-04-29 00:21:18.098358 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 03:36:09.258593 semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 03:36:09.259027 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 03:36:09.259911 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-14 03:36:09.260336 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 03:36:09.261065 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 03:36:09.261495 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 03:36:09.261836 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-14 03:36:09.262309 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 03:36:09.262723 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 03:36:09.263484 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-14 03:36:09.263900 semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-14 03:36:09.264367 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 03:36:09.264992 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 03:36:09.265522 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-29 00:21:18.098851 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-14 03:36:09.267164 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-14 03:36:09.267627 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 03:36:09.268042 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-14 03:36:09.268607 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 03:36:09.269045 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-14 03:36:09.269480 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 03:36:09.269880 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-14 03:36:09.270280 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-14 03:36:09.270855 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-14 03:36:09.271313 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-14 03:36:09.271775 semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 23:48:28.669001 semantic_kernel-0.2.8.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 23:48:28.669455 semantic_kernel-0.2.8.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     6467 2023-05-12 22:13:00.910173 semantic_kernel-0.2.8.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-14 03:36:09.272351 semantic_kernel-0.2.8.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-14 03:36:09.272775 semantic_kernel-0.2.8.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-14 03:36:09.273176 semantic_kernel-0.2.8.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-14 03:36:09.274119 semantic_kernel-0.2.8.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 semantic_kernel-0.2.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.955726 semantic_kernel-0.2.9.dev0/pip/README.md
+-rw-r--r--   0        0        0      835 2023-05-30 18:59:46.699650 semantic_kernel-0.2.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1227 2023-05-08 23:38:10.959435 semantic_kernel-0.2.9.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.153018 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0      709 2023-05-25 17:48:21.153502 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-30 18:57:02.985239 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-30 18:57:02.985587 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     4980 2023-05-25 17:48:21.154076 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.960592 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.030156 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.032300 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.034473 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     7130 2023-05-25 17:48:21.154688 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5296 2023-05-25 17:48:21.155487 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.041646 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      679 2023-05-25 17:48:21.156192 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.334054 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14953 2023-05-18 17:32:52.334557 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     3568 2023-05-18 17:32:52.335005 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      691 2023-05-19 18:06:11.089827 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.044314 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3164 2023-05-15 18:12:57.045974 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7504 2023-05-25 23:34:34.714729 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    27735 2023-05-19 23:02:13.063161 semantic_kernel-0.2.9.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.2.9.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-30 18:57:02.996159 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3090 2023-05-08 23:38:10.963328 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.063945 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-13 23:12:46.175270 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6045 2023-05-08 23:26:22.334494 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1196 2023-04-30 18:57:02.998063 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.047968 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.064609 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    15915 2023-05-08 23:26:29.698891 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      158 2023-05-08 23:38:10.963774 semantic_kernel-0.2.9.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0     7287 2023-05-25 17:48:21.156811 semantic_kernel-0.2.9.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0      396 2023-05-08 23:26:29.700122 semantic_kernel-0.2.9.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0      932 2023-05-19 23:02:13.065230 semantic_kernel-0.2.9.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-05-19 23:02:13.065627 semantic_kernel-0.2.9.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4269 2023-04-30 18:57:02.999997 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-13 23:12:46.186028 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.2.9.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.2.9.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     6467 2023-05-15 18:12:57.049895 semantic_kernel-0.2.9.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.2.9.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-14 00:51:57.213683 semantic_kernel-0.2.9.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.2.9.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.2.9.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 semantic_kernel-0.2.9.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.8.dev0/pip/README.md` & `semantic_kernel-0.2.9.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/pyproject.toml` & `semantic_kernel-0.2.9.dev0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.2.8.dev"
+version = "0.2.9.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -18,20 +18,24 @@
 ipykernel = "^6.21.1"
 pytest = "7.2.0"
 ruff = "^0.0.257"
 pytest-asyncio = "^0.21.0"
 
 
 [tool.poetry.group.hugging_face.dependencies]
-torch = "^2.0.0"
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
+torch = "2.0.0"
+
+[tool.poetry.group.chromadb.dependencies]
+chromadb = "^0.3.23"
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
+from threading import Thread
 from typing import Optional
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.complete_request_settings import (
     CompleteRequestSettings,
 )
 from semantic_kernel.connectors.ai.text_completion_client_base import (
@@ -98,7 +99,39 @@
                     AIException.ErrorCodes.InvalidConfiguration,
                     "Unsupported hugging face pipeline task: only \
                         text-generation, text2text-generation, and summarization are supported.",
                 )
 
         except Exception as e:
             raise AIException("Hugging Face completion failed", e)
+
+    async def complete_stream_async(
+        self, prompt: str, request_settings: CompleteRequestSettings
+    ):
+        try:
+            import transformers
+
+            generation_config = transformers.GenerationConfig(
+                temperature=request_settings.temperature,
+                top_p=request_settings.top_p,
+                max_new_tokens=request_settings.max_tokens,
+                pad_token_id=50256,  # EOS token
+            )
+            tokenizer = transformers.AutoTokenizer.from_pretrained(self._model_id)
+            streamer = transformers.TextIteratorStreamer(tokenizer)
+            args = {"prompt": prompt}
+            kwargs = {
+                "num_return_sequences": 1,
+                "generation_config": generation_config,
+                "streamer": streamer,
+            }
+
+            thread = Thread(target=self.generator, args=args, kwargs=kwargs)
+            thread.start()
+
+            for new_text in streamer:
+                yield new_text
+
+            thread.join()
+
+        except Exception as e:
+            raise AIException("Hugging Face completion failed", e)
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,147 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
-from typing import Any, List, Optional, Tuple
+from typing import Any, Optional
 
 import openai
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
-from semantic_kernel.connectors.ai.chat_completion_client_base import (
-    ChatCompletionClientBase,
-)
-from semantic_kernel.connectors.ai.chat_request_settings import ChatRequestSettings
 from semantic_kernel.connectors.ai.complete_request_settings import (
     CompleteRequestSettings,
 )
 from semantic_kernel.connectors.ai.text_completion_client_base import (
     TextCompletionClientBase,
 )
 from semantic_kernel.utils.null_logger import NullLogger
 
 
-class OpenAIChatCompletion(ChatCompletionClientBase, TextCompletionClientBase):
+class OpenAITextCompletion(TextCompletionClientBase):
     _model_id: str
     _api_key: str
-    _org_id: Optional[str] = None
     _api_type: Optional[str] = None
     _api_version: Optional[str] = None
     _endpoint: Optional[str] = None
+    _org_id: Optional[str] = None
     _log: Logger
 
     def __init__(
         self,
         model_id: str,
         api_key: str,
         org_id: Optional[str] = None,
         api_type: Optional[str] = None,
         api_version: Optional[str] = None,
         endpoint: Optional[str] = None,
         log: Optional[Logger] = None,
     ) -> None:
         """
-        Initializes a new instance of the OpenAIChatCompletion class.
+        Initializes a new instance of the OpenAITextCompletion class.
 
         Arguments:
             model_id {str} -- OpenAI model name, see
                 https://platform.openai.com/docs/models
             api_key {str} -- OpenAI API key, see
                 https://platform.openai.com/account/api-keys
             org_id {Optional[str]} -- OpenAI organization ID.
                 This is usually optional unless your
                 account belongs to multiple organizations.
         """
         self._model_id = model_id
         self._api_key = api_key
-        self._org_id = org_id
         self._api_type = api_type
         self._api_version = api_version
         self._endpoint = endpoint
+        self._org_id = org_id
         self._log = log if log is not None else NullLogger()
-        self._messages = []
 
-    async def complete_chat_async(
-        self, messages: List[Tuple[str, str]], request_settings: ChatRequestSettings
+    async def complete_async(
+        self, prompt: str, request_settings: CompleteRequestSettings
     ) -> str:
+        # TODO: tracking on token counts/etc.
+        response = await self._send_completion_request(prompt, request_settings, False)
+        return response.choices[0].text
+
+    # TODO: complete w/ multiple...
+
+    async def complete_stream_async(
+        self, prompt: str, request_settings: CompleteRequestSettings
+    ):
+        response = await self._send_completion_request(prompt, request_settings, True)
+        async for chunk in response:
+            yield chunk.choices[0].text
+
+    async def _send_completion_request(
+        self, prompt: str, request_settings: CompleteRequestSettings, stream: bool
+    ):
         """
-        Completes the given user message. Returns a single string completion.
+        Completes the given prompt. Returns a single string completion.
+        Cannot return multiple completions. Cannot return logprobs.
 
         Arguments:
-            user_message {str} -- The message (from a user) to respond to.
-            request_settings {ChatRequestSettings} -- The request settings.
+            prompt {str} -- The prompt to complete.
+            request_settings {CompleteRequestSettings} -- The request settings.
 
         Returns:
             str -- The completed text.
         """
+        if not prompt:
+            raise ValueError("The prompt cannot be `None` or empty")
         if request_settings is None:
             raise ValueError("The request settings cannot be `None`")
 
         if request_settings.max_tokens < 1:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
                 "The max tokens must be greater than 0, "
                 f"but was {request_settings.max_tokens}",
             )
 
-        if len(messages) <= 0:
+        if request_settings.number_of_responses != 1:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
-                "To complete a chat you need at least one message",
+                "complete_async only supports a single completion, "
+                f"but {request_settings.number_of_responses} were requested",
             )
 
-        if messages[-1][0] != "user":
+        if request_settings.logprobs != 0:
             raise AIException(
                 AIException.ErrorCodes.InvalidRequest,
-                "The last message must be from the user",
+                "complete_async does not support logprobs, "
+                f"but logprobs={request_settings.logprobs} was requested",
             )
 
         model_args = {}
         if self._api_type in ["azure", "azure_ad"]:
             model_args["engine"] = self._model_id
         else:
             model_args["model"] = self._model_id
 
-        formatted_messages = [
-            {"role": role, "content": message} for role, message in messages
-        ]
-
         try:
-            response: Any = await openai.ChatCompletion.acreate(
+            response: Any = await openai.Completion.acreate(
                 **model_args,
                 api_key=self._api_key,
                 api_type=self._api_type,
                 api_base=self._endpoint,
                 api_version=self._api_version,
                 organization=self._org_id,
-                messages=formatted_messages,
+                prompt=prompt,
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 presence_penalty=request_settings.presence_penalty,
                 frequency_penalty=request_settings.frequency_penalty,
                 max_tokens=request_settings.max_tokens,
+                stream=stream,
+                stop=(
+                    request_settings.stop_sequences
+                    if request_settings.stop_sequences is not None
+                    and len(request_settings.stop_sequences) > 0
+                    else None
+                ),
             )
         except Exception as ex:
             raise AIException(
                 AIException.ErrorCodes.ServiceError,
-                "OpenAI service failed to complete the chat",
+                "OpenAI service failed to complete the prompt",
                 ex,
             )
-
-        # TODO: tracking on token counts/etc.
-
-        return response.choices[0].message.content
-
-    async def complete_async(
-        self, prompt: str, request_settings: CompleteRequestSettings
-    ) -> str:
-        """
-        Completes the given prompt. Returns a single string completion.
-        Cannot return multiple completions. Cannot return logprobs.
-
-        Arguments:
-            prompt {str} -- The prompt to complete.
-            request_settings {CompleteRequestSettings} -- The request settings.
-
-        Returns:
-            str -- The completed text.
-        """
-        prompt_to_message = [("user", prompt)]
-        chat_settings = ChatRequestSettings(
-            temperature=request_settings.temperature,
-            top_p=request_settings.top_p,
-            presence_penalty=request_settings.presence_penalty,
-            frequency_penalty=request_settings.frequency_penalty,
-            max_tokens=request_settings.max_tokens,
-        )
-        return await self.complete_chat_async(prompt_to_message, chat_settings)
+        return response
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,11 +12,10 @@
 
 __all__ = [
     "TextMemorySkill",
     "TextSkill",
     "FileIOSkill",
     "TimeSkill",
     "HttpSkill",
-    "BasicPlanner",
     "ConversationSummarySkill",
     "MathSkill",
 ]
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/kernel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+import glob
+import importlib
 import inspect
+import os
 from logging import Logger
 from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union
+from uuid import uuid4
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.chat_completion_client_base import (
     ChatCompletionClientBase,
 )
 from semantic_kernel.connectors.ai.chat_request_settings import ChatRequestSettings
 from semantic_kernel.connectors.ai.complete_request_settings import (
@@ -14,28 +18,31 @@
 )
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import (
     EmbeddingGeneratorBase,
 )
 from semantic_kernel.connectors.ai.text_completion_client_base import (
     TextCompletionClientBase,
 )
-from semantic_kernel.kernel_base import KernelBase
 from semantic_kernel.kernel_exception import KernelException
-from semantic_kernel.kernel_extensions import KernelExtensions
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.memory.null_memory import NullMemory
+from semantic_kernel.memory.semantic_text_memory import SemanticTextMemory
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.orchestration.sk_function import SKFunction
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.reliability.pass_through_without_retry import (
     PassThroughWithoutRetry,
 )
-from semantic_kernel.reliability.retry_mechanism import RetryMechanism
+from semantic_kernel.reliability.retry_mechanism_base import RetryMechanismBase
+from semantic_kernel.semantic_functions.prompt_template import PromptTemplate
+from semantic_kernel.semantic_functions.prompt_template_config import (
+    PromptTemplateConfig,
+)
 from semantic_kernel.semantic_functions.semantic_function_config import (
     SemanticFunctionConfig,
 )
 from semantic_kernel.skill_definition.read_only_skill_collection_base import (
     ReadOnlySkillCollectionBase,
 )
 from semantic_kernel.skill_definition.skill_collection import SkillCollection
@@ -46,15 +53,15 @@
 )
 from semantic_kernel.utils.null_logger import NullLogger
 from semantic_kernel.utils.validation import validate_function_name, validate_skill_name
 
 T = TypeVar("T")
 
 
-class Kernel(KernelBase, KernelExtensions):
+class Kernel:
     _log: Logger
     _skill_collection: SkillCollectionBase
     _prompt_template_engine: PromptTemplatingEngine
     _memory: SemanticTextMemoryBase
 
     def __init__(
         self,
@@ -71,31 +78,28 @@
             prompt_template_engine
             if prompt_template_engine
             else PromptTemplateEngine(self._log)
         )
         self._memory = memory if memory else NullMemory()
 
         self._text_completion_services: Dict[
-            str, Callable[["KernelBase"], TextCompletionClientBase]
+            str, Callable[["Kernel"], TextCompletionClientBase]
         ] = {}
         self._chat_services: Dict[
-            str, Callable[["KernelBase"], ChatCompletionClientBase]
+            str, Callable[["Kernel"], ChatCompletionClientBase]
         ] = {}
         self._text_embedding_generation_services: Dict[
-            str, Callable[["KernelBase"], EmbeddingGeneratorBase]
+            str, Callable[["Kernel"], EmbeddingGeneratorBase]
         ] = {}
 
         self._default_text_completion_service: Optional[str] = None
         self._default_chat_service: Optional[str] = None
         self._default_text_embedding_generation_service: Optional[str] = None
 
-        self._retry_mechanism: RetryMechanism = PassThroughWithoutRetry()
-
-    def kernel(self) -> KernelBase:
-        return self
+        self._retry_mechanism: RetryMechanismBase = PassThroughWithoutRetry()
 
     @property
     def logger(self) -> Logger:
         return self._log
 
     @property
     def memory(self) -> SemanticTextMemoryBase:
@@ -208,14 +212,37 @@
 
     def func(self, skill_name: str, function_name: str) -> SKFunctionBase:
         if self.skills.has_native_function(skill_name, function_name):
             return self.skills.get_native_function(skill_name, function_name)
 
         return self.skills.get_semantic_function(skill_name, function_name)
 
+    def use_memory(
+        self,
+        storage: MemoryStoreBase,
+        embeddings_generator: Optional[EmbeddingGeneratorBase] = None,
+    ) -> None:
+        if embeddings_generator is None:
+            service_id = self.get_text_embedding_generation_service_id()
+            if not service_id:
+                raise ValueError("The embedding service id cannot be `None` or empty")
+
+            embeddings_service = self.get_ai_service(EmbeddingGeneratorBase, service_id)
+            if not embeddings_service:
+                raise ValueError(f"AI configuration is missing for: {service_id}")
+
+            embeddings_generator = embeddings_service(self)
+
+        if storage is None:
+            raise ValueError("The storage instance provided cannot be `None`")
+        if embeddings_generator is None:
+            raise ValueError("The embedding generator cannot be `None`")
+
+        self.register_memory(SemanticTextMemory(storage, embeddings_generator))
+
     def register_memory(self, memory: SemanticTextMemoryBase) -> None:
         self._memory = memory
 
     def register_memory_store(self, memory_store: MemoryStoreBase) -> None:
         self.use_memory(memory_store)
 
     def create_new_context(self) -> SKContext:
@@ -263,15 +290,15 @@
             self._skill_collection.add_native_function(function)
             skill[function.name] = function
 
         return skill
 
     def get_ai_service(
         self, type: Type[T], service_id: Optional[str] = None
-    ) -> Callable[["KernelBase"], T]:
+    ) -> Callable[["Kernel"], T]:
         matching_type = {}
         if type == TextCompletionClientBase:
             service_id = service_id or self._default_text_completion_service
             matching_type = self._text_completion_services
         elif type == ChatCompletionClientBase:
             service_id = service_id or self._default_chat_service
             matching_type = self._chat_services
@@ -297,15 +324,15 @@
     def all_text_embedding_generation_services(self) -> List[str]:
         return list(self._text_embedding_generation_services.keys())
 
     def add_text_completion_service(
         self,
         service_id: str,
         service: Union[
-            TextCompletionClientBase, Callable[["KernelBase"], TextCompletionClientBase]
+            TextCompletionClientBase, Callable[["Kernel"], TextCompletionClientBase]
         ],
         overwrite: bool = True,
     ) -> "Kernel":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
         if not overwrite and service_id in self._text_completion_services:
             raise ValueError(
@@ -320,15 +347,15 @@
 
         return self
 
     def add_chat_service(
         self,
         service_id: str,
         service: Union[
-            ChatCompletionClientBase, Callable[["KernelBase"], ChatCompletionClientBase]
+            ChatCompletionClientBase, Callable[["Kernel"], ChatCompletionClientBase]
         ],
         overwrite: bool = True,
     ) -> "Kernel":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
         if not overwrite and service_id in self._chat_services:
             raise ValueError(
@@ -348,15 +375,15 @@
 
         return self
 
     def add_text_embedding_generation_service(
         self,
         service_id: str,
         service: Union[
-            EmbeddingGeneratorBase, Callable[["KernelBase"], EmbeddingGeneratorBase]
+            EmbeddingGeneratorBase, Callable[["Kernel"], EmbeddingGeneratorBase]
         ],
         overwrite: bool = False,
     ) -> "Kernel":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
         if not overwrite and service_id in self._text_embedding_generation_services:
             raise ValueError(
@@ -563,7 +590,141 @@
                     "Function description: "
                     "{function_config.prompt_template_config.description}",
                 )
 
             function.set_ai_service(lambda: service(self))
 
         return function
+
+    def import_native_skill_from_directory(
+        self, parent_directory: str, skill_directory_name: str
+    ) -> Dict[str, SKFunctionBase]:
+        MODULE_NAME = "native_function"
+
+        validate_skill_name(skill_directory_name)
+
+        skill_directory = os.path.abspath(
+            os.path.join(parent_directory, skill_directory_name)
+        )
+        native_py_file_path = os.path.join(skill_directory, f"{MODULE_NAME}.py")
+
+        if not os.path.exists(native_py_file_path):
+            raise ValueError(
+                f"Native Skill Python File does not exist: {native_py_file_path}"
+            )
+
+        skill_name = os.path.basename(skill_directory)
+        try:
+            spec = importlib.util.spec_from_file_location(
+                MODULE_NAME, native_py_file_path
+            )
+            module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(module)
+
+            class_name = next(
+                (
+                    name
+                    for name, cls in inspect.getmembers(module, inspect.isclass)
+                    if cls.__module__ == MODULE_NAME
+                ),
+                None,
+            )
+            if class_name:
+                skill_obj = getattr(module, class_name)()
+                return self.import_skill(skill_obj, skill_name)
+        except Exception:
+            pass
+
+        return {}
+
+    def import_semantic_skill_from_directory(
+        self, parent_directory: str, skill_directory_name: str
+    ) -> Dict[str, SKFunctionBase]:
+        CONFIG_FILE = "config.json"
+        PROMPT_FILE = "skprompt.txt"
+
+        validate_skill_name(skill_directory_name)
+
+        skill_directory = os.path.join(parent_directory, skill_directory_name)
+        skill_directory = os.path.abspath(skill_directory)
+
+        if not os.path.exists(skill_directory):
+            raise ValueError(f"Skill directory does not exist: {skill_directory_name}")
+
+        skill = {}
+
+        directories = glob.glob(skill_directory + "/*/")
+        for directory in directories:
+            dir_name = os.path.dirname(directory)
+            function_name = os.path.basename(dir_name)
+            prompt_path = os.path.join(directory, PROMPT_FILE)
+
+            # Continue only if the prompt template exists
+            if not os.path.exists(prompt_path):
+                continue
+
+            config = PromptTemplateConfig()
+            config_path = os.path.join(directory, CONFIG_FILE)
+            with open(config_path, "r") as config_file:
+                config = config.from_json(config_file.read())
+
+            # Load Prompt Template
+            with open(prompt_path, "r") as prompt_file:
+                template = PromptTemplate(
+                    prompt_file.read(), self.prompt_template_engine, config
+                )
+
+            # Prepare lambda wrapping AI logic
+            function_config = SemanticFunctionConfig(config, template)
+
+            skill[function_name] = self.register_semantic_function(
+                skill_directory_name, function_name, function_config
+            )
+
+        return skill
+
+    def create_semantic_function(
+        self,
+        prompt_template: str,
+        function_name: Optional[str] = None,
+        skill_name: Optional[str] = None,
+        description: Optional[str] = None,
+        max_tokens: int = 256,
+        temperature: float = 0.0,
+        top_p: float = 1.0,
+        presence_penalty: float = 0.0,
+        frequency_penalty: float = 0.0,
+        stop_sequences: Optional[List[str]] = None,
+    ) -> "SKFunctionBase":
+        function_name = (
+            function_name
+            if function_name is not None
+            else f"f_{str(uuid4()).replace('-', '_')}"
+        )
+
+        config = PromptTemplateConfig(
+            description=(
+                description
+                if description is not None
+                else "Generic function, unknown purpose"
+            ),
+            type="completion",
+            completion=PromptTemplateConfig.CompletionConfig(
+                temperature,
+                top_p,
+                presence_penalty,
+                frequency_penalty,
+                max_tokens,
+                stop_sequences if stop_sequences is not None else [],
+            ),
+        )
+
+        validate_function_name(function_name)
+        if skill_name is not None:
+            validate_skill_name(skill_name)
+
+        template = PromptTemplate(prompt_template, self.prompt_template_engine, config)
+        function_config = SemanticFunctionConfig(config, template)
+
+        return self.register_semantic_function(
+            skill_name, function_name, function_config
+        )
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from typing import List, Tuple
 
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 
-class MemoryStoreBase:
+class MemoryStoreBase(ABC):
     @abstractmethod
     async def create_collection_async(self, collection_name: str) -> None:
         pass
 
     @abstractmethod
     async def get_collections_async(
         self,
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,16 +143,16 @@
         matches = matches and _return_is_str(signature)
         matches = matches and awaitable
         return matches
 
     @staticmethod
     @_infers(DelegateTypes.InStringAndContext)
     def infer_in_string_and_context(signature: Signature, awaitable: bool) -> bool:
-        matches = _first_param_is_str(signature)
-        matches = matches and _first_param_is_context(signature)
+        matches = _first_param_is_str(signature, only=False)
+        matches = matches and _has_two_params_second_is_context(signature)
         matches = matches and _no_return(signature)
         matches = matches and not awaitable
         return matches
 
     @staticmethod
     @_infers(DelegateTypes.InStringAndContextOutString)
     def infer_in_string_and_context_out_string(
@@ -219,15 +219,15 @@
         matches = _has_no_params(signature)
         matches = matches and _no_return(signature)
         matches = matches and awaitable
         return matches
 
     @staticmethod
     @_infers(DelegateTypes.Unknown)
-    def infer_unknown(signature: Signature) -> NoReturn:
+    def infer_unknown(signature: Signature, awaitable: bool) -> NoReturn:
         raise KernelException(
             KernelException.ErrorCodes.FunctionTypeNotSupported,
             "Invalid function type detected, unable to infer DelegateType.",
         )
 
     @staticmethod
     def infer_delegate_type(function) -> DelegateTypes:
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 [OUTPUT]
     {
         "input": "Valentine's Day Date Ideas",
         "subtasks": [
             {"function": "WriterSkill.Brainstorm"},
             {"function": "EdgarAllenPoeSkill.Poe"},
             {"function": "WriterSkill.EmailTo", "args": {"recipient": "significant_other"}},
-            {"function": "translate", "args": {"language": "French"}}
+            {"function": "WriterSkill.Translate", "args": {"language": "French"}}
         ]
     }
 
 [AVAILABLE FUNCTIONS]
 {{$available_functions}}
 
 [GOAL]
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from typing import Awaitable, Callable, TypeVar
 
-from semantic_kernel.reliability.retry_mechanism import RetryMechanism
+from semantic_kernel.reliability.retry_mechanism_base import RetryMechanismBase
 
 T = TypeVar("T")
 
 
-class PassThroughWithoutRetry(RetryMechanism):
+class PassThroughWithoutRetry(RetryMechanismBase):
     """A retry mechanism that does not retry."""
 
     async def execute_with_retry_async(
         self, action: Callable[[], Awaitable[T]], log: logging.Logger
     ) -> Awaitable[T]:
         """Executes the given action with retry logic.
```

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.9.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.8.dev0/PKG-INFO` & `semantic_kernel-0.2.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.2.8.dev0
+Version: 0.2.9.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

