# Comparing `tmp/oqtant-0.15.0.tar.gz` & `tmp/oqtant-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqtant-0.15.0.tar", max compression
+gzip compressed data, was "oqtant-0.15.1.tar", max compression
```

## Comparing `oqtant-0.15.0.tar` & `oqtant-0.15.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    11341 2023-05-02 20:10:18.126527 oqtant-0.15.0/LICENSE
--rw-r--r--   0        0        0     2470 2023-05-31 16:33:52.539128 oqtant-0.15.0/README.md
--rw-r--r--   0        0        0     8005 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/INSTALL.md
--rw-r--r--   0        0        0    10904 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/job_analysis_docs.md
--rw-r--r--   0        0        0     4429 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/oqtant_api_docs.md
--rw-r--r--   0        0        0    10273 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/oqtant_client_docs.md
--rw-r--r--   0        0        0    14940 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb
--rw-r--r--   0        0        0    10097 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_1_bec_jobs.md
--rw-r--r--   0        0        0    14392 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb
--rw-r--r--   0        0        0     9745 2023-05-31 16:33:52.539128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_2_barrier_jobs.md
--rw-r--r--   0        0        0    31808 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_3_abstractions.ipynb
--rw-r--r--   0        0        0    22140 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_3_abstractions.md
--rw-r--r--   0        0        0    17763 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_4_experiment.ipynb
--rw-r--r--   0        0        0    12609 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_4_experiment.md
--rw-r--r--   0        0        0    16851 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_5_optimization.ipynb
--rw-r--r--   0        0        0    11560 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthrough_5_optimization.md
--rw-r--r--   0        0        0      452 2023-05-31 16:33:52.543128 oqtant-0.15.0/documentation/walkthroughs/walkthroughs.md
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/__init__.py
--rw-r--r--   0        0        0    21848 2023-05-25 15:03:01.160254 oqtant-0.15.0/oqtant/oqtant_client.py
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/schemas/__init__.py
--rw-r--r--   0        0        0    17813 2023-05-18 18:23:18.769901 oqtant-0.15.0/oqtant/schemas/job.py
--rw-r--r--   0        0        0      994 2023-05-25 15:03:01.160254 oqtant-0.15.0/oqtant/settings.py
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/util/__init__.py
--rw-r--r--   0        0        0     2805 2023-05-18 18:23:18.769901 oqtant-0.15.0/oqtant/util/auth.py
--rw-r--r--   0        0        0     1023 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/util/exceptions.py
--rw-r--r--   0        0        0      474 2023-05-16 16:24:46.335446 oqtant-0.15.0/oqtant/util/server.py
--rw-r--r--   0        0        0     3203 2023-05-31 16:33:52.543128 oqtant-0.15.0/pyproject.toml
--rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 oqtant-0.15.0/setup.py
--rw-r--r--   0        0        0     3751 1970-01-01 00:00:00.000000 oqtant-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-02 20:10:18.126527 oqtant-0.15.1/LICENSE
+-rw-r--r--   0        0        0     2470 2023-05-31 16:33:52.539128 oqtant-0.15.1/README.md
+-rw-r--r--   0        0        0     8005 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/INSTALL.md
+-rw-r--r--   0        0        0     4436 2023-06-09 18:32:33.704834 oqtant-0.15.1/documentation/albert_api_docs.md
+-rw-r--r--   0        0        0    10904 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/job_analysis_docs.md
+-rw-r--r--   0        0        0     4429 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/oqtant_api_docs.md
+-rw-r--r--   0        0        0    10273 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/oqtant_client_docs.md
+-rw-r--r--   0        0        0    14940 2023-06-12 13:13:09.730118 oqtant-0.15.1/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb
+-rw-r--r--   0        0        0    10097 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/walkthroughs/walkthrough_1_bec_jobs.md
+-rw-r--r--   0        0        0    14392 2023-06-09 18:24:55.746209 oqtant-0.15.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb
+-rw-r--r--   0        0        0     9745 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.md
+-rw-r--r--   0        0        0    31808 2023-06-01 20:50:58.385110 oqtant-0.15.1/documentation/walkthroughs/walkthrough_3_abstractions.ipynb
+-rw-r--r--   0        0        0    22140 2023-05-31 16:33:52.543128 oqtant-0.15.1/documentation/walkthroughs/walkthrough_3_abstractions.md
+-rw-r--r--   0        0        0    16253 2023-06-12 13:13:09.730118 oqtant-0.15.1/documentation/walkthroughs/walkthrough_4_experiment.ipynb
+-rw-r--r--   0        0        0    11238 2023-06-09 18:34:38.592484 oqtant-0.15.1/documentation/walkthroughs/walkthrough_4_experiment.md
+-rw-r--r--   0        0        0    14224 2023-06-12 13:13:09.730118 oqtant-0.15.1/documentation/walkthroughs/walkthrough_5_optimization.ipynb
+-rw-r--r--   0        0        0     9127 2023-06-09 18:35:19.660472 oqtant-0.15.1/documentation/walkthroughs/walkthrough_5_optimization.md
+-rw-r--r--   0        0        0      452 2023-05-31 16:33:52.543128 oqtant-0.15.1/documentation/walkthroughs/walkthroughs.md
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/__init__.py
+-rw-r--r--   0        0        0    21848 2023-05-25 15:03:01.160254 oqtant-0.15.1/oqtant/oqtant_client.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/schemas/__init__.py
+-rw-r--r--   0        0        0    17813 2023-05-18 18:23:18.769901 oqtant-0.15.1/oqtant/schemas/job.py
+-rw-r--r--   0        0        0      994 2023-06-07 21:25:59.477067 oqtant-0.15.1/oqtant/settings.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/util/__init__.py
+-rw-r--r--   0        0        0     2805 2023-05-18 18:23:18.769901 oqtant-0.15.1/oqtant/util/auth.py
+-rw-r--r--   0        0        0     1023 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/util/exceptions.py
+-rw-r--r--   0        0        0      474 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/util/server.py
+-rw-r--r--   0        0        0     3310 2023-06-09 18:33:02.108747 oqtant-0.15.1/pyproject.toml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 oqtant-0.15.1/setup.py
+-rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 oqtant-0.15.1/PKG-INFO
```

### Comparing `oqtant-0.15.0/LICENSE` & `oqtant-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/README.md` & `oqtant-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/INSTALL.md` & `oqtant-0.15.1/documentation/INSTALL.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/job_analysis_docs.md` & `oqtant-0.15.1/documentation/job_analysis_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/oqtant_api_docs.md` & `oqtant-0.15.1/documentation/oqtant_api_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/oqtant_client_docs.md` & `oqtant-0.15.1/documentation/oqtant_client_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_1_bec_jobs.md` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_1_bec_jobs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_2_barrier_jobs.md` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_3_abstractions.ipynb` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_3_abstractions.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_3_abstractions.md` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_3_abstractions.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_4_experiment.ipynb` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_4_experiment.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9737273493127003%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Oqtant Walkthrough 4: BEC Experimentation #\\n')], "*

 * *            "delete: [0]}, 'attachments': OrderedDict()}, 2: {'source': {delete: [15, 3, 2, 1]}}, "*

 * *            "5: {'source': {insert: [(5, '1. The final frequency of the rf knife\\n'), (9, ' - "*

 * *            "Temperature (calculated from TOF images)\\n'), (10, ' - Atom number and condensate "*

 * *            "fraction (calculated from TOF images)')], delete: [11, 10, 6, 5]}, 'attachments': "*

 * *            "OrderedDi […]*

```diff
@@ -1,14 +1,15 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oqtant Walkthrough 3: BEC Experimentation #\n",
+                "# Oqtant Walkthrough 4: BEC Experimentation #\n",
                 "\n",
                 "### This walkthrough covers best practices for conducting experiments on the Oqtant system, including submitting batches of jobs, tracking experiment progress, and handling output data for later analysis. ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\n",
                 "\n",
                 "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*"
             ]
