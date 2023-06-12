# Comparing `tmp/mozilla_nimbus_shared-2.3.0.tar.gz` & `tmp/mozilla_nimbus_shared-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_nimbus_shared-2.3.0.tar", max compression
+gzip compressed data, was "mozilla_nimbus_shared-2.4.0.tar", max compression
```

## Comparing `mozilla_nimbus_shared-2.3.0.tar` & `mozilla_nimbus_shared-2.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      628 2022-06-16 17:41:54.490623 mozilla_nimbus_shared-2.3.0/README.md
--rw-r--r--   0        0        0     1660 2022-06-16 17:38:10.474193 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/__init__.py
--rw-r--r--   0        0        0    29846 2023-05-17 21:29:45.310597 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/data.json
--rw-r--r--   0        0        0    13724 2023-05-17 21:29:45.313005 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json
--rw-r--r--   0        0        0     2559 2023-05-17 21:29:45.313508 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/features/Feature.json
--rw-r--r--   0        0        0    25972 2022-06-16 17:43:18.606633 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json
--rw-r--r--   0        0        0     9789 2022-06-16 17:43:18.606730 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json
--rw-r--r--   0        0        0     4368 2022-06-16 17:43:18.606822 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json
--rw-r--r--   0        0        0      493 2023-05-17 21:29:45.314833 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/AddonRollbackArguments.json
--rw-r--r--   0        0        0      689 2023-05-17 21:29:45.314354 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json
--rw-r--r--   0        0        0     2015 2023-05-17 21:29:45.314730 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json
--rw-r--r--   0        0        0      434 2023-05-17 21:29:45.313759 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/ConsoleLogArguments.json
--rw-r--r--   0        0        0     2528 2023-05-17 21:29:45.314607 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json
--rw-r--r--   0        0        0     4064 2023-05-17 21:29:45.314939 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json
--rw-r--r--   0        0        0    18244 2023-05-17 21:29:45.314223 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json
--rw-r--r--   0        0        0     1149 2023-05-17 21:29:45.315050 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json
--rw-r--r--   0        0        0     3038 2023-05-17 21:29:45.313992 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json
--rw-r--r--   0        0        0      467 2023-05-17 21:29:45.313876 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRollbackArguments.json
--rw-r--r--   0        0        0     1280 2023-05-17 21:29:45.314481 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json
--rw-r--r--   0        0        0     2077 2023-05-17 21:29:45.314104 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json
--rw-r--r--   0        0        0    13302 2023-03-08 17:02:15.454267 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json
--rw-r--r--   0        0        0     2559 2023-03-08 17:02:15.454465 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json
--rw-r--r--   0        0        0      493 2023-03-08 17:02:15.455590 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRollbackArguments.json
--rw-r--r--   0        0        0      689 2023-03-08 17:02:15.455191 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json
--rw-r--r--   0        0        0     2015 2023-03-08 17:02:15.455491 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json
--rw-r--r--   0        0        0      434 2023-03-08 17:02:15.454671 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/ConsoleLogArguments.json
--rw-r--r--   0        0        0     2528 2023-03-08 17:02:15.455393 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json
--rw-r--r--   0        0        0     4064 2023-03-08 17:02:15.455693 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json
--rw-r--r--   0        0        0    18244 2023-03-08 17:02:15.455095 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json
--rw-r--r--   0        0        0     1149 2023-03-08 17:02:15.455786 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json
--rw-r--r--   0        0        0     3038 2023-03-08 17:02:15.454883 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json
--rw-r--r--   0        0        0      467 2023-03-08 17:02:15.454780 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRollbackArguments.json
--rw-r--r--   0        0        0     1280 2023-03-08 17:02:15.455291 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json
--rw-r--r--   0        0        0     2077 2023-03-08 17:02:15.454991 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json
--rw-r--r--   0        0        0      736 2023-03-08 17:02:15.454067 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json
--rw-r--r--   0        0        0      449 2023-03-08 17:02:15.453853 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/test/FoodColors.json
--rw-r--r--   0        0        0      736 2023-05-17 21:29:45.312790 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/targeting/Audience.json
--rw-r--r--   0        0        0      449 2023-05-17 21:29:45.312551 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/test/FoodColors.json
--rw-r--r--   0        0        0      999 2022-06-16 17:38:10.474263 mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/test.py
--rw-r--r--   0        0        0      524 2023-05-17 21:29:45.302778 mozilla_nimbus_shared-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.3.0/setup.py
--rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      628 2022-06-16 17:41:54.490623 mozilla_nimbus_shared-2.4.0/README.md
+-rw-r--r--   0        0        0     1660 2022-06-16 17:38:10.474193 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/__init__.py
+-rw-r--r--   0        0        0    29846 2023-06-12 15:29:45.117179 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/data.json
+-rw-r--r--   0        0        0    13859 2023-06-12 15:29:45.119562 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json
+-rw-r--r--   0        0        0     2559 2023-06-12 15:29:45.119943 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/features/Feature.json
+-rw-r--r--   0        0        0    25972 2022-06-16 17:43:18.606633 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json
+-rw-r--r--   0        0        0     9789 2022-06-16 17:43:18.606730 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json
+-rw-r--r--   0        0        0     4368 2022-06-16 17:43:18.606822 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json
+-rw-r--r--   0        0        0      493 2023-06-12 15:29:45.121376 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/AddonRollbackArguments.json
+-rw-r--r--   0        0        0      689 2023-06-12 15:29:45.120891 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json
+-rw-r--r--   0        0        0     2015 2023-06-12 15:29:45.121253 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json
+-rw-r--r--   0        0        0      434 2023-06-12 15:29:45.120237 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/ConsoleLogArguments.json
+-rw-r--r--   0        0        0     2528 2023-06-12 15:29:45.121140 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json
+-rw-r--r--   0        0        0     4064 2023-06-12 15:29:45.121504 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json
+-rw-r--r--   0        0        0    18244 2023-06-12 15:29:45.120774 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json
+-rw-r--r--   0        0        0     1149 2023-06-12 15:29:45.121715 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json
+-rw-r--r--   0        0        0     3038 2023-06-12 15:29:45.120492 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json
+-rw-r--r--   0        0        0      467 2023-06-12 15:29:45.120367 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRollbackArguments.json
+-rw-r--r--   0        0        0     1280 2023-06-12 15:29:45.121012 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json
+-rw-r--r--   0        0        0     2077 2023-06-12 15:29:45.120632 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json
+-rw-r--r--   0        0        0    13302 2023-03-08 17:02:15.454267 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json
+-rw-r--r--   0        0        0     2559 2023-03-08 17:02:15.454465 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json
+-rw-r--r--   0        0        0      493 2023-03-08 17:02:15.455590 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRollbackArguments.json
+-rw-r--r--   0        0        0      689 2023-03-08 17:02:15.455191 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json
+-rw-r--r--   0        0        0     2015 2023-03-08 17:02:15.455491 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json
+-rw-r--r--   0        0        0      434 2023-03-08 17:02:15.454671 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/ConsoleLogArguments.json
+-rw-r--r--   0        0        0     2528 2023-03-08 17:02:15.455393 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json
+-rw-r--r--   0        0        0     4064 2023-03-08 17:02:15.455693 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json
+-rw-r--r--   0        0        0    18244 2023-03-08 17:02:15.455095 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json
+-rw-r--r--   0        0        0     1149 2023-03-08 17:02:15.455786 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json
+-rw-r--r--   0        0        0     3038 2023-03-08 17:02:15.454883 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json
+-rw-r--r--   0        0        0      467 2023-03-08 17:02:15.454780 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRollbackArguments.json
+-rw-r--r--   0        0        0     1280 2023-03-08 17:02:15.455291 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json
+-rw-r--r--   0        0        0     2077 2023-03-08 17:02:15.454991 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json
+-rw-r--r--   0        0        0      736 2023-03-08 17:02:15.454067 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json
+-rw-r--r--   0        0        0      449 2023-03-08 17:02:15.453853 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/test/FoodColors.json
+-rw-r--r--   0        0        0      736 2023-06-12 15:29:45.119104 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/targeting/Audience.json
+-rw-r--r--   0        0        0      449 2023-06-12 15:29:45.118874 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/test/FoodColors.json
+-rw-r--r--   0        0        0      999 2022-06-16 17:38:10.474263 mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/test.py
+-rw-r--r--   0        0        0      524 2023-06-12 15:29:45.110118 mozilla_nimbus_shared-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.4.0/setup.py
+-rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.4.0/PKG-INFO
```

### Comparing `mozilla_nimbus_shared-2.3.0/README.md` & `mozilla_nimbus_shared-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/__init__.py` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/data.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/data.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998372395833334%*

 * *Differences: {"'definitions'": "{'NimbusExperiment': {'properties': {'locales': {'anyOf': "*

 * *                  "[OrderedDict([('type', 'array'), ('items', OrderedDict([('type', "*

 * *                  "'string')]))]), OrderedDict([('type', 'null')])], delete: ['type', 'items']}}}}"}*

```diff
@@ -245,19 +245,26 @@
                     "type": "boolean"
                 },
                 "isRollout": {
                     "description": "When this property is set to true, treat this experiment as a rollout. Rollouts are currently handled as single-branch experiments separated from the bucketing namespace for normal experiments. See also: https://mozilla-hub.atlassian.net/browse/SDK-405",
                     "type": "boolean"
                 },
                 "locales": {
-                    "description": "The list of locale codes (e.g., \"en-US\" or \"fr\") that this experiment is targeting.\n\nIf null, all locales are targeted.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
+                    "anyOf": [
+                        {
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": "array"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "description": "The list of locale codes (e.g., \"en-US\" or \"fr\") that this experiment is targeting.\n\nIf null, all locales are targeted."
                 },
                 "localizations": {
                     "anyOf": [
                         {
                             "additionalProperties": {
                                 "additionalProperties": {
                                     "type": "string"
```

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/features/Feature.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/features/Feature.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/schemas/targeting/Audience.json` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/schemas/targeting/Audience.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/mozilla_nimbus_shared/test.py` & `mozilla_nimbus_shared-2.4.0/mozilla_nimbus_shared/test.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.3.0/pyproject.toml` & `mozilla_nimbus_shared-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mozilla_nimbus_shared"
 description = "Shared data and schemas for Project Nimbus"
 readme = "README.md"
 authors = ["Michael Cooper <mcooper@mozilla.com>"]
-version = "2.3.0"
+version = "2.4.0"
 license = "MPL-2.0"
 include = [
   "mozilla_nimbus_shared/schemas/**/*.json",
   "mozilla_nimbus_shared/data.json",
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `mozilla_nimbus_shared-2.3.0/setup.py` & `mozilla_nimbus_shared-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                            'schemas/test/*']}
 
 install_requires = \
 ['jsonschema>=4.17.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'mozilla-nimbus-shared',
-    'version': '2.3.0',
+    'version': '2.4.0',
     'description': 'Shared data and schemas for Project Nimbus',
     'long_description': '# Nimbus Shared ![CircleCI](https://img.shields.io/circleci/build/github/mozilla/nimbus-shared) ![npm (scoped)](https://img.shields.io/npm/v/@mozilla/nimbus-shared)\n\nThis is a place to define data and schemas used across Project Nimbus.\n\nAny data that moves between systems should have TypeScript types defined here, which will be\nautomatically converted to JSON Schema. Any data that needs to be re-used by multiple systems should\nbe stored here to be shared.\n\nFor more information on the data and schemas included here, how to use them, and how to add to them,\nsee the documentation at https://mozilla.github.io/nimbus-shared\n',
     'author': 'Michael Cooper',
     'author_email': 'mcooper@mozilla.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mozilla_nimbus_shared-2.3.0/PKG-INFO` & `mozilla_nimbus_shared-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-nimbus-shared
-Version: 2.3.0
+Version: 2.4.0
 Summary: Shared data and schemas for Project Nimbus
 License: MPL-2.0
 Author: Michael Cooper
 Author-email: mcooper@mozilla.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

