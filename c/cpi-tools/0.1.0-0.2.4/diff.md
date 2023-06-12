# Comparing `tmp/cpi_tools-0.1.0.tar.gz` & `tmp/cpi_tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpi_tools-0.1.0.tar", last modified: Thu May 18 16:49:26 2023, max compression
+gzip compressed data, was "/Users/nikitamarini/Desktop/CPI/cpi_tools/dist/.tmp-piqjlkg3/cpi_tools-0.2.4.tar", last modified: Fri Jun  9 13:34:33 2023, max compression
```

## Comparing `cpi_tools-0.1.0.tar` & `cpi_tools-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 16:49:26.869068 cpi_tools-0.1.0/
--rw-rw-rw-   0        0        0     1074 2023-01-26 16:53:27.000000 cpi_tools-0.1.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-01-27 16:40:16.000000 cpi_tools-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      941 2023-05-18 16:49:26.870068 cpi_tools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-01-27 16:58:15.000000 cpi_tools-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 16:49:26.859066 cpi_tools-0.1.0/cpi_tools/
--rw-rw-rw-   0        0        0        0 2023-01-26 16:53:26.000000 cpi_tools-0.1.0/cpi_tools/__init__.py
--rw-rw-rw-   0        0        0     2375 2023-01-27 16:56:14.000000 cpi_tools-0.1.0/cpi_tools/aws_tools.py
--rw-rw-rw-   0        0        0     4633 2023-03-11 17:03:11.000000 cpi_tools-0.1.0/cpi_tools/cpi_validation.py
--rw-rw-rw-   0        0        0    14930 2023-05-18 16:41:26.000000 cpi_tools-0.1.0/cpi_tools/tracking_processing_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:49:26.868070 cpi_tools-0.1.0/cpi_tools.egg-info/
--rw-rw-rw-   0        0        0      941 2023-05-18 16:49:26.000000 cpi_tools-0.1.0/cpi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-05-18 16:49:26.000000 cpi_tools-0.1.0/cpi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 16:49:26.000000 cpi_tools-0.1.0/cpi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 16:49:26.000000 cpi_tools-0.1.0/cpi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-01-27 16:46:45.000000 cpi_tools-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      566 2023-05-18 16:49:26.871068 cpi_tools-0.1.0/setup.cfg
+drwxr-xr-x   0 nikitamarini   (501) staff       (20)        0 2023-06-09 13:34:33.297533 cpi_tools-0.2.4/
+-rw-r--r--   0 nikitamarini   (501) staff       (20)     1074 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/LICENSE
+-rw-r--r--   0 nikitamarini   (501) staff       (20)        0 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/MANIFEST.in
+-rw-r--r--   0 nikitamarini   (501) staff       (20)      911 2023-06-09 13:34:33.297597 cpi_tools-0.2.4/PKG-INFO
+-rw-r--r--   0 nikitamarini   (501) staff       (20)      442 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/README.md
+drwxr-xr-x   0 nikitamarini   (501) staff       (20)        0 2023-06-09 13:34:33.296774 cpi_tools-0.2.4/cpi_tools/
+-rw-r--r--   0 nikitamarini   (501) staff       (20)        0 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/cpi_tools/__init__.py
+-rw-r--r--   0 nikitamarini   (501) staff       (20)     2375 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/cpi_tools/aws_tools.py
+-rw-r--r--   0 nikitamarini   (501) staff       (20)     4535 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/cpi_tools/cpi_validation.py
+-rw-r--r--   0 nikitamarini   (501) staff       (20)     7278 2023-06-09 13:33:43.000000 cpi_tools-0.2.4/cpi_tools/fuzzy_matching_cpi.py
+-rw-r--r--   0 nikitamarini   (501) staff       (20)    14573 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/cpi_tools/tracking_processing_tools.py
+drwxr-xr-x   0 nikitamarini   (501) staff       (20)        0 2023-06-09 13:34:33.297419 cpi_tools-0.2.4/cpi_tools.egg-info/
+-rw-r--r--   0 nikitamarini   (501) staff       (20)      911 2023-06-09 13:34:33.000000 cpi_tools-0.2.4/cpi_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nikitamarini   (501) staff       (20)      330 2023-06-09 13:34:33.000000 cpi_tools-0.2.4/cpi_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitamarini   (501) staff       (20)        1 2023-06-09 13:34:33.000000 cpi_tools-0.2.4/cpi_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitamarini   (501) staff       (20)       10 2023-06-09 13:34:33.000000 cpi_tools-0.2.4/cpi_tools.egg-info/top_level.txt
+-rw-r--r--   0 nikitamarini   (501) staff       (20)      103 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/pyproject.toml
+-rw-r--r--   0 nikitamarini   (501) staff       (20)      558 2023-06-09 13:34:33.297921 cpi_tools-0.2.4/setup.cfg
```

### Comparing `cpi_tools-0.1.0/LICENSE` & `cpi_tools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.1.0/PKG-INFO` & `cpi_tools-0.2.4/cpi_tools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: cpi_tools
-Version: 0.1.0
-Summary: Repository of functions used across CPI
-Home-page: https://github.com/climatepolicydata/cpi_tools
-Author: Jake Connolly
-Author-email: datascience@cpiglobal.org
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CPI Data Tools
-
-A repository of commonly used tools across CPI
-
-## Instructions
-
-1. Install:
-
-```
-pip install cpi_tools
-```
-
-AWS Tools
-
-```python
-from cpi_tools import aws_tools
-
-#S3 Bucket
-bucket = 'YOUR_BUCKET'
-#Path within S3
-path = 'PATH_IN_BUCKET'
-#S3 File name 
-file_name = 'FILE_NAME'
-
-#Read file from S3
-df = aws_tools.read_from_s3(bucket, path, file_name)
-
-#Write file to S3
-aws_tools.write_to_s3(df, bucket, path, file_name)
-```
-
+Metadata-Version: 2.1
+Name: cpi-tools
+Version: 0.2.4
+Summary: Repository of functions used across CPI
+Home-page: https://github.com/climatepolicydata/cpi_tools
+Author: Jake Connolly, Nikita Marini
+Author-email: datascience@cpiglobal.org
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CPI Data Tools
+
+A repository of commonly used tools across CPI
+
+## Instructions
+
+1. Install:
+
+```
+pip install cpi_tools
+```
+
+AWS Tools
+
+```python
+from cpi_tools import aws_tools
+
+#S3 Bucket
+bucket = 'YOUR_BUCKET'
+#Path within S3
+path = 'PATH_IN_BUCKET'
+#S3 File name 
+file_name = 'FILE_NAME'
+
+#Read file from S3
+df = aws_tools.read_from_s3(bucket, path, file_name)
+
+#Write file to S3
+aws_tools.write_to_s3(df, bucket, path, file_name)
+```
+
```

### Comparing `cpi_tools-0.1.0/cpi_tools/aws_tools.py` & `cpi_tools-0.2.4/cpi_tools/aws_tools.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.1.0/cpi_tools/cpi_validation.py` & `cpi_tools-0.2.4/cpi_tools/cpi_validation.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import pandas as pd
-import pandera as pa
-from cpi_tools import aws_tools
-import boto3
-import s3fs
-
-def get_valid_ref_values(ref_file, ref_column) -> list[str]:
-    """ Retrieve valid GLCF column values from ref table"""
-    ref_bucket = 'cpi-reference-data'
-    ref_file_path = 'cpi/processed'
-    ref_table = aws_tools.read_from_s3(ref_bucket, ref_file_path, ref_file)
-    return list(ref_table[ref_column].unique())
-
-
-def validate_glcf_data(df: pd.DataFrame, min_date: int = 2019, max_date:int = 2020) -> None:
-
-    '''
-    Input:
-
-    df: pandas DataFrame containing GLCF data to be validated
-    min_date (optional): integer representing the minimum year for valid data (default value is 2019)
-    max_date (optional): integer representing the maximum year for valid data (default value is 2020)
-
-    Returns: None
-
-    This function validates a pandas DataFrame containing GLCF data, ensuring that it conforms to a specified schema. 
-    The schema includes checks for valid values in various columns, such as sector, sub_sector, country, region, and institution type. 
-    The function uses the validate method from the pandas_schema library to validate the DataFrame against the schema, 
-    and raises an exception if the validation fails. If the validation is successful, the function prints a message 
-    indicating that the DataFrame is GLCF compatible.
-        
-    '''
-
-    # Get or define valid column values
-    valid_sector_values = get_valid_ref_values('ref_project_type', 'sector')
-    valid_sub_sector_values = get_valid_ref_values('ref_project_type', 'sub_sector')
-    valid_solution_values = get_valid_ref_values('ref_project_type', 'solution')
-    valid_country_values = get_valid_ref_values('ref_geog_list_cpi', 'country_cpi')
-    valid_region_values = get_valid_ref_values('ref_geog_list_cpi', 'region_cpi')
-    
-    valid_institution_type_layer2_values =  ["Bilateral DFI", "Commercial FI", 'Corporation', 'Export Credit Agency (ECA)',
-                            'Funds','Government', 'Household/Individual', 'Institutional Investors', 
-                            'Multilateral Climate Funds','Multilateral DFI','National DFI', 'Public Fund',
-                            'SOE', 'State-owned FI', 'Unknown']
-    
-    valid_institution_type_layer1_values = ['Public', 'Private']
-
-    valid_domestic_international_values = ['Domestic', 'International']
-
-    valid_use_values = ['Mitigation', 'Adaptation', 'Multiple Objectives']
-
-
-    # Define GLCF Schema
-    schema = pa.DataFrameSchema({
-        "id_glcf": pa.Column(str),
-        "data_source_id": pa.Column(str, required=False),
-        "data_source": pa.Column(str),
-        "year": pa.Column(int, checks=pa.Check.in_range(min_date, max_date)),
-        "project_name": pa.Column(str),
-        "project_description": pa.Column(str, nullable=True),
-        "country_origin_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
-        "region_origin_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
-        "oecd_origin_cpi": pa.Column(str),
-        "country_destination_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
-        "region_destination_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
-        "oecd_destination_cpi": pa.Column(str),
-        "institution_cpi": pa.Column(str),
-        "institution_type_layer1": pa.Column(str, pa.Check.isin(valid_institution_type_layer1_values)),
-        "institution_type_layer2": pa.Column(str, pa.Check.isin(valid_institution_type_layer2_values)),
-        "recipient_type_layer1": pa.Column(str),
-        "domestic_international": pa.Column(str, pa.Check.isin(valid_domestic_international_values)),
-        "value_USDm": pa.Column(float, pa.Check.ge(0)), #Greater than or equal to 0
-        "instrument_cpi": pa.Column(str),
-        "sector_original": pa.Column(str),
-        "sector_key_cpi": pa.Column(str),
-        "sector_cpi": pa.Column(str, checks=pa.Check.isin(valid_sector_values)),
-        "sub_sector_cpi": pa.Column(str, pa.Check.isin(valid_sub_sector_values)),
-        "solution_cpi": pa.Column(str, pa.Check.isin(valid_solution_values)),
-        "use_cpi": pa.Column(str, pa.Check.isin(valid_use_values)),
-        "gender_cpi": pa.Column(str),
-        "exclude_include": pa.Column(str)
-    })
-
-    # Attempt Validation
-    try:
-        schema.validate(df, lazy=True)
-        print('Dataframe GLCF Compatible')
-    except pa.errors.SchemaErrors as e:
-        #Display Errors upon validation failure
-        display(e.failure_cases)
-
-
-
-    
-    
-    
-    
-    
+import pandas as pd
+import pandera as pa
+from cpi_tools import aws_tools
+import boto3
+import s3fs
+
+def get_valid_ref_values(ref_file, ref_column) -> list[str]:
+    """ Retrieve valid GLCF column values from ref table"""
+    ref_bucket = 'cpi-reference-data'
+    ref_file_path = 'cpi/processed'
+    ref_table = aws_tools.read_from_s3(ref_bucket, ref_file_path, ref_file)
+    return list(ref_table[ref_column].unique())
+
+
+def validate_glcf_data(df: pd.DataFrame, min_date: int = 2019, max_date:int = 2020) -> None:
+
+    '''
+    Input:
+
+    df: pandas DataFrame containing GLCF data to be validated
+    min_date (optional): integer representing the minimum year for valid data (default value is 2019)
+    max_date (optional): integer representing the maximum year for valid data (default value is 2020)
+
+    Returns: None
+
+    This function validates a pandas DataFrame containing GLCF data, ensuring that it conforms to a specified schema. 
+    The schema includes checks for valid values in various columns, such as sector, sub_sector, country, region, and institution type. 
+    The function uses the validate method from the pandas_schema library to validate the DataFrame against the schema, 
+    and raises an exception if the validation fails. If the validation is successful, the function prints a message 
+    indicating that the DataFrame is GLCF compatible.
+        
+    '''
+
+    # Get or define valid column values
+    valid_sector_values = get_valid_ref_values('ref_project_type', 'sector')
+    valid_sub_sector_values = get_valid_ref_values('ref_project_type', 'sub_sector')
+    valid_solution_values = get_valid_ref_values('ref_project_type', 'solution')
+    valid_country_values = get_valid_ref_values('ref_geog_list_cpi', 'country_cpi')
+    valid_region_values = get_valid_ref_values('ref_geog_list_cpi', 'region_cpi')
+    
+    valid_institution_type_layer2_values =  ["Bilateral DFI", "Commercial FI", 'Corporation', 'Export Credit Agency (ECA)',
+                            'Funds','Government', 'Household/Individual', 'Institutional Investors', 
+                            'Multilateral Climate Funds','Multilateral DFI','National DFI', 'Public Fund',
+                            'SOE', 'State-owned FI', 'Unknown']
+    
+    valid_institution_type_layer1_values = ['Public', 'Private']
+
+    valid_domestic_international_values = ['Domestic', 'International']
+
+    valid_use_values = ['Mitigation', 'Adaptation', 'Multiple Objectives']
+
+
+    # Define GLCF Schema
+    schema = pa.DataFrameSchema({
+        "id_glcf": pa.Column(str),
+        "data_source_id": pa.Column(str, required=False),
+        "data_source": pa.Column(str),
+        "year": pa.Column(int, checks=pa.Check.in_range(min_date, max_date)),
+        "project_name": pa.Column(str),
+        "project_description": pa.Column(str, nullable=True),
+        "country_origin_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
+        "region_origin_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
+        "oecd_origin_cpi": pa.Column(str),
+        "country_destination_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
+        "region_destination_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
+        "oecd_destination_cpi": pa.Column(str),
+        "institution_cpi": pa.Column(str),
+        "institution_type_layer1": pa.Column(str, pa.Check.isin(valid_institution_type_layer1_values)),
+        "institution_type_layer2": pa.Column(str, pa.Check.isin(valid_institution_type_layer2_values)),
+        "recipient_type_layer1": pa.Column(str),
+        "domestic_international": pa.Column(str, pa.Check.isin(valid_domestic_international_values)),
+        "value_USDm": pa.Column(float, pa.Check.ge(0)), #Greater than or equal to 0
+        "instrument_cpi": pa.Column(str),
+        "sector_original": pa.Column(str),
+        "sector_key_cpi": pa.Column(str),
+        "sector_cpi": pa.Column(str, checks=pa.Check.isin(valid_sector_values)),
+        "sub_sector_cpi": pa.Column(str, pa.Check.isin(valid_sub_sector_values)),
+        "solution_cpi": pa.Column(str, pa.Check.isin(valid_solution_values)),
+        "use_cpi": pa.Column(str, pa.Check.isin(valid_use_values)),
+        "gender_cpi": pa.Column(str),
+        "exclude_include": pa.Column(str)
+    })
+
+    # Attempt Validation
+    try:
+        schema.validate(df, lazy=True)
+        print('Dataframe GLCF Compatible')
+    except pa.errors.SchemaErrors as e:
+        #Display Errors upon validation failure
+        display(e.failure_cases)
+
+
+
+    
+    
+    
+    
+
```

### Comparing `cpi_tools-0.1.0/cpi_tools/tracking_processing_tools.py` & `cpi_tools-0.2.4/cpi_tools/tracking_processing_tools.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,357 +1,357 @@
-import dropbox
-from dropbox.exceptions import AuthError
-from dropbox import DropboxOAuth2FlowNoRedirect
-import os
-import pandas as pd
-import numpy as np
-import io
-import unicodedata
-from datetime import date
-import uuid
-from dotenv import load_dotenv, find_dotenv
-import s3fs
-import boto3
-load_dotenv(find_dotenv())
-from cpi_tools import aws_tools
-
-S3_REFERENCE_BUCKET = 'cpi-reference-data'
-
-"""
-######################################################################################################
-######################## Dropbox and reference table processing functions ############################
-######################################################################################################
-
-"""
-
-
-def dropbox_authorisation(app_key:str, secret_key:str):
-    """
-    This function initiates an authorization process for a Dropbox App. 
-
-    Parameters:
-    app_key (str): The app key for your Dropbox app. You get this when you create an app on the Dropbox developers' site.
-    secret_key (str): The secret key for your Dropbox app. This is also provided when you create an app.
-
-    Returns:
-    oauth_result: A DropboxOAuth2FlowNoRedirect result object which contains access token and other information.
-    """
-
-    # Creating an instance of DropboxOAuth2FlowNoRedirect using app_key and secret_key.
-    # This class performs the second half of the OAuth2 'code' flow, where a code is exchanged for a token.
-    auth_flow = DropboxOAuth2FlowNoRedirect(app_key, secret_key)
-
-    # Starting the OAuth2 flow and getting the authorization URL.
-    authorize_url = auth_flow.start()
-
-    # Printing instructions for the user.
-    print ("1. Go to: " + authorize_url)
-    print ("2. Click 'Allow' (you might have to log in first).")
-    print ("3. Copy the authorization code.")
-
-    # Taking the authorization code input from the user.
-    auth_code = input("Enter the authorization code here: ").strip()
-
-    # Trying to finish the OAuth2 flow using the authorization code and obtaining the result.
-    try:
-        oauth_result = auth_flow.finish(auth_code)
-    except Exception as e:
-        print("Error: %s" % (e,))
-
-    # Return the result which can be used for making Dropbox API calls.
-    return oauth_result
-
-
-
-def export_dropbox_file_to_s3(dropbox_file_path:str, s3_bucket:str, s3_path:str, s3_file_name:str):
-    """
-    This function exports a file from Dropbox to an Amazon S3 bucket.
-
-    Parameters:
-    dropbox_file_path (str): The path of the file in Dropbox.
-    s3_bucket (str): The name of the S3 bucket to which the file is to be uploaded.
-    s3_path (str): The path in the S3 bucket where the file should be placed.
-    s3_file_name (str): The name with which the file should be stored in the S3 bucket.
-
-    Returns:
-    None
-    """
-    
-    # Attempt to load environment variables for Dropbox app key and secret key
-    try:
-        app_key = os.getenv('DROPBOX_APP_KEY')
-        secret_key = os.getenv('DROPBOX_SECRET_KEY')
-    except Exception as e:
-        print('Error Loading Dropbox app and secret key. Ensure variables are in your .env file: ' + str(e))
-
-    # Authorize Dropbox API usage with the app key and secret key
-    oauth = dropbox_authorisation(app_key=app_key, secret_key=secret_key)
-    
-    # Attempt to download the file from Dropbox and upload to S3
-    try:
-        # Set up Dropbox client with OAuth credentials
-        with dropbox.Dropbox(oauth2_access_token=oauth.access_token,
-                             oauth2_access_token_expiration=oauth.expires_at,
-                             oauth2_refresh_token=oauth.refresh_token,
-                             app_key=app_key,
-                             app_secret=secret_key) as dbx:
-
-            print("Successfully set up client!")
-
-            # Download the file from Dropbox
-            metadata, result = dbx.files_download(path=dropbox_file_path)
-
-            try: 
-                # Set up S3 client
-                s3 = boto3.resource('s3')
-                # Upload the file to S3
-                s3.Bucket(s3_bucket).put_object(Key=f'{s3_path}/{s3_file_name}', Body=result.content)
-            except Exception as e:
-                print('Error uploading dropbox data to S3: ' + str(e))
-
-    except Exception as e:
-        print('Error downloading file from Dropbox: ' + str(e))
-
-    return None
-
-
-def process_reference_data(base_data, file_name=None, sql_field_name=None, col_name_row=0, start_row=3, project_type=False): 
-    '''
-    This function takes an unprocessed reference dataframe taken from the master reference table excel and converts it
-    into a format useable within processing code
-    
-    If a filename is provided, it then writes this processed data to an s3 bucket 
-    
-    Parameters:
-    base_data: Pandas Dataframe
-    file_name: String
-    sql_field_name: String - If the reference table has a SQL Field name column, this is dropped
-    col_name_row: Int - selects the row that is used as the column names for the processed data
-    start_row: Int - Selects the row to start from, drops the rows prior to this one
-    project_type: Boolean - If project_type reference data, apply additional processing steps
-    
-    Returns
-    df: Pandas Dataframe - processed reference data
-    '''
-    
-    df = base_data.copy()
-
-    #Set the column names to the correct rows
-    df.columns = df.iloc[col_name_row]
-    
-    #If the ref table has a sql field, drop it
-    if sql_field_name:
-
-        df.drop(columns = sql_field_name, inplace=True)
-    
-    #Select the row to start from
-    df = df.iloc[start_row:]
-    
-    #Drop columns called nan
-    df = df.loc[:, df.columns.notna()]
-    
-    #If ref_project_type reference data, create a use column
-    if project_type:
-            df['use'] = df.apply(lambda x: generate_project_type_use(x['MI'], x['AD']), axis=1)
-        
-    
-    #Drop rows where all values are nan
-    df.dropna(axis = 0, how = 'all', inplace = True)
-
-    #Remove whitespace from strings and column names
-    df.rename(columns=lambda x: x.strip(), inplace=True)
-    df = df.applymap(lambda x: x.strip() if isinstance(x, str) else x)
-
-    #Enforce unicode conversion
-    df = df.applymap(lambda x: unicodedata.normalize("NFKD",x) if isinstance(x, str) else x)
-    
-    #Write to S3 if filename is provided
-    if file_name:
-            
-        aws_tools.write_to_s3(df, S3_REFERENCE_BUCKET, 'cpi/processed', file_name)
-        
-def generate_project_type_use(mi, ad):
-    '''
-    This function generates a Use column in the project type reference data using the MI and AD columns
-    
-    mi: Boolean Column
-    ad: Boolean Column
-    
-    Returns
-    use: String Column
-    
-    '''
-
-    if ((mi == 1) & (ad == 1)):
-        use = 'Multiple Objectives'
-    elif mi == 1:
-        use = 'Mitigation'
-    elif ad == 1:
-        use = 'Adaptation'
-    else:
-        use = np.nan
-
-    return use
-
-def extract_reference_sheets():
-    """
-    This function extracts multiple reference sheets from an Excel file stored in an Amazon S3 bucket.
-    It then processes each sheet using the 'process_reference_data' function.
-
-    Parameters: None
-
-    Returns: None
-    """
-    # Define the path to the file in the S3 bucket
-    s3_file_path = 'cpi/raw'
-    # Define the name of the file
-    file_name = 'master_ref.xlsm'
-    
-    # For each sheet in the Excel file, read the data into a pandas DataFrame
-    # and then process that data using the 'process_reference_data' function.
-    # The arguments passed to 'process_reference_data' vary depending on the specific sheet being processed.
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='coeff'),
-                           'ref_coef', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='double_counting'),
-                           'ref_double_counting', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='fx'),
-                           'ref_fx', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='gearing'),
-                           'ref_gearing')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='gender'),
-                           'ref_gender', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='geog_list_all'),
-                           'ref_geog_list_all', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='geog_list_cpi'),
-                           'ref_geog_list_cpi', 'SQL Field Name', 1,4)
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='institution_list_all'),
-                           'ref_institution_list_all', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='institution_list_cpi'),
-                           'ref_institution_list_cpi','SQL Field Name', start_row=4)
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='instr'),
-                           'ref_instr', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='multiplier'),
-                           'ref_multiplier')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='recipient'),
-                           'ref_recipient')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='project_type'),
-                           'ref_project_type', 'SQL Field Name', project_type=True)
-        
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='ownership'),
-                           'ref_ownership')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='sector'),
-                           'ref_sector', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='soe'),
-                           'ref_soe', 'SQL Field Name')
-
-    return None
-
-
-def update_ref_tables():
-    """
-    This function updates reference tables by reading a master reference table from Dropbox,
-    exporting it to an Amazon S3 bucket, and then extracting reference data from the table.
-
-    Parameters: None
-
-    Returns: None
-    """
-
-    # Output status update
-    print('Reading Master Reference Table...')
-
-    # Define the path to the file in Dropbox
-    reference_metadata_dropbox_path = '/CF-Program/1.Workstreams/Tracking/GLCF/GLCF MASTER/3. Reference Tables Excel/Reference Tables_v1_MASTER_2022.xlsm'
-    
-    # Export the file from Dropbox to an S3 bucket
-    export_dropbox_file_to_s3(reference_metadata_dropbox_path, s3_bucket='cpi-reference-data',
-                              s3_path='cpi/raw', s3_file_name='master_ref.xlsm')
-    
-    # Output status update
-    print('Extracting reference data')
-
-    # Extract reference data from the master reference table
-    extract_reference_sheets()
-
-    return None
-
-
-
-def get_reference_tables(update=False):
-    """
-    This function retrieves various reference tables stored in an Amazon S3 bucket as pandas DataFrames.
-    If the 'update' parameter is set to True, it will first update the reference tables
-    by calling the 'update_ref_tables' function.
-
-    Parameters:
-    update (bool): If True, the reference tables are updated before being retrieved.
-
-    Returns:
-    tuple: A tuple of pandas DataFrames, each one representing a reference table.
-    """
-    
-    # If the 'update' parameter is set to True, update the reference tables
-    if update:
-        update_ref_tables()
-
-    # Define the path to the folder in the S3 bucket where the reference tables are stored
-    cpi_reference_folder = 'cpi/processed'
-
-    # Retrieve each reference table from the S3 bucket and read it into a pandas DataFrame.
-    # Note that each file is read with 'utf-8' encoding.
-    # Each DataFrame is stored in a separate variable.
-
-    # Data Source Geography Names
-    ref_geog_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_all.csv', encoding='utf-8')
-    
-    # Coefficient table
-    ref_coeff =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_coef.csv', encoding='utf-8')
-    
-    # Foreign exchange rates
-    ref_fx =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_fx.csv', encoding='utf-8')
-    
-    # Gender table
-    ref_gender =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_gender.csv', encoding='utf-8')
-    
-    # CPI Geography Names
-    ref_geog_list_cpi =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_cpi.csv', encoding='utf-8')
-    
-    # Data Source Institution names
-    ref_institution_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_all.csv', encoding='utf-8')
-    
-    # CPI Institution names
-    ref_institution_list_cpi = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_cpi.csv', encoding='utf-8')
-
-    # Ownership table
-    ref_ownership = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_ownership.csv', encoding='utf-8')
-    
-    # Project type table
-    ref_project_type = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_project_type.csv')
-    
-    # Sector table
-    ref_sector = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_sector.csv', encoding='utf-8')
-    
-    # Instrument table
-    ref_instr = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_instr.csv', encoding='utf-8')
-    
-    # Recipient table
-    ref_recipient = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_recipient.csv', encoding='utf-8')
-
-    # Return all the DataFrames as a tuple
-    return ref_geog_list_all, ref_coeff, ref_fx, ref_gender, ref_geog_list_all, ref_geog_list_cpi, ref_institution_list_all, \
-    ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_recipient
-
+import dropbox
+from dropbox.exceptions import AuthError
+from dropbox import DropboxOAuth2FlowNoRedirect
+import os
+import pandas as pd
+import numpy as np
+import io
+import unicodedata
+from datetime import date
+import uuid
+from dotenv import load_dotenv, find_dotenv
+import s3fs
+import boto3
+load_dotenv(find_dotenv())
+from cpi_tools import aws_tools
+
+S3_REFERENCE_BUCKET = 'cpi-reference-data'
+
+"""
+######################################################################################################
+######################## Dropbox and reference table processing functions ############################
+######################################################################################################
+
+"""
+
+
+def dropbox_authorisation(app_key:str, secret_key:str):
+    """
+    This function initiates an authorization process for a Dropbox App. 
+
+    Parameters:
+    app_key (str): The app key for your Dropbox app. You get this when you create an app on the Dropbox developers' site.
+    secret_key (str): The secret key for your Dropbox app. This is also provided when you create an app.
+
+    Returns:
+    oauth_result: A DropboxOAuth2FlowNoRedirect result object which contains access token and other information.
+    """
+
+    # Creating an instance of DropboxOAuth2FlowNoRedirect using app_key and secret_key.
+    # This class performs the second half of the OAuth2 'code' flow, where a code is exchanged for a token.
+    auth_flow = DropboxOAuth2FlowNoRedirect(app_key, secret_key)
+
+    # Starting the OAuth2 flow and getting the authorization URL.
+    authorize_url = auth_flow.start()
+
+    # Printing instructions for the user.
+    print ("1. Go to: " + authorize_url)
+    print ("2. Click 'Allow' (you might have to log in first).")
+    print ("3. Copy the authorization code.")
+
+    # Taking the authorization code input from the user.
+    auth_code = input("Enter the authorization code here: ").strip()
+
+    # Trying to finish the OAuth2 flow using the authorization code and obtaining the result.
+    try:
+        oauth_result = auth_flow.finish(auth_code)
+    except Exception as e:
+        print("Error: %s" % (e,))
+
+    # Return the result which can be used for making Dropbox API calls.
+    return oauth_result
+
+
+
+def export_dropbox_file_to_s3(dropbox_file_path:str, s3_bucket:str, s3_path:str, s3_file_name:str):
+    """
+    This function exports a file from Dropbox to an Amazon S3 bucket.
+
+    Parameters:
+    dropbox_file_path (str): The path of the file in Dropbox.
+    s3_bucket (str): The name of the S3 bucket to which the file is to be uploaded.
+    s3_path (str): The path in the S3 bucket where the file should be placed.
+    s3_file_name (str): The name with which the file should be stored in the S3 bucket.
+
+    Returns:
+    None
+    """
+    
+    # Attempt to load environment variables for Dropbox app key and secret key
+    try:
+        app_key = os.getenv('DROPBOX_APP_KEY')
+        secret_key = os.getenv('DROPBOX_SECRET_KEY')
+    except Exception as e:
+        print('Error Loading Dropbox app and secret key. Ensure variables are in your .env file: ' + str(e))
+
+    # Authorize Dropbox API usage with the app key and secret key
+    oauth = dropbox_authorisation(app_key=app_key, secret_key=secret_key)
+    
+    # Attempt to download the file from Dropbox and upload to S3
+    try:
+        # Set up Dropbox client with OAuth credentials
+        with dropbox.Dropbox(oauth2_access_token=oauth.access_token,
+                             oauth2_access_token_expiration=oauth.expires_at,
+                             oauth2_refresh_token=oauth.refresh_token,
+                             app_key=app_key,
+                             app_secret=secret_key) as dbx:
+
+            print("Successfully set up client!")
+
+            # Download the file from Dropbox
+            metadata, result = dbx.files_download(path=dropbox_file_path)
+
+            try: 
+                # Set up S3 client
+                s3 = boto3.resource('s3')
+                # Upload the file to S3
+                s3.Bucket(s3_bucket).put_object(Key=f'{s3_path}/{s3_file_name}', Body=result.content)
+            except Exception as e:
+                print('Error uploading dropbox data to S3: ' + str(e))
+
+    except Exception as e:
+        print('Error downloading file from Dropbox: ' + str(e))
+
+    return None
+
+
+def process_reference_data(base_data, file_name=None, sql_field_name=None, col_name_row=0, start_row=3, project_type=False): 
+    '''
+    This function takes an unprocessed reference dataframe taken from the master reference table excel and converts it
+    into a format useable within processing code
+    
+    If a filename is provided, it then writes this processed data to an s3 bucket 
+    
+    Parameters:
+    base_data: Pandas Dataframe
+    file_name: String
+    sql_field_name: String - If the reference table has a SQL Field name column, this is dropped
+    col_name_row: Int - selects the row that is used as the column names for the processed data
+    start_row: Int - Selects the row to start from, drops the rows prior to this one
+    project_type: Boolean - If project_type reference data, apply additional processing steps
+    
+    Returns
+    df: Pandas Dataframe - processed reference data
+    '''
+    
+    df = base_data.copy()
+
+    #Set the column names to the correct rows
+    df.columns = df.iloc[col_name_row]
+    
+    #If the ref table has a sql field, drop it
+    if sql_field_name:
+
+        df.drop(columns = sql_field_name, inplace=True)
+    
+    #Select the row to start from
+    df = df.iloc[start_row:]
+    
+    #Drop columns called nan
+    df = df.loc[:, df.columns.notna()]
+    
+    #If ref_project_type reference data, create a use column
+    if project_type:
+            df['use'] = df.apply(lambda x: generate_project_type_use(x['MI'], x['AD']), axis=1)
+        
+    
+    #Drop rows where all values are nan
+    df.dropna(axis = 0, how = 'all', inplace = True)
+
+    #Remove whitespace from strings and column names
+    df.rename(columns=lambda x: x.strip(), inplace=True)
+    df = df.applymap(lambda x: x.strip() if isinstance(x, str) else x)
+
+    #Enforce unicode conversion
+    df = df.applymap(lambda x: unicodedata.normalize("NFKD",x) if isinstance(x, str) else x)
+    
+    #Write to S3 if filename is provided
+    if file_name:
+            
+        aws_tools.write_to_s3(df, S3_REFERENCE_BUCKET, 'cpi/processed', file_name)
+        
+def generate_project_type_use(mi, ad):
+    '''
+    This function generates a Use column in the project type reference data using the MI and AD columns
+    
+    mi: Boolean Column
+    ad: Boolean Column
+    
+    Returns
+    use: String Column
+    
+    '''
+
+    if ((mi == 1) & (ad == 1)):
+        use = 'Multiple Objectives'
+    elif mi == 1:
+        use = 'Mitigation'
+    elif ad == 1:
+        use = 'Adaptation'
+    else:
+        use = np.nan
+
+    return use
+
+def extract_reference_sheets():
+    """
+    This function extracts multiple reference sheets from an Excel file stored in an Amazon S3 bucket.
+    It then processes each sheet using the 'process_reference_data' function.
+
+    Parameters: None
+
+    Returns: None
+    """
+    # Define the path to the file in the S3 bucket
+    s3_file_path = 'cpi/raw'
+    # Define the name of the file
+    file_name = 'master_ref.xlsm'
+    
+    # For each sheet in the Excel file, read the data into a pandas DataFrame
+    # and then process that data using the 'process_reference_data' function.
+    # The arguments passed to 'process_reference_data' vary depending on the specific sheet being processed.
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='coeff'),
+                           'ref_coef', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='double_counting'),
+                           'ref_double_counting', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='fx'),
+                           'ref_fx', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='gearing'),
+                           'ref_gearing')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='gender'),
+                           'ref_gender', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='geog_list_all'),
+                           'ref_geog_list_all', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='geog_list_cpi'),
+                           'ref_geog_list_cpi', 'SQL Field Name', 1,4)
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='institution_list_all'),
+                           'ref_institution_list_all', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='institution_list_cpi'),
+                           'ref_institution_list_cpi','SQL Field Name', start_row=4)
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='instr'),
+                           'ref_instr', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='multiplier'),
+                           'ref_multiplier')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='recipient'),
+                           'ref_recipient')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='project_type'),
+                           'ref_project_type', 'SQL Field Name', project_type=True)
+        
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='ownership'),
+                           'ref_ownership')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='sector'),
+                           'ref_sector', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='soe'),
+                           'ref_soe', 'SQL Field Name')
+
+    return None
+
+
+def update_ref_tables():
+    """
+    This function updates reference tables by reading a master reference table from Dropbox,
+    exporting it to an Amazon S3 bucket, and then extracting reference data from the table.
+
+    Parameters: None
+
+    Returns: None
+    """
+
+    # Output status update
+    print('Reading Master Reference Table...')
+
+    # Define the path to the file in Dropbox
+    reference_metadata_dropbox_path = '/CF-Program/1.Workstreams/Tracking/GLCF/GLCF MASTER/3. Reference Tables Excel/Reference Tables_v1_MASTER_2022.xlsm'
+    
+    # Export the file from Dropbox to an S3 bucket
+    export_dropbox_file_to_s3(reference_metadata_dropbox_path, s3_bucket='cpi-reference-data',
+                              s3_path='cpi/raw', s3_file_name='master_ref.xlsm')
+    
+    # Output status update
+    print('Extracting reference data')
+
+    # Extract reference data from the master reference table
+    extract_reference_sheets()
+
+    return None
+
+
+
+def get_reference_tables(update=False):
+    """
+    This function retrieves various reference tables stored in an Amazon S3 bucket as pandas DataFrames.
+    If the 'update' parameter is set to True, it will first update the reference tables
+    by calling the 'update_ref_tables' function.
+
+    Parameters:
+    update (bool): If True, the reference tables are updated before being retrieved.
+
+    Returns:
+    tuple: A tuple of pandas DataFrames, each one representing a reference table.
+    """
+    
+    # If the 'update' parameter is set to True, update the reference tables
+    if update:
+        update_ref_tables()
+
+    # Define the path to the folder in the S3 bucket where the reference tables are stored
+    cpi_reference_folder = 'cpi/processed'
+
+    # Retrieve each reference table from the S3 bucket and read it into a pandas DataFrame.
+    # Note that each file is read with 'utf-8' encoding.
+    # Each DataFrame is stored in a separate variable.
+
+    # Data Source Geography Names
+    ref_geog_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_all.csv', encoding='utf-8')
+    
+    # Coefficient table
+    ref_coeff =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_coef.csv', encoding='utf-8')
+    
+    # Foreign exchange rates
+    ref_fx =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_fx.csv', encoding='utf-8')
+    
+    # Gender table
+    ref_gender =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_gender.csv', encoding='utf-8')
+    
+    # CPI Geography Names
+    ref_geog_list_cpi =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_cpi.csv', encoding='utf-8')
+    
+    # Data Source Institution names
+    ref_institution_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_all.csv', encoding='utf-8')
+    
+    # CPI Institution names
+    ref_institution_list_cpi = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_cpi.csv', encoding='utf-8')
+
+    # Ownership table
+    ref_ownership = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_ownership.csv', encoding='utf-8')
+    
+    # Project type table
+    ref_project_type = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_project_type.csv')
+    
+    # Sector table
+    ref_sector = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_sector.csv', encoding='utf-8')
+    
+    # Instrument table
+    ref_instr = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_instr.csv', encoding='utf-8')
+    
+    # Recipient table
+    ref_recipient = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_recipient.csv', encoding='utf-8')
+
+    # Return all the DataFrames as a tuple
+    return ref_geog_list_all, ref_coeff, ref_fx, ref_gender, ref_geog_list_all, ref_geog_list_cpi, ref_institution_list_all, \
+    ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_recipient
+
```

### Comparing `cpi_tools-0.1.0/cpi_tools.egg-info/PKG-INFO` & `cpi_tools-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: cpi-tools
-Version: 0.1.0
-Summary: Repository of functions used across CPI
-Home-page: https://github.com/climatepolicydata/cpi_tools
-Author: Jake Connolly
-Author-email: datascience@cpiglobal.org
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CPI Data Tools
-
-A repository of commonly used tools across CPI
-
-## Instructions
-
-1. Install:
-
-```
-pip install cpi_tools
-```
-
-AWS Tools
-
-```python
-from cpi_tools import aws_tools
-
-#S3 Bucket
-bucket = 'YOUR_BUCKET'
-#Path within S3
-path = 'PATH_IN_BUCKET'
-#S3 File name 
-file_name = 'FILE_NAME'
-
-#Read file from S3
-df = aws_tools.read_from_s3(bucket, path, file_name)
-
-#Write file to S3
-aws_tools.write_to_s3(df, bucket, path, file_name)
-```
-
+Metadata-Version: 2.1
+Name: cpi_tools
+Version: 0.2.4
+Summary: Repository of functions used across CPI
+Home-page: https://github.com/climatepolicydata/cpi_tools
+Author: Jake Connolly, Nikita Marini
+Author-email: datascience@cpiglobal.org
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CPI Data Tools
+
+A repository of commonly used tools across CPI
+
+## Instructions
+
+1. Install:
+
+```
+pip install cpi_tools
+```
+
+AWS Tools
+
+```python
+from cpi_tools import aws_tools
+
+#S3 Bucket
+bucket = 'YOUR_BUCKET'
+#Path within S3
+path = 'PATH_IN_BUCKET'
+#S3 File name 
+file_name = 'FILE_NAME'
+
+#Read file from S3
+df = aws_tools.read_from_s3(bucket, path, file_name)
+
+#Write file to S3
+aws_tools.write_to_s3(df, bucket, path, file_name)
+```
+
```

