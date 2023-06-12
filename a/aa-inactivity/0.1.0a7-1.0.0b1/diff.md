# Comparing `tmp/aa-inactivity-0.1.0a7.tar.gz` & `tmp/aa_inactivity-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-inactivity-0.1.0a7.tar", last modified: Sun May 21 19:45:45 2023, max compression
+gzip compressed data, was "aa_inactivity-1.0.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa-inactivity-0.1.0a7.tar` & `aa_inactivity-1.0.0b1.tar`

### file list

```diff
@@ -1,63 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.090696 aa-inactivity-0.1.0a7/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3160 2023-05-21 19:45:45.090696 aa-inactivity-0.1.0a7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2232 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.082696 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3160 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.084696 aa-inactivity-0.1.0a7/inactivity/
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1355 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.085696 aa-inactivity-0.1.0a7/inactivity/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5731 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/0002_add_manage_leave_perm.py
--rw-rw-rw-   0 root         (0) root         (0)     4250 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/0003_add_webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/0004_django4_update.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7431 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.079696 aa-inactivity-0.1.0a7/inactivity/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.080696 aa-inactivity-0.1.0a7/inactivity/static/inactivity/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.086696 aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/aa-bootstrap-fix.css
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/aa-bootstrap-fix.min.css
--rw-rw-rw-   0 root         (0) root         (0)     2497 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/inactivity.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.086696 aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.087696 aa-inactivity-0.1.0a7/inactivity/static/inactivity/js/
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/js/loa_request_list.js
--rw-rw-rw-   0 root         (0) root         (0)     2565 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/js/pending_loa_request_list.js
--rw-rw-rw-   0 root         (0) root         (0)     3265 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.080696 aa-inactivity-0.1.0a7/inactivity/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.088696 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/base.html
--rw-rw-rw-   0 root         (0) root         (0)     1985 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/create_loa.html
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/index.html
--rw-rw-rw-   0 root         (0) root         (0)     2148 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/manage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.088696 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/modal_dialog.html
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/view_request_content.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.089696 aa-inactivity-0.1.0a7/inactivity/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3480 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5107 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/views.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-21 19:45:45.090696 aa-inactivity-0.1.0a7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.090696 aa-inactivity-0.1.0a7/testauth/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10000 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/wsgi.py
+-rw-r--r--   0        0        0    35149 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2931 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/README.md
+-rw-r--r--   0        0        0      107 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/admin.py
+-rw-r--r--   0        0        0      173 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/app_settings.py
+-rw-r--r--   0        0        0      195 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/apps.py
+-rw-r--r--   0        0        0     1052 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/auth_hooks.py
+-rw-r--r--   0        0        0     2262 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/forms.py
+-rw-r--r--   0        0        0     1552 2023-06-12 13:23:21.233775 aa_inactivity-1.0.0b1/inactivity/helpers.py
+-rw-r--r--   0        0        0     2313 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/managers.py
+-rw-r--r--   0        0        0     5731 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0001_initial.py
+-rw-r--r--   0        0        0      598 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0002_add_manage_leave_perm.py
+-rw-r--r--   0        0        0     4250 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0003_add_webhooks.py
+-rw-r--r--   0        0        0     1102 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0004_django4_update.py
+-rw-r--r--   0        0        0     2183 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/migrations/0005_various_improvements.py
+-rw-r--r--   0        0        0        0 2023-06-12 13:23:21.256775 aa_inactivity-1.0.0b1/inactivity/migrations/__init__.py
+-rw-r--r--   0        0        0     9119 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/models.py
+-rw-r--r--   0        0        0      291 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/aa-bootstrap-fix.css
+-rw-r--r--   0        0        0      107 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0        0        0     1445 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/inactivity.css
+-rw-r--r--   0        0        0      383 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/manage_requests.css
+-rw-r--r--   0        0        0      232 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/css/my_requests.css
+-rw-r--r--   0        0        0    43262 2023-06-12 13:23:21.234775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     5726 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tasks.py
+-rw-r--r--   0        0        0      311 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/base.html
+-rw-r--r--   0        0        0     1685 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/create_loa.html
+-rw-r--r--   0        0        0     3436 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/inactive_users.html
+-rw-r--r--   0        0        0     5778 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/manage_requests.html
+-rw-r--r--   0        0        0     1069 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/modals/modal_dialog.html
+-rw-r--r--   0        0        0     1275 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/modals/view_request_content.html
+-rw-r--r--   0        0        0     5532 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/my_requests.html
+-rw-r--r--   0        0        0     1862 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/partials/menu.html
+-rw-r--r--   0        0        0      936 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/templates/inactivity/reject_request.html
+-rw-r--r--   0        0        0        0 2023-06-12 13:23:21.257775 aa_inactivity-1.0.0b1/inactivity/tests/__init__.py
+-rw-r--r--   0        0        0     6152 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/factories.py
+-rw-r--r--   0        0        0     4671 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/test_forms.py
+-rw-r--r--   0        0        0     5173 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/test_integration.py
+-rw-r--r--   0        0        0     2474 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/test_managers.py
+-rw-r--r--   0        0        0     3775 2023-06-12 13:23:21.235775 aa_inactivity-1.0.0b1/inactivity/tests/test_models.py
+-rw-r--r--   0        0        0     8207 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/inactivity/tests/test_tasks.py
+-rw-r--r--   0        0        0     5390 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/inactivity/tests/test_views.py
+-rw-r--r--   0        0        0     1445 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/inactivity/urls.py
+-rw-r--r--   0        0        0     8737 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/inactivity/views.py
+-rw-r--r--   0        0        0     1634 2023-06-12 13:23:21.236775 aa_inactivity-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4144 1970-01-01 00:00:00.000000 aa_inactivity-1.0.0b1/PKG-INFO
```

