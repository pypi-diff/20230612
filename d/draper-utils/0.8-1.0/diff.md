# Comparing `tmp/draper-utils-0.8.tar.gz` & `tmp/draper-utils-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draper-utils-0.8.tar", last modified: Mon Jun  5 16:49:08 2023, max compression
+gzip compressed data, was "draper-utils-1.0.tar", last modified: Mon Jun 12 21:49:34 2023, max compression
```

## Comparing `draper-utils-0.8.tar` & `draper-utils-1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:49:08.859015 draper-utils-0.8/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 draper-utils-0.8/LICENCE.txt
--rw-rw-rw-   0        0        0      355 2023-06-05 16:49:08.858015 draper-utils-0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 draper-utils-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:49:08.812013 draper-utils-0.8/draper_utils/
--rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-0.8/draper_utils/__init__.py
--rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-0.8/draper_utils/admin.py
--rw-rw-rw-   0        0        0      161 2023-01-28 21:06:51.000000 draper-utils-0.8/draper_utils/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:49:08.838015 draper-utils-0.8/draper_utils/management/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 draper-utils-0.8/draper_utils/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:49:08.842015 draper-utils-0.8/draper_utils/management/commands/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 draper-utils-0.8/draper_utils/management/commands/__init__.py
--rw-rw-rw-   0        0        0    13812 2023-06-05 11:54:07.000000 draper-utils-0.8/draper_utils/management/commands/import_projects.py
--rw-rw-rw-   0        0        0     3326 2023-06-05 11:39:22.000000 draper-utils-0.8/draper_utils/management/commands/setup_project_center.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:49:08.843015 draper-utils-0.8/draper_utils/migrations/
--rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-0.8/draper_utils/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-01-28 21:06:51.000000 draper-utils-0.8/draper_utils/models.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:49:08.857015 draper-utils-0.8/draper_utils/sql/
--rw-rw-rw-   0        0        0       79 2023-01-04 12:10:24.000000 draper-utils-0.8/draper_utils/sql/list_project_activities.sql
--rw-rw-rw-   0        0        0      279 2023-02-09 18:41:35.000000 draper-utils-0.8/draper_utils/sql/list_project_assigned_users.sql
--rw-rw-rw-   0        0        0      228 2023-02-16 02:03:32.000000 draper-utils-0.8/draper_utils/sql/list_project_categories.sql
--rw-rw-rw-   0        0        0      172 2023-01-02 16:39:10.000000 draper-utils-0.8/draper_utils/sql/list_project_stages.sql
--rw-rw-rw-   0        0        0      178 2023-01-02 16:22:17.000000 draper-utils-0.8/draper_utils/sql/list_project_statuses.sql
--rw-rw-rw-   0        0        0      609 2023-02-05 20:55:33.000000 draper-utils-0.8/draper_utils/sql/list_project_users.sql
--rw-rw-rw-   0        0        0      399 2023-01-14 16:07:20.000000 draper-utils-0.8/draper_utils/sql/list_projects.sql
--rw-rw-rw-   0        0        0       63 2023-01-28 21:06:51.000000 draper-utils-0.8/draper_utils/tests.py
--rw-rw-rw-   0        0        0     7345 2023-01-29 13:45:21.000000 draper-utils-0.8/draper_utils/utils.py
--rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-0.8/draper_utils/views.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:49:08.837015 draper-utils-0.8/draper_utils.egg-info/
--rw-rw-rw-   0        0        0      355 2023-06-05 16:49:08.000000 draper-utils-0.8/draper_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      925 2023-06-05 16:49:08.000000 draper-utils-0.8/draper_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:49:08.000000 draper-utils-0.8/draper_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-31 20:41:35.000000 draper-utils-0.8/draper_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-05 16:49:08.000000 draper-utils-0.8/draper_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 16:49:08.000000 draper-utils-0.8/draper_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:49:08.859015 draper-utils-0.8/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-06-05 16:48:25.000000 draper-utils-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.450743 draper-utils-1.0/
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 draper-utils-1.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      355 2023-06-12 21:49:34.450743 draper-utils-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 draper-utils-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.372744 draper-utils-1.0/draper_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/admin.py
+-rw-rw-rw-   0        0        0      161 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.392744 draper-utils-1.0/draper_utils/management/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 draper-utils-1.0/draper_utils/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.407744 draper-utils-1.0/draper_utils/management/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 draper-utils-1.0/draper_utils/management/commands/__init__.py
+-rw-rw-rw-   0        0        0    14141 2023-06-12 12:15:19.000000 draper-utils-1.0/draper_utils/management/commands/import_projects.py
+-rw-rw-rw-   0        0        0     3326 2023-06-05 11:39:22.000000 draper-utils-1.0/draper_utils/management/commands/setup_project_center.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.409742 draper-utils-1.0/draper_utils/migrations/
+-rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/models.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.449743 draper-utils-1.0/draper_utils/sql/
+-rw-rw-rw-   0        0        0       79 2023-01-04 12:10:24.000000 draper-utils-1.0/draper_utils/sql/list_project_activities.sql
+-rw-rw-rw-   0        0        0      279 2023-02-09 18:41:35.000000 draper-utils-1.0/draper_utils/sql/list_project_assigned_users.sql
+-rw-rw-rw-   0        0        0      228 2023-02-16 02:03:32.000000 draper-utils-1.0/draper_utils/sql/list_project_categories.sql
+-rw-rw-rw-   0        0        0      172 2023-01-02 16:39:10.000000 draper-utils-1.0/draper_utils/sql/list_project_stages.sql
+-rw-rw-rw-   0        0        0      178 2023-01-02 16:22:17.000000 draper-utils-1.0/draper_utils/sql/list_project_statuses.sql
+-rw-rw-rw-   0        0        0      609 2023-02-05 20:55:33.000000 draper-utils-1.0/draper_utils/sql/list_project_users.sql
+-rw-rw-rw-   0        0        0      399 2023-01-14 16:07:20.000000 draper-utils-1.0/draper_utils/sql/list_projects.sql
+-rw-rw-rw-   0        0        0       63 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/tests.py
+-rw-rw-rw-   0        0        0     7345 2023-01-29 13:45:21.000000 draper-utils-1.0/draper_utils/utils.py
+-rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/views.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.391744 draper-utils-1.0/draper_utils.egg-info/
+-rw-rw-rw-   0        0        0      355 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      925 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-31 20:41:35.000000 draper-utils-1.0/draper_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 21:49:34.450743 draper-utils-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-06-12 21:49:22.000000 draper-utils-1.0/setup.py
```

### Comparing `draper-utils-0.8/draper_utils/management/commands/import_projects.py` & `draper-utils-1.0/draper_utils/management/commands/import_projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,18 @@
                     print('Importing Project ' + project.title + '...')
                     activities = self.import_project_activities(
                         engine=engine,
                         file=full_path('../../sql/list_project_activities.sql'),
                         project=project,
                         limit=None)
                     assigned_users = self.import_project_assigned_users(engine=engine, project=project, limit=None)