@@ -27,29 +28,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from matplotlib import pyplot as plt\n",
-                "from lmfit import Model\n",
-                "import numpy as np\n",
-                "import inspect\n",
                 "import copy\n",
                 "from oqtant.oqtant_client import get_oqtant_client\n",
                 "from oqtant.util.auth import get_user_token\n",
                 "from bert_schemas import job as JobSchema\n",
                 "from oqtant.schemas.job import (\n",
                 "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
                 "    round_sig\n",
                 ")\n",
-                "import csv\n",
                 "\n",
                 "token = get_user_token()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -67,74 +64,73 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "oqtant_client = get_oqtant_client(token)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Design a simple experiment ##\n",
                 "\n",
                 "For this example, we will investigate the effect of altering the final frequency of the RF knife on the evolution of the condensate and its temperature. \n",
                 "\n",
                 "### Variables ###\n",
-                "1. **rf_e_mhz** - the final frequency of the rf knife (at t=1600ms)\n",
-                "2. **time_of_flight_ms** - the TOF interval in ms. varying the time will give us snapshots of the condensate as it expands\n",
+                "1. The final frequency of the rf knife\n",
                 "\n",
                 "### Observables ###\n",
                 " - TOF images\n",
-                " - temperature (calculated from TOF images)\n",
-                " - condensate fraction (calculated from TOF images)"
+                " - Temperature (calculated from TOF images)\n",
+                " - Atom number and condensate fraction (calculated from TOF images)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Let us explore the interplay between the final RF evaporation frequency and the resulting cloud temperature in a one-parameter scan \"experiment\".  "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rf_e_values = [0.07, 0.03, 0.05]\n",
-                "tof_interval_values = [10, 12, 15]"
+                "final_rf_freqs_mhz = [0.07, 0.03, 0.05]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Performing the experiment ## \n",
                 "\n",
                 "Depending on your subscription tier there are two different options for performing this experiment\n",
                 "\n",
                 "- Users in the GROUND tier can create 3 separate jobs with each job's input representing a step in the experiment\n",
                 "\n",
                 "- Users in the EXPLORER and INNOVATOR tiers can create a single job that contains three inputs for all of the steps in the experiment\n",
                 "\n",
-                "The rest of this walkthrough will showcase how to perform and analyze the experiment using both options"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Generating job parameters as GROUND ## \n",
+                "The rest of this walkthrough will showcase how to perform and analyze the experiment using both options.\n",
                 "\n",
