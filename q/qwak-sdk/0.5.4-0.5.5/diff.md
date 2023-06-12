# Comparing `tmp/qwak_sdk-0.5.4.tar.gz` & `tmp/qwak_sdk-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_sdk-0.5.4.tar", max compression
+gzip compressed data, was "qwak_sdk-0.5.5.tar", max compression
```

## Comparing `qwak_sdk-0.5.4.tar` & `qwak_sdk-0.5.5.tar`

### file list

```diff
@@ -1,302 +1,303 @@
--rw-r--r--   0        0        0      183 2023-05-23 09:13:41.962545 qwak_sdk-0.5.4/README.md
--rw-r--r--   0        0        0     2608 2023-05-23 09:14:33.918873 qwak_sdk-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      134 2023-05-23 09:14:33.918873 qwak_sdk-0.5.4/qwak_sdk/__init__.py
--rw-r--r--   0        0        0     2039 2023-05-23 09:13:41.962545 qwak_sdk-0.5.4/qwak_sdk/cli.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.962545 qwak_sdk-0.5.4/qwak_sdk/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.962545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/__init__.py
--rw-r--r--   0        0        0      327 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/admin_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/__init__.py
--rw-r--r--   0        0        0      467 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/__init__.py
--rw-r--r--   0        0        0      677 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/_logic.py
--rw-r--r--   0        0        0     1393 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
--rw-r--r--   0        0        0      796 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
--rw-r--r--   0        0        0      942 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/__init__.py
--rw-r--r--   0        0        0      367 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/config_base.py
--rw-r--r--   0        0        0      885 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
--rw-r--r--   0        0        0      886 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
--rw-r--r--   0        0        0     1626 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
--rw-r--r--   0        0        0      817 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
--rw-r--r--   0        0        0      340 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
--rw-r--r--   0        0        0      277 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/spec.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/__init__.py
--rw-r--r--   0        0        0       49 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
--rw-r--r--   0        0        0     3326 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/config.py
--rw-r--r--   0        0        0      646 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/__init__.py
--rw-r--r--   0        0        0     1359 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/_logic.py
--rw-r--r--   0        0        0      949 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/ui.py
--rw-r--r--   0        0        0      277 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/__init__.py
--rw-r--r--   0        0        0      857 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/automations_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/delete/__init__.py
--rw-r--r--   0        0        0      235 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/delete/_logic.py
--rw-r--r--   0        0        0      604 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/delete/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/__init__.py
--rw-r--r--   0        0        0      346 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/executions_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/list/__init__.py
--rw-r--r--   0        0        0      330 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/list/_logic.py
--rw-r--r--   0        0        0      669 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/list/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/list/__init__.py
--rw-r--r--   0        0        0      252 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/list/_logic.py
--rw-r--r--   0        0        0      546 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/list/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/__init__.py
--rw-r--r--   0        0        0     1624 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/_logic.py
--rw-r--r--   0        0        0     1331 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/_logic.py
--rw-r--r--   0        0        0     1039 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/ui.py
--rw-r--r--   0        0        0     1002 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/feature_store_command_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/list/__init__.py
--rw-r--r--   0        0        0     4145 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/list/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/pause/__init__.py
--rw-r--r--   0        0        0      695 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/pause/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/__init__.py
--rw-r--r--   0        0        0    10893 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/_logic.py
--rw-r--r--   0        0        0     2822 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/resume/__init__.py
--rw-r--r--   0        0        0      700 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/resume/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/trigger/__init__.py
--rw-r--r--   0        0        0     1015 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/trigger/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/_logic/__init__.py
--rw-r--r--   0        0        0     2050 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/__init__.py
--rw-r--r--   0        0        0     2005 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/build_steps.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
--rw-r--r--   0        0        0     6185 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
--rw-r--r--   0        0        0     4383 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
--rw-r--r--   0        0        0     2908 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
--rw-r--r--   0        0        0     1369 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
--rw-r--r--   0        0        0     1435 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
--rw-r--r--   0        0        0      359 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
--rw-r--r--   0        0        0      975 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
--rw-r--r--   0        0        0      311 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
--rw-r--r--   0        0        0     9258 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/config/config_v1.py
--rw-r--r--   0        0        0      131 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
--rw-r--r--   0        0        0      881 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/step_description.py
--rw-r--r--   0        0        0       73 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
--rw-r--r--   0        0        0      189 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
--rw-r--r--   0        0        0     1872 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/context.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/__init__.py
--rw-r--r--   0        0        0      568 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
--rw-r--r--   0        0        0      745 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/__init__.py
--rw-r--r--   0        0        0      421 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
--rw-r--r--   0        0        0     1929 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      957 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     1917 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     2589 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     2025 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2232 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     4459 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
--rw-r--r--   0        0        0     5385 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
--rw-r--r--   0        0        0      274 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      611 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1605 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0    11882 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0      183 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
--rw-r--r--   0        0        0     2169 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
--rw-r--r--   0        0        0     1644 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/__init__.py
--rw-r--r--   0        0        0     1686 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
--rw-r--r--   0        0        0     1181 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
--rw-r--r--   0        0        0      188 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/text.py
--rw-r--r--   0        0        0     6357 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/__init__.py
--rw-r--r--   0        0        0      491 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/builds_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/cancel/__init__.py
--rw-r--r--   0        0        0      181 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/cancel/_logic.py
--rw-r--r--   0        0        0      518 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/cancel/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/logs/__init__.py
--rw-r--r--   0        0        0     1054 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/logs/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/status/__init__.py
--rw-r--r--   0        0        0      256 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/status/_logic.py
--rw-r--r--   0        0        0      973 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/status/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/create/__init__.py
--rw-r--r--   0        0        0     1335 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/create/_logic.py
--rw-r--r--   0        0        0     1016 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/create/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/delete/__init__.py
--rw-r--r--   0        0        0      186 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/delete/_logic.py
--rw-r--r--   0        0        0      638 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/delete/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
--rw-r--r--   0        0        0     1251 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
--rw-r--r--   0        0        0     2494 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
--rw-r--r--   0        0        0     8227 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
--rw-r--r--   0        0        0    13221 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
--rw-r--r--   0        0        0     3900 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
--rw-r--r--   0        0        0     5799 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
--rw-r--r--   0        0        0      770 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
--rw-r--r--   0        0        0     1067 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
--rw-r--r--   0        0        0     3166 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
--rw-r--r--   0        0        0      495 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      903 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3015 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
--rw-r--r--   0        0        0      500 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
--rw-r--r--   0        0        0      902 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      907 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3621 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     4917 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
--rw-r--r--   0        0        0      905 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
--rw-r--r--   0        0        0     1500 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     5381 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
--rw-r--r--   0        0        0     5773 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
--rw-r--r--   0        0        0     3036 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
--rw-r--r--   0        0        0     2083 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/cancel/__init__.py
--rw-r--r--   0        0        0      409 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/cancel/_logic.py
--rw-r--r--   0        0        0      828 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/cancel/ui.py
--rw-r--r--   0        0        0      789 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/execution_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/__init__.py
--rw-r--r--   0        0        0      533 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/_logic.py
--rw-r--r--   0        0        0     1435 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/__init__.py
--rw-r--r--   0        0        0      605 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/_logic.py
--rw-r--r--   0        0        0     5158 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/status/__init__.py
--rw-r--r--   0        0        0      480 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/status/_logic.py
--rw-r--r--   0        0        0      820 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/status/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/__init__.py
--rw-r--r--   0        0        0     1375 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
--rw-r--r--   0        0        0       35 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       84 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      164 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0   129370 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3610 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0     1030 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
--rw-r--r--   0        0        0       41 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       74 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      161 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0    53393 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3967 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
--rw-r--r--   0        0        0      139 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      120 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
--rw-r--r--   0        0        0      140 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
--rw-r--r--   0        0        0     2169 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
--rw-r--r--   0        0        0      117 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
--rw-r--r--   0        0        0       61 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      182 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0     3353 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      751 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
--rw-r--r--   0        0        0       68 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0      448 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      752 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0     1906 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/list/__init__.py
--rw-r--r--   0        0        0      166 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/list/_logic.py
--rw-r--r--   0        0        0     1135 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/list/ui.py
--rw-r--r--   0        0        0     1241 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/models_command_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/__init__.py
--rw-r--r--   0        0        0     2678 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/_logic.py
--rw-r--r--   0        0        0     1378 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/logs/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/logs/ui.py
--rw-r--r--   0        0        0      693 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/runtime_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
--rw-r--r--   0        0        0     1811 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
--rw-r--r--   0        0        0     3160 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
--rw-r--r--   0        0        0     1212 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/update/__init__.py
--rw-r--r--   0        0        0      393 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/update/_logic.py
--rw-r--r--   0        0        0      622 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/update/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/create/__init__.py
--rw-r--r--   0        0        0      259 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/create/_logic.py
--rw-r--r--   0        0        0      691 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/create/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/delete/__init__.py
--rw-r--r--   0        0        0      203 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/delete/_logic.py
--rw-r--r--   0        0        0      557 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/delete/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/list/__init__.py
--rw-r--r--   0        0        0      182 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/list/_logic.py
--rw-r--r--   0        0        0     1124 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/list/ui.py
--rw-r--r--   0        0        0      589 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/projects_command_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/delete/__init__.py
--rw-r--r--   0        0        0      141 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/delete/_logic.py
--rw-r--r--   0        0        0      741 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/delete/ui.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/get/__init__.py
--rw-r--r--   0        0        0      142 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/get/_logic.py
--rw-r--r--   0        0        0      574 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/get/ui.py
--rw-r--r--   0        0        0      502 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/secrets_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/set/__init__.py
--rw-r--r--   0        0        0      149 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/set/_logic.py
--rw-r--r--   0        0        0      615 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/set/ui.py
--rw-r--r--   0        0        0      430 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/ui_tools.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/common/__init__.py
--rw-r--r--   0        0        0      437 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/common/run_config/__init__.py
--rw-r--r--   0        0        0     3166 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/common/run_config/base.py
--rw-r--r--   0        0        0     6087 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/common/run_config/utils.py
--rw-r--r--   0        0        0      381 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0       48 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_command_exception.py
--rw-r--r--   0        0        0      133 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
--rw-r--r--   0        0        0      424 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      130 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0       48 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_resource_not_found.py
--rw-r--r--   0        0        0      746 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/__init__.py
--rw-r--r--   0        0        0     3164 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/file_registry.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/__init__.py
--rw-r--r--   0        0        0     4541 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/cli_tools.py
--rw-r--r--   0        0        0      488 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/config_handler.py
--rw-r--r--   0        0        0       71 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/__init__.py
--rw-r--r--   0        0        0     8869 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/logging.yml
--rw-r--r--   0        0        0     1013 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/tracking.py
--rw-r--r--   0        0        0      136 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/main.py
--rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/__init__.py
--rw-r--r--   0        0        0      287 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/colors.py
--rw-r--r--   0        0        0     2257 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/files.py
--rw-r--r--   0        0        0     5616 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/log_handling.py
--rw-r--r--   0        0        0     1168 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/utils.py
--rw-r--r--   0        0        0     8327 1970-01-01 00:00:00.000000 qwak_sdk-0.5.4/setup.py
--rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 qwak_sdk-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      183 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/README.md
+-rw-r--r--   0        0        0     2609 2023-06-12 14:22:09.524702 qwak_sdk-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-12 14:22:09.524702 qwak_sdk-0.5.5/qwak_sdk/__init__.py
+-rw-r--r--   0        0        0     2039 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/qwak_sdk/cli.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/qwak_sdk/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/__init__.py
+-rw-r--r--   0        0        0      327 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/admin_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/__init__.py
+-rw-r--r--   0        0        0      467 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/generate/__init__.py
+-rw-r--r--   0        0        0      677 2023-06-12 14:21:18.035822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/generate/_logic.py
+-rw-r--r--   0        0        0     1393 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/generate/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
+-rw-r--r--   0        0        0      942 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/revoke/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/config_base.py
+-rw-r--r--   0        0        0      885 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
+-rw-r--r--   0        0        0      886 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
+-rw-r--r--   0        0        0     1626 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
+-rw-r--r--   0        0        0      817 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
+-rw-r--r--   0        0        0      340 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
+-rw-r--r--   0        0        0      277 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/spec.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/_logic/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
+-rw-r--r--   0        0        0     3326 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/_logic/config/config.py
+-rw-r--r--   0        0        0      646 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/attach/__init__.py
+-rw-r--r--   0        0        0     1359 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/attach/_logic.py
+-rw-r--r--   0        0        0      949 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/attach/ui.py
+-rw-r--r--   0        0        0      277 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/__init__.py
+-rw-r--r--   0        0        0      857 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/automations_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/delete/__init__.py
+-rw-r--r--   0        0        0      235 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/delete/_logic.py
+-rw-r--r--   0        0        0      604 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/executions/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/executions/executions_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/executions/list/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/executions/list/_logic.py
+-rw-r--r--   0        0        0      669 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/executions/list/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/list/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/list/_logic.py
+-rw-r--r--   0        0        0      546 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/list/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/register/__init__.py
+-rw-r--r--   0        0        0     1624 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/register/_logic.py
+-rw-r--r--   0        0        0     1331 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/automations/register/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/delete/__init__.py
+-rw-r--r--   0        0        0     1716 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/delete/_logic.py
+-rw-r--r--   0        0        0     1039 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/delete/ui.py
+-rw-r--r--   0        0        0     1002 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/feature_store_command_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/list/__init__.py
+-rw-r--r--   0        0        0     4145 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/list/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/pause/__init__.py
+-rw-r--r--   0        0        0      695 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/pause/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/register/__init__.py
+-rw-r--r--   0        0        0    10893 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/register/_logic.py
+-rw-r--r--   0        0        0     2822 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/register/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/resume/__init__.py
+-rw-r--r--   0        0        0      700 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/resume/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/trigger/__init__.py
+-rw-r--r--   0        0        0     1015 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/trigger/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/_logic/__init__.py
+-rw-r--r--   0        0        0     1497 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/_logic/instance_template.py
+-rw-r--r--   0        0        0     2050 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/__init__.py
+-rw-r--r--   0        0        0     2003 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/build_steps.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
+-rw-r--r--   0        0        0     6185 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
+-rw-r--r--   0        0        0     4383 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
+-rw-r--r--   0        0        0     2908 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
+-rw-r--r--   0        0        0     1369 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
+-rw-r--r--   0        0        0     1435 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
+-rw-r--r--   0        0        0      359 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
+-rw-r--r--   0        0        0      975 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
+-rw-r--r--   0        0        0      311 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
+-rw-r--r--   0        0        0     9548 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/config/config_v1.py
+-rw-r--r--   0        0        0      131 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
+-rw-r--r--   0        0        0      881 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/constant/step_description.py
+-rw-r--r--   0        0        0       73 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
+-rw-r--r--   0        0        0      189 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
+-rw-r--r--   0        0        0     1911 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/context.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/interface/__init__.py
+-rw-r--r--   0        0        0      568 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
+-rw-r--r--   0        0        0      745 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
+-rw-r--r--   0        0        0     1929 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     1917 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     2589 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     4731 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     2025 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2232 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     4459 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
+-rw-r--r--   0        0        0     7241 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0      274 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1605 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0    12278 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0      182 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
+-rw-r--r--   0        0        0     2169 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
+-rw-r--r--   0        0        0     2249 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/util/__init__.py
+-rw-r--r--   0        0        0     1686 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
+-rw-r--r--   0        0        0     1181 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
+-rw-r--r--   0        0        0      188 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/util/text.py
+-rw-r--r--   0        0        0     6701 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/build/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/builds_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/cancel/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/cancel/_logic.py
+-rw-r--r--   0        0        0      518 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/cancel/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/logs/__init__.py
+-rw-r--r--   0        0        0     1054 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/logs/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/status/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/status/_logic.py
+-rw-r--r--   0        0        0      973 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/status/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/create/__init__.py
+-rw-r--r--   0        0        0     1335 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/create/_logic.py
+-rw-r--r--   0        0        0     1016 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/create/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/delete/__init__.py
+-rw-r--r--   0        0        0      186 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/delete/_logic.py
+-rw-r--r--   0        0        0      638 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
+-rw-r--r--   0        0        0     1251 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
+-rw-r--r--   0        0        0     2652 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
+-rw-r--r--   0        0        0     8355 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
+-rw-r--r--   0        0        0    13221 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
+-rw-r--r--   0        0        0     4087 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
+-rw-r--r--   0        0        0     5799 2023-06-12 14:21:18.039822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
+-rw-r--r--   0        0        0     2167 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
+-rw-r--r--   0        0        0     1067 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
+-rw-r--r--   0        0        0     3166 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      946 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3182 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
+-rw-r--r--   0        0        0      500 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
+-rw-r--r--   0        0        0      902 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      950 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3621 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     4714 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
+-rw-r--r--   0        0        0      948 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     1500 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     5548 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/undeploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
+-rw-r--r--   0        0        0     5773 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
+-rw-r--r--   0        0        0     3036 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
+-rw-r--r--   0        0        0     2083 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/undeploy/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/cancel/__init__.py
+-rw-r--r--   0        0        0      409 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/cancel/_logic.py
+-rw-r--r--   0        0        0      828 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/cancel/ui.py
+-rw-r--r--   0        0        0      789 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/execution_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/report/__init__.py
+-rw-r--r--   0        0        0      533 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/report/_logic.py
+-rw-r--r--   0        0        0     1435 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/report/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/start/__init__.py
+-rw-r--r--   0        0        0      926 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/start/_logic.py
+-rw-r--r--   0        0        0     5328 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/start/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/status/__init__.py
+-rw-r--r--   0        0        0      480 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/status/_logic.py
+-rw-r--r--   0        0        0      820 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/status/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/__init__.py
+-rw-r--r--   0        0        0     1375 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
+-rw-r--r--   0        0        0       35 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0   129370 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3640 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0     1030 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
+-rw-r--r--   0        0        0       41 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       74 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0    53393 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3994 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
+-rw-r--r--   0        0        0     2169 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0     3353 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0     3353 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0      448 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      752 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0     1906 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/init/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/list/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/list/_logic.py
+-rw-r--r--   0        0        0     1135 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/list/ui.py
+-rw-r--r--   0        0        0     1241 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/models_command_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/feedback/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/feedback/_logic.py
+-rw-r--r--   0        0        0     1378 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/feedback/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/logs/__init__.py
+-rw-r--r--   0        0        0     1577 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/logs/ui.py
+-rw-r--r--   0        0        0      693 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/runtime_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
+-rw-r--r--   0        0        0     1811 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
+-rw-r--r--   0        0        0     3160 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
+-rw-r--r--   0        0        0     1212 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/traffic_update/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/update/__init__.py
+-rw-r--r--   0        0        0      393 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/update/_logic.py
+-rw-r--r--   0        0        0      622 2023-06-12 14:21:18.043822 qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/update/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/create/__init__.py
+-rw-r--r--   0        0        0      259 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/create/_logic.py
+-rw-r--r--   0        0        0      691 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/create/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/delete/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/delete/_logic.py
+-rw-r--r--   0        0        0      557 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/list/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/list/_logic.py
+-rw-r--r--   0        0        0     1124 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/list/ui.py
+-rw-r--r--   0        0        0      589 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/projects/projects_command_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/delete/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/delete/_logic.py
+-rw-r--r--   0        0        0      741 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/get/__init__.py
+-rw-r--r--   0        0        0      142 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/get/_logic.py
+-rw-r--r--   0        0        0      574 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/get/ui.py
+-rw-r--r--   0        0        0      502 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/secrets_commands_group.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/set/__init__.py
+-rw-r--r--   0        0        0      149 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/set/_logic.py
+-rw-r--r--   0        0        0      615 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/secrets/set/ui.py
+-rw-r--r--   0        0        0      430 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/commands/ui_tools.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/common/__init__.py
+-rw-r--r--   0        0        0      437 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/common/run_config/__init__.py
+-rw-r--r--   0        0        0     3166 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/common/run_config/base.py
+-rw-r--r--   0        0        0     6087 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/common/run_config/utils.py
+-rw-r--r--   0        0        0      381 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/exceptions/qwak_command_exception.py
+-rw-r--r--   0        0        0      133 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
+-rw-r--r--   0        0        0      424 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      130 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0       48 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/exceptions/qwak_resource_not_found.py
+-rw-r--r--   0        0        0      746 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/__init__.py
+-rw-r--r--   0        0        0     3164 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/file_registry.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/tools/__init__.py
+-rw-r--r--   0        0        0     4541 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/tools/cli_tools.py
+-rw-r--r--   0        0        0      488 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/tools/config_handler.py
+-rw-r--r--   0        0        0       71 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/tools/logger/__init__.py
+-rw-r--r--   0        0        0     8869 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/tools/logger/logging.yml
+-rw-r--r--   0        0        0     1013 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/inner/tools/tracking.py
+-rw-r--r--   0        0        0      136 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/tools/__init__.py
+-rw-r--r--   0        0        0      287 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/tools/colors.py
+-rw-r--r--   0        0        0     2257 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/tools/files.py
+-rw-r--r--   0        0        0     5616 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/tools/log_handling.py
+-rw-r--r--   0        0        0     1168 2023-06-12 14:21:18.047822 qwak_sdk-0.5.5/qwak_sdk/tools/utils.py
+-rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 qwak_sdk-0.5.5/setup.py
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 qwak_sdk-0.5.5/PKG-INFO
```

### Comparing `qwak_sdk-0.5.4/pyproject.toml` & `qwak_sdk-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-sdk"
-version = "0.5.4"
+version = "0.5.5"
 description = "Qwak SDK and CLI for qwak models"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak_sdk"},
 ]