+                    if project.last_activity():
+                        project.last_activity_name = project.last_activity().name if project.last_activity() else None
+                        project.last_activity_date = project.last_activity().date if project.last_activity() else None
+                        project.save()
                     print('Project {title} import complete. Activities: {num_activities}. Users: {num_users}'.format(
                         title=project.title,
                         num_users=str(len(assigned_users)),
                         num_activities=str(len(activities))))
 
     def import_project_categories(self, engine, file):
         with engine.connect() as conn:
```

### Comparing `draper-utils-0.8/draper_utils/management/commands/setup_project_center.py` & `draper-utils-1.0/draper_utils/management/commands/setup_project_center.py`

 * *Files identical despite different names*

### Comparing `draper-utils-0.8/draper_utils/sql/list_project_users.sql` & `draper-utils-1.0/draper_utils/sql/list_project_users.sql`

 * *Files identical despite different names*

### Comparing `draper-utils-0.8/draper_utils/utils.py` & `draper-utils-1.0/draper_utils/utils.py`

 * *Files identical despite different names*

### Comparing `draper-utils-0.8/draper_utils.egg-info/SOURCES.txt` & `draper-utils-1.0/draper_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draper-utils-0.8/setup.py` & `draper-utils-1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = []
 
 setup(
     name='draper-utils',
-    version='0.8',
+    version='1.0',
     description='Project Management Module for Django - Utils',
     author='siteshell.net',
     author_email='pdbethke@siteshell.net',
     url='https://github.com/pdbethke/draper-utils',
     packages=find_packages(exclude=('tests', 'docs')),
     package_dir={'draper_utils': 'draper_utils'},
     package_data={'draper_utils': ['sql/*', 'management/*', 'migrations/*']},
```