-                "This experiment will consist of 3 jobs and no repeated trials. Below we will create a BEC job with default parameters and copy it three times. Once we have three instances of the same job we can update the inputs for each one to match the steps in the experiment.\n",
-                "\n",
-                "Print out the jobs once updated to review the input parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**"
+                "Both submission options / subscription tiers will make use of a 'base' job definition:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "default_bec_job = {\n",
+                "base_bec_job = {\n",
                 "    \"name\": \"RF Sweep Experiment\",\n",
                 "    \"job_type\": \"BEC\",\n",
                 "    \"inputs\": [\n",
                 "        {\n",
                 "            \"values\": {\n",
                 "                \"time_of_flight_ms\": 8.0,\n",
                 "                \"image_type\": \"TIME_OF_FLIGHT\",\n",
@@ -147,43 +143,51 @@
                 "                },\n",
                 "                \"optical_barriers\": None,\n",
                 "                \"optical_landscape\": None,\n",
                 "                \"lasers\": None,\n",
                 "            },\n",
                 "        }\n",
                 "    ],\n",
-                "}\n",
+                "}"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Generating parameter scan jobs as GROUND ## \n",
                 "\n",
-                "experiment_step_one_job = copy.deepcopy(default_bec_job)\n",
-                "experiment_step_one_job[\"name\"] = \"RF Sweep Experiment Step One\"\n",
-                "experiment_step_one_job[\"notes\"] = \"RF Sweep Experiment Step One\"\n",
-                "experiment_step_two_job = copy.deepcopy(default_bec_job)\n",
-                "experiment_step_two_job[\"name\"] = \"RF Sweep Experiment Step Two\"\n",
-                "experiment_step_two_job[\"notes\"] = \"RF Sweep Experiment Step Two\"\n",
-                "experiment_step_three_job = copy.deepcopy(default_bec_job)\n",
-                "experiment_step_three_job[\"name\"] = \"RF Sweep Experiment Step Three\"\n",
-                "experiment_step_three_job[\"notes\"] = \"RF Sweep Experiment Step Three\"\n",
-                "\n",
-                "experiment_jobs = [\n",
-                "    experiment_step_one_job,\n",
-                "    experiment_step_two_job,\n",
-                "    experiment_step_three_job\n",
-                "]\n",
-                "\n",
-                "for step in range(3):\n",
-                "    experiment_jobs[step][\"inputs\"][0][\"values\"][\"time_of_flight_ms\"] = tof_interval_values[step]\n",
-                "    experiment_jobs[step][\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][4] = rf_e_values[step]\n",
-                "    \n",
-                "experiment_jobs = [oqtant_client.generate_oqtant_job(job=job) for job in experiment_jobs]\n",
+                "This experiment will consist of 3 jobs and no repeated trials. Below we will create a BEC job with default parameters and copy it three times. Once we have three instances of the same job we can update the inputs for each one to match the steps in the experiment.\n",
+                "\n",
+                "Print out the jobs once updated to review the input parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "njobs = len(final_rf_freqs_mhz)\n",
+                "jobs = []\n",
+                "for step in range(njobs):\n",
+                "    job = copy.deepcopy(base_bec_job)\n",
+                "    job[\"name\"] = \"RF sweep experiment step \" + str(step+1)\n",
+                "    job[\"notes\"] = \"RF sweep experiment step \" + str(step+1) + \" of \" + str(njobs)\n",
+                "    job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][-1] = final_rf_freqs_mhz[step]\n",
+                "    jobs.append(job)\n",
+                "\n",
+                "jobs = [oqtant_client.generate_oqtant_job(job=job) for job in jobs]\n",
                 "    \n",
-                "for experiment_job in experiment_jobs:\n",
+                "for job in jobs:\n",
                 "    print(\n",
-                "        experiment_job.name,\n",
+                "        job.name,\n",
                 "        \"\\n\",\n",
-                "        experiment_job.inputs[0].values,\n",
+                "        job.inputs[0].values,\n",
                 "        \"\\n\"\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -197,67 +201,47 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "default_bec_input = {\n",
-                "    \"values\": {\n",
-                "        \"time_of_flight_ms\": 8.0,\n",
-                "        \"image_type\": \"TIME_OF_FLIGHT\",\n",
-                "        \"end_time_ms\": 0.0,\n",
-                "        \"rf_evaporation\": {\n",
-                "            \"frequencies_mhz\": [17.0, 8.0, 4.0, 1.2, 0.045],\n",
-                "            \"powers_mw\": [500.0, 500.0, 475.0, 360.0, 220.0],\n",
-                "            \"interpolation\": \"LINEAR\",\n",
-                "            \"times_ms\": [-1600, -1200, -800, -400, 0],\n",
-                "        },\n",
-                "        \"optical_barriers\": None,\n",
-                "        \"optical_landscape\": None,\n",
-                "        \"lasers\": None,\n",
-                "    }\n",
-                "}\n",
-                "\n",
-                "experiment_inputs = [\n",
-                "    copy.deepcopy(default_bec_input),\n",
-                "    copy.deepcopy(default_bec_input),\n",
-                "    copy.deepcopy(default_bec_input)\n",
-                "]\n",
-                "\n",
-                "for step in range(3):\n",
-                "    experiment_inputs[step][\"values\"][\"time_of_flight_ms\"] = tof_interval_values[step]\n",
-                "    experiment_inputs[step][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][4] = rf_e_values[step]\n",
-                "    \n",
-                "experiment_job = oqtant_client.generate_oqtant_job(job={\n",
-                "    \"name\": \"RF Sweep Experiment\",\n",
-                "    \"notes\": \"RF Sweep Experiment\",\n",
-                "    \"job_type\": \"BEC\",\n",
-                "    \"inputs\": experiment_inputs,  \n",
-                "})\n",
+                "batch_job = copy.deepcopy(base_bec_job)\n",
+                "batch_job[\"inputs\"] = []\n",
+                "batch_job[\"name\"] = \"RF sweep experiment\"\n",
+                "batch_job[\"notes\"] = \"RF sweep experiment as sequential runs\"\n",
+                "\n",
+                "for step in range(njobs):\n",
+                "    input = copy.deepcopy(base_bec_job[\"inputs\"][0])\n",
+                "    input[\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][-1] = final_rf_freqs_mhz[step]\n",
+                "    batch_job[\"inputs\"].append(input)\n",
                 "\n",
-                "for experiment_input in experiment_job.inputs:\n",
+                "print(batch_job[\"name\"])\n",
+                "for input in batch_job[\"inputs\"]:\n",
                 "    print(\n",
-                "        experiment_input.values,\n",
+                "        input,\n",
                 "        \"\\n\"\n",
-                "    )"
+                "    )\n",
+                "    \n",
+                "batch_job = oqtant_client.generate_oqtant_job(job=batch_job)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
                 "## Accessing the fields of an OqtantJob ##\n",
                 "\n",
-                "The OqtantJob class is the python representation of an Oqtant job's input parameters and if completed it's output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.\n",
+                "The OqtantJob class is the python representation of an Oqtant job's input parameters and (if completed) its output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.\n",
                 "\n",
                 "To get the input parameters for this experiment you would do the following:\n",
                 "\n",
-                "**EXEPERIMENT_JOB.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST**\n",
+                "**JOB.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST**\n",
                 "\n",
                 "All OqtantJobs contain the same high-level input parameters, with some being empty depending on the type of job.\n",
                 "\n",
                 "For BEC jobs the following parameters are used and required:\n",
                 "\n",
                 "- end_time_ms\n",
                 "- image_type\n",
@@ -278,28 +262,30 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# if using the GROUND option\n",
-                "for experiment_step_job in experiment_jobs:\n",
+                "for job in jobs:\n",
                 "    print(\n",
-                "        experiment_step_job.name,\n",
-                "        experiment_step_job.inputs[0].values.rf_evaporation.frequencies_mhz[4],\n",
-                "        experiment_step_job.inputs[0].values.time_of_flight_ms\n",
+                "        job.name,\n",
+                "        job.inputs[0].values.rf_evaporation.frequencies_mhz[-1],\n",
+                "        job.inputs[0].values.time_of_flight_ms\n",
                 "    )\n",
                 "\n",
+                "print(\"\\n\")\n",
+                "\n",
                 "# if using the EXPLORER / INNOVATOR option\n",
-                "for i, experiment_input in enumerate(experiment_job.inputs):\n",
+                "for i, input in enumerate(batch_job.inputs):\n",
                 "    print(\n",
-                "        experiment_job.name,\n",
+                "        batch_job.name,\n",
                 "        f\"input run #{i + 1}\",\n",
-                "        experiment_input.values.rf_evaporation.frequencies_mhz[4],\n",
-                "        experiment_input.values.time_of_flight_ms\n",
+                "        input.values.rf_evaporation.frequencies_mhz[-1],\n",
+                "        input.values.time_of_flight_ms\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -315,21 +301,19 @@
                 "\n",
                 "Option to run the jobs and wait for results (**track_status=True**) OR submit the jobs and return later to retrieve the results (**track_status=False**). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "scrolled": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "# track the status \n",
-                "rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=experiment_jobs, track_status=True)\n",
+                "rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=jobs, track_status=True)\n",
                 "\n",
                 "# dont track the status \n",
                 "# rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=experiment_jobs, track_status=False)\n",
                 "\n",
                 "with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:\n",
                 "    for experiment_step_job_id in rf_sweep_experiment_job_ids:\n",
                 "        filewriter.write(experiment_step_job_id)"
@@ -355,15 +339,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# track the status \n",
-                "rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[experiment_job], track_status=True)[0]\n",
+                "rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[batch_job], track_status=True)[0]\n",
                 "\n",
                 "# dont track the status \n",
                 "# rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[experiment_job], track_status=False)[0]\n",
                 "\n",
                 "with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:\n",
                 "    filewriter.write(rf_sweep_experiment_job_id)"
             ]
@@ -422,21 +406,14 @@
                 "        \n",
                 "# now we can display the second input/output entry results\n",
                 "for a, job in oqtant_client.active_jobs.items():\n",
                 "    if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:\n",
                 "        job.atoms_2dplot()\n",
                 "        job.atoms_sliceplot()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -447,15 +424,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.10.10"
         },
         "vscode": {
             "interpreter": {
                 "hash": "9d324fb170b849c0db1b04a4eaa5a753613b2d729749991e51e49ca6f200afbc"
             }
         }
     },
```

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_4_experiment.md` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_4_experiment.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Oqtant Walkthrough 3: BEC Experimentation
+# Oqtant Walkthrough 3: BEC Experimentation #
 
 ### This walkthrough covers best practices for conducting experiments on the Oqtant system, including submitting batches of jobs, tracking experiment progress, and handling output data for later analysis. ###
 
 For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
 
 *Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
 
@@ -11,82 +11,74 @@
 ## Before you can view and submit jobs you must first sign into your Oqtant account
 
 Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out of that tab and return to this notebook.
 
 
 ```python
 from matplotlib import pyplot as plt
-from lmfit import Model
-import numpy as np
-import inspect
 import copy
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
 from bert_schemas import job as JobSchema
 from oqtant.schemas.job import (
     OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
-import csv
 
 token = get_user_token()
 ```
 
 ## Creating a Oqtant Client Instance ##
 
 ### After successfully logged in, create an authorized session with the Oqtant Client ###
-- the oqtant_client interacts with the Oqtant server to perform remote lab functions. 
+- the oqtant_client interacts with the Oqtant server to perform remote lab functions.
 - the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
 
 
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
 ## Design a simple experiment ##
 
-For this example, we will investigate the effect of altering the final frequency of the RF knife on the evolution of the condensate and its temperature. 
+For this example, we will investigate the effect of altering the final frequency of the RF knife on the evolution of the condensate and its temperature.
 
 ### Variables ###
-1. **rf_e_mhz** - the final frequency of the rf knife (at t=1600ms)
-2. **time_of_flight_ms** - the TOF interval in ms. varying the time will give us snapshots of the condensate as it expands
+1. The final frequency of the rf knife
 
 ### Observables ###
  - TOF images
- - temperature (calculated from TOF images)
- - condensate fraction (calculated from TOF images)
+ - Temperature (calculated from TOF images)
+ - Atom number and condensate fraction (calculated from TOF images)
+
+Let us explore the interplay between the final RF evaporation frequency and the resulting cloud temperature in a one-parameter scan "experiment".
 
 
 ```python
-rf_e_values = [0.07, 0.03, 0.05]
-tof_interval_values = [10, 12, 15]
+final_rf_freqs_mhz = [0.07, 0.03, 0.05]
 ```
 
