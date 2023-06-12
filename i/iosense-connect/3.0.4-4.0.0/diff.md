# Comparing `tmp/iosense_connect-3.0.4.tar.gz` & `tmp/iosense_connect-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-3.0.4.tar", last modified: Mon Jun 12 05:32:47 2023, max compression
+gzip compressed data, was "dist\iosense_connect-4.0.0.tar", last modified: Mon Jun 12 13:46:17 2023, max compression
```

## Comparing `iosense_connect-3.0.4.tar` & `iosense_connect-4.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 05:32:47.416088 iosense_connect-3.0.4/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-3.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-06-12 05:32:47.412998 iosense_connect-3.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-3.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 05:32:47.376254 iosense_connect-3.0.4/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-3.0.4/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    24109 2023-06-12 05:32:32.000000 iosense_connect-3.0.4/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:32:47.409995 iosense_connect-3.0.4/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-06-12 05:32:47.000000 iosense_connect-3.0.4/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-12 05:32:47.000000 iosense_connect-3.0.4/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 05:32:47.000000 iosense_connect-3.0.4/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-12 05:32:47.000000 iosense_connect-3.0.4/iosense_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 05:32:47.000000 iosense_connect-3.0.4/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 05:32:47.416088 iosense_connect-3.0.4/setup.cfg
--rw-rw-rw-   0        0        0      794 2023-06-12 05:32:32.000000 iosense_connect-3.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:46:17.205919 iosense_connect-4.0.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-12 13:46:17.205919 iosense_connect-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 13:46:17.096781 iosense_connect-4.0.0/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.0/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    25075 2023-06-12 13:46:12.000000 iosense_connect-4.0.0/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:46:17.205919 iosense_connect-4.0.0/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 13:46:16.000000 iosense_connect-4.0.0/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 13:46:17.205919 iosense_connect-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      848 2023-06-12 13:45:02.000000 iosense_connect-4.0.0/setup.py
```

### Comparing `iosense_connect-3.0.4/LICENSE.txt` & `iosense_connect-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-3.0.4/PKG-INFO` & `iosense_connect-4.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 3.0.4
+Version: 4.0.0
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-3.0.4/README.md` & `iosense_connect-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-3.0.4/iosense_connect/data_access.py` & `iosense_connect-4.0.0/iosense_connect/data_access.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import json
-import os
-import re
 import sys
-import time
-import numpy as np
-import pandas as pd
+import fsspec
 import requests
-import random
 import urllib3
-from azure.storage.blob import BlobServiceClient
+import numpy as np
+import pandas as pd
 from concurrent.futures import ThreadPoolExecutor
+from cryptography.fernet import Fernet
 from datetime import datetime, timezone
 from datetime import timedelta
 
 pd.options.mode.chained_assignment = None
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-
 class DataAccess:
-    def __init__(self, userid, url, connection_string, container_name):
+    def __init__(self, userid, url, key):
         self.userid = userid
         self.url = url
-        self.connection_string = connection_string
-        self.container_name = container_name
+        self.key = key
 
     def get_caliberation(self, device_id, metadata, df,onpremise=False):
         """
         :param metadata:
         :param df: Dataframe
         :param device_id: string
         :return: Calibrated dataframe
@@ -83,15 +78,14 @@
             if str(onpremise).lower() == 'true':
                 url = "http://" + self.url + "/api/metaData/device/" + device_id
             else:
                 url = "https://" + self.url + "/api/metaData/device/" + device_id
             header = {'userID': self.userid}
             payload = {}
             response = requests.request('GET', url, headers=header, data=payload, verify=False)
-
             if response.status_code != 200:
                 raw = json.loads(response.text)
                 raise ValueError(raw['error'])
             else:
                 raw_data = json.loads(response.text)['data']
                 return raw_data
 
@@ -191,14 +185,57 @@
                 df_raw = pd.DataFrame(raw_data)
                 return df_raw
 
         except Exception as e:
             print('Failed to fetch device Details')
             print(e)
 
+    def get_load_entities(self,mongoid=None,onpremise=False):
+        try:
+            if mongoid == None or len(mongoid) < 25 or type(mongoid) == "list" or type(mongoid) == "int":
+                raise Exception("Message: Please Enter Valid mongoid")
+            if str(onpremise).lower() == 'true':
+                url = "http://"+self.url+"/api/metaData/fetchLoadEntity/"+mongoid
+            else:
+                url = "https://"+self.url+"/api/metaData/fetchLoadEntity/"+mongoid
+            header = {'userID': self.userid}
+            payload = {}
+            response = requests.request('GET', url, headers=header, data=payload, verify=False)
+
+            if response.status_code != 200:
+                raw = json.loads(response.text)
+                raise ValueError(raw['error'])
+            else:
+                raw_data = json.loads(response.text)['data']
+                return raw_data
+        except Exception as e:
+            print('Failed to Fetch Load Entities \t',e)
+
+    def get_database_credentials(self,db):
+        try:
+            header = {"userID":self.userid}
+            payload = {}
+            url = "https://"+self.url+"/api/metaData/getCredentials/"+str(db)
+            response = requests.request('GET',url,headers=header,json=payload,verify=False)
+            if response.status_code != 200:
+                raw = json.loads(response.text)
+                raise ValueError(raw)
+            else:
+                credentials = json.loads(response.text)['data']
+                cipher = Fernet(self.key)
+                if type(credentials) == list:
+                    credentials[0] = cipher.decrypt(credentials[0].encode('utf-8')).decode()
+
+                    credentials[1] = cipher.decrypt(credentials[1].encode('utf-8')).decode()
+                else:
+                    credentials = cipher.decrypt(credentials.encode('utf-8')).decode()
+                return credentials
+        except Exception as e:
+            print(e)
+
     def get_dp(self, device_id, sensors=None, n=1, cal=True, end_time=datetime.now(),alias=True, IST=True,onpremise=False):
         """
 
         :param device_id: string
         :param sensors: IST of sensors
         :param n: number of data points (default: 1)
         :param cal: bool (default: True)