@@ -23,16 +23,16 @@
 "Home page" = "https://www.qwak.com/"
 
 [tool.poetry.scripts]
 qwak = "qwak_sdk.main:qwak_cli"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-qwak-core = "==0.0.69"
-qwak-inference = "==0.1.2"
+qwak-core = "==0.0.106"
+qwak-inference = "==0.1.4"
 tabulate = ">=0.8.0"
 python-json-logger = ">=2.0.2"
 pydantic = "*"
 yaspin = ">=2.0.0"
 assertpy = "^1.1"
 cookiecutter = "*"
 gitpython = ">=2.1.0"
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/cli.py` & `qwak_sdk-0.5.5/qwak_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/generate/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/generate/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/revoke/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/admin/apikeys/revoke/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/parser.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/config.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/_logic/config/config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/parser.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/attach/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/auto_scalling/attach/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/automations/automations_commands_group.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/automations/automations_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/automations/delete/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/automations/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/list/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/automations/executions/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/automations/list/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/automations/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/automations/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/automations/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/delete/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/feature_store_command_group.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/feature_store_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/list/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/pause/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/pause/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/resume/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/resume/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/trigger/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/feature_store/trigger/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/_logic/variations.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/build_steps.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/build_steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .config.config_v1 import ConfigV1
 from .constant.step_description import BuildPhase, PhaseDetails
 from .context import Context
 from .interface.step_inteface import Step
 from .phase.a_fetch_model_code import get_fetch_model_code_steps
 from .phase.b_remote_register_qwak_build import get_remote_register_qwak_build_steps