-## Performing the experiment ## 
+## Performing the experiment ##
 
 Depending on your subscription tier there are two different options for performing this experiment
 
 - Users in the GROUND tier can create 3 separate jobs with each job's input representing a step in the experiment
 
 - Users in the EXPLORER and INNOVATOR tiers can create a single job that contains three inputs for all of the steps in the experiment
 
-The rest of this walkthrough will showcase how to perform and analyze the experiment using both options
-
-## Generating job parameters as GROUND ## 
-
-This experiment will consist of 3 jobs and no repeated trials. Below we will create a BEC job with default parameters and copy it three times. Once we have three instances of the same job we can update the inputs for each one to match the steps in the experiment.
+The rest of this walkthrough will showcase how to perform and analyze the experiment using both options.
 
-Print out the jobs once updated to review the input parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
+Both submission options / subscription tiers will make use of a 'base' job definition:
 
 
 ```python
-default_bec_job = {
+base_bec_job = {
     "name": "RF Sweep Experiment",
     "job_type": "BEC",
     "inputs": [
         {
             "values": {
                 "time_of_flight_ms": 8.0,
                 "image_type": "TIME_OF_FLIGHT",
@@ -100,103 +92,80 @@
                 "optical_barriers": None,
                 "optical_landscape": None,
                 "lasers": None,
             },
         }
     ],
 }
+```
+
+## Generating parameter scan jobs as GROUND ##
+
+This experiment will consist of 3 jobs and no repeated trials. Below we will create a BEC job with default parameters and copy it three times. Once we have three instances of the same job we can update the inputs for each one to match the steps in the experiment.
+
+Print out the jobs once updated to review the input parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
 
-experiment_step_one_job = copy.deepcopy(default_bec_job)
-experiment_step_one_job["name"] = "RF Sweep Experiment Step One"
-experiment_step_one_job["notes"] = "RF Sweep Experiment Step One"
-experiment_step_two_job = copy.deepcopy(default_bec_job)
-experiment_step_two_job["name"] = "RF Sweep Experiment Step Two"
-experiment_step_two_job["notes"] = "RF Sweep Experiment Step Two"
-experiment_step_three_job = copy.deepcopy(default_bec_job)
-experiment_step_three_job["name"] = "RF Sweep Experiment Step Three"
-experiment_step_three_job["notes"] = "RF Sweep Experiment Step Three"
-
-experiment_jobs = [
-    experiment_step_one_job,
-    experiment_step_two_job,
-    experiment_step_three_job
-]
-
-for step in range(3):
-    experiment_jobs[step]["inputs"][0]["values"]["time_of_flight_ms"] = tof_interval_values[step]
-    experiment_jobs[step]["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"][4] = rf_e_values[step]
-    
-experiment_jobs = [oqtant_client.generate_oqtant_job(job=job) for job in experiment_jobs]
-    
-for experiment_job in experiment_jobs:
+
+```python
+njobs = len(final_rf_freqs_mhz)
+jobs = []
+for step in range(njobs):
+    job = copy.deepcopy(base_bec_job)
+    job["name"] = "RF sweep experiment step " + str(step+1)
+    job["notes"] = "RF sweep experiment step " + str(step+1) + " of " + str(njobs)
+    job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"][-1] = final_rf_freqs_mhz[step]
+    jobs.append(job)
+
+jobs = [oqtant_client.generate_oqtant_job(job=job) for job in jobs]
+
+for job in jobs:
     print(
-        experiment_job.name,
+        job.name,
         "\n",
-        experiment_job.inputs[0].values,
+        job.inputs[0].values,
         "\n"
     )
 ```
 
-## Generating job parameters as EXPLORER / INNOVATOR ## 
+## Generating job parameters as EXPLORER / INNOVATOR ##
 
 This experiment will consist of a single job with 3 inputs and no repeated trials. Below we will create an input object with default BEC parameters. Next we will copy this input three times and make updates to match the steps in the experiment.
 
 Print out the job inputs once updated to review the parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
 
 
 ```python
-default_bec_input = {
-    "values": {
-        "time_of_flight_ms": 8.0,
-        "image_type": "TIME_OF_FLIGHT",
-        "end_time_ms": 0.0,
-        "rf_evaporation": {
-            "frequencies_mhz": [17.0, 8.0, 4.0, 1.2, 0.045],
-            "powers_mw": [500.0, 500.0, 475.0, 360.0, 220.0],
-            "interpolation": "LINEAR",
-            "times_ms": [-1600, -1200, -800, -400, 0],
-        },
-        "optical_barriers": None,
-        "optical_landscape": None,
-        "lasers": None,
-    }
-}
+batch_job = copy.deepcopy(base_bec_job)
+batch_job["inputs"] = []
+batch_job["name"] = "RF sweep experiment"
+batch_job["notes"] = "RF sweep experiment as sequential runs"
+
+for step in range(njobs):
+    input = copy.deepcopy(base_bec_job["inputs"][0])
+    input["values"]["rf_evaporation"]["frequencies_mhz"][-1] = final_rf_freqs_mhz[step]
+    batch_job["inputs"].append(input)
 
-experiment_inputs = [
-    copy.deepcopy(default_bec_input),
-    copy.deepcopy(default_bec_input),
-    copy.deepcopy(default_bec_input)
-]
-
-for step in range(3):
-    experiment_inputs[step]["values"]["time_of_flight_ms"] = tof_interval_values[step]
-    experiment_inputs[step]["values"]["rf_evaporation"]["frequencies_mhz"][4] = rf_e_values[step]
-    
-experiment_job = oqtant_client.generate_oqtant_job(job={
-    "name": "RF Sweep Experiment",
-    "notes": "RF Sweep Experiment",
-    "job_type": "BEC",
-    "inputs": experiment_inputs,  
-})
-
-for experiment_input in experiment_job.inputs:
+print(batch_job["name"])
+for input in batch_job["inputs"]:
     print(
-        experiment_input.values,
+        input,
         "\n"
     )
+
+batch_job = oqtant_client.generate_oqtant_job(job=batch_job)
 ```
 
 
 ## Accessing the fields of an OqtantJob ##
 
-The OqtantJob class is the python representation of an Oqtant job's input parameters and if completed it's output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.
+The OqtantJob class is the python representation of an Oqtant job's input parameters and (if completed) its output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.
 
 To get the input parameters for this experiment you would do the following:
 
-**EXEPERIMENT_JOB.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST**
+**JOB.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST**
 
 All OqtantJobs contain the same high-level input parameters, with some being empty depending on the type of job.
 
 For BEC jobs the following parameters are used and required:
 
 - end_time_ms
 - image_type
@@ -212,28 +181,30 @@
 - optical_barriers
 
 All of these inputs have constraints on them which are validated when given values. To view these constraints you can refer to 'Schemas' section of our OpenAPI Documentation: https://albert-dev.coldquanta.com/api/docs
 
 
 ```python
 # if using the GROUND option
-for experiment_step_job in experiment_jobs:
+for job in jobs:
     print(
-        experiment_step_job.name,
-        experiment_step_job.inputs[0].values.rf_evaporation.frequencies_mhz[4],
-        experiment_step_job.inputs[0].values.time_of_flight_ms
+        job.name,
+        job.inputs[0].values.rf_evaporation.frequencies_mhz[-1],
+        job.inputs[0].values.time_of_flight_ms
     )
 
+print("\n")
+
 # if using the EXPLORER / INNOVATOR option
-for i, experiment_input in enumerate(experiment_job.inputs):
+for i, input in enumerate(batch_job.inputs):
     print(
-        experiment_job.name,
+        batch_job.name,
         f"input run #{i + 1}",
-        experiment_input.values.rf_evaporation.frequencies_mhz[4],
-        experiment_input.values.time_of_flight_ms
+        input.values.rf_evaporation.frequencies_mhz[-1],
+        input.values.time_of_flight_ms
     )
 ```
 
 ## Submiting jobs and storing the job IDs as GROUND ##
 
 Once you are ready to submit the experiment jobs you will have two options. One will be to track the status of them as they are processed and the other will be to not track their status. When you choose to track the status of your submitted jobs the function will not return immediately and will instead continuously ping the Albert service until all of the jobs have finished.
 