@@ -358,15 +395,15 @@
             if len(df.columns) == 2:
                 df['sensor'] = sensors[0]
             if str(alias).lower() == "true":
                 df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata,onpremise=onpremise)
             df = DataAccess.get_cleaned_table(self, df)
         return df
 
-    def data_query(self, device_id, sensors,start_time, end_time=str(datetime.now()), alias=True,cal=True, bands=None,onpremise=False,compute=None,api=False,IST=True):
+    def data_query(self, device_id, sensors,start_time, end_time=datetime.now(), db=None,alias=True,cal=True, bands=None,onpremise=False,compute=None,api=False,IST=True):
         """
 
         :param device_id: string
         :param start_time: yyyy-MM-dd HH:MM:SS
         :param end_time: yyyy-MM-dd HH:MM:SS
         :param cal: bool
         :param bands: None
@@ -374,158 +411,161 @@
         :return: df
 
         If requested data exists in feature store fetch data from the container.
         IF data is not available the data is fetched from influxdb
 
         """
         try:
-            if type(end_time) == "str":
+            if db == None:
+                raise Exception("Invalid DB")
+            def get_month_year(filename):
+                parts = filename.split('.')[0].split('-')
+                month = int(parts[0])
+                year = int(parts[1])
+                return datetime(year, month, 1)
+
+            def generate_month_year_dates(start_date, end_date):
                 try:
-                    end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
-                except Exception:
-                    if type(end_time) == str:
-                        end_time = str(end_time) + " 23:59:59"
+                    end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
+                except:
                     pass
-            unique_id = random.randint(10000, 100000000)
-            df = pd.DataFrame()
-            metadata = {}
-            folder_path = f"{device_id}/"
-            blob_svc = BlobServiceClient.from_connection_string(conn_str=self.connection_string)
-            container_client = blob_svc.get_container_client(self.container_name)
-            processed_blobs = [blob.name[len(folder_path):].lstrip("/").rsplit(".", 1)[0].split("-") for blob in
-                               container_client.list_blobs(name_starts_with=folder_path)]
-            sorted_blobs = sorted(processed_blobs, key=lambda x: (int(x[1]), int(x[0])))
-
-            date_month_list = []
-            for month, year in sorted_blobs:
-                val = f"{month}-{year}"
-                date_month_list.append(val)
-
-            def check_device(device_id):
-                flag = False
-                blob_list = container_client.list_blobs()
-                for blob in blob_list:
-                    split_text = blob.name.split('/')
-                    if device_id == split_text[0]:
-                        flag = True
-                return flag
-
-            def get_dates():
-                temp_list = []
-                match_start_str = re.search(r'\d{4}-\d{2}-\d{2}', start_time)
-                match_end_str = re.search(r'\d{4}-\d{2}-\d{2}', end_time)
-
-                start_t = (datetime.strptime(match_start_str.group(), '%Y-%m-%d').date())
-                end_t = (datetime.strptime(match_end_str.group(), '%Y-%m-%d').date())
-                curr_date = start_t
-                date_list = []
-                while curr_date <= end_t:
-                    date_list.append(curr_date)
-                    curr_date += timedelta(days=1)
-
-                for date_value in date_list:
-                    month_value = date_value.month
-                    year_value = date_value.year
-                    str_format = str(month_value) + '-' + str(year_value)
-                    temp_list.append(str_format)
-
-                def sort_dates(dates):
-                    def date_key(date_string):
-                        return datetime.strptime(date_string, '%m-%Y')
-                    return sorted(dates, key=date_key)
-
-                filtered_list = [*set(temp_list)]
-                date_range = sort_dates(filtered_list)
-                list_of_dates_in_azure = list(set(date_month_list).intersection(date_range))
-                return list_of_dates_in_azure
-
-            def read_one(blobfile):
-                blob = blob_svc.get_blob_client(self.container_name, device_id + '/' + blobfile + '.parquet')
-                blob_data = blob.download_blob()
-                with open(str(unique_id)+'_'+blobfile+ '.parquet', "wb") as my_blob:
-                    blob_data.readinto(my_blob)
-                df = pd.read_parquet(str(unique_id)+'_'+blobfile+ '.parquet')
-                os.remove(str(unique_id)+'_'+blobfile+ '.parquet')
+                end_date = str(end_date)
+                if len(start_date.split()) == 1:
+                    start_date += " 00:00:00"
+                if len(str(end_date).split()) == 1:
+                    end_date += " 00:00:00"
+
+                current_date = datetime.strptime(start_date, "%Y-%m-%d %H:%M:%S")
+                end_date = datetime.strptime(end_date, "%Y-%m-%d %H:%M:%S")
+                dates = []
+                while current_date <= end_date:
+                    month_year = current_date.strftime("%#m-%Y") + ".parquet"
+                    dates.append(month_year)
+                    current_date += timedelta(days=32)
+                    current_date = current_date.replace(day=1)
+
+                return dates
+
+            def read_one(filenames):
+                with connector.open(container_name + str(device_id) + "/" + str(filenames),
+                                 "rb") as src_file:
+                    df = pd.read_parquet(src_file)
                 return df
 
