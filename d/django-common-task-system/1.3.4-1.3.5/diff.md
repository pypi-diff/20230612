# Comparing `tmp/django-common-task-system-1.3.4.tar.gz` & `tmp/django-common-task-system-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.3.4.tar", last modified: Thu May 25 03:49:47 2023, max compression
+gzip compressed data, was "django-common-task-system-1.3.5.tar", last modified: Mon Jun 12 02:00:18 2023, max compression
```

## Comparing `django-common-task-system-1.3.4.tar` & `django-common-task-system-1.3.5.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.094928 django-common-task-system-1.3.4/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.3.4/LICENSE
--rw-rw-rw-   0        0        0      189 2023-05-20 07:32:40.000000 django-common-task-system-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      307 2023-05-25 03:49:47.094928 django-common-task-system-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.3.4/README.md
--rw-rw-rw-   0        0        0        0 2023-05-24 09:43:33.000000 django-common-task-system-1.3.4/deploy.sh
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.027918 django-common-task-system-1.3.4/django_common_task_system/
--rw-rw-rw-   0        0        0     3015 2023-05-24 09:35:14.000000 django-common-task-system-1.3.4/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0    11644 2023-05-17 06:20:23.000000 django-common-task-system-1.3.4/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.3.4/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.3.4/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0    20540 2023-05-23 08:16:03.000000 django-common-task-system-1.3.4/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.051130 django-common-task-system-1.3.4/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7635 2023-05-23 09:02:13.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
--rw-rw-rw-   0        0        0      490 2023-05-09 02:37:58.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/0008_taskschedule_strict_mode.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.3.4/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.3.4/django_common_task_system/mixin.py
--rw-rw-rw-   0        0        0    37016 2023-05-23 09:01:47.000000 django-common-task-system-1.3.4/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.3.4/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2756 2023-05-25 02:51:03.000000 django-common-task-system-1.3.4/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.013409 django-common-task-system-1.3.4/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.013409 django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.052130 django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.054137 django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
--rw-rw-rw-   0        0        0     1688 2023-05-23 08:07:41.000000 django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/js/task_type_admin.js
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.056138 django-common-task-system-1.3.4/django_common_task_system/static/custom_programs/
--rw-rw-rw-   0        0        0       29 2023-05-23 06:02:29.000000 django-common-task-system-1.3.4/django_common_task_system/static/custom_programs/python_test.py
--rw-rw-rw-   0        0        0       19 2023-05-18 09:30:02.000000 django-common-task-system-1.3.4/django_common_task_system/static/custom_programs/shell_test.sh
--rw-rw-rw-   0        0        0      317 2023-05-23 06:44:01.000000 django-common-task-system-1.3.4/django_common_task_system/static/custom_programs/zip_test.zip
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.063792 django-common-task-system-1.3.4/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     5370 2023-05-25 03:17:35.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0    15100 2023-05-25 02:25:35.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/builtins.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     8704 2023-05-23 08:21:17.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.068799 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10423 2023-05-23 09:02:19.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
--rw-rw-rw-   0        0        0      454 2023-05-09 02:37:58.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0008_systemschedule_strict_mode.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0     4706 2023-05-15 05:40:55.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      877 2023-05-15 09:14:29.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     6405 2023-05-18 08:18:37.000000 django-common-task-system-1.3.4/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.070243 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.073384 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     2542 2023-05-25 02:44:13.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.079929 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      669 2023-05-18 08:40:30.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-18 09:42:50.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     5738 2023-05-23 06:41:42.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/custom_program.py
--rw-rw-rw-   0        0        0     3543 2023-05-25 03:47:30.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      834 2023-05-15 07:46:24.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     2170 2023-05-23 08:40:46.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0    11026 2023-05-17 09:31:21.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/settings.py
--rw-rw-rw-   0        0        0     1258 2023-05-17 09:10:41.000000 django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.015409 django-common-task-system-1.3.4/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.015409 django-common-task-system-1.3.4/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.079929 django-common-task-system-1.3.4/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.3.4/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.084930 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      576 2023-05-22 09:21:21.000000 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/custom_program.html
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0      689 2023-05-23 08:02:57.000000 django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/sql_config.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.3.4/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0     1089 2023-05-15 09:14:29.000000 django-common-task-system-1.3.4/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.087931 django-common-task-system-1.3.4/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.3.4/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.3.4/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.3.4/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0     1150 2023-05-25 02:36:14.000000 django-common-task-system-1.3.4/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.3.4/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    12546 2023-05-25 03:48:44.000000 django-common-task-system-1.3.4/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.043869 django-common-task-system-1.3.4/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-25 03:49:46.000000 django-common-task-system-1.3.4/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5612 2023-05-25 03:49:47.000000 django-common-task-system-1.3.4/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 03:49:46.000000 django-common-task-system-1.3.4/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-25 03:49:46.000000 django-common-task-system-1.3.4/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       59 2023-05-25 03:49:46.000000 django-common-task-system-1.3.4/django_common_task_system.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.090929 django-common-task-system-1.3.4/django_common_task_system_server/
--rw-rw-rw-   0        0        0        0 2023-05-24 03:33:23.000000 django-common-task-system-1.3.4/django_common_task_system_server/__init__.py
--rw-rw-rw-   0        0        0      684 2023-05-24 09:44:29.000000 django-common-task-system-1.3.4/django_common_task_system_server/manage.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.093927 django-common-task-system-1.3.4/django_common_task_system_server/server/
--rw-rw-rw-   0        0        0        0 2023-05-24 02:04:52.000000 django-common-task-system-1.3.4/django_common_task_system_server/server/__init__.py
--rw-rw-rw-   0        0        0      405 2023-05-24 02:04:52.000000 django-common-task-system-1.3.4/django_common_task_system_server/server/asgi.py
--rw-rw-rw-   0        0        0     3537 2023-05-24 09:22:43.000000 django-common-task-system-1.3.4/django_common_task_system_server/server/settings.py
--rw-rw-rw-   0        0        0      769 2023-05-24 02:04:52.000000 django-common-task-system-1.3.4/django_common_task_system_server/server/urls.py
--rw-rw-rw-   0        0        0      405 2023-05-24 02:04:52.000000 django-common-task-system-1.3.4/django_common_task_system_server/server/wsgi.py
--rw-rw-rw-   0        0        0       42 2023-05-25 03:49:47.094928 django-common-task-system-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-05-25 03:48:50.000000 django-common-task-system-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 03:49:47.093927 django-common-task-system-1.3.4/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.3.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:18.167201 django-common-task-system-1.3.5/
+-rw-rw-rw-   0        0        0      873 2023-05-24 08:34:51.000000 django-common-task-system-1.3.5/Dockerfile
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0      189 2023-05-26 08:17:44.000000 django-common-task-system-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      307 2023-06-12 02:00:18.166202 django-common-task-system-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.619871 django-common-task-system-1.3.5/django_common_task_system/
+-rw-rw-rw-   0        0        0     3015 2023-05-24 09:35:14.000000 django-common-task-system-1.3.5/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    11644 2023-05-17 06:20:23.000000 django-common-task-system-1.3.5/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.3.5/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.3.5/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0    20540 2023-05-23 08:16:03.000000 django-common-task-system-1.3.5/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.702099 django-common-task-system-1.3.5/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7635 2023-05-23 09:02:13.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
+-rw-rw-rw-   0        0        0      490 2023-05-09 02:37:58.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/0008_taskschedule_strict_mode.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.3.5/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.3.5/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    37094 2023-05-26 08:18:29.000000 django-common-task-system-1.3.5/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.3.5/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2756 2023-05-25 02:51:03.000000 django-common-task-system-1.3.5/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.508350 django-common-task-system-1.3.5/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.508350 django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.718104 django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.778967 django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+-rw-rw-rw-   0        0        0     1688 2023-05-23 08:07:41.000000 django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/js/task_type_admin.js
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.798732 django-common-task-system-1.3.5/django_common_task_system/static/custom_programs/
+-rw-rw-rw-   0        0        0       29 2023-05-23 06:02:29.000000 django-common-task-system-1.3.5/django_common_task_system/static/custom_programs/python_test.py
+-rw-rw-rw-   0        0        0       19 2023-05-18 09:30:02.000000 django-common-task-system-1.3.5/django_common_task_system/static/custom_programs/shell_test.sh
+-rw-rw-rw-   0        0        0      317 2023-05-23 06:44:01.000000 django-common-task-system-1.3.5/django_common_task_system/static/custom_programs/zip_test.zip
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.877375 django-common-task-system-1.3.5/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     5370 2023-05-25 03:17:35.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0    15100 2023-05-25 02:25:35.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/builtins.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     8704 2023-05-23 08:21:17.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.935028 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10423 2023-05-23 09:02:19.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
+-rw-rw-rw-   0        0        0      454 2023-05-09 02:37:58.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0008_systemschedule_strict_mode.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4706 2023-05-15 05:40:55.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      877 2023-05-15 09:14:29.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     6405 2023-05-18 08:18:37.000000 django-common-task-system-1.3.5/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.941535 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.970186 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-05-25 02:44:13.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:18.013889 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      669 2023-05-18 08:40:30.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-18 09:42:50.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     5738 2023-05-23 06:41:42.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/custom_program.py
+-rw-rw-rw-   0        0        0     3543 2023-05-25 03:47:30.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      835 2023-06-12 01:57:50.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     2230 2023-05-25 09:36:19.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0    11026 2023-05-17 09:31:21.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/settings.py
+-rw-rw-rw-   0        0        0     1258 2023-05-17 09:10:41.000000 django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.509354 django-common-task-system-1.3.5/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.509354 django-common-task-system-1.3.5/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:18.038344 django-common-task-system-1.3.5/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.3.5/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:18.101293 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      576 2023-05-22 09:21:21.000000 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/custom_program.html
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0      689 2023-05-23 08:02:57.000000 django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/sql_config.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.3.5/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0     1089 2023-05-15 09:14:29.000000 django-common-task-system-1.3.5/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:18.129166 django-common-task-system-1.3.5/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.3.5/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.3.5/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.3.5/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0     1150 2023-05-25 02:36:14.000000 django-common-task-system-1.3.5/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.3.5/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    12546 2023-05-25 03:48:44.000000 django-common-task-system-1.3.5/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:17.641127 django-common-task-system-1.3.5/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-06-12 02:00:17.000000 django-common-task-system-1.3.5/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5665 2023-06-12 02:00:17.000000 django-common-task-system-1.3.5/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:00:17.000000 django-common-task-system-1.3.5/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-06-12 02:00:17.000000 django-common-task-system-1.3.5/django_common_task_system.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      122 2023-06-12 02:00:17.000000 django-common-task-system-1.3.5/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       59 2023-06-12 02:00:17.000000 django-common-task-system-1.3.5/django_common_task_system.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:18.135274 django-common-task-system-1.3.5/django_common_task_system_server/
+-rw-rw-rw-   0        0        0        0 2023-05-24 03:33:23.000000 django-common-task-system-1.3.5/django_common_task_system_server/__init__.py
+-rw-rw-rw-   0        0        0     3411 2023-05-26 09:58:56.000000 django-common-task-system-1.3.5/django_common_task_system_server/manage.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:18.164687 django-common-task-system-1.3.5/django_common_task_system_server/server/
+-rw-rw-rw-   0        0        0        0 2023-05-24 02:04:52.000000 django-common-task-system-1.3.5/django_common_task_system_server/server/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-05-24 02:04:52.000000 django-common-task-system-1.3.5/django_common_task_system_server/server/asgi.py
+-rw-rw-rw-   0        0        0     3628 2023-05-26 09:09:46.000000 django-common-task-system-1.3.5/django_common_task_system_server/server/settings.py
+-rw-rw-rw-   0        0        0      918 2023-05-26 07:44:07.000000 django-common-task-system-1.3.5/django_common_task_system_server/server/urls.py
+-rw-rw-rw-   0        0        0      405 2023-05-24 02:04:52.000000 django-common-task-system-1.3.5/django_common_task_system_server/server/wsgi.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 02:00:18.167201 django-common-task-system-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-06-12 01:59:32.000000 django-common-task-system-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:18.165192 django-common-task-system-1.3.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.3.5/tests/__init__.py
```

### Comparing `django-common-task-system-1.3.4/LICENSE` & `django-common-task-system-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/__init__.py` & `django-common-task-system-1.3.5/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/admin.py` & `django-common-task-system-1.3.5/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/choices.py` & `django-common-task-system-1.3.5/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/forms.py` & `django-common-task-system-1.3.5/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.3.5/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.3.5/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.3.5/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.3.5/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py` & `django-common-task-system-1.3.5/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/mixin.py` & `django-common-task-system-1.3.5/django_common_task_system/mixin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/models.py` & `django-common-task-system-1.3.5/django_common_task_system/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from . permissions import ConsumerPermissionValidator
 import re
 import os
 from django.core.validators import ValidationError
 from django.dispatch import Signal, receiver
 from threading import Event
 from collections import OrderedDict
