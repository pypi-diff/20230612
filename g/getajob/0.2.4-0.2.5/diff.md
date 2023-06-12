# Comparing `tmp/getajob-0.2.4.tar.gz` & `tmp/getajob-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.2.4.tar", max compression
+gzip compressed data, was "getajob-0.2.5.tar", max compression
```

## Comparing `getajob-0.2.4.tar` & `getajob-0.2.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    11357 2023-06-11 17:37:49.776135 getajob-0.2.4/LICENSE
--rw-r--r--   0        0        0       69 2023-06-11 17:37:49.776135 getajob-0.2.4/README.md
--rw-r--r--   0        0        0       22 2023-06-11 17:37:49.776135 getajob-0.2.4/getajob/__init__.py
--rw-r--r--   0        0        0     1811 2023-06-11 17:37:49.776135 getajob-0.2.4/getajob/abstractions/models.py
--rw-r--r--   0        0        0     8332 2023-06-11 17:37:49.776135 getajob-0.2.4/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     1341 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      141 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      394 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      598 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/ai/text/__init__.py
--rw-r--r--   0        0        0      823 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0      102 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0      395 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/jobs/__init__.py
--rw-r--r--   0        0        0     3021 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1120 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1556 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/static/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      516 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0       89 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/models.py
--rw-r--r--   0        0        0      470 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0      196 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      462 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      306 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/skills/__init__.py
--rw-r--r--   0        0        0      404 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      491 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0     2318 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/exceptions.py
--rw-r--r--   0        0        0      375 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     1848 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0      413 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2120 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1614 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2624 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1339 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     1839 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0     9580 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/firebase.py
--rw-r--r--   0        0        0        0 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      724 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1254 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      221 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1480 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      589 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1862 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      251 2023-06-11 17:37:49.780135 getajob-0.2.4/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1742 2023-06-11 17:37:49.780135 getajob-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-12 21:15:39.354895 getajob-0.2.5/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-12 21:15:39.354895 getajob-0.2.5/README.md
+-rw-r--r--   0        0        0       22 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/__init__.py
+-rw-r--r--   0        0        0     1811 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/abstractions/models.py
+-rw-r--r--   0        0        0     8332 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0     1341 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      394 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      598 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/ai/text/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/ai/text/models.py
+-rw-r--r--   0        0        0     2470 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/ai/text/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0      395 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/jobs/__init__.py
+-rw-r--r--   0        0        0     3021 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/jobs/models.py
+-rw-r--r--   0        0        0     1120 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/jobs/repository.py
+-rw-r--r--   0        0        0      462 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/jobs/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1556 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/static/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      516 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0       89 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0      568 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      462 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/skills/__init__.py
+-rw-r--r--   0        0        0      404 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/skills/models.py
+-rw-r--r--   0        0        0      491 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/skills/repository.py
+-rw-r--r--   0        0        0     2318 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/exceptions.py
+-rw-r--r--   0        0        0      375 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     1848 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0      413 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2120 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1748 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2774 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1320 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     1839 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0     9580 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/firebase.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      724 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0      320 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0     1254 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/kafka.py
+-rw-r--r--   0        0        0      221 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1480 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0      589 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0     1862 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/openai.py
+-rw-r--r--   0        0        0      599 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/sendgrid/sendgrid.py
+-rw-r--r--   0        0        0      251 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1742 2023-06-12 21:15:39.358895 getajob-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.5/PKG-INFO
```

### Comparing `getajob-0.2.4/LICENSE` & `getajob-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/abstractions/models.py` & `getajob-0.2.5/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/abstractions/repository.py` & `getajob-0.2.5/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/config/settings.py` & `getajob-0.2.5/getajob/config/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/admin/users/models.py` & `getajob-0.2.5/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/admin/users/repository.py` & `getajob-0.2.5/getajob/contexts/admin/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/ai/text/models.py` & `getajob-0.2.5/getajob/contexts/ai/text/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/ai/text/repository.py` & `getajob-0.2.5/getajob/contexts/ai/text/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/jobs/models.py` & `getajob-0.2.5/getajob/contexts/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/jobs/repository.py` & `getajob-0.2.5/getajob/contexts/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/scheduled_events/models.py` & `getajob-0.2.5/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/scheduled_events/repository.py` & `getajob-0.2.5/getajob/contexts/scheduled_events/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/static/repository.py` & `getajob-0.2.5/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.2.5/getajob/contexts/users/cover_letters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/exceptions.py` & `getajob-0.2.5/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/clerk/companies/models.py` & `getajob-0.2.5/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/clerk/companies/repository.py` & `getajob-0.2.5/getajob/vendor/clerk/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.2.5/getajob/vendor/clerk/recruiters/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from pydantic import BaseModel
 
-from getajob.vendor.clerk.companies.models import ClerkCompany, ClerkCompanyCreated
+from getajob.vendor.clerk.companies.models import ClerkCompanyCreated
 from getajob.vendor.clerk.models import (
     ClerkBaseModel,
     ClerkWebhookEvent,
     ClerkCompanyMemberType,
 )
 
 