-            def thread_read():
+            def thread_read(filenames):
                 results = []
-                blob_list = get_dates()
-                if len(blob_list) !=0:
+                if len(filenames) != 0:
                     with ThreadPoolExecutor(max_workers=40) as executor:  # function to thread
-                        for record in range(len(blob_list)):
+                        for record in range(len(filenames)):
                             sys.stdout.write('\r')
                             sys.stdout.write("Please Wait .. ")
                             sys.stdout.flush()
-                        results = executor.map(read_one, blob_list)
+                        results = executor.map(read_one, filenames)
                     fetched_df = pd.concat(results, axis=0)
                 else:
-                    fetched_df=pd.DataFrame()
+                    fetched_df = pd.DataFrame()
                 return fetched_df
+            if type(end_time) == str:
+                try:
+                    end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
+                except Exception:
 
-            flag = check_device(device_id)
-            if flag and api==False:
-                df = thread_read()
-                if len(df) != 0:
-                    try:
-                        start_time = datetime.strptime(start_time, '%Y-%m-%d %H:%M:%S')
-                        end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
-                        df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
-                    except ValueError:
-                        df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
-                        pass
-                    except Exception as e:
-                        print('Message: \t',e)
-                    if len(df) !=0:
-                        if sensors is None:
-                            sensors = list(df.columns)
-                            sensors.remove('time')
-                        sensor_list_df = list(df.columns)
-                        sensor_list_df.remove('time')
-                        sensors_filtered = list(set(sensor_list_df).intersection(sensors))
-                        if sensors != None and len(sensors_filtered) != 0:
-                            sensors_filtered.insert(0,'time')
-                            df =  df[sensors_filtered]
-                        if len(sensors_filtered) == 0:
-                            df = pd.DataFrame()
-                        df.sort_values(['time'], inplace=True)
-                        df.reset_index(drop=True, inplace=True)
-                        last_date = str(df['time'].iloc[-1])
-                        start_date = df['time'].iloc[-1].date() + timedelta(days=1)
+                    if type(end_time) == str:
+                        end_time = str(end_time) + " 23:59:59"
+                    pass
+            df = pd.DataFrame()
+            metadata = {}
+            connector = None
+            container_name = None
+            credentials = DataAccess.get_database_credentials(self,db)
+            if db == "gcs":
+                credentials = eval(credentials)
+                connector = fsspec.filesystem("gs", project=credentials['project_id'],
+                                              token=credentials)
+                container_name = "faclon-ds-feature-store/"
+
+            elif db == "az":
+                connector = fsspec.filesystem("az", account_name=credentials[0],
+                                              account_key=credentials[1])
+                container_name = "feature-store/"
+
+            elif db == "s3":
+                connector = fsspec.filesystem("s3", key=credentials[0],
+                                              secret=credentials[1])
+                container_name = "faclon-ai-public-bucket/"
 
