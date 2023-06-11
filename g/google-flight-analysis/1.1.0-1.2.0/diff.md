# Comparing `tmp/google-flight-analysis-1.1.0.tar.gz` & `tmp/google-flight-analysis-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-flight-analysis-1.1.0.tar", last modified: Mon May  8 01:03:54 2023, max compression
+gzip compressed data, was "google-flight-analysis-1.2.0.tar", last modified: Sun Jun 11 23:16:05 2023, max compression
```

## Comparing `google-flight-analysis-1.1.0.tar` & `google-flight-analysis-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.github/workflows/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/.github/workflows/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.github/workflows/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/src/google_flight_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/flight.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/src/google_flight_analysis/scrape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.893623 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 01:03:54.000000 google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:03:54.897623 google-flight-analysis-1.1.0/tests/test_data/.access/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/.access/CDG-IST.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/.access/LGA-RDU.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/CDG-IST.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/LGA-RDU.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/test1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-08 01:03:45.000000 google-flight-analysis-1.1.0/tests/test_data/test2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.741348 google-flight-analysis-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.737348 google-flight-analysis-1.2.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.737348 google-flight-analysis-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.737348 google-flight-analysis-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/.github/workflows/publish-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/.github/workflows/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.737348 google-flight-analysis-1.2.0/.github/workflows/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/.github/workflows/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-11 23:16:05.741348 google-flight-analysis-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-11 23:16:05.741348 google-flight-analysis-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.737348 google-flight-analysis-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.741348 google-flight-analysis-1.2.0/src/google_flight_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/src/google_flight_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/src/google_flight_analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/src/google_flight_analysis/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/src/google_flight_analysis/flight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/src/google_flight_analysis/scrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.741348 google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-11 23:16:05.000000 google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-11 23:16:05.000000 google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:16:05.000000 google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-11 23:16:05.000000 google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-11 23:16:05.000000 google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 23:16:05.000000 google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.741348 google-flight-analysis-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.741348 google-flight-analysis-1.2.0/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:16:05.741348 google-flight-analysis-1.2.0/tests/test_data/.access/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/tests/test_data/.access/CDG-IST.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/tests/test_data/.access/LGA-RDU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/tests/test_data/CDG-IST.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/tests/test_data/LGA-RDU.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/tests/test_data/test1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-11 23:15:54.000000 google-flight-analysis-1.2.0/tests/test_data/test2.csv
```

### Comparing `google-flight-analysis-1.1.0/.circleci/config.yml` & `google-flight-analysis-1.2.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.1.0/.github/workflows/scripts/release.py` & `google-flight-analysis-1.2.0/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.1.0/LICENSE` & `google-flight-analysis-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.1.0/PKG-INFO` & `google-flight-analysis-1.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-flight-analysis
-Version: 1.1.0
+Version: 1.2.0
 Summary: Scraping flight data from Google Flights and analyzing.
 Home-page: https://github.com/kcelebi/flight_analysis
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
 Project-URL: Bug Tracker, https://github.com/kcelebi/flight_analysis/issues
 Project-URL: Changelog, https://github.com/kcelebi/flight_analysis/releases
 Classifier: Programming Language :: Python :: 3