### Comparing `aa-inactivity-0.1.0a7/LICENSE` & `aa_inactivity-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a7/README.md` & `aa_inactivity-1.0.0b1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -8,35 +8,57 @@
 ![django](https://img.shields.io/pypi/djversions/aa-inactivity?label=django)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 ## Content
 
 - [Features](#features)
+- [Screenshots](#screenshots)
 - [Installation](#installation)
 - [Permissions](#permissions)
 
 ## Features
 
-- Notify users inactive for a specified time.
-- Notify administrators when users meet an inactivity threshold.
-- Keep track of leave of absence requests.
-- Notify administrators when leave of absence requests are created or approved.
+- Automatically notify users who become inactive.
+- Automatically notify managers when users become inactive.
+- Approval process for leave of absence requests
+- Can inform managers about various events via Discord webhook
+- List of inactive users
+- Define through policies after how many days a user of absence a user is considered inactive
+- Fetching the last login dates from Member Audit to determine how long a user has been inactive
+
+Users are notified on Alliance Auth. If you want those notifications to be forwarded as DM on Discord, please check out this app: [Discord Notify](https://gitlab.com/ErikKalkoken/aa-discordnotify).
+
+## Screenshots
+
+A user creating a new leave of absence request:
+
+![request](https://imgpile.com/images/9oMUiC.png)
+
+A manager reviewing a leave of absence request:
+
+![pending](https://imgpile.com/images/9oKyoP.png)
+
+A manager looking through the list of currently inactive and notified users:
+
+![notified](https://imgpile.com/images/9oMIrx.png)
 
 ## Installation
 
-### Requirements
+### Step 0 - Requirements
 
-This app needs [Member Audit](https://gitlab.com/ErikKalkoken/aa-memberaudit) (and optionally, but ideally, [DiscordBot](https://github.com/pvyParts/allianceauth-discordbot)) to function. Please make sure they are installed before continuing.
+This app needs [Member Audit](https://gitlab.com/ErikKalkoken/aa-memberaudit) to function. Please make sure it is installed before continuing.
 
 ### Step 1 - Install the Package
 
 Make sure you are in the virtual environment (venv) of your Alliance Auth installation. Then install the newest release from PyPI:
 
-`pip install aa-inactivity`
+```bash
+pip install aa-inactivity`
+```
 
 ### Step 2 - Config
 
 Add `inactivity` to your `INSTALLED_APPS`, and add the following task definition:
 
 ```python
 CELERYBEAT_SCHEDULE['inactivity_check_inactivity'] = {
```

### Comparing `aa-inactivity-0.1.0a7/inactivity/auth_hooks.py` & `aa_inactivity-1.0.0b1/inactivity/auth_hooks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from django.utils.translation import gettext_lazy as _
 
 from allianceauth import hooks
 from allianceauth.services.hooks import MenuItemHook, UrlHook
 
 from . import urls
+from .models import LeaveOfAbsence
 
 
 class LeaveOfAbsenceMenuItem(MenuItemHook):
     def __init__(self):
         MenuItemHook.__init__(
             self,
             _("Leave of Absence"),
             "fas fa-business-time fa-fw",
             "inactivity:index",
             navactive=["inactivity:"],
         )
 
     def render(self, request):
+        if request.user.has_perm("inactivity:manage_requests"):
+            app_count = LeaveOfAbsence.objects.unapproved_count()
+            self.count = app_count if app_count and app_count > 0 else None
         if request.user.has_perm("inactivity.basic_access"):
             return MenuItemHook.render(self, request)
         return ""
 
 
 @hooks.register("menu_item_hook")
 def register_menu():
```

### Comparing `aa-inactivity-0.1.0a7/inactivity/migrations/0001_initial.py` & `aa_inactivity-1.0.0b1/inactivity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a7/inactivity/migrations/0002_add_manage_leave_perm.py` & `aa_inactivity-1.0.0b1/inactivity/migrations/0002_add_manage_leave_perm.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a7/inactivity/migrations/0003_add_webhooks.py` & `aa_inactivity-1.0.0b1/inactivity/migrations/0003_add_webhooks.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a7/inactivity/migrations/0004_django4_update.py` & `aa_inactivity-1.0.0b1/inactivity/migrations/0004_django4_update.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a7/inactivity/models.py` & `aa_inactivity-1.0.0b1/inactivity/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-import dhooks_lite
+import humanize
 from multiselectfield import MultiSelectField
 
 from django.contrib.auth.models import Group, User
-from django.core.exceptions import ValidationError
 from django.db import models
-from django.db.models import Q
+from django.utils.html import format_html
+from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 
 from allianceauth.authentication.models import State
 
+from .app_settings import INACTIVITY_TASKS_DEFAULT_PRIORITY
+from .helpers import user_for_display
+from .managers import InactivityPingConfigManager, LeaveOfAbsenceManager, WebhookManager
+
 
 class General(models.Model):
     """Meta model for app permissions"""
 
     class Meta:
         managed = False
         default_permissions = ()
         permissions = (
             ("basic_access", "Can access this app"),
             ("manage_leave", "Can manage leave of absence requests"),
         )
 
 
 class InactivityPingConfig(models.Model):
+    """A ping configuration."""
+
     name = models.CharField(
         max_length=48,
         unique=True,
         help_text=_("Internal name for the inactivity policy. Must be unique."),
     )
     days = models.PositiveIntegerField(
         help_text=_("The number of days the user must be inactive.")
@@ -49,162 +55,234 @@
         blank=True,
         help_text=_(
             "States subject to the inactivity policy. If empty, applies to all states."
         ),
         related_name="+",
     )
 
+    objects = InactivityPingConfigManager()
+
     class Meta:
         default_permissions = ()
-        verbose_name = "inactivity policy"
-        verbose_name_plural = "inactivity policies"
+        verbose_name = _("inactivity policy")
+        verbose_name_plural = _("inactivity policies")
 
     def __str__(self):
         return _("inactivity policy: %(name)s") % {"name": self.name}
 
     def is_applicable_to(self, user: User) -> bool:
         is_applicable = True
         if self.groups.count() > 0:
             is_applicable &= self.groups.filter(user=user).count() > 0
         if self.states.count() > 0:
             is_applicable &= self.states.filter(userprofile=user.profile).count() > 0
         return is_applicable
 
 
 class InactivityPing(models.Model):
+    """An inactive user who has been notified."""
+
     config = models.ForeignKey(InactivityPingConfig, on_delete=models.CASCADE)
-    timestamp = models.DateTimeField()
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
+    last_login_at = models.DateTimeField(null=True, default=None)
+    timestamp = models.DateTimeField(auto_now_add=True)
+    user = models.ForeignKey(User, on_delete=models.CASCADE, related_name="+")
 
     class Meta:
         default_permissions = ()
 
     def __str__(self):
         return _("ping [policy='%(config_name)s' user='%(user_name)s']") % {
             "config_name": self.config.name,
             "user_name": self.user.profile.main_character.character_name
             if self.user.profile.main_character
             else "None",
         }
 
 
 class LeaveOfAbsence(models.Model):
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
+    """A leave of absence request."""
+
+    class Status(models.TextChoices):
+        PENDING = "pending"
+        APPROVED = "approved"
+        DENIED = "denied"
+
     approver = models.ForeignKey(
         User, on_delete=models.SET_NULL, blank=True, null=True, related_name="+"
     )
-    start = models.DateField(help_text=_("The start of the leave of absence."))
+    created_at = models.DateTimeField(null=True, default=None)
+    reason = models.TextField(
+        blank=True,
+        null=True,
+        default=None,
+        help_text=_("Reason for rejecting a request"),
+    )
     end = models.DateField(
         blank=True,
         null=True,
         help_text=_(
             "The end of the leave of absence. Leave blank for an indefinite leave."
         ),
     )
-    notes = models.TextField(blank=True)
+    notes = models.TextField(
+        blank=True,
+        verbose_name="description",
+        help_text=_("Description what this leave of absence request is about."),
+    )
+    start = models.DateField(help_text=_("The start of the leave of absence."))
+    user = models.ForeignKey(
+        User,
+        on_delete=models.CASCADE,
+        related_name="leave_of_absence_requests",
+        help_text="The requestor",
+    )
+
+    objects = LeaveOfAbsenceManager()
 
     class Meta:
         default_permissions = ()
 
-    def save(self, *args, **kwargs):
-        orig = LeaveOfAbsence.objects.filter(pk=self.pk).first()
-        # find possible configs that could apply to the user, then alert based on that
-        configs = []
-        for config in InactivityPingConfig.objects.all():
-            if config.is_applicable_to(self.user):
-                configs.append(config)
-        webhooks = Webhook.objects.filter(
-            Q(ping_configs__in=configs) | Q(ping_configs=None), Q(is_active=True)
-        )
-        if self._state.adding:
-            for webhook in webhooks:
-                if str(Webhook.NOTIFICATION_TYPE_LOA_NEW) in webhook.notification_types:
-                    if webhook.webhook_type == Webhook.WEBHOOK_TYPE_DISCORD:
-                        hook = dhooks_lite.Webhook(webhook.url)
-                        hook.execute(
-                            "**%(user_name)s** has submitted a new leave of absence from **%(start)s** to **%(end)s**"
-                            % {
-                                "user_name": self.user.profile.main_character.character_name,
-                                "start": self.start,
-                                "end": self.end if self.end else "—",
-                            }
-                        )
-        elif self.approver and not orig.approver:
-            for webhook in webhooks:
-                if (
-                    str(Webhook.NOTIFICATION_TYPE_LOA_APPROVED)
-                    in webhook.notification_types
-                ):
-                    if webhook.webhook_type == Webhook.WEBHOOK_TYPE_DISCORD:
-                        hook = dhooks_lite.Webhook(webhook.url)
-                        hook.execute(
-                            "**%(user_name)s**'s leave of absence from **%(start)s** to **%(end)s** has been approved by **%(approver_name)s**"
-                            % {
-                                "user_name": self.user.profile.main_character.character_name,
-                                "approver_name": self.approver.profile.main_character.character_name,
-                                "start": self.start,
-                                "end": self.end if self.end else "—",
-                            }
-                        )
-
-        super(LeaveOfAbsence, self).save(*args, **kwargs)
-
     def __str__(self):
-        return _("%(user_name)s's leave starting %(start)s") % {
+        requestor = user_for_display(self.user)
+        return _(
+            "%(requestor)s's leave of absence request "
+            "from %(start)s to %(end)s %(details)s"
+        ) % {
+            "end": self.end_text,
             "start": self.start,
-            "user_name": self.user.profile.main_character.character_name,
+            "requestor": requestor.name_with_ticker,
+            "details": f'"{self.notes[:25]}"' if self.notes else "",
         }
 
-    def clean(self):
-        if self.end and self.end < self.start:
-            raise ValidationError(_("End date must be after start date."))
+    def save(self, *args, **kwargs) -> None:
+        is_new = self._state.adding is True
+        if is_new and not self.created_at:
+            self.created_at = now()
+        return super().save(*args, **kwargs)
+
+    @property
+    def approver_name(self) -> str:
+        """Name of the approver."""
+        if not self.approver:
+            return ""
+        approver = user_for_display(self.approver)
+        return approver.name_with_ticker
+
+    @property
+    def end_text(self) -> str:
+        return str(self.end) if self.end else _("open end")
+
+    @property
+    def requestor_name(self) -> str:
+        """Name of the requestor."""
+        requestor = user_for_display(self.user)
+        return requestor.name_with_ticker
+
+    def to_output_dict(self) -> dict:
+        requestor_display = user_for_display(self.user)
+        approver_display = user_for_display(self.approver) if self.approver else None
+        duration = (
+            humanize.naturaldelta(self.end - self.start) if self.end else _("open end")
+        )
+        created_at_display = (
+            humanize.naturaltime(self.created_at, when=now())
+            if self.created_at
+            else "?"
+        )
+        try:
+            status = self.status
+        except AttributeError:
+            status_html = ""
+        else:
+            if status == self.Status.DENIED:
+                status_html = format_html(
+                    '<span class="text-danger text-underline-dotted" title="{}">{}</span>',
+                    f"Reason: {self.reason}",
+                    status,
+                )
+            else:
+                status_html = format_html(
+                    '<span class="text-success">{}</span>', status
+                )
+
+        result = {
+            "approver": approver_display.name if approver_display else "",
+            "approver_html": approver_display.html if self.approver else "",
+            "created_at": {
+                "display": created_at_display,
+                "sort": self.created_at.isoformat() if self.created_at else "",
+            },
+            "duration": duration,
+            "end": self.end_text,
+            "notes": self.notes if self.notes else "-",
+            "requestor": requestor_display.name,
+            "requestor_html": requestor_display.html,
+            "pk": self.pk,
+            "start": self.start,
+            "status_html": status_html,
+        }
+        return result
 
 
 class Webhook(models.Model):
-    NOTIFICATION_TYPE_INACTIVE_USER = 1
-    NOTIFICATION_TYPE_LOA_NEW = 10
-    NOTIFICATION_TYPE_LOA_APPROVED = 11
-
-    NOTIFICATION_TYPE_CHOICES = [
-        (NOTIFICATION_TYPE_INACTIVE_USER, "Inactive User"),
-        (NOTIFICATION_TYPE_LOA_NEW, "Leave of Absence - Created"),
-        (NOTIFICATION_TYPE_LOA_APPROVED, "Leave of Absence - Approved"),
-    ]
-
-    WEBHOOK_TYPE_DISCORD = 1
-
-    WEBHOOK_TYPE_CHOICES = [
-        (WEBHOOK_TYPE_DISCORD, _("Discord Webhook")),
-    ]
+    "A webhook configuration to send message to."
+
+    class NotificationType(models.IntegerChoices):
+        INACTIVE_USER = 1, "Inactive User"
+        LOA_NEW = 10, "Leave of Absence - Created"
+        LOA_APPROVED = 11, "Leave of Absence - Approved"
+
+    class WebhookType(models.IntegerChoices):
+        DISCORD = 1, _("Discord Webhook")
 
     name = models.CharField(
-        max_length=64, unique=True, help_text="short name to identify this webhook"
+        max_length=64, unique=True, help_text=_("short name to identify this webhook")
     )
 
     notification_types = MultiSelectField(
-        choices=NOTIFICATION_TYPE_CHOICES,
-        help_text=("only notifications of the selected types are sent to this webhook"),
+        choices=NotificationType.choices,
+        help_text=_(
+            "only notifications of the selected types are sent to this webhook"
+        ),
     )
 
     ping_configs = models.ManyToManyField(
         InactivityPingConfig,
         blank=True,
-        help_text="The inactivity policies to alert for. If left blank, all policies are alerted for.",
+        help_text=_(
+            "The inactivity policies to alert for. "
+            "If left blank, all policies are alerted for."
+        ),
     )
 
     url = models.CharField(
         max_length=255,
         unique=True,
-        help_text=(
+        help_text=_(
             "URL of this webhook, e.g. "
             "https://discordapp.com/api/webhooks/123456/abcdef"
         ),
     )
     webhook_type = models.IntegerField(
-        choices=WEBHOOK_TYPE_CHOICES,
-        default=WEBHOOK_TYPE_DISCORD,
-        help_text="type of this webhook",
+        choices=WebhookType.choices,
+        default=WebhookType.DISCORD,
+        help_text=_("type of this webhook"),
     )
     is_active = models.BooleanField(
         default=True,
-        help_text="whether notifications are currently sent to this webhook",
+        help_text=_("whether notifications are currently sent to this webhook"),
     )
+
+    objects = WebhookManager()
+
+    def __str__(self):
+        return self.name
+
+    def send_message(self, content: str):
+        """Send message to webhook asynchronously."""
+        from .tasks import send_message_to_webhook
+
+        if self.webhook_type == self.WebhookType.DISCORD:
+            send_message_to_webhook.apply_async(
+                kwargs={"webhook_pk": self.pk, "content": content},
+                priority=INACTIVITY_TASKS_DEFAULT_PRIORITY,
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif` & `aa_inactivity-1.0.0b1/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif` & `aa_inactivity-1.0.0b1/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a7/inactivity/templates/inactivity/create_loa.html` & `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/create_loa.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 00000000: 7b25 2065 7874 656e 6473 2027 696e 6163  {% extends 'inac
 00000010: 7469 7669 7479 2f62 6173 652e 6874 6d6c  tivity/base.html
 00000020: 2720 257d 0a7b 2520 6c6f 6164 2069 3138  ' %}.{% load i18
 00000030: 6e20 257d 0a7b 2520 6c6f 6164 2068 756d  n %}.{% load hum
 00000040: 616e 697a 6520 257d 0a7b 2520 6c6f 6164  anize %}.{% load
 00000050: 2073 7461 7469 6320 257d 0a7b 2520 6c6f   static %}.{% lo
 00000060: 6164 2062 6f6f 7473 7472 6170 2025 7d0a  ad bootstrap %}.
-00000070: 7b25 2062 6c6f 636b 2064 6574 6169 6c73  {% block details
-00000080: 2025 7d0a 0a20 2020 203c 6469 7620 636c   %}..    <div cl
+00000070: 0a7b 2520 626c 6f63 6b20 6465 7461 696c  .{% block detail
+00000080: 7320 257d 0a20 2020 203c 6469 7620 636c  s %}.    <div cl
 00000090: 6173 733d 2270 616e 656c 2070 616e 656c  ass="panel panel
 000000a0: 2d70 7269 6d61 7279 223e 0a20 2020 2020  -primary">.     
 000000b0: 2020 203c 6469 7620 636c 6173 733d 2270     <div class="p
 000000c0: 616e 656c 2d68 6561 6469 6e67 223e 0a20  anel-heading">. 
 000000d0: 2020 2020 2020 2020 2020 203c 6833 2063             <h3 c
 000000e0: 6c61 7373 3d22 7061 6e65 6c2d 7469 746c  lass="panel-titl
 000000f0: 6522 3e7b 2520 7472 616e 736c 6174 6520  e">{% translate 
@@ -25,101 +25,82 @@
 00000180: 2220 6d65 7468 6f64 3d22 504f 5354 2220  " method="POST" 
 00000190: 6163 7469 6f6e 3d22 7b25 2075 726c 2027  action="{% url '
 000001a0: 696e 6163 7469 7669 7479 3a63 7265 6174  inactivity:creat
 000001b0: 655f 6c6f 615f 7265 7175 6573 7427 2025  e_loa_request' %
 000001c0: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
 000001d0: 2020 2020 7b25 2063 7372 665f 746f 6b65      {% csrf_toke
 000001e0: 6e20 257d 0a20 2020 2020 2020 2020 2020  n %}.           
-000001f0: 2020 2020 207b 7b20 6372 6561 7465 5f66       {{ create_f
-00000200: 6f72 6d7c 626f 6f74 7374 7261 7020 7d7d  orm|bootstrap }}
-00000210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000220: 203c 6469 7620 636c 6173 733d 2266 6f72   <div class="for
-00000230: 6d2d 6772 6f75 7022 3e0a 2020 2020 2020  m-group">.      
-00000240: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000250: 6976 2063 6c61 7373 3d22 7075 6c6c 2d72  iv class="pull-r
-00000260: 6967 6874 223e 0a20 2020 2020 2020 2020  ight">.         
-00000270: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000280: 6275 7474 6f6e 2074 7970 653d 2273 7562  button type="sub
-00000290: 6d69 7422 2063 6c61 7373 3d22 6274 6e20  mit" class="btn 
-000002a0: 6274 6e2d 7072 696d 6172 7922 3e53 7562  btn-primary">Sub
-000002b0: 6d69 743c 2f62 7574 746f 6e3e 0a20 2020  mit</button>.   
-000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002d0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-000002e0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-000002f0: 2020 2020 2020 2020 2020 203c 2f66 6f72             </for
-00000300: 6d3e 0a20 2020 2020 2020 203c 2f64 6976  m>.        </div
-00000310: 3e0a 2020 2020 3c2f 6469 763e 0a0a 7b25  >.    </div>..{%
-00000320: 2065 6e64 626c 6f63 6b20 257d 0a0a 7b25   endblock %}..{%
-00000330: 2062 6c6f 636b 2065 7874 7261 5f6a 6176   block extra_jav
-00000340: 6173 6372 6970 7420 257d 0a7b 2520 696e  ascript %}.{% in
-00000350: 636c 7564 6520 2762 756e 646c 6573 2f64  clude 'bundles/d
-00000360: 6174 6174 6162 6c65 732d 6a73 2e68 746d  atatables-js.htm
-00000370: 6c27 2025 7d0a 3c73 6372 6970 7420 7479  l' %}.<script ty
-00000380: 7065 3d22 6170 706c 6963 6174 696f 6e2f  pe="application/
-00000390: 6a61 7661 7363 7269 7074 223e 0a0a 2020  javascript">..  
-000003a0: 2020 6c65 7420 6c6f 6153 6574 7469 6e67    let loaSetting
-000003b0: 7320 3d20 7b0a 2020 2020 2020 2020 6c69  s = {.        li
-000003c0: 7374 5265 7175 6573 7473 5572 6c3a 2027  stRequestsUrl: '
-000003d0: 7b25 2075 726c 2022 696e 6163 7469 7669  {% url "inactivi
-000003e0: 7479 3a6c 6973 745f 6c6f 615f 7265 7175  ty:list_loa_requ
-000003f0: 6573 7473 2220 257d 272c 0a20 2020 2020  ests" %}',.     
-00000400: 2020 2061 7070 726f 7665 5265 7175 6573     approveReques
-00000410: 7455 726c 3a27 7b25 2075 726c 2022 696e  tUrl:'{% url "in
-00000420: 6163 7469 7669 7479 3a61 7070 726f 7665  activity:approve
-00000430: 5f6c 6f61 5f72 6571 7565 7374 2220 7265  _loa_request" re
-00000440: 7175 6573 745f 6964 3d31 3233 3435 2025  quest_id=12345 %
-00000450: 7d27 2c0a 2020 2020 2020 2020 6361 6e63  }',.        canc
-00000460: 656c 5265 7175 6573 7455 726c 3a27 7b25  elRequestUrl:'{%
-00000470: 2075 726c 2022 696e 6163 7469 7669 7479   url "inactivity
-00000480: 3a63 616e 6365 6c5f 6c6f 615f 7265 7175  :cancel_loa_requ
-00000490: 6573 7422 2072 6571 7565 7374 5f69 643d  est" request_id=
-000004a0: 3132 3334 3520 257d 272c 0a20 2020 2020  12345 %}',.     
-000004b0: 2020 2063 7372 6654 6f6b 656e 3a20 277b     csrfToken: '{
-000004c0: 2520 6373 7266 5f74 6f6b 656e 2025 7d27  % csrf_token %}'
-000004d0: 2c0a 2020 2020 7d3b 0a0a 3c2f 7363 7269  ,.    };..</scri
-000004e0: 7074 3e0a 3c73 6372 6970 7420 7479 7065  pt>.<script type
-000004f0: 3d22 6170 706c 6963 6174 696f 6e2f 6a61  ="application/ja
-00000500: 7661 7363 7269 7074 2220 7372 633d 227b  vascript" src="{
-00000510: 2520 7374 6174 6963 2027 696e 6163 7469  % static 'inacti
-00000520: 7669 7479 2f6a 732f 6c6f 615f 7265 7175  vity/js/loa_requ
-00000530: 6573 745f 6c69 7374 2e6a 7327 2025 7d22  est_list.js' %}"
-00000540: 203e 3c2f 7363 7269 7074 3e0a 3c73 6372   ></script>.<scr
-00000550: 6970 7420 7372 633d 2268 7474 7073 3a2f  ipt src="https:/
-00000560: 2f63 646e 6a73 2e63 6c6f 7564 666c 6172  /cdnjs.cloudflar
-00000570: 652e 636f 6d2f 616a 6178 2f6c 6962 732f  e.com/ajax/libs/
-00000580: 6a71 7565 7279 7569 2f31 2e31 322e 312f  jqueryui/1.12.1/
-00000590: 6a71 7565 7279 2d75 692e 6d69 6e2e 6a73  jquery-ui.min.js
-000005a0: 2220 696e 7465 6772 6974 793d 2273 6861  " integrity="sha
-000005b0: 3531 322d 7574 6f39 6d6c 517a 7273 3539  512-uto9mlQzrs59
-000005c0: 5677 494c 634c 6952 5965 4c4b 5050 6253  VwILcLiRYeLKPPbS
-000005d0: 2f62 5437 3164 612f 4f45 4259 4577 6364  /bT71da/OEBYEwcd
-000005e0: 4e55 6b38 6a59 4979 2b44 3137 3652 596f  NUk8jYIy+D176RYo
-000005f0: 6f70 3144 612b 6639 6d76 6b59 726d 6a35  op1Da+f9mvkYrmj5
-00000600: 4d43 4c5a 5745 7451 7541 3d3d 2220 6372  MCLZWEtQuA==" cr
-00000610: 6f73 736f 7269 6769 6e3d 2261 6e6f 6e79  ossorigin="anony
-00000620: 6d6f 7573 223e 3c2f 7363 7269 7074 3e0a  mous"></script>.
-00000630: 0a20 203c 7363 7269 7074 3e0a 2020 2428  .  <script>.  $(
-00000640: 2066 756e 6374 696f 6e28 2920 7b0a 2020   function() {.  
-00000650: 2020 6c65 7420 7061 7261 6d73 203d 207b    let params = {
-00000660: 0a20 2020 2020 2020 2064 6174 6546 6f72  .        dateFor
-00000670: 6d61 743a 2022 7979 2d6d 6d2d 6464 220a  mat: "yy-mm-dd".
-00000680: 2020 2020 7d3b 0a20 2020 2024 2820 2223      };.    $( "#
-00000690: 6964 5f73 7461 7274 2220 292e 6461 7465  id_start" ).date
-000006a0: 7069 636b 6572 2870 6172 616d 7329 3b0a  picker(params);.
-000006b0: 2020 2020 2428 2022 2369 645f 656e 6422      $( "#id_end"
-000006c0: 2029 2e64 6174 6570 6963 6b65 7228 7061   ).datepicker(pa
-000006d0: 7261 6d73 293b 0a20 207d 2029 3b0a 2020  rams);.  } );.  
-000006e0: 3c2f 7363 7269 7074 3e0a 7b25 2065 6e64  </script>.{% end
-000006f0: 626c 6f63 6b20 257d 0a0a 7b25 2062 6c6f  block %}..{% blo
-00000700: 636b 2065 7874 7261 5f63 7373 2025 7d0a  ck extra_css %}.
-00000710: 3c6c 696e 6b20 7265 6c3d 2273 7479 6c65  <link rel="style
-00000720: 7368 6565 7422 2068 7265 663d 2268 7474  sheet" href="htt
-00000730: 7073 3a2f 2f63 646e 6a73 2e63 6c6f 7564  ps://cdnjs.cloud
-00000740: 666c 6172 652e 636f 6d2f 616a 6178 2f6c  flare.com/ajax/l
-00000750: 6962 732f 6a71 7565 7279 7569 2f31 2e31  ibs/jqueryui/1.1
-00000760: 322e 312f 6a71 7565 7279 2d75 692e 6d69  2.1/jquery-ui.mi
-00000770: 6e2e 6373 7322 2020 7479 7065 3d22 7465  n.css"  type="te
-00000780: 7874 2f63 7373 223e 0a7b 2520 656e 6462  xt/css">.{% endb
-00000790: 6c6f 636b 2025 7d0a 0a7b 2520 626c 6f63  lock %}..{% bloc
-000007a0: 6b20 6578 7472 615f 7363 7269 7074 2025  k extra_script %
-000007b0: 7d0a 7b25 2065 6e64 626c 6f63 6b20 257d  }.{% endblock %}
-000007c0: 0a                                       .
+000001f0: 2020 2020 207b 7b20 666f 726d 7c62 6f6f       {{ form|boo
+00000200: 7473 7472 6170 207d 7d0a 2020 2020 2020  tstrap }}.      
+00000210: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000220: 6c61 7373 3d22 666f 726d 2d67 726f 7570  lass="form-group
+00000230: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000240: 2020 2020 2020 203c 6120 636c 6173 733d         <a class=
+00000250: 2262 746e 2062 746e 2d64 6566 6175 6c74  "btn btn-default
+00000260: 2220 6872 6566 3d22 7b25 2075 726c 2027  " href="{% url '
+00000270: 696e 6163 7469 7669 7479 3a6d 795f 7265  inactivity:my_re
+00000280: 7175 6573 7473 2720 257d 223e 7b25 2074  quests' %}">{% t
+00000290: 7261 6e73 6c61 7465 2022 4361 6e63 656c  ranslate "Cancel
+000002a0: 2220 257d 3c2f 613e 0a20 2020 2020 2020  " %}</a>.       
+000002b0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000002c0: 7620 636c 6173 733d 2270 756c 6c2d 7269  v class="pull-ri
+000002d0: 6768 7422 3e0a 2020 2020 2020 2020 2020  ght">.          
+000002e0: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
+000002f0: 7574 746f 6e20 7479 7065 3d22 7375 626d  utton type="subm
+00000300: 6974 2220 636c 6173 733d 2262 746e 2062  it" class="btn b
+00000310: 746e 2d70 7269 6d61 7279 223e 5375 626d  tn-primary">Subm
+00000320: 6974 3c2f 6275 7474 6f6e 3e0a 2020 2020  it</button>.    
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000350: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00000360: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
+00000370: 3e0a 2020 2020 2020 2020 3c2f 6469 763e  >.        </div>
+00000380: 0a20 2020 203c 2f64 6976 3e0a 7b25 2065  .    </div>.{% e
+00000390: 6e64 626c 6f63 6b20 257d 0a0a 7b25 2062  ndblock %}..{% b
+000003a0: 6c6f 636b 2065 7874 7261 5f6a 6176 6173  lock extra_javas
+000003b0: 6372 6970 7420 257d 0a0a 2020 2020 3c73  cript %}..    <s
+000003c0: 6372 6970 7420 7372 633d 2268 7474 7073  cript src="https
+000003d0: 3a2f 2f63 646e 6a73 2e63 6c6f 7564 666c  ://cdnjs.cloudfl
+000003e0: 6172 652e 636f 6d2f 616a 6178 2f6c 6962  are.com/ajax/lib
+000003f0: 732f 6a71 7565 7279 7569 2f31 2e31 322e  s/jqueryui/1.12.
+00000400: 312f 6a71 7565 7279 2d75 692e 6d69 6e2e  1/jquery-ui.min.
+00000410: 6a73 2220 696e 7465 6772 6974 793d 2273  js" integrity="s
+00000420: 6861 3531 322d 7574 6f39 6d6c 517a 7273  ha512-uto9mlQzrs
+00000430: 3539 5677 494c 634c 6952 5965 4c4b 5050  59VwILcLiRYeLKPP
+00000440: 6253 2f62 5437 3164 612f 4f45 4259 4577  bS/bT71da/OEBYEw
+00000450: 6364 4e55 6b38 6a59 4979 2b44 3137 3652  cdNUk8jYIy+D176R
+00000460: 596f 6f70 3144 612b 6639 6d76 6b59 726d  Yoop1Da+f9mvkYrm
+00000470: 6a35 4d43 4c5a 5745 7451 7541 3d3d 2220  j5MCLZWEtQuA==" 
+00000480: 6372 6f73 736f 7269 6769 6e3d 2261 6e6f  crossorigin="ano
+00000490: 6e79 6d6f 7573 223e 3c2f 7363 7269 7074  nymous"></script
+000004a0: 3e0a 0a20 2020 203c 7363 7269 7074 3e0a  >..    <script>.
+000004b0: 2020 2020 2020 2020 2275 7365 2073 7472          "use str
+000004c0: 6963 7422 3b0a 2020 2020 2020 2020 2428  ict";.        $(
+000004d0: 646f 6375 6d65 6e74 292e 7265 6164 7928  document).ready(
+000004e0: 6675 6e63 7469 6f6e 2028 2920 7b0a 2020  function () {.  
+000004f0: 2020 2020 2020 2020 2020 6c65 7420 7061            let pa
+00000500: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
+00000510: 2020 2020 2020 2020 2064 6174 6546 6f72           dateFor
+00000520: 6d61 743a 2022 7979 2d6d 6d2d 6464 220a  mat: "yy-mm-dd".
+00000530: 2020 2020 2020 2020 2020 2020 7d3b 0a20              };. 
+00000540: 2020 2020 2020 2020 2020 2024 2820 2223             $( "#
+00000550: 6964 5f73 7461 7274 2220 292e 6461 7465  id_start" ).date
+00000560: 7069 636b 6572 2870 6172 616d 7329 3b0a  picker(params);.
+00000570: 2020 2020 2020 2020 2020 2020 2428 2022              $( "
+00000580: 2369 645f 656e 6422 2029 2e64 6174 6570  #id_end" ).datep
+00000590: 6963 6b65 7228 7061 7261 6d73 293b 0a20  icker(params);. 
+000005a0: 2020 2020 2020 207d 2029 3b0a 2020 2020         } );.    
+000005b0: 3c2f 7363 7269 7074 3e0a 7b25 2065 6e64  </script>.{% end
+000005c0: 626c 6f63 6b20 257d 0a0a 7b25 2062 6c6f  block %}..{% blo
+000005d0: 636b 2065 7874 7261 5f63 7373 2025 7d0a  ck extra_css %}.
+000005e0: 2020 2020 3c6c 696e 6b20 7265 6c3d 2273      <link rel="s
+000005f0: 7479 6c65 7368 6565 7422 2068 7265 663d  tylesheet" href=
+00000600: 2268 7474 7073 3a2f 2f63 646e 6a73 2e63  "https://cdnjs.c
+00000610: 6c6f 7564 666c 6172 652e 636f 6d2f 616a  loudflare.com/aj
+00000620: 6178 2f6c 6962 732f 6a71 7565 7279 7569  ax/libs/jqueryui
+00000630: 2f31 2e31 322e 312f 6a71 7565 7279 2d75  /1.12.1/jquery-u
+00000640: 692e 6d69 6e2e 6373 7322 2020 7479 7065  i.min.css"  type
+00000650: 3d22 7465 7874 2f63 7373 223e 0a7b 2520  ="text/css">.{% 
+00000660: 656e 6462 6c6f 636b 2025 7d0a 0a7b 2520  endblock %}..{% 
+00000670: 626c 6f63 6b20 6578 7472 615f 7363 7269  block extra_scri
+00000680: 7074 2025 7d0a 7b25 2065 6e64 626c 6f63  pt %}.{% endbloc
+00000690: 6b20 257d 0a                             k %}.
```

### Comparing `aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/modal_dialog.html` & `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/view_request_content.html` & `aa_inactivity-1.0.0b1/inactivity/templates/inactivity/modals/view_request_content.html`

 * *Files identical despite different names*