@@ -243,18 +214,18 @@
 
 Regardless of which method you choose, it is always a good idea to save the IDs of your jobs for future reference.
 
 Option to run the jobs and wait for results (**track_status=True**) OR submit the jobs and return later to retrieve the results (**track_status=False**). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing.
 
 
 ```python
-# track the status 
-rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=experiment_jobs, track_status=True)
+# track the status
+rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=jobs, track_status=True)
 
-# dont track the status 
+# dont track the status
 # rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=experiment_jobs, track_status=False)
 
 with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:
     for experiment_step_job_id in rf_sweep_experiment_job_ids:
         filewriter.write(experiment_step_job_id)
 ```
 
@@ -268,58 +239,55 @@
 
 Regardless of which method you choose, it is always a good idea to save the IDs of your jobs for future reference.
 
 Option to run the jobs and wait for results (**track_status=True**) OR submit the jobs and return later to retrieve the results (**track_status=False**). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing.
 
 
 ```python
-# track the status 
-rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[experiment_job], track_status=True)[0]
+# track the status
+rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[batch_job], track_status=True)[0]
 
-# dont track the status 
+# dont track the status
 # rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[experiment_job], track_status=False)[0]
 
 with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:
     filewriter.write(rf_sweep_experiment_job_id)
 ```
 
 ## Load results from completed jobs ##
 
-Use **load_jobs_from_id** to retrieve jobs in any state from a previous run. 
+Use **load_jobs_from_id** to retrieve jobs in any state from a previous run.
 
 
 ```python
 with open('bec_rf_sweep_experiment.txt', 'r') as filereader:
     for line in filereader:
         # remove linebreak which is the last character of the string
         oqtant_client.load_job_from_id(line)
-        
 for job_id, job in oqtant_client.active_jobs.items():
     print("id: ", job_id, job.job_type, job.status)
 ```
 
 ## Plot completed jobs ##
 
 When job status is COMPLETE above, plot the results
 
 
 ```python
 for a, job in oqtant_client.active_jobs.items():
     if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:
         job.atoms_2dplot()
         job.atoms_sliceplot()
-        
 # by default jobs that are loaded will only contain the first input/output entry
 # if you have more than one input for a job you can view its details by specifying the 'run' like below
 desired_input_run = 2 # here we are asking for the second input/output entry
 with open('bec_rf_sweep_experiment.txt', 'r') as filereader:
     for line in filereader:
         # remove linebreak which is the last character of the string
         oqtant_client.load_job_from_id(line, run=desired_input_run)
-        
 # now we can display the second input/output entry results
 for a, job in oqtant_client.active_jobs.items():
     if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:
         job.atoms_2dplot()
         job.atoms_sliceplot()
 ```
```

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_5_optimization.ipynb` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_5_optimization.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9859073867124715%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Oqtant Walkthrough 5: BEC Optimization #\\n')], "*

 * *            "delete: [0]}}, 3: {'source': {insert: [(3, '- the oqtant_client interacts with the "*

 * *            "Oraqle server to perform remote lab functions. \\n')], delete: [3]}}, 5: {'source': "*

 * *            "{insert: [(10, 'This cost function is for a 5-dimensional optimization space, where "*

 * *            "the 5 dimensions are the RF corner frequencies.')], delete: [13, 12, 11, 10]}}, 6: "*

 * *            "{'source': […]*