-from .phase.c_deploy import get_deploy_stepss
+from .phase.c_deploy import get_deploy_steps
 
 
 class StepsPipeline:
     def __init__(
         self,
         config: ConfigV1,
         context: Context = None,
@@ -57,12 +57,12 @@
     steps_root.add_phase(
         steps=get_remote_register_qwak_build_steps(),
         build_phase=BuildPhase.REGISTERING_QWAK_BUILD,
     )
 
     if config.deploy:
         steps_root.add_phase(
-            steps=get_deploy_stepss(),
+            steps=get_deploy_steps(),
             build_phase=BuildPhase.DEPLOY_PHASE,
         )
 
     return steps_root
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/logger.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/messages.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/messages.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/config/config_v1.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/config/config_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,19 @@
         "iam_role_arn", "build_env.docker.assumed_iam_role_arn", validate_string
     ),
     # RemoteConf
     ConfigCliMap("cpus", "build_env.remote.resources.cpus", validate_float),
     ConfigCliMap("memory", "build_env.remote.resources.memory", validate_string),
     ConfigCliMap("gpu_type", "build_env.remote.resources.gpu_type", validate_string),
     ConfigCliMap("gpu_amount", "build_env.remote.resources.gpu_amount", validate_int),
+    ConfigCliMap("instance", "build_env.remote.resources.instance", validate_string),
     # Verbosity level
     ConfigCliMap("verbose", "verbose", validate_int),
     ConfigCliMap("deploy", "deploy", validate_bool),