-from django.db.utils import ProgrammingError
+from django.db.utils import ProgrammingError, OperationalError
 
 system_initialize_signal = Signal()
 system_schedule_event = Event()
 system_signal_sent = False
 
 mdays = [0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 
@@ -682,15 +682,15 @@
     model_unique_kwargs = ['code']
 
     def __init__(self):
         super(BaseBuiltinQueues, self).__init__()
         try:
             for m in self.model.objects.filter(status=True):
                 self.add(m)
-        except ProgrammingError:
+        except (ProgrammingError, OperationalError):
             pass
 
     def add(self, instance: AbstractTaskScheduleQueue, key=None):
         if instance.status:
             old = self.get(instance.code)
             if not old or old.module != instance.module or old.config != instance.config:
                 instance.queue = import_string(instance.module)(**instance.config)
@@ -725,15 +725,15 @@
     model_unique_kwargs = ['queue']
 
     def __init__(self):
         super(BaseBuiltinProducers, self).__init__()
         try:
             for m in self.model.objects.filter(status=True):
                 self.add(m)
-        except ProgrammingError:
+        except (ProgrammingError, OperationalError):
             pass
 
     def add(self, instance: AbstractTaskScheduleProducer, key=None):
         if instance.status:
             old = self.get(instance.id)
             if not old or old.queue != instance.queue:
                 self[instance.id] = instance
@@ -775,15 +775,15 @@
     model_unique_kwargs = ['producer', 'type']
 
     def __init__(self):
         super(BaseConsumerPermissions, self).__init__()
         try:
             for m in self.model.objects.filter(status=True):
                 self.add(m)
-        except ProgrammingError:
+        except (ProgrammingError, OperationalError):
             pass
 
     def add(self, instance: AbstractConsumerPermission, key=None):
         if instance.status:
             old = self.get(instance.producer_id)
             if not old or old.type != instance.type or old.config != instance.config:
                 validator = ConsumerPermissionValidator.get(instance.type)
```

### Comparing `django-common-task-system-1.3.4/django_common_task_system/permissions.py` & `django-common-task-system-1.3.5/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/serializers.py` & `django-common-task-system-1.3.5/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/static/common_task_system/js/task_type_admin.js` & `django-common-task-system-1.3.5/django_common_task_system/static/common_task_system/js/task_type_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/builtins.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/builtins.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/models.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/process.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task/views.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/custom_program.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/custom_program.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class ShellExecutor(BaseExecutor):
     name = builtins.tasks.shell_execution_parent_task.name
 
     def execute(self):
         if sys.platform == 'win32':
             raise RuntimeError('Windows系统不支持shell命令执行')
 
-        commands = self.schedule.task.config.get('shell', '').split(';')
+        commands = self.schedule.task.config.get('script', '').split(';')
         filename = '/tmp/shell_executor.sh'
         with open(filename, 'w') as f:
             f.write('#!/bin/bash -e \n')
             f.write('; \n'.join(commands))
         p = subprocess.Popen(f'/bin/bash {filename}', shell=True, stdout=subprocess.PIPE)
         out, err = p.communicate()
         if err:
```

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,17 @@
                 if sql:
                     if sql.lower().startswith('select'):
                         cursor.execute(sql)
                         cmd_result = {
                             'script': sql,
                             'result': cursor.fetchall()
                         }
-                    elif sql.lower().startswith('insert') or sql.lower().startswith('replace'):
-                        raise NoRetryException('insert or replace not support')
+                    elif sql.lower().startswith('replace'):
+                        # 需要允许执行select语句，比如会有insert into select语句的场景
+                        raise NoRetryException('replace not support')
                     else:
                         cmd_result = {
                             'script': sql,
                             'result': cursor.execute(sql)
                         }
                     result.append(cmd_result)
         return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/executors/strict_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/system_task_execution/system_task_execution/utils.py` & `django-common-task-system-1.3.5/django_common_task_system/system_task_execution/system_task_execution/utils.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.3.5/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/custom_program.html` & `django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/custom_program.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/templates/task_schedule/sql_config.html` & `django-common-task-system-1.3.5/django_common_task_system/templates/task_schedule/sql_config.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/urls.py` & `django-common-task-system-1.3.5/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.3.5/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.3.5/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.3.5/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system/views.py` & `django-common-task-system-1.3.5/django_common_task_system/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.3.4/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.3.5/django_common_task_system.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+Dockerfile
 LICENSE
 MANIFEST.in
 README.md
-deploy.sh
 setup.py
 django_common_task_system/__init__.py
 django_common_task_system/admin.py
 django_common_task_system/apps.py
 django_common_task_system/choices.py
 django_common_task_system/forms.py
 django_common_task_system/mixin.py
@@ -14,14 +14,15 @@
 django_common_task_system/serializers.py
 django_common_task_system/tests.py
 django_common_task_system/urls.py
 django_common_task_system/views.py
 django_common_task_system.egg-info/PKG-INFO
 django_common_task_system.egg-info/SOURCES.txt
 django_common_task_system.egg-info/dependency_links.txt
+django_common_task_system.egg-info/entry_points.txt
 django_common_task_system.egg-info/requires.txt
 django_common_task_system.egg-info/top_level.txt
 django_common_task_system/migrations/0001_initial.py
 django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
 django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
 django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
 django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
```

### Comparing `django-common-task-system-1.3.4/django_common_task_system_server/server/settings.py` & `django-common-task-system-1.3.5/django_common_task_system_server/server/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 For more information on this file, see
 https://docs.djangoproject.com/en/4.1/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/4.1/ref/settings/
 """
-
+import os
 from pathlib import Path
 from django_common_objects.settings import rewrite_to
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 
@@ -49,15 +49,15 @@
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
 ]
 
-ROOT_URLCONF = 'server.urls'
+ROOT_URLCONF = 'django_common_task_system_server.server.urls'
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [],
         'APP_DIRS': True,
         'OPTIONS': {
@@ -67,24 +67,24 @@
                 'django.contrib.auth.context_processors.auth',
                 'django.contrib.messages.context_processors.messages',
             ],
         },
     },
 ]
 
-WSGI_APPLICATION = 'server.wsgi.application'
+WSGI_APPLICATION = 'django_common_task_system_server.server.wsgi.application'
 
 
 # Database
 # https://docs.djangoproject.com/en/4.1/ref/settings/#databases
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': BASE_DIR / 'db.sqlite3',
+        'NAME': os.path.join(os.getcwd(), 'db.sqlite3'),
     }
 }
 
 
 # Password validation
 # https://docs.djangoproject.com/en/4.1/ref/settings/#auth-password-validators
```

### Comparing `django-common-task-system-1.3.4/django_common_task_system_server/server/urls.py` & `django-common-task-system-1.3.5/django_common_task_system_server/server/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,14 @@
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.contrib import admin
-from django.urls import path
+from django.urls import path, include
 
 urlpatterns = [
     path('admin/', admin.site.urls),
+    # path('task/', include('django_common_task_system.urls')),
+    path('system', include('django_common_task_system.system_task.urls'))
 ]
```

### Comparing `django-common-task-system-1.3.4/setup.py` & `django-common-task-system-1.3.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests', 'tests']),
-    version='1.3.4',
+    version='1.3.5',
     install_requires=[
-        "django-common-objects>=1.0.7",
+        "django-common-objects>=1.0.8",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
     ],
     include_package_data=True,
     author='cone387',
     maintainer_email='1183008540@qq.com',
     license='MIT',
     url='https://github.com/cone387/DjangoCommonTaskSystem.git',
     python_requires='>=3.7, <4',
+    entry_points={
+        'console_scripts': [
+            'django-common-task-system=django_common_task_system_server.manage:main',
+        ],
+    },
 )
```