-                        last_date = datetime.strptime(last_date, "%Y-%m-%d %H:%M:%S.%f")
-                        try:
-                            end_time = datetime.strptime(str(end_time), "%Y-%m-%d %H:%M:%S.%f")
-                        except ValueError:
-                            end_time = datetime.strptime(str(end_time), "%Y-%m-%d %H:%M:%S")
-
-                        if last_date.year != end_time.year or last_date.month != end_time.month or last_date.day != end_time.day and last_date.hour != end_time.hour:
-                            df1 = DataAccess.fetch_data(self, device_id, start_time=str(start_date), alias=False,
-                                                        end_time=end_time, sensors=sensors, echo=True,
-                                                        onpremise=onpremise, IST=True)
-                            df = pd.concat([df, df1])
-                            df.reset_index(drop=True, inplace=True)
             else:
-                df_devices = DataAccess.get_device_details(self,onpremise=onpremise)
+                raise Exception('Enter correct Database name')
+
+            blobs = connector.ls(container_name)
+            device_list = [blob.split("/")[1] for blob in blobs]
+            if device_id in device_list:
+                blobs = [blob_name.split("/")[2] for blob_name in connector.ls(container_name + str(device_id) + "/")]
+                dates = generate_month_year_dates(start_time, end_time)
+
+                filenames = list(set(dates).intersection(blobs))
+                filenames = sorted(filenames, key=get_month_year)
+                df = thread_read(filenames)
+            else:
+                df_devices = DataAccess.get_device_details(self)
                 device_list = df_devices['devID'].tolist()
                 if device_id in device_list:
-                    df = DataAccess.fetch_data(self, device_id, start_time,end_time, alias,sensors=sensors,echo=True,onpremise=onpremise,IST=IST)
+                    df = DataAccess.fetch_data(self, device_id, start_time, end_time, alias, sensors=sensors, echo=True,
+                                               onpremise=onpremise, IST=IST)
                 else:
                     raise Exception('Message: Device not added in account')
             if len(df) != 0:
+
+                try:
+                    start_time = datetime.strptime(start_time, '%Y-%m-%d %H:%M:%S')
+                    end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
+                except ValueError:
+                    pass
+                except Exception as e:
+                    print('Message:', e)
+
+                df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
+                if len(df) != 0:
+                    if sensors is None:
+                        sensors = list(df.columns)
+                        sensors.remove('time')
+
+                    sensors_filtered = list(set(df.columns).intersection(sensors))
+                    if sensors and len(sensors_filtered) != 0:
+                        sensors_filtered.insert(0, 'time')
+                        df = df[sensors_filtered]
+                    else:
+                        df = pd.DataFrame()
+                    df.sort_values(['time'], inplace=True)
+                    df.reset_index(drop=True, inplace=True)
+                    last_date = df['time'].iloc[-1]
+
+                    if str(last_date) < str(end_time):
+                        df1 = DataAccess.fetch_data(self, device_id, start_time=last_date, alias=False,
+                                                    end_time=end_time, sensors=sensors, echo=True,
+                                                    onpremise=onpremise, IST=True)
+                        df = pd.concat([df, df1])
+                        df.reset_index(drop=True, inplace=True)
+
+
+
+            if len(df) != 0:
                 if str(alias).lower() == "true":
-                    df,metadata = DataAccess.get_sensor_alias(self,device_id,df,metadata,onpremise=onpremise)
+                    df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
+
 
                 if str(cal).lower() == 'true':
-                    df = DataAccess.get_caliberation(self, device_id, metadata, df,onpremise=onpremise)
+                    df = DataAccess.get_caliberation(self, device_id, metadata, df, onpremise=onpremise)
+
                 if bands is not None:
-                    df = DataAccess.time_grouping(self, df, bands,compute)
+                    df = DataAccess.time_grouping(self, df, bands, compute)
                 df = df.set_index(['time'])
                 df = df.fillna(value=np.nan)
                 df.dropna(axis=0, how='all', inplace=True)
                 df.reset_index(drop=False, inplace=True)
                 df.drop_duplicates(inplace=True)
                 if IST == False:
-                    df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5,minutes=30)
+                    df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5, minutes=30)
             return df
         except Exception as e:
-            print(e)
+            print(e)
+
```

### Comparing `iosense_connect-3.0.4/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-4.0.0/iosense_connect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 3.0.4
+Version: 4.0.0
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-3.0.4/setup.py` & `iosense_connect-4.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "3.0.4",
+    version = "4.0.0",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     install_requires=[
         'numpy',
         'pandas',
         'pyarrow',
         'requests',
         'azure-storage-blob',
         'azure-core',
-        'pytz'
+        'pytz',
+        'fsspec',
+        'gcsfs',
+        's3fs'
     ],
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 )
```