+    ConfigCliMap("deployment_instance", "deployment_instance", validate_string),
 ]
 
 
 @protobuf_factory(BuildConfiguration, exclude_fields=["deploy"])
 @dataclass
 class ConfigV1(YamlConfigMixin, QwakConfigBase):
     @property
@@ -191,14 +193,15 @@
             @protobuf_factory(RemoteBuildResources)
             @dataclass
             class RemoteBuildResources:
                 cpus: Optional[float] = field(default=None)
                 memory: Optional[str] = field(default=None)
                 gpu_type: Optional[str] = field(default=None)
                 gpu_amount: Optional[int] = field(default=None)
+                instance: Optional[str] = field(default=None)
 
             is_remote: bool = field(default=True)
             resources: RemoteBuildResources = field(
                 default_factory=RemoteBuildResources
             )
 
         docker: DockerConf = field(default_factory=DockerConf)
@@ -207,14 +210,15 @@
 
     build_properties: BuildProperties = field(default_factory=BuildProperties)
     build_env: Optional[BuildEnv] = field(default_factory=BuildEnv)
     pre_build: Optional[BuildEnv] = field(default=None)
     post_build: Optional[BuildEnv] = field(default=None)
     step: Step = field(default_factory=Step)
     deploy: bool = field(default=False)