@@ -12,26 +12,29 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![kcelebi](https://circleci.com/gh/celebi-pkg/flight-analysis.svg?style=svg)](https://circleci.com/gh/celebi-pkg/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://img.shields.io/badge/PyPI-1.0.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-1.2.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
+[![TestPyPI](https://img.shields.io/badge/PyPI-1.1.1--alpha.11-blue)](https://test.pypi.org/project/google-flight-analysis/1.1.1a11/)
 
 # Flight Analysis
 
-This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
+This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 5/25/2023) are:
 
-- Scraping tools for Google Flights
+- Detailed scraping and querying tools for Google Flights
+- Ability to store data locally or to SQL tables
 - Base analytical tools/methods for price forecasting/summary
 
 The features in development are:
 
 - Models to demonstrate ML techniques on forecasting
+- Querying of advanced features
 - API for access to previously collected data
 
 ## Table of Contents
 - [Overview](#Overview)
 - [Usage](#usage)
 - [Updates & New Features](#updates-&-new-features)
 - [Real Usage](#real-usage) 😄
@@ -71,27 +74,54 @@
 	import sys
 	sys.path.append('src/google_flight_analysis')
 	from scrape import *
 
 
 Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
-	# Try to keep the dates in format YYYY-mm-dd
-	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-10') # obtain our scrape object
-	dataframe = result.data # outputs a Pandas DF with flight prices/info
-	origin = result.origin # 'JFK'
-	dest = result.dest # 'IST'
-	date_leave = result.date_leave # '2023-05-20'
-	date_return = result.date_return # '2023-06-10'
+	# Keep the dates in format YYYY-mm-dd
+	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-20') # obtain our scrape object, represents out query
+	result.type # This is in a round-trip format
+	result.origin # ['JFK', 'IST']
+	result.dest # ['IST', 'JFK']
+	result.dates # ['2023-07-20', '2023-08-20']
+	print(result) # get unqueried str representation
+
+A `Scrape` object represents a Google Flights query to be run. It maintains flights as a sequence of one or more one-way flights which have a origin, destination, and flight date. The above object for a round-trip flight from JFK to IST is a sequence of JFK --> IST, then IST --> JFK. We can obtain the data as follows:
+
+	ScrapeObjects(result) # runs selenium through ChromeDriver, modifies results in-place
+	result.data # returns pandas DF
+	print(result) # get queried representation of result
 
-You can also scrape for one-way trips now:
+You can also scrape for one-way trips:
 
 	results = Scrape('JFK', 'IST', '2023-08-20')
-	result.data.head() #see data
+	ScrapeObjects(result)
+	result.data #see data
 
+You can also scrape chain-trips, which are defined as a sequence of one-way flights that have no direct relation to each other, other than being in chronological order. 
+
+	# chain-trip format: origin, dest, date, origin, dest, date, ...
+	result = Scrape('JFK', 'IST', '2023-08-20', 'RDU', 'LGA', '2023-12-25', 'EWR', 'SFO', '2024-01-20')
+	result.type # chain-trip
+	ScrapeObjects(result)
+	result.data # see data
+
+You can also scrape perfect-chains, which are defined as a sequence of one-way flights such that the destination of the previous flight is the origin of the next and the origin of the chain is the final destination of the chain (a cycle).
+
+	# perfect-chain format: origin, date, origin, date, ..., first_origin
+	result = Scrape("JFK", "2023-09-20", "IST", "2023-09-25", "CDG", "2023-10-10", "LHR", "2023-11-01", "JFK")
+	result.type # perfect-chain
+	ScrapeObjects(result)
+	result.data # see data
+
+You can read more about the different type of trips in the documentation. Scrape objects can be added to one another to create larger queries. This is under the conditions:
+
+1. The objects being added are the same type of trip (one-way, round-trip, etc)
+2. The objects being added are either both unqueried or both queried
 
 ## Updates & New Features
 
 Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
 
 
 <!--
```

### Comparing `google-flight-analysis-1.1.0/README.md` & `google-flight-analysis-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [![kcelebi](https://circleci.com/gh/celebi-pkg/flight-analysis.svg?style=svg)](https://circleci.com/gh/celebi-pkg/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://img.shields.io/badge/PyPI-1.0.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-1.2.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
+[![TestPyPI](https://img.shields.io/badge/PyPI-1.1.1--alpha.11-blue)](https://test.pypi.org/project/google-flight-analysis/1.1.1a11/)
 
 # Flight Analysis
 
-This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
+This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 5/25/2023) are:
 
-- Scraping tools for Google Flights
+- Detailed scraping and querying tools for Google Flights
+- Ability to store data locally or to SQL tables
 - Base analytical tools/methods for price forecasting/summary
 
 The features in development are:
 
 - Models to demonstrate ML techniques on forecasting
+- Querying of advanced features
 - API for access to previously collected data
 
 ## Table of Contents
 - [Overview](#Overview)
 - [Usage](#usage)
 - [Updates & New Features](#updates-&-new-features)
 - [Real Usage](#real-usage) 😄
@@ -55,27 +58,54 @@
 	import sys
 	sys.path.append('src/google_flight_analysis')
 	from scrape import *
 
 
 Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
-	# Try to keep the dates in format YYYY-mm-dd
-	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-10') # obtain our scrape object
-	dataframe = result.data # outputs a Pandas DF with flight prices/info
-	origin = result.origin # 'JFK'
-	dest = result.dest # 'IST'
-	date_leave = result.date_leave # '2023-05-20'
-	date_return = result.date_return # '2023-06-10'
+	# Keep the dates in format YYYY-mm-dd
+	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-20') # obtain our scrape object, represents out query
+	result.type # This is in a round-trip format
+	result.origin # ['JFK', 'IST']
+	result.dest # ['IST', 'JFK']
+	result.dates # ['2023-07-20', '2023-08-20']
+	print(result) # get unqueried str representation
+
+A `Scrape` object represents a Google Flights query to be run. It maintains flights as a sequence of one or more one-way flights which have a origin, destination, and flight date. The above object for a round-trip flight from JFK to IST is a sequence of JFK --> IST, then IST --> JFK. We can obtain the data as follows:
+
+	ScrapeObjects(result) # runs selenium through ChromeDriver, modifies results in-place
+	result.data # returns pandas DF
+	print(result) # get queried representation of result
 
-You can also scrape for one-way trips now:
+You can also scrape for one-way trips:
 
 	results = Scrape('JFK', 'IST', '2023-08-20')
-	result.data.head() #see data
+	ScrapeObjects(result)
+	result.data #see data
 
+You can also scrape chain-trips, which are defined as a sequence of one-way flights that have no direct relation to each other, other than being in chronological order. 
+
+	# chain-trip format: origin, dest, date, origin, dest, date, ...
+	result = Scrape('JFK', 'IST', '2023-08-20', 'RDU', 'LGA', '2023-12-25', 'EWR', 'SFO', '2024-01-20')
+	result.type # chain-trip
+	ScrapeObjects(result)
+	result.data # see data
+
+You can also scrape perfect-chains, which are defined as a sequence of one-way flights such that the destination of the previous flight is the origin of the next and the origin of the chain is the final destination of the chain (a cycle).
+
+	# perfect-chain format: origin, date, origin, date, ..., first_origin
+	result = Scrape("JFK", "2023-09-20", "IST", "2023-09-25", "CDG", "2023-10-10", "LHR", "2023-11-01", "JFK")
+	result.type # perfect-chain
+	ScrapeObjects(result)
+	result.data # see data
+
+You can read more about the different type of trips in the documentation. Scrape objects can be added to one another to create larger queries. This is under the conditions:
+
+1. The objects being added are the same type of trip (one-way, round-trip, etc)
+2. The objects being added are either both unqueried or both queried
 
 ## Updates & New Features
 
 Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
 
 
 <!--
```

### Comparing `google-flight-analysis-1.1.0/setup.cfg` & `google-flight-analysis-1.2.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	tqdm
 	numpy
 	pandas
 	selenium
+	sqlalchemy
+	chromedriver-autoinstaller
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	flight_analysis = flight_analysis.app:entry_point
```

### Comparing `google-flight-analysis-1.1.0/src/google_flight_analysis/cache.py` & `google-flight-analysis-1.2.0/src/google_flight_analysis/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   Written by Kaya Celebi, April 2023
 ****************************************************************************************************************************************************************/'''
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 from datetime import date, datetime, timedelta
-import sqlite3
+from sqlalchemy import create_engine, insert, delete
 import json
 import os
 
 __all__ = ['CacheControl']
 
 class _CacheControl:
 
@@ -22,28 +22,40 @@
 	'''
 	def __call__(self, *args):
 		self.directory, self.access = _CacheControl._check_dir(args[0])
 		for obj in tqdm(args[1:-1], desc = "Caching Data"):
 			if _CacheControl._check_scrape(obj):
 				self.cache(obj, args[-1])
 
+
 	def __str__(self):
 		return "Function to store scraped data."
 
 	def __repr__(self):
 		return "<Function to store scraped data: CacheControl>"
 
-	def cache(self, obj, db):
+	def cache(self, obj, db = True):
 		fname = self.directory + _CacheControl._get_file_name(obj.origin, obj.dest, access = False)
 		access = self.access + _CacheControl._get_file_name(obj.origin, obj.dest, access = True)
 		df = obj.data
 		current_access = df['Access Date'].values[0]
 
 		if db:
-			...
+			if not os.path.isfile(self.directory):
+				try:
+					print('DB does not exist, creating DB file')
+					os.system('touch {db}'.format(db = self.directory))
+				except:
+					raise Exception("The provided db file name does not exist or URL is malformed.")
+		
+			engine = create_engine("sqlite:///{db}".format(db = self.directory))
+			df.to_sql(name='flights', index = False, if_exists='append', con=engine)
+			engine.dispose()
+
+			return
 
 		# If file already exists
 		if os.path.isfile(fname):
 			# Check if most recent access is today
 			with open(access) as file:
 				recent_access = file.readline()
 				if recent_access != current_access:
@@ -52,43 +64,30 @@
 				else:
 					return # Data already in csv, redundant
 
 		df.to_csv(fname)
 		with open(access, 'w') as file:
 			file.write(current_access)
 
-
-	def connect_db(self):
-		conn = sqlite3.connect(self.directory + 'flights.db')
-
-		return conn
-
-	def disconnect_db(self, conn):
-		conn.close()
-
-	def create_table():
-		...
-
-
 	'''
 		Check that the scraping instance is valid
 	'''
 	@staticmethod
 	def _check_scrape(arg):
 		return True#isinstance(arg, _Scrape)
 
 	'''
 		Check root directory formatting
 	'''
 	@staticmethod
 	def _check_dir(arg):
-		arg = arg if arg[-1] == '/' else arg + '/'
+		arg = arg if arg[-1] == '/' or arg.endswith('.db') else arg + '/'
 
 		# Initializing .access metadata for new directory type
-		if not os.path.exists(arg + '.access/'):
+		if not os.path.exists(arg + '.access/') and not arg.endswith('.db'):
 			os.system('mkdir {dir}.access'.format(dir = arg))
 
 		return arg, arg + '.access/'
 		
 
 	'''
 		Generate a filename given the object
```

### Comparing `google-flight-analysis-1.1.0/src/google_flight_analysis/flight.py` & `google-flight-analysis-1.2.0/src/google_flight_analysis/flight.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from tqdm import tqdm
 
 __all__ = ['Flight']
 
 
 class Flight:
 
-	def __init__(self, dl, *args):
+	def __init__(self, date, *args):
 		self._id = 1
 		self._origin = None
 		self._dest = None
-		self._date = dl
-		self._dow = datetime.strptime(dl, '%Y-%m-%d').isoweekday() # day of week
+		self._date = date
+		self._dow = datetime.strptime(date, '%Y-%m-%d').isoweekday() # day of week
 		self._airline = None
 		self._flight_time = None
 		self._num_stops = None
 		self._stops = None
 		self._co2 = None
 		self._emissions = None
 		self._price = None
@@ -25,18 +25,20 @@
 		self._time_leave = None
 		self._time_arrive = None
 		self._trash = []
 
 		self._parse_args(*args)
 
 	def __repr__(self):
-		return "__repr__ To be Implemented"
+		return "Flight(id:{id}, {org}-->{dest} on {date})".format(
+			id = self._id, org = self._origin, dest = self._dest, date = self._date
+		)
 
 	def __str__(self):
-		return "__str__ To be Implemented"
+		return self.__repr__()
 
 	@property
 	def id(self):
 		return self._id
 
 	@property
 	def origin(self):
@@ -99,15 +101,15 @@
 		return self._time_leave
 
 	@property
 	def time_arrive(self):
 		return self._time_arrive
 
 	def _classify_arg(self, arg):
-		if ('AM' in arg or 'PM' in arg) and len(self._times) < 2:
+		if ('AM' in arg or 'PM' in arg) and len(self._times) < 2 and ':' in arg:
 			# arrival or departure time
 			delta = timedelta(days = 0)
 			if arg[-2] == '+':
 				delta = timedelta(days = int(arg[-1]))
 				arg = arg[:-2]
 
 			date_format = "%Y-%m-%d %I:%M%p"
@@ -155,25 +157,25 @@
 			self._classify_arg(arg)
 
 	@staticmethod
 	def dataframe(flights):
 		data = {
 			'Departure datetime': [],
 			'Arrival datetime': [],
-			'Airline(s)' : [],
-			'Travel Time' : [],
 			'Origin' : [],
 			'Destination' : [],
+			'Airline(s)' : [],
+			'Travel Time' : [],
+			'Price ($)' : [],
 			'Num Stops' : [],
 			'Layover' : [],
+			'Access Date' : [],
 			#'Stop Location' : [],
 			'CO2 Emission (kg)' : [],
-			'Emission Diff (%)' : [],
-			'Price ($)' : [],
-			'Access Date' : []
+			'Emission Diff (%)' : []
 		}
 
 		for flight in flights:
 			data['Departure datetime'] += [flight.time_leave]
 			data['Arrival datetime'] += [flight.time_arrive]
 
 			data['Airline(s)'] += [flight.airline]
```

### Comparing `google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/PKG-INFO` & `google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-flight-analysis
-Version: 1.1.0
+Version: 1.2.0
 Summary: Scraping flight data from Google Flights and analyzing.
 Home-page: https://github.com/kcelebi/flight_analysis
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
 Project-URL: Bug Tracker, https://github.com/kcelebi/flight_analysis/issues
 Project-URL: Changelog, https://github.com/kcelebi/flight_analysis/releases
 Classifier: Programming Language :: Python :: 3
@@ -12,26 +12,29 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![kcelebi](https://circleci.com/gh/celebi-pkg/flight-analysis.svg?style=svg)](https://circleci.com/gh/celebi-pkg/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://img.shields.io/badge/PyPI-1.0.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-1.2.0-brightgreen)](https://pypi.org/project/google-flight-analysis/)
+[![TestPyPI](https://img.shields.io/badge/PyPI-1.1.1--alpha.11-blue)](https://test.pypi.org/project/google-flight-analysis/1.1.1a11/)
 
 # Flight Analysis
 
-This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
+This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 5/25/2023) are:
 
-- Scraping tools for Google Flights
+- Detailed scraping and querying tools for Google Flights
+- Ability to store data locally or to SQL tables
 - Base analytical tools/methods for price forecasting/summary
 
 The features in development are:
 
 - Models to demonstrate ML techniques on forecasting
+- Querying of advanced features
 - API for access to previously collected data
 
 ## Table of Contents
 - [Overview](#Overview)
 - [Usage](#usage)
 - [Updates & New Features](#updates-&-new-features)
 - [Real Usage](#real-usage) 😄
@@ -71,27 +74,54 @@
 	import sys
 	sys.path.append('src/google_flight_analysis')
 	from scrape import *
 
 
 Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
-	# Try to keep the dates in format YYYY-mm-dd
-	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-10') # obtain our scrape object
-	dataframe = result.data # outputs a Pandas DF with flight prices/info
-	origin = result.origin # 'JFK'
-	dest = result.dest # 'IST'
-	date_leave = result.date_leave # '2023-05-20'
-	date_return = result.date_return # '2023-06-10'
+	# Keep the dates in format YYYY-mm-dd
+	result = Scrape('JFK', 'IST', '2023-07-20', '2023-08-20') # obtain our scrape object, represents out query
+	result.type # This is in a round-trip format
+	result.origin # ['JFK', 'IST']
+	result.dest # ['IST', 'JFK']
+	result.dates # ['2023-07-20', '2023-08-20']
+	print(result) # get unqueried str representation
+
+A `Scrape` object represents a Google Flights query to be run. It maintains flights as a sequence of one or more one-way flights which have a origin, destination, and flight date. The above object for a round-trip flight from JFK to IST is a sequence of JFK --> IST, then IST --> JFK. We can obtain the data as follows:
+
+	ScrapeObjects(result) # runs selenium through ChromeDriver, modifies results in-place
+	result.data # returns pandas DF
+	print(result) # get queried representation of result
 
-You can also scrape for one-way trips now:
+You can also scrape for one-way trips:
 
 	results = Scrape('JFK', 'IST', '2023-08-20')
-	result.data.head() #see data
+	ScrapeObjects(result)
+	result.data #see data
 
+You can also scrape chain-trips, which are defined as a sequence of one-way flights that have no direct relation to each other, other than being in chronological order. 
+
+	# chain-trip format: origin, dest, date, origin, dest, date, ...
+	result = Scrape('JFK', 'IST', '2023-08-20', 'RDU', 'LGA', '2023-12-25', 'EWR', 'SFO', '2024-01-20')
+	result.type # chain-trip
+	ScrapeObjects(result)
+	result.data # see data
+
+You can also scrape perfect-chains, which are defined as a sequence of one-way flights such that the destination of the previous flight is the origin of the next and the origin of the chain is the final destination of the chain (a cycle).
+
+	# perfect-chain format: origin, date, origin, date, ..., first_origin
+	result = Scrape("JFK", "2023-09-20", "IST", "2023-09-25", "CDG", "2023-10-10", "LHR", "2023-11-01", "JFK")
+	result.type # perfect-chain
+	ScrapeObjects(result)
+	result.data # see data
+
+You can read more about the different type of trips in the documentation. Scrape objects can be added to one another to create larger queries. This is under the conditions:
+
+1. The objects being added are the same type of trip (one-way, round-trip, etc)
+2. The objects being added are either both unqueried or both queried
 
 ## Updates & New Features
 
 Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
 
 
 <!--
```

### Comparing `google-flight-analysis-1.1.0/src/google_flight_analysis.egg-info/SOURCES.txt` & `google-flight-analysis-1.2.0/src/google_flight_analysis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+pytest.ini
 requirements.txt
 setup.cfg
 .circleci/config.yml
+.github/workflows/publish-test.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 .github/workflows/scripts/release.py
 src/google_flight_analysis/__init__.py
 src/google_flight_analysis/analysis.py
 src/google_flight_analysis/cache.py
 src/google_flight_analysis/flight.py
```

### Comparing `google-flight-analysis-1.1.0/tests/test_data/CDG-IST.csv` & `google-flight-analysis-1.2.0/tests/test_data/CDG-IST.csv`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.1.0/tests/test_data/LGA-RDU.csv` & `google-flight-analysis-1.2.0/tests/test_data/LGA-RDU.csv`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.1.0/tests/test_data/test1.csv` & `google-flight-analysis-1.2.0/tests/test_data/test1.csv`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-1.1.0/tests/test_data/test2.csv` & `google-flight-analysis-1.2.0/tests/test_data/test2.csv`

 * *Files identical despite different names*

