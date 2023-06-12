# Comparing `tmp/wagtail-mailchimp-integration-0.0.6.tar.gz` & `tmp/wagtail-mailchimp-integration-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-mailchimp-integration-0.0.6.tar", last modified: Thu May 25 20:22:33 2023, max compression
+gzip compressed data, was "wagtail-mailchimp-integration-0.0.7.tar", last modified: Mon Jun 12 13:10:52 2023, max compression
```

## Comparing `wagtail-mailchimp-integration-0.0.6.tar` & `wagtail-mailchimp-integration-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.971623 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.971623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.971623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 13:10:52.000000 wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.224516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:10:52.228516 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-12 13:10:35.000000 wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/widgets.py
```

### Comparing `wagtail-mailchimp-integration-0.0.6/LICENSE` & `wagtail-mailchimp-integration-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/PKG-INFO` & `wagtail-mailchimp-integration-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.6
+Version: 0.0.7
 Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -197,16 +197,16 @@
 ![Mailchimp Integration Button](screenshots/mailchimp_integration_button.png)
 
 Click it, and it will open a page, where you will match the Mailchimp signup form fields, with the fields in your form.
 
 Make sure you do the matching correctly as this will inform Mailchimp on how to extract your user data from your Custom
 form.
 
-Once again, make sure for `choice options o=in your page form` match exactly
-the `choice options in your mailchimp audience signup form`
+Once again, make sure for `choice options in your page form fields` match exactly
+the `choice options in your mailchimp audience signup form on Mailchimp`
 
 ![Mailchimp fields mapping](screenshots/mailchimp_fields_mapping.png)
 
 After following the above steps and rendering the form in your template, the `Join Our Mailing List` checkbox will be
 appended at the end of your form fields.
 
 You can try it to make sure everything works and users are being added to your mailing list before making the page
```

### Comparing `wagtail-mailchimp-integration-0.0.6/README.md` & `wagtail-mailchimp-integration-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -175,16 +175,16 @@
 ![Mailchimp Integration Button](screenshots/mailchimp_integration_button.png)
 
 Click it, and it will open a page, where you will match the Mailchimp signup form fields, with the fields in your form.
 
 Make sure you do the matching correctly as this will inform Mailchimp on how to extract your user data from your Custom
 form.
 
-Once again, make sure for `choice options o=in your page form` match exactly
-the `choice options in your mailchimp audience signup form`
+Once again, make sure for `choice options in your page form fields` match exactly
+the `choice options in your mailchimp audience signup form on Mailchimp`
 
 ![Mailchimp fields mapping](screenshots/mailchimp_fields_mapping.png)
 
 After following the above steps and rendering the form in your template, the `Join Our Mailing List` checkbox will be
 appended at the end of your form fields.
 
 You can try it to make sure everything works and users are being added to your mailing list before making the page
```

### Comparing `wagtail-mailchimp-integration-0.0.6/setup.cfg` & `wagtail-mailchimp-integration-0.0.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-mailchimp-integration
-version = 0.0.6
+version = 0.0.7
 description = Integration of Mailchimp Email Marketing in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-mailchimp-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/PKG-INFO` & `wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.6
+Version: 0.0.7
 Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -197,16 +197,16 @@
 ![Mailchimp Integration Button](screenshots/mailchimp_integration_button.png)
 
 Click it, and it will open a page, where you will match the Mailchimp signup form fields, with the fields in your form.
 
 Make sure you do the matching correctly as this will inform Mailchimp on how to extract your user data from your Custom
 form.
 
-Once again, make sure for `choice options o=in your page form` match exactly
-the `choice options in your mailchimp audience signup form`
+Once again, make sure for `choice options in your page form fields` match exactly
+the `choice options in your mailchimp audience signup form on Mailchimp`
 
 ![Mailchimp fields mapping](screenshots/mailchimp_fields_mapping.png)
 
 After following the above steps and rendering the form in your template, the `Join Our Mailing List` checkbox will be
 appended at the end of your form fields.
 
 You can try it to make sure everything works and users are being added to your mailing list before making the page
```

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/SOURCES.txt` & `wagtail-mailchimp-integration-0.0.7/wagtail_mailchimp_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/api.py` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/api.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/forms.py` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/migrations/0001_initial.py` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/models.py` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/views.py` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/wagtail_hooks.py` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/widgets.py` & `wagtail-mailchimp-integration-0.0.7/wagtailmailchimp/widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.db.utils import ProgrammingError
 from django.forms.widgets import Input, Select
 from wagtail.models import Site
 
 from .api import MailchimpApi
 
 
 class CustomSelect(Select):
@@ -42,14 +43,18 @@
             audience_choices.append([audience.get("id"), audience.get("name")])
 
         self.choices = audience_choices
 
     def get_mailchimp_audience_lists(self):
         from .models import MailchimpSettings
 
-        current_site = Site.objects.get(is_default_site=True)
+        # catch error where 'wagtailcore_site' relation is not migrated to db yet
+        try:
+            current_site = Site.objects.get(is_default_site=True)
+        except ProgrammingError:
+            return []
 
         mc_settings = MailchimpSettings.for_site(current_site)
         mailchimp = MailchimpApi(api_key=mc_settings.api_key)
         lists = mailchimp.get_lists()
 
         return lists
```