```diff
@@ -1,14 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oqtant Walkthrough 4: BEC Experimentation #\n",
+                "# Oqtant Walkthrough 5: BEC Optimization #\n",
                 "\n",
                 "### This walkthrough reviews authorizing an Oqtant session and an example of optimization for BEC. ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\n",
                 "\n",
                 "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*"
             ]
@@ -58,15 +58,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating a Oqtant Client Instance ##\n",
                 "\n",
                 "### After successful login, create an authorized session with the Oqtant Client ###\n",
-                "- the oqtant_client interacts with the albert server to perform remote lab functions. \n",
+                "- the oqtant_client interacts with the Oraqle server to perform remote lab functions. \n",
                 "- the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -85,30 +85,26 @@
                 "\n",
                 "Larger value = Good:  Condensed and total atom number, condensate fraction \n",
                 "Smaller value = Good: Thermal atom number, temperature \n",
                 "\n",
                 "Ad hoc Cost function: **C = (Nth*T)/Nc**\n",
                 "\n",
                 "### cost_func_5D ### \n",
-                "This cost function is for a 5-dimensional optimization space, where the 5 dimensions are the RF corner frequencies.\n",
-                "\n",
-                "### cost_func_9D ### \n",
-                "This cost function is for a 9-dimensional optimization space, where the 9 dimensions are the RF corner frequencies and the RF powers."
+                "This cost function is for a 5-dimensional optimization space, where the 5 dimensions are the RF corner frequencies."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "costs_9D = []\n",
                 "costs_5D = []\n",
                 "\n",
-                "default_bec_job = {\n",
+                "base_bec_job = {\n",
                 "    \"name\": \"Example Ultracold Matter Generator Job\",\n",
                 "    \"job_type\": \"BEC\",\n",
                 "    \"inputs\": [\n",
                 "        {\n",
                 "            \"values\": {\n",
                 "                \"time_of_flight_ms\": 8.0,\n",
                 "                \"image_type\": \"TIME_OF_FLIGHT\",\n",
@@ -123,34 +119,19 @@
                 "                \"optical_landscape\": None,\n",
                 "                \"lasers\": None,\n",
                 "            },\n",
                 "        }\n",
                 "    ],\n",
                 "}\n",
                 "\n",
-                "def cost_func_9D(RF_freqs_RF_powers):\n",
-                "    RF_freqs = RF_freqs_RF_powers[:5]\n",
-                "    RF_powers = RF_freqs_RF_powers[5:] # this needs to have 5 powers in it now\n",
-                "    default_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"] = RF_freqs\n",
-                "    default_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"powers_mw\"] = RF_powers\n",
-                "    albert_job = oqtant_client.generate_oqtant_job(job=default_bec_job)\n",
-                "    [job_id] = oqtant_client.run_jobs(job_list=[albert_job], track_status=True)\n",
-                "    job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values\n",
-                "    Nth = job_output.thermal_atom_number\n",
-                "    T = job_output.temperature_uk\n",
-                "    Nc = job_output.condensed_atom_number+1\n",
-                "    C = (Nth*T)/Nc\n",
-                "    costs_9D.append(C)\n",
-                "    return C\n",
-                "\n",
-                "def cost_func_5D(RF_freqs, RF_powers = [500, 475, 450, 400, 400]): # added 5th power to default\n",
-                "    default_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"] = RF_freqs\n",
-                "    default_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"powers_mw\"] = RF_powers\n",
-                "    albert_job = oqtant_client.generate_oqtant_job(job=default_bec_job)\n",
-                "    [job_id] = oqtant_client.run_jobs(job_list=[albert_job], track_status=True)\n",
+                "def cost_func_5D(RF_freqs = [17.0, 8.0, 4.0, 1.2, 0.045]): # added 5th power to default\n",
+                "    base_bec_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"] = list(RF_freqs)\n",
+                "    print(base_bec_job)\n",
+                "    job = oqtant_client.generate_oqtant_job(job=base_bec_job)\n",
+                "    [job_id] = oqtant_client.run_jobs(job_list=[job], track_status=True)\n",
                 "    job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values\n",
                 "    Nth = job_output.thermal_atom_number\n",
                 "    T = job_output.temperature_uk\n",
                 "    Nc = job_output.condensed_atom_number\n",
                 "    C = (Nth*T)/Nc\n",
                 "    costs_5D.append(C)\n",
                 "    return C"
@@ -167,16 +148,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))\n",
-                "bnds_9d = ((0,50),(0,50),(0,50),(0,50),(0,50),(0,500),(0,500),(0,500),(0,500))"
+                "bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Choose an optimization algorithm ##\n",
@@ -196,23 +176,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "#res_5d = minimize(cost_func_5D, method=\"TNC\", bounds=bnds_5d, x0 = np.array([17,8,4,1.2,0.05]), options={'maxiter':10})\n",
-                "#res_9d = minimize(cost_func_10D, method=\"TNC\", \n",
-                "#                   x0 = np.array([17,8,4,1.2,0.07,500,475,450,400]), bounds = bnds_9d,options={'maxiter':10})\n",
+                "res_5d = minimize(cost_func_5D, method=\"TNC\", bounds=bnds_5d, x0 = [17,8,4,1.2,0.05], options={'maxiter':10})\n",
                 "\n",
-                "#print(\"optimization results freq tuning only:\")\n",
-                "#print(res_5d)\n",
-                "\n",
-                "#print(\"optimization results freq and power tuning:\")\n",
-                "#print(res_9d)"
+                "print(\"optimization results freq tuning:\")\n",
+                "print(res_5d)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Bayesian Optimization with a Gaussian Process model ##\n"
@@ -220,18 +195,18 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Extract and shape the training data: ##\n",
                 "\n",
-                "X_train_array-like of shape (n_samples, n_features) or list of object\n",
+                "x_train : array-like of shape (n_samples, n_features) or list of object\n",
                 "Feature vectors or other representations of training data (also required for prediction).\n",
                 "\n",
-                "y_train_array-like of shape (n_samples,) or (n_samples, n_targets)\n",
+                "y_train : array-like of shape (n_samples,) or (n_samples, n_targets)\n",
                 "Target values in training data (also required for prediction)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -246,55 +221,48 @@
             "source": [
                 "def cost(Nc, Nth, T):\n",
                 "    C = (Nth*T)/Nc\n",
                 "    return C"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The optimization jobs run above will now be included in your list of currently active jobs:"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "X_global_train = []\n",
-                "y_global_train = []\n",
-                "with open('output.csv', newline='') as csvfile:\n",
-                "    r = csv.reader(csvfile, delimiter=' ', quotechar='|')\n",
-                "    for row in r:\n",
-                "        if len(row)==26:\n",
-                "            \n",
-                "            rf_a_mhz = float(row[4][:-1])\n",
-                "            rf_b_mhz = float(row[6][:-1])\n",
-                "            rf_c_mhz = float(row[8][:-1])\n",
-                "            rf_d_mhz = float(row[10][:-1])\n",
-                "            rf_e_mhz = float(row[12][:-1])\n",
-                "            pow_a_mw = float(row[14][:-1])\n",
-                "            pow_b_mw = float(row[16][:-1])\n",
-                "            pow_c_mw = float(row[18][:-1])\n",
-                "            pow_d_mw = float(row[20][:-27])\n",
-                "            \n",
-                "            condensed_atom_number = round(float(row[23][:-1]))\n",
-                "            thermal_atom_number = round(float(row[21][:-1]))\n",
-                "            temperature_uk = float(row[25][:-2])\n",
-                "            if temperature_uk > 0 and condensed_atom_number > 100:\n",
-                "                X_global_train.append([rf_a_mhz,\n",
-                "                                       rf_b_mhz,\n",
-                "                                       rf_c_mhz,\n",
-                "                                       rf_d_mhz,\n",
-                "                                       rf_e_mhz,\n",
-                "                                      pow_a_mw, \n",
-                "                                      pow_b_mw, \n",
-                "                                      pow_c_mw, \n",
-                "                                      pow_d_mw])\n",
-                "                y_global_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk))\n",
-                "\n",
-                "#X_global_train = np.asarray(X_global_train)\n",
-                "#y_global_train = np.asarray(y_global_train)\n",
-                "\n",
-                "                "
+                "oqtant_client.see_active_jobs()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x_train = []\n",
+                "y_train = []\n",
+                "for job_id in oqtant_client.active_jobs:\n",
+                "    job = oqtant_client.active_jobs[job_id]\n",
+                "    output = job.inputs[0].output.values\n",
+                "    condensed_atom_number = output.condensed_atom_number\n",
+                "    thermal_atom_number = output.thermal_atom_number\n",
+                "    temperature_uk = output.temperature_uk\n",
+                "    input = job.inputs[0].values\n",
+                "    x_train.append(input.rf_evaporation.frequencies_mhz)\n",
+                "    y_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk)) \n",
+                "    "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -410,41 +378,36 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "#X = sample_domain\n",
-                "#y = np.asarray([cost_func_9D(x) for x in X])\n",
-                "#Oqtant_model = GPR()\n",
-                "#Oqtant_model.fit(X, y)\n",
-                "\n",
-                "X = X_global_train\n",
-                "y = y_global_train\n",
+                "X = x_train\n",
+                "Y = y_train\n",
                 "Oqtant_model = GPR()\n",
-                "Oqtant_model.fit(X_global_train, y_global_train)\n",
+                "Oqtant_model.fit(x_train, y_train)\n",
                 "\n",
                 "cost = []\n",
                 "\n",
-                "for i in range(20):\n",
+                "for i in range(10):\n",
                 "    # select the next point to sample\n",
-                "    x = optimize_acquisition(X, y, Oqtant_model, 500)\n",
+                "    x = optimize_acquisition(X, Y, Oqtant_model, 500)\n",
                 "    print('x', x)\n",
                 "    # sample the point\n",
-                "    actual = cost_func_9D(x)\n",
+                "    actual = cost_func_5D(x)\n",
                 "    cost.append(actual)\n",
                 "    # summarize the finding\n",
                 "    est, _ = surrogate(Oqtant_model, [x])\n",
                 "    print(x, est, actual)\n",
                 "    # add the data to the dataset\n",
                 "    X = np.vstack((X, [x]))\n",
-                "    y.append(actual)\n",
+                "    Y.append(actual)\n",
                 "    # update the model\n",
-                "    Oqtant_model.fit(X, y)"
+                "    Oqtant_model.fit(X, Y)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -454,16 +417,16 @@
                 "#plt.yscale(\"log\")\n",
                 "plt.xlabel(\"function evaluations\")\n",
                 "plt.ylabel(\"Cost\")\n",
                 "plt.title(\"20 evaluations, 500 surrogate samples, 335pm 5_5_21\")\n",
                 "plt.savefig(\"335pm 5_5_21.png\")\n",
                 "plt.show()\n",
                 "# best result\n",
-                "ix = np.argmax(y)\n",
-                "print('Best Result:'+str([X[ix], y[ix]]))"
+                "ix = np.argmax(Y)\n",
+                "print('Best Result:'+str([X[ix], Y[ix]]))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -475,13 +438,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `oqtant-0.15.0/documentation/walkthroughs/walkthrough_5_optimization.md` & `oqtant-0.15.1/documentation/walkthroughs/walkthrough_5_optimization.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Oqtant Walkthrough 4: BEC Experimentation
+# Oqtant Walkthrough 5: BEC Optimization #
 
 ### This walkthrough reviews authorizing an Oqtant session and an example of optimization for BEC. ###
 
 For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
 
 *Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
 