+    deployment_instance: Optional[str] = field(default=None)
     verbose: int = field(default=0)
 
     def __post_init__(self):
         if (
             self.build_env.remote.resources.gpu_type
             and self.build_env.docker.base_image
             == ConfigV1.BuildEnv.DockerConf.base_image
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/step_description.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/constant/step_description.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/context.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/context.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 
-from qwak.clients.build_management import BuildsManagementClient
 from qwak.clients.build_orchestrator import BuildOrchestratorClient
+from qwak.clients.instance_template.client import InstanceTemplateManagementClient
 from qwak.clients.model_management import ModelsManagementClient
 from qwak.inner.di_configuration import UserAccountConfiguration
 from qwak.inner.di_configuration.account import UserAccount
 
 
 class DependencyManagerType(Enum):
     UNKNOWN = 0
@@ -21,20 +21,20 @@
 
 @dataclass
 class Context:
     # Clients
     client_builds_orchestrator: BuildOrchestratorClient = field(
         default_factory=BuildOrchestratorClient
     )
-    client_build_management: BuildsManagementClient = field(
-        default_factory=BuildsManagementClient
-    )
     client_models_management: ModelsManagementClient = field(
         default_factory=ModelsManagementClient
     )
+    client_instance_template: InstanceTemplateManagementClient = field(
+        default_factory=InstanceTemplateManagementClient
+    )
 
     # General
     user_account: UserAccount = field(
         default_factory=UserAccountConfiguration().get_user_config
     )
 
     # Pre fetch validation
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,25 +88,27 @@
             )
             dirs_to_include += deps_folders
 
         self.notifier.debug("Zipping skinny model code")
         skinny_size_zip_file = zip_model(
             build_dir=self.context.host_temp_local_build_dir,
             dependency_file=self.context.model_relative_dependency_file,
+            deps_lock_file=self.context.model_relative_dependency_lock_file,
             dirs_to_include=dirs_to_include,
             zip_name="skinny_size_model_code",
             ignored_patterns=ignored_patterns,
             max_bytes=_MAX_FILE_SIZE_BYTES,
         )
 
         # Full size model
         self.notifier.debug("Zipping full model code")
         full_size_zip_file = zip_model(
             build_dir=self.context.host_temp_local_build_dir,
             dependency_file=self.context.model_relative_dependency_file,
+            deps_lock_file=self.context.model_relative_dependency_lock_file,
             dirs_to_include=dirs_to_include,
             zip_name="full_size_model_code",
             ignored_patterns=ignored_patterns,
         )
 
         # Dump config file for upload
         config_file_temp = self.context.host_temp_local_build_dir / "build.conf"
@@ -238,14 +240,15 @@
 def zip_model(
     build_dir: Path,
     dependency_file: Path,
     dirs_to_include: list[str],
     zip_name: str,
     ignored_patterns: Iterable[str],
     max_bytes: Optional[int] = None,
+    deps_lock_file: Optional[Path] = None,
 ):
     try:
         filtered_model = build_dir / zip_name
         ignored_patterns = get_files_to_ignore(
             directory=build_dir / TEMP_LOCAL_MODEL_DIR, patterns=ignored_patterns
         )
 
@@ -256,17 +259,20 @@
                     src=build_dir / TEMP_LOCAL_MODEL_DIR / included_dir,
                     dst=filtered_model / included_dir,
                     ignore=shutil.ignore_patterns(*ignored_patterns),
                     dirs_exist_ok=True,
                 )
 
         deps_file = build_dir / TEMP_LOCAL_MODEL_DIR / dependency_file
-
         shutil.copy(deps_file, filtered_model / dependency_file)
 