@@ -26,25 +26,30 @@
     last_name: str
     profile_image_url: str | None = None
     user_id: str
 
 
 class ClerkCompanyMember(CreateClerkCompanyMember):
     id: str
+    role: ClerkCompanyMemberType
 
 
 class UpdateClerkCompanyMember(BaseModel):
     first_name: str | None = None
     identifier: str | None = None
     image_url: str | None = None
     last_name: str | None = None
     profile_image_url: str | None = None
     user_id: str | None = None
 
 
+class UpdateClerkCompanyMemberWithRole(UpdateClerkCompanyMember):
+    role: ClerkCompanyMemberType | None = None
+
+
 class ClerkCompanyMembership(ClerkBaseModel):
     created_at: int
     organization: ClerkCompanyCreated
     public_user_data: CreateClerkCompanyMember
     role: ClerkCompanyMemberType
     updated_at: int
```

### Comparing `getajob-0.2.4/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.2.5/getajob/vendor/clerk/recruiters/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from getajob.vendor.firebase import FirestoreDB
 from getajob.vendor.kafka.repository import KafkaRepository
 from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
 from getajob.abstractions.repository import BaseRepository
 from getajob.abstractions.models import Entity, EntityModels
 
+
 from .models import (
     ClerkCompanyMembershipWebhookEvent,
     ClerkCompanyMembership,
     ClerkCompanyMembershipWebhookType,
-    CreateClerkCompanyMember,
-    UpdateClerkCompanyMember,
     ClerkUpdateCompanyMembership,
     ClerkCompanyMember,
+    UpdateClerkCompanyMemberWithRole,
 )
 
 entity_models = EntityModels(entity=ClerkCompanyMember)
 
 
 class WebhookCompanyMembershipRepository(BaseRepository):
     def __init__(self, db: FirestoreDB, kafka: t.Optional[KafkaRepository] = None):
@@ -37,29 +37,35 @@
             ClerkCompanyMembershipWebhookType.organization_membership_updated: self.update_recruiter,
             ClerkCompanyMembershipWebhookType.organization_membership_deleted: self.delete_recruiter,
         }
         return event_dict[event.type](event)
 
     def create_recruiter(self, event: ClerkCompanyMembershipWebhookEvent):
         create_event = ClerkCompanyMembership(**event.data)
-        recruiter = CreateClerkCompanyMember(**create_event.public_user_data.dict())
+        recruiter = ClerkCompanyMember(
+            **create_event.public_user_data.dict(),
+            id=create_event.id,
+            role=create_event.role
+        )
         return self.create(
             data=recruiter,
             provided_id=create_event.id,
-            parent_collections={"companies": create_event.organization.id},
+            parent_collections={Entity.COMPANIES.value: create_event.organization.id},
         )
 
     def delete_recruiter(self, event: ClerkCompanyMembershipWebhookEvent):
         delete_event = ClerkUpdateCompanyMembership(**event.data)
         return self.delete(
             doc_id=delete_event.id,
-            parent_collections={"companies": delete_event.organization.id},
+            parent_collections={Entity.COMPANIES.value: delete_event.organization.id},
         )
 
     def update_recruiter(self, event: ClerkCompanyMembershipWebhookEvent):
         update_event = ClerkUpdateCompanyMembership(**event.data)
-        recruiter = UpdateClerkCompanyMember(**update_event.public_user_data.dict())
+        recruiter = UpdateClerkCompanyMemberWithRole(
+            **update_event.public_user_data.dict(), role=update_event.role
+        )
         return self.update(
             doc_id=update_event.id,
             data=recruiter,
-            parent_collections={"companies": update_event.organization.id},
+            parent_collections={Entity.COMPANIES.value: update_event.organization.id},
         )
```

### Comparing `getajob-0.2.4/getajob/vendor/clerk/users/models.py` & `getajob-0.2.5/getajob/vendor/clerk/users/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import typing as t
 from enum import Enum
 
 from getajob.vendor.clerk.models import ClerkBaseModel, ClerkWebhookEvent
 
 
 class ClerkUserWebhookType(str, Enum):
     user_created = "user.created"
```

### Comparing `getajob-0.2.4/getajob/vendor/clerk/users/repository.py` & `getajob-0.2.5/getajob/vendor/clerk/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/firebase.py` & `getajob-0.2.5/getajob/vendor/firebase.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/kafka/authentication.py` & `getajob-0.2.5/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/kafka/kafka.py` & `getajob-0.2.5/getajob/vendor/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/kafka/models.py` & `getajob-0.2.5/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/kafka/repository.py` & `getajob-0.2.5/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/openai.py` & `getajob-0.2.5/getajob/vendor/openai.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/getajob/vendor/sendgrid/sendgrid.py` & `getajob-0.2.5/getajob/vendor/sendgrid/sendgrid.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.4/pyproject.toml` & `getajob-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.2.4/PKG-INFO` & `getajob-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