@@ -38,43 +38,40 @@
 
 token = get_user_token()
 ```
 
 ## Creating a Oqtant Client Instance ##
 
 ### After successful login, create an authorized session with the Oqtant Client ###
-- the oqtant_client interacts with the albert server to perform remote lab functions. 
+- the oqtant_client interacts with the Oraqle server to perform remote lab functions.
 - the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
 
 
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
-## Define a cost function for optimization ## 
+## Define a cost function for optimization ##
 
 A cost function is a metric calculated for the system of interest which is lowered over time via some optimization script 
 
-Larger value = Good:  Condensed and total atom number, condensate fraction 
-Smaller value = Good: Thermal atom number, temperature 
+Larger value = Good:  Condensed and total atom number, condensate fraction
+Smaller value = Good: Thermal atom number, temperature
 
 Ad hoc Cost function: **C = (Nth*T)/Nc**
 
-### cost_func_5D ### 
+### cost_func_5D ###
 This cost function is for a 5-dimensional optimization space, where the 5 dimensions are the RF corner frequencies.
 
-### cost_func_9D ### 
-This cost function is for a 9-dimensional optimization space, where the 9 dimensions are the RF corner frequencies and the RF powers.
 
 
 ```python
-costs_9D = []
 costs_5D = []
 
-default_bec_job = {
+base_bec_job = {
     "name": "Example Ultracold Matter Generator Job",
     "job_type": "BEC",
     "inputs": [
         {
             "values": {
                 "time_of_flight_ms": 8.0,
                 "image_type": "TIME_OF_FLIGHT",
@@ -89,152 +86,114 @@
                 "optical_landscape": None,
                 "lasers": None,
             },
         }
     ],
 }
 
-def cost_func_9D(RF_freqs_RF_powers):
-    RF_freqs = RF_freqs_RF_powers[:5]
-    RF_powers = RF_freqs_RF_powers[5:] # this needs to have 5 powers in it now
-    default_bec_job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"] = RF_freqs
-    default_bec_job["inputs"][0]["values"]["rf_evaporation"]["powers_mw"] = RF_powers
-    albert_job = oqtant_client.generate_oqtant_job(job=default_bec_job)
-    [job_id] = oqtant_client.run_jobs(job_list=[albert_job], track_status=True)
-    job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values
-    Nth = job_output.thermal_atom_number
-    T = job_output.temperature_uk
-    Nc = job_output.condensed_atom_number+1
-    C = (Nth*T)/Nc
-    costs_9D.append(C)
-    return C
-
-def cost_func_5D(RF_freqs, RF_powers = [500, 475, 450, 400, 400]): # added 5th power to default
-    default_bec_job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"] = RF_freqs
-    default_bec_job["inputs"][0]["values"]["rf_evaporation"]["powers_mw"] = RF_powers
-    albert_job = oqtant_client.generate_oqtant_job(job=default_bec_job)
-    [job_id] = oqtant_client.run_jobs(job_list=[albert_job], track_status=True)
+def cost_func_5D(RF_freqs = [17.0, 8.0, 4.0, 1.2, 0.045]): # added 5th power to default
+    base_bec_job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"] = list(RF_freqs)
+    print(base_bec_job)
+    job = oqtant_client.generate_oqtant_job(job=base_bec_job)
+    [job_id] = oqtant_client.run_jobs(job_list=[job], track_status=True)
     job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values
     Nth = job_output.thermal_atom_number
     T = job_output.temperature_uk
     Nc = job_output.condensed_atom_number
     C = (Nth*T)/Nc
     costs_5D.append(C)
     return C
 ```
 
-## Set bounds for optimization ## 
+## Set bounds for optimization ##
 
 Bounds will prevent invalid jobs parameters from being submitted to the job runner.
 
 
 ```python
 bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))
-bnds_9d = ((0,50),(0,50),(0,50),(0,50),(0,50),(0,500),(0,500),(0,500),(0,500))
 ```
 
 ## Choose an optimization algorithm ##
 
 Here, I chose a truncated Newton method (TNC). TNC uses a truncated Newton algorithm to minimize a function with variables subject to bounds. Within scipy.optimize.minimize there are several options for optimizers which allow for bounded variables:  
 
- - L-BFGS-B 
+ - L-BFGS-B
  - TNC
  - COBYLA
  - SLSQP
- 
- 
+
+
  ## Provide initial conditions and max iterations ##
- 
- I chose the web app default parameters for a mixed cloud for the x0 initial conditions. Specify iterations with **options={'maxiter':10}**. Note that each iteration may involve several evaluations of the cost function (which means several jobs), so setting **'maxiter':30** will not run within a single 24 hour period. 
 
+ I chose the web app default parameters for a mixed cloud for the x0 initial conditions. Specify iterations with **options={'maxiter':10}**. Note that each iteration may involve several evaluations of the cost function (which means several jobs), so setting **'maxiter':30** will not run within a single 24 hour period.
 
-```python
-#res_5d = minimize(cost_func_5D, method="TNC", bounds=bnds_5d, x0 = np.array([17,8,4,1.2,0.05]), options={'maxiter':10})
-#res_9d = minimize(cost_func_10D, method="TNC", 
-#                   x0 = np.array([17,8,4,1.2,0.07,500,475,450,400]), bounds = bnds_9d,options={'maxiter':10})
 
-#print("optimization results freq tuning only:")
-#print(res_5d)
+```python
+res_5d = minimize(cost_func_5D, method="TNC", bounds=bnds_5d, x0 = [17,8,4,1.2,0.05], options={'maxiter':10})
 
-#print("optimization results freq and power tuning:")
-#print(res_9d)
+print("optimization results freq tuning:")
+print(res_5d)
 ```
 
 ## Bayesian Optimization with a Gaussian Process model ##
 
 
 ## Extract and shape the training data: ##
 
-X_train_array-like of shape (n_samples, n_features) or list of object
+x_train : array-like of shape (n_samples, n_features) or list of object
 Feature vectors or other representations of training data (also required for prediction).
 
-y_train_array-like of shape (n_samples,) or (n_samples, n_targets)
+y_train : array-like of shape (n_samples,) or (n_samples, n_targets)
 Target values in training data (also required for prediction)
 
 ## Define a new target cost function ##
 
 
 ```python
 def cost(Nc, Nth, T):
     C = (Nth*T)/Nc
     return C
 ```
 
+The optimization jobs run above will now be included in your list of currently active jobs:
+
 
 ```python
-X_global_train = []
-y_global_train = []
-with open('output.csv', newline='') as csvfile:
-    r = csv.reader(csvfile, delimiter=' ', quotechar='|')
-    for row in r:
-        if len(row)==26:
-            
-            rf_a_mhz = float(row[4][:-1])
-            rf_b_mhz = float(row[6][:-1])
-            rf_c_mhz = float(row[8][:-1])
-            rf_d_mhz = float(row[10][:-1])
-            rf_e_mhz = float(row[12][:-1])
-            pow_a_mw = float(row[14][:-1])
-            pow_b_mw = float(row[16][:-1])
-            pow_c_mw = float(row[18][:-1])
-            pow_d_mw = float(row[20][:-27])
-            
-            condensed_atom_number = round(float(row[23][:-1]))
-            thermal_atom_number = round(float(row[21][:-1]))
-            temperature_uk = float(row[25][:-2])
-            if temperature_uk > 0 and condensed_atom_number > 100:
-                X_global_train.append([rf_a_mhz,
-                                       rf_b_mhz,
-                                       rf_c_mhz,
-                                       rf_d_mhz,
-                                       rf_e_mhz,
-                                      pow_a_mw, 
-                                      pow_b_mw, 
-                                      pow_c_mw, 
-                                      pow_d_mw])
-                y_global_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk))
+oqtant_client.see_active_jobs()
+```
 