+        if deps_lock_file:
+            deps_lock_file_full_path = build_dir / TEMP_LOCAL_MODEL_DIR / deps_lock_file
+            shutil.copy(deps_lock_file_full_path, filtered_model / deps_lock_file)
+
         _replace_large_files_with_too_large_file_message(filtered_model, max_bytes)
 
         zip_path = Path(
             shutil.make_archive(
                 base_name=str(filtered_model),
                 format="zip",
                 root_dir=filtered_model,
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 from __future__ import annotations
 
-from typing import Any, Dict
+from typing import List
+
+from _qwak_proto.qwak.instance_template.instance_template_pb2 import (
+    InstanceTemplateSpec,
+    InstanceType,
+)
 
 from qwak_sdk.commands.models.build._logic.client_logs.messages import (
     FAILED_DEPLOY_BUILD_SUGGESTION,
 )
 from qwak_sdk.commands.models.build._logic.interface.step_inteface import Step
 from qwak_sdk.commands.models.deployments.deploy.realtime.ui import deploy_realtime
 from qwak_sdk.exceptions.qwak_deploy_new_build_failed import (
     QwakDeployNewBuildFailedException,
 )
 
 
 class DeployBuildStep(Step):
-    SMALL_DEPLOYMENT: Dict[str, Any] = {
-        "pods": 1,
-        "cpus": 2,
-        "memory": 2048,
-    }
     DEPLOY_FAILURE_EXCEPTION_MESSAGE = "Deploying the build failed due to {e}"
 
     def description(self) -> str:
         return "Deploying Build"
 
     def execute(self) -> None:
         self.notifier.info(f"Deploying build {self.context.build_id}")
         try:
+            if self.config.deployment_instance:
+                template_id = self.config.deployment_instance
+            else:
+                template_id = self.get_smallest_deployment_template_id()
             deploy_config = {
                 "build_id": self.context.build_id,
                 "model_id": self.context.model_id,
+                "instance": template_id,
             }
-            deploy_config.update(self.SMALL_DEPLOYMENT)
             deploy_realtime(from_file=None, out_conf=False, sync=False, **deploy_config)
             self.notifier.info(f"Finished deploying build {self.context.build_id}")
         except Exception as e:
             raise QwakDeployNewBuildFailedException(
                 message=self.DEPLOY_FAILURE_EXCEPTION_MESSAGE.format(e=e),
                 suggestion=FAILED_DEPLOY_BUILD_SUGGESTION.format(
                     build_id=self.context.build_id,
                     model_id=self.context.model_id,
                     project_uuid=self.context.project_uuid,
                 ),
             )
+
+    def get_smallest_deployment_template_id(self):
+        instances: List[
+            InstanceTemplateSpec
+        ] = self.context.client_instance_template.list_instance_templates()
+        return list(
+            filter(
+                lambda template: template.order == 1
+                and template.instance_type == InstanceType.INSTANCE_TYPE_CPU,
+                instances,
+            )
+        )[0].id
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/step_decorator.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/_logic/util/step_decorator.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/build/ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -183,14 +183,28 @@
     "--deploy",
     help="Whether you want to deploy the build if it finishes successfully. "
     "Choosing this will follow the build process in the terminal and will trigger a deployment when the "
     "build finishes.",
     default=False,
     is_flag=True,
 )
+@click.option(
+    "--instance",
+    required=False,
+    type=str,
+    help="The instance size to build on - 'small', 'medium', 'large', etc...",
+    default=None,
+)
+@click.option(
+    "--deployment-instance",
+    required=False,
+    type=str,
+    help="The instance size to deploy on - 'small', 'medium', 'large', etc...",
+    default=None,
+)
 @click.argument("uri", required=False)
 def models_build(**kwargs):
     return build(**kwargs)
 
 
 def build(
     from_file: str,
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/cancel/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/cancel/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/logs/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/status/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/builds/status/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/create/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/create/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/create/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/delete/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from time import sleep
 from typing import List
 
 from _qwak_proto.qwak.deployment.deployment_pb2 import ModelDeploymentStatus
 from _qwak_proto.qwak.deployment.deployment_service_pb2 import DeployModelResponse
 from qwak.clients.administration.eco_system.client import EcosystemClient
 from qwak.clients.deployment.client import DeploymentManagementClient
+from qwak.clients.instance_template.client import InstanceTemplateManagementClient
 from qwak.inner.di_configuration import UserAccountConfiguration
 
 from qwak_sdk.commands.models.deployments.deploy._logic.deploy_config import (
     DeployConfig,
 )
 
 FAILED_STATUS = [
@@ -22,14 +23,15 @@
 
 class BaseDeployExecutor(ABC):
     def __init__(self, config: DeployConfig):
         self.config = config
         self.deploy_client = DeploymentManagementClient()
         self.ecosystem_client = EcosystemClient()
         self.user_config = UserAccountConfiguration().get_user_config()
+        self.instance_template_client = InstanceTemplateManagementClient()
 
     def poll_until_complete(self, deployment_id: str, poll_period: int):
         def deployment_status():
             status_response = self.deploy_client.get_deployment_status(
                 deployment_named_id=deployment_id
             )
             if ModelDeploymentStatus.Name(status_response.status) in END_STATUSES:
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     # Batch
     # Resources
     ConfigCliMap("pods", "resources.pods", validate_int, False),
     ConfigCliMap("cpus", "resources.cpus", validate_int, False),
     ConfigCliMap("memory", "resources.memory", validate_int, False),
     ConfigCliMap("gpu_type", "resources.gpu_type", validate_string, False),
     ConfigCliMap("gpu_amount", "resources.gpu_amount", validate_int, False),
+    ConfigCliMap("instance", "resources.instance_size", validate_string, False),
     # Permissions
     ConfigCliMap(
         "iam_role_arn", "advanced_options.iam_role_arn", validate_string, False
     ),
     ConfigCliMap(
         "purchase_option",
         "advanced_options.purchase_option",
@@ -220,14 +221,15 @@
     @dataclass
     class Resources:
         pods: int = field(default=1)
         cpus: int = field(default=2)
         memory: int = field(default=512)
         gpu_type: str = field(default=None)
         gpu_amount: int = field(default=0)
+        instance_size: str = field(default="")
 
     @dataclass
     class AdvancedOptions:
         iam_role_arn: str = field(default=None)
         purchase_option: str = field(default=PurchaseOption.SPOT.value)
 
     model_id: str = field(default="")
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     HostingService,
     KubeDeployment,
     KubeDeploymentType,
     ServingStrategy,
 )
 from qwak.clients.administration.eco_system.client import EcosystemClient
 from qwak.clients.deployment.client import DeploymentManagementClient
+from qwak.clients.instance_template.client import InstanceTemplateManagementClient
 from qwak.exceptions import QwakException
 
 from qwak_sdk.commands.models.deployments.deploy._logic.advance_deployment_options_handler import (
     get_advanced_deployment_options_from_deploy_config,
 )
 from qwak_sdk.commands.models.deployments.deploy._logic.deploy_config import (
     DeployConfig,
@@ -37,16 +38,19 @@
 
 
 def get_env_to_deployment_message(
     deploy_config: DeployConfig,
     kube_deployment_type: KubeDeploymentType,
     deployment_client: DeploymentManagementClient,
     ecosystem_client: EcosystemClient,
+    instance_template_client: InstanceTemplateManagementClient,
 ) -> Dict[str, EnvironmentDeploymentMessage]:
-    deployment_size = deployment_size_from_deploy_config(deploy_config)
+    deployment_size = deployment_size_from_deploy_config(
+        deploy_config, instance_template_client
+    )
     advanced_deployment_options = get_advanced_deployment_options_from_deploy_config(
         deploy_config, kube_deployment_type
     )
     environment_variables = {}
     if kube_deployment_type == KubeDeploymentType.ONLINE:
         model_traffic = deployment_client.get_model_traffic_config(
             deploy_config.model_id
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 class BatchDeployExecutor(BaseDeployExecutor):
     def deploy(self) -> DeployModelResponse:
         env_deployment_messages = get_env_to_deployment_message(
             self.config,
             KubeDeploymentType.BATCH,
             self.deploy_client,
             self.ecosystem_client,
+            self.instance_template_client,
         )
         return self.deploy_client.deploy_model(
             model_id=self.config.model_id,
             build_id=self.config.build_id,
             env_deployment_messages=env_deployment_messages,
         )
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/batch/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,14 +86,21 @@
 )
 @click.option(
     "--purchase-option",
     required=False,
     type=click.Choice([i.value for i in PurchaseOption], case_sensitive=False),
     help="Indicate the instance deployments type, whether it is spot/ondemand.  Default is spot",
 )
+@click.option(
+    "--instance",
+    required=False,
+    type=str,
+    help="The instance size to deploy on - 'small', 'medium', 'large', etc...",
+    default=None,
+)
 def batch(verbose: bool, from_file: str, out_conf: bool, sync: bool, **kwargs):
     set_qwak_logger_stdout_verbosity_level(verbose + 1)
     config: DeployConfig = config_handler(
         config=DeployConfig,
         from_file=from_file,
         out_conf=out_conf,
         sections=("batch",),
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 class RealtimeDeployExecutor(BaseDeployExecutor):
     def deploy(self) -> DeployModelResponse:
         env_deployment_messages = get_env_to_deployment_message(
             self.config,
             KubeDeploymentType.ONLINE,
             self.deploy_client,
             self.ecosystem_client,
+            self.instance_template_client,
         )
         return self.deploy_client.deploy_model(
             model_id=self.config.model_id,
             build_id=self.config.build_id,
             env_deployment_messages=env_deployment_messages,
         )
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,28 +17,14 @@
 from qwak_sdk.commands.models.deployments.deploy.realtime._logic.deploy_executor import (
     RealtimeDeployExecutor,
 )
 from qwak_sdk.inner.tools.cli_tools import QwakCommand
 from qwak_sdk.inner.tools.config_handler import config_handler
 
 logger = get_qwak_logger()
-PENDING_STATUSES = [
-    "INITIATING_DEPLOYMENT",
-    "PENDING_DEPLOYMENT",
-    "INITIATING_UNDEPLOYMENT",
-    "PENDING_UNDEPLOYMENT",
-]
-DEPLOYED_STATUSES = ["SUCCESSFUL_DEPLOYMENT"]
-UNDEPLOYED_STATUSES = ["SUCCESSFUL_UNDEPLOYMENT"]
-FAILED_STATUSES = [
-    "INVALID_DEPLOYMENT",
-    "FAILED_INITIATING_DEPLOYMENT",
-    "FAILED_DEPLOYMENT",
-    "FAILED_UNDEPLOYMENT",
-]
 
 
 @click.command("realtime", help="Deploy realtime model.", cls=QwakCommand)
 @click.option(
     "--build-id",
     help="Build ID, If not specified latest successful build will deployed.",
     type=str,
@@ -141,28 +127,35 @@
 @click.option(
     "--purchase-option",
     required=False,
     type=click.Choice([i.value for i in PurchaseOption], case_sensitive=False),
     help="Indicate the instance deployments type, whether it is spot/ondemand. Default is spot",
 )
 @click.option(
-    "--deployments-timeout",
+    "--deployment-timeout",
     type=int,
     help="The number of seconds the deployments can be in progress before it is considered as failed. This is useful "
     "in cases where a deployments has a high number of pods to replace, scarce resources (gpu), or large build "
     "size. Default is 1800 seconds (30 minutes).",
 )
 @click.option(
     "-E",
     "--env-vars",
     required=False,
     metavar="NAME=VALUE",
     multiple=True,
     help="A parameter for the deployments, of the form -E name=value",
 )
+@click.option(
+    "--instance",
+    required=False,
+    type=str,
+    help="The instance size to deploy on - 'small', 'medium', 'large', etc...",
+    default=None,
+)
 def realtime(
     verbose: bool, from_file: Optional[str], out_conf: bool, sync: bool, **kwargs
 ):
     set_qwak_logger_stdout_verbosity_level(verbose + 1)
     deploy_realtime(from_file, out_conf, sync, **kwargs)
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 class StreamDeployExecutor(BaseDeployExecutor):
     def deploy(self) -> DeployModelResponse:
         env_deployment_messages = get_env_to_deployment_message(
             self.config,
             KubeDeploymentType.STREAM,
             self.deploy_client,
             self.ecosystem_client,
+            self.instance_template_client,
         )
         return self.deploy_client.deploy_model(
             model_id=self.config.model_id,
             build_id=self.config.build_id,
             env_deployment_messages=env_deployment_messages,
         )
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,14 +176,21 @@
     "-E",
     "--env-vars",
     required=False,
     metavar="NAME=VALUE",
     multiple=True,
     help="A parameter for the deployments, of the form -E name=value",
 )
+@click.option(
+    "--instance",
+    required=False,
+    type=str,
+    help="The instance size to deploy on - 'small', 'medium', 'large', etc...",
+    default=None,
+)
 def stream(
     verbose: bool, from_file: str, out_conf: bool, local: bool, sync: bool, **kwargs
 ):
     set_qwak_logger_stdout_verbosity_level(verbose + 1)
     config: DeployConfig = config_handler(
         config=DeployConfig,
         from_file=from_file,
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/deployments/undeploy/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/cancel/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/cancel/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/execution_commands_group.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/execution_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/report/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/report/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/start/_logic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from typing import Tuple
 
 from qwak.clients.batch_job_management import BatchJobManagerClient
 from qwak.clients.batch_job_management.executions_config import ExecutionConfig
 from qwak.clients.batch_job_management.results import StartExecutionResult
+from qwak.clients.instance_template.client import InstanceTemplateManagementClient
+
+from qwak_sdk.commands.models._logic.instance_template import verify_template_id
 
 
 def execute_start_execution(config: ExecutionConfig) -> Tuple[str, bool, str]:
+    if config.resources.instance_size:
+        verify_template_id(
+            config.resources.instance_size, InstanceTemplateManagementClient()
+        )
     batch_job_start_response: StartExecutionResult = (
         BatchJobManagerClient().start_execution(config)
     )
     return (
         batch_job_start_response.execution_id,
         batch_job_start_response.success,
         batch_job_start_response.failure_message,
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/start/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,21 @@
     "-P",
     "--param-list",
     required=False,
     metavar="NAME=VALUE",
     multiple=True,
     help="A parameter for the batch execution, of the form -P name=value",
 )
+@click.option(
+    "--instance",
+    required=False,
+    type=str,
+    help="The instance size to run batch on - 'small', 'medium', 'large', etc...",
+    default=None,
+)
 def execution_start(from_file: str, out_conf: bool, **kwargs):
     config: ExecutionConfig = config_handler(
         config=ExecutionConfig,
         from_file=from_file,
         out_conf=out_conf,
         sections=("execution", "resources"),
         **kwargs,
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/status/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/executions/status/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,9 +87,9 @@
         )
         return model_schema
 
     @qwak.api()
     def predict(self, df):
         df = df.drop(["User_Id"], axis=1)
         return pd.DataFrame(
-            self.catboost.predict_proba(df)[:, 1], columns=["Churn_Probability"]
+            self.catboost.predict_proba(df[self.catboost.feature_names_])[:, 1], columns=["Churn_Probability"]
         )
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,9 +100,9 @@
             outputs=[InferenceOutput(name="Default_Probability", type=float)],
         )
 
     @qwak.api()
     def predict(self, df: pd.DataFrame) -> pd.DataFrame:
         df = df.drop(["UserId"], axis=1)
         return pd.DataFrame(
-            self.model.predict_proba(df)[:, 1], columns=["Default_Probability"]
+            self.model.predict_proba(df[self.model.feature_names_])[:, 1], columns=["Default_Probability"]
         )
```

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/init/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/list/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/models_command_group.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/models_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/_logic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/feedback/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/feedback/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/logs/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/runtime_commands_group.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/runtime_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/traffic_update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/update/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/models/runtime/update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/projects/create/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/projects/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/projects/delete/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/projects/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/projects/list/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/projects/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/projects/projects_command_group.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/projects/projects_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/secrets/delete/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/secrets/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/secrets/get/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/secrets/get/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/commands/secrets/set/ui.py` & `qwak_sdk-0.5.5/qwak_sdk/commands/secrets/set/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/common/run_config/base.py` & `qwak_sdk-0.5.5/qwak_sdk/common/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/common/run_config/utils.py` & `qwak_sdk-0.5.5/qwak_sdk/common/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_suggestion_exception.py` & `qwak_sdk-0.5.5/qwak_sdk/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/inner/file_registry.py` & `qwak_sdk-0.5.5/qwak_sdk/inner/file_registry.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/inner/tools/cli_tools.py` & `qwak_sdk-0.5.5/qwak_sdk/inner/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/logger.py` & `qwak_sdk-0.5.5/qwak_sdk/inner/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/logging.yml` & `qwak_sdk-0.5.5/qwak_sdk/inner/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/inner/tools/tracking.py` & `qwak_sdk-0.5.5/qwak_sdk/inner/tools/tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/tools/files.py` & `qwak_sdk-0.5.5/qwak_sdk/tools/files.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/tools/log_handling.py` & `qwak_sdk-0.5.5/qwak_sdk/tools/log_handling.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/qwak_sdk/tools/utils.py` & `qwak_sdk-0.5.5/qwak_sdk/tools/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.4/setup.py` & `qwak_sdk-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,16 @@
 
 install_requires = \
 ['assertpy>=1.1,<2.0',
  'cookiecutter',
  'gitpython>=2.1.0',
  'pydantic',
  'python-json-logger>=2.0.2',
- 'qwak-core==0.0.69',
- 'qwak-inference==0.1.2',
+ 'qwak-core==0.0.106',
+ 'qwak-inference==0.1.4',
  'tabulate>=0.8.0',
  'yaspin>=2.0.0']
 
 extras_require = \
 {'batch': ['boto3>=1.24.116,<2.0.0',
            'joblib>=1.1.0,<2.0.0',
            'pyarrow>=6.0.0,<11.0.0'],
@@ -147,15 +147,15 @@
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['qwak = qwak_sdk.main:qwak_cli']}
 
 setup_kwargs = {
     'name': 'qwak-sdk',
-    'version': '0.5.4',
+    'version': '0.5.5',
     'description': 'Qwak SDK and CLI for qwak models',
     'long_description': '# Qwak SDK\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_sdk-0.5.4/PKG-INFO` & `qwak_sdk-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sdk
-Version: 0.5.4
+Version: 0.5.5
 Summary: Qwak SDK and CLI for qwak models
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,16 +25,16 @@
 Requires-Dist: gitpython (>=2.1.0)
 Requires-Dist: joblib (>=1.1.0,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: pandas (<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pandas (>=1.4.3,<2.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pyarrow (>=6.0.0,<11.0.0) ; extra == "batch"
 Requires-Dist: pydantic
 Requires-Dist: python-json-logger (>=2.0.2)
-Requires-Dist: qwak-core (==0.0.69)
-Requires-Dist: qwak-inference (==0.1.2)
+Requires-Dist: qwak-core (==0.0.106)
+Requires-Dist: qwak-inference (==0.1.4)
 Requires-Dist: tabulate (>=0.8.0)
 Requires-Dist: yaspin (>=2.0.0)
 Project-URL: Home page, https://www.qwak.com/
 Description-Content-Type: text/markdown
 
 # Qwak SDK
```