-#X_global_train = np.asarray(X_global_train)
-#y_global_train = np.asarray(y_global_train)
 
-                
+```python
+x_train = []
+y_train = []
+for job_id in oqtant_client.active_jobs:
+    job = oqtant_client.active_jobs[job_id]
+    output = job.inputs[0].output.values
+    condensed_atom_number = output.condensed_atom_number
+    thermal_atom_number = output.thermal_atom_number
+    temperature_uk = output.temperature_uk
+    input = job.inputs[0].values
+    x_train.append(input.rf_evaporation.frequencies_mhz)
+    y_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk))
+
 ```
 
 
 ```python
 # surrogate or approximation for the objective function
 def surrogate(model, X):
     # catch any warning generated when making a prediction
     with catch_warnings():
         # ignore generated warnings
         simplefilter("ignore")
         return model.predict(X, return_std=True)
 ```
 
-## Define an acquisition function ## 
+## Define an acquisition function ##
 
 This is a score assigned to each candidate sample on the domain. 
 
 The surrogate function can be used as an acquisition (minimizing the surrogate is the goal after all)
 
 OR
 
@@ -277,15 +236,14 @@
     random_number = np.random.uniform()+(1E-9)
     sample = scale*random_number+domain[1]
     return sample
 ```
 
 ## Define an optimizer on the acquisition function ##
 
-Here I have chosen a random search over the domain, but other search algorithms can be used. 
 
 
 ```python
 def optimize_acquisition(X, y, model, sample_population):
     # random search, generate random samples
     Xsamples = np.asarray([[rand_domain_sample(domain[i]) for i in range(len(X[0]))] for j in range(sample_population)])
     Xsamples = Xsamples.reshape(len(Xsamples), len(X[0]))
@@ -296,50 +254,45 @@
     return Xsamples[ix]
 ```
 
 ## Perform the optimization ##
 
 
 ```python
-#X = sample_domain
-#y = np.asarray([cost_func_9D(x) for x in X])
-#Oqtant_model = GPR()
-#Oqtant_model.fit(X, y)
-
-X = X_global_train
-y = y_global_train
+X = x_train
+Y = y_train
 Oqtant_model = GPR()
-Oqtant_model.fit(X_global_train, y_global_train)
+Oqtant_model.fit(x_train, y_train)
 
 cost = []
 
-for i in range(20):
+for i in range(10):
     # select the next point to sample
-    x = optimize_acquisition(X, y, Oqtant_model, 500)
+    x = optimize_acquisition(X, Y, Oqtant_model, 500)
     print('x', x)
     # sample the point
-    actual = cost_func_9D(x)
+    actual = cost_func_5D(x)
     cost.append(actual)
     # summarize the finding
     est, _ = surrogate(Oqtant_model, [x])
     print(x, est, actual)
     # add the data to the dataset
     X = np.vstack((X, [x]))
-    y.append(actual)
+    Y.append(actual)
     # update the model
-    Oqtant_model.fit(X, y)
+    Oqtant_model.fit(X, Y)
 ```
 
 
 ```python
 # plot all samples and the final surrogate function
 plt.plot(cost[5:])
 #plt.yscale("log")
 plt.xlabel("function evaluations")
 plt.ylabel("Cost")
 plt.title("20 evaluations, 500 surrogate samples, 335pm 5_5_21")
 plt.savefig("335pm 5_5_21.png")
 plt.show()
 # best result
-ix = np.argmax(y)
-print('Best Result:'+str([X[ix], y[ix]]))
+ix = np.argmax(Y)
+print('Best Result:'+str([X[ix], Y[ix]]))
 ```
```

### Comparing `oqtant-0.15.0/oqtant/oqtant_client.py` & `oqtant-0.15.1/oqtant/oqtant_client.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/oqtant/schemas/job.py` & `oqtant-0.15.1/oqtant/schemas/job.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/oqtant/settings.py` & `oqtant-0.15.1/oqtant/settings.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/oqtant/util/auth.py` & `oqtant-0.15.1/oqtant/util/auth.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/oqtant/util/exceptions.py` & `oqtant-0.15.1/oqtant/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.0/pyproject.toml` & `oqtant-0.15.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqtant"
-version = "0.15.0"
+version = "0.15.1"
 description = "Oqtant Desktop Suite"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Hannah North <hannah.north@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
@@ -18,14 +18,16 @@
 exclude = [
   "oqtant/.pytest_cache/**/*",
   "oqtant/**/__pycache__",
   "oqtant/.gitignore",
   "oqtant/tests/**/*",
   "oqtant/README-DEV.md",
 ]
+homepage = "https://albert-dev.coldquanta.com/"
+repository = "https://gitlab.com/infleqtion/albert/oqtant"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 matplotlib = "~3.6.2"
 numpy = "^1.23.2"
 pydantic = "^1.10.1"
 requests = "^2.28.1"
```

### Comparing `oqtant-0.15.0/setup.py` & `oqtant-0.15.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 
 entry_points = \
 {'console_scripts': ['authorize = '
                      'oqtant.tests.integration.authorize:authorize']}
 
 setup_kwargs = {
     'name': 'oqtant',
-    'version': '0.15.0',
+    'version': '0.15.1',
     'description': 'Oqtant Desktop Suite',
     'long_description': "# Oqtant\n\n[![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)\n[![pypi](https://img.shields.io/pypi/v/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)\n[![versions](https://img.shields.io/pypi/pyversions/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)\n[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)\n\n## 🚀 Quick Install\n\n```python\npip install oqtant\n```\n\n## 🧭 Introduction\n\nThis API contains tools to:\n\n- Access all the functionality of the Albert Web App (https://albert-dev.coldquanta.com)\n\n  - BARRIER (Barrier Manipulator) jobs\n  - BEC (Ultracold Matter) jobs\n\n- Build parameterized (i.e. optimization) experiments using OqtantJobs\n\n- Submit and retrieve OqtantJob results\n\n## 🤖 How Oqtant Works\n\n- Construct a single or list of jobs using the OqtantJob class\n\n  - 1D parameter sweeps are supported\n\n- Run a single or list of jobs using run_jobs(). The jobs are submitted to run on hardware in FIFO queue.\n\n  - job lists are run sequentially (uninterrupted) unless list exceeds 30 jobs\n\n- As jobs run, OqtantJob objects are created automatically and stored in active_jobs.\n\n  - View these jobs with see_active_jobs()\n  - These jobs are available until the python session ends.\n\n- To operate on jobs from a current or previous session, load them into active_jobs with\n\n  - load_job_from_id(), load_job_from_id_list(), load_job_from_file(), load_job_from_file_list()\n\n- To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.\n\nNeed help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!\n\n## 📓 Documentation\n\n- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, how to run the walkthrough notebooks)\n- [Walkthroughs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/walkthroughs/walkthroughs.md) (demos for creating and submitting jobs)\n- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oqtant_api_docs.md)\n- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/albert_api_docs.md)\n- [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)\n",
     'author': 'Larry Buza',
     'author_email': 'lawrence.buza@coldquanta.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://albert-dev.coldquanta.com/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<3.12',
 }
```

### Comparing `oqtant-0.15.0/PKG-INFO` & `oqtant-0.15.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: oqtant
-Version: 0.15.0
+Version: 0.15.1
 Summary: Oqtant Desktop Suite
+Home-page: https://albert-dev.coldquanta.com/
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +26,15 @@
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0)
+Project-URL: Repository, https://gitlab.com/infleqtion/albert/oqtant
 Description-Content-Type: text/markdown
 
 # Oqtant
 
 [![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
 [![pypi](https://img.shields.io/pypi/v/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)
 [![versions](https://img.shields.io/pypi/pyversions/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)
```

