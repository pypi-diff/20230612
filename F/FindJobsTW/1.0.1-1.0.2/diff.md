# Comparing `tmp/FindJobsTW-1.0.1.tar.gz` & `tmp/FindJobsTW-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-1.0.1.tar", last modified: Mon Jun 12 09:37:51 2023, max compression
+gzip compressed data, was "FindJobsTW-1.0.2.tar", last modified: Mon Jun 12 09:46:33 2023, max compression
```

## Comparing `FindJobsTW-1.0.1.tar` & `FindJobsTW-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.839067 FindJobsTW-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.820070 FindJobsTW-1.0.1/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       72 2023-06-12 09:32:38.000000 FindJobsTW-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      591 2023-06-12 09:37:51.838070 FindJobsTW-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.831072 FindJobsTW-1.0.1/findJobs/
--rw-rw-rw-   0        0        0    17529 2023-06-12 09:09:07.000000 FindJobsTW-1.0.1/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0      133 2023-06-12 09:19:48.000000 FindJobsTW-1.0.1/findJobs/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-06-12 09:15:10.000000 FindJobsTW-1.0.1/findJobs/app.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.834077 FindJobsTW-1.0.1/findJobs/static/
--rw-rw-rw-   0        0        0      382 2023-06-12 08:30:14.000000 FindJobsTW-1.0.1/findJobs/static/styles.css
-drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.836068 FindJobsTW-1.0.1/findJobs/templates/
--rw-rw-rw-   0        0        0    28017 2023-06-12 08:41:44.000000 FindJobsTW-1.0.1/findJobs/templates/index.html
--rw-rw-rw-   0        0        0     4908 2023-06-12 04:00:23.000000 FindJobsTW-1.0.1/findJobs/url.py
--rw-rw-rw-   0        0        0       42 2023-06-12 09:37:51.839067 FindJobsTW-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      936 2023-06-12 09:37:47.000000 FindJobsTW-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.084308 FindJobsTW-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.037751 FindJobsTW-1.0.2/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-06-12 09:32:38.000000 FindJobsTW-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      591 2023-06-12 09:46:33.083305 FindJobsTW-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.046778 FindJobsTW-1.0.2/findJobs/
+-rw-rw-rw-   0        0        0    17529 2023-06-12 09:45:45.000000 FindJobsTW-1.0.2/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0      133 2023-06-12 09:19:48.000000 FindJobsTW-1.0.2/findJobs/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-06-12 09:15:10.000000 FindJobsTW-1.0.2/findJobs/app.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.049778 FindJobsTW-1.0.2/findJobs/static/
+-rw-rw-rw-   0        0        0      382 2023-06-12 08:30:14.000000 FindJobsTW-1.0.2/findJobs/static/styles.css
+drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.080307 FindJobsTW-1.0.2/findJobs/templates/
+-rw-rw-rw-   0        0        0    27906 2023-06-12 09:45:41.000000 FindJobsTW-1.0.2/findJobs/templates/index.html
+-rw-rw-rw-   0        0        0     4908 2023-06-12 04:00:23.000000 FindJobsTW-1.0.2/findJobs/url.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 09:46:33.084308 FindJobsTW-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      936 2023-06-12 09:46:17.000000 FindJobsTW-1.0.2/setup.py
```

### Comparing `FindJobsTW-1.0.1/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-1.0.2/FindJobsTW.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.1/LICENSE` & `FindJobsTW-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.1/PKG-INFO` & `FindJobsTW-1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.1/findJobs/FindJobs.py` & `FindJobsTW-1.0.2/findJobs/FindJobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                 job_data = {**dict_data_jobs, **job_data}
                 data.append(job_data)
                 print(f"正在爬取第{i+1}/{min(self.job_links.shape[0], max_jobs)}個工作")
             except KeyboardInterrupt:
                 break
             except:
                 continue
-            if i == max_jobs-1:
+            if i >= max_jobs-1:
                 break        
         fields =['公司名稱', '職缺名稱', '職缺連結', '職務名稱', '職務類別', '工作待遇',
                  '薪資型態', '薪資下限', '薪資上限',
                  '工作性質', '上班地點', '遠端工作', '管理責任', '出差外派', '上班時段',
                  '休假制度', '可上班日', '需求人數', '語文條件', '工作經歷', '學歷要求',
                  '科系要求', '擅長工具', '工作技能', '具備駕照', '具備證照', '法定項目',
                  '其他福利', '招募福利']
```

### Comparing `FindJobsTW-1.0.1/findJobs/app.py` & `FindJobsTW-1.0.2/findJobs/app.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.1/findJobs/templates/index.html` & `FindJobsTW-1.0.2/findJobs/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label>查詢數量:</label>
                                 <div class="input-group">
                                     <input type="number" class="form-control" id="JobNumber" name="JobNumber" placeholder="搜尋工作數量(建議不要超過100以免等待過久)" min="0"  value="{{ current_JobNumber if current_JobNumber else '20' }}">  
                                 </div>
-                                <small class="form-text text-muted">選擇自訂薪資條件時填寫</small>
                             </div>
                             <div class="form-group">
                                 <label for="job_type">選擇工作類型:</label>
                                 <select name="job_type" id="job_type" class="form-control">
                                     <option value="不限"{% if current_job_type == '不限' %}selected{% endif %}>不限</option>
                                     <option value="經營／人資類"{% if current_job_type == '經營／人資類' %}selected{% endif %}>經營／人資類</option>
                                     <option value="行政／總務／法務類"{% if current_job_type == '行政／總務／法務類' %}selected{% endif %}>行政／總務／法務類</option>
```

#### html2text {}

```diff
@@ -3,15 +3,14 @@
 Welcome to the Job Finder. Please select the job type and click the button
 below.
 æ¸é¤
 ééµå­:
 [Unknown INPUT type]
 æ¥è©¢æ¸é:
 [Unknown INPUT type]
-é¸æèªè¨èªè³æ¢ä»¶æå¡«å¯«
 % if current_job_type == 'ä¸é' %}selected{% endif %}>ä¸é
 % if current_job_type == 'ç¶çï¼äººè³é¡' %}selected{% endif
 %}>ç¶çï¼äººè³é¡
 % if current_job_type == 'è¡æ¿ï¼ç¸½åï¼æ³åé¡' %}selected{% endif
 %}>è¡æ¿ï¼ç¸½åï¼æ³åé¡
 % if current_job_type == 'è²¡æï¼éèå°æ¥­é¡' %}selected{% endif
 %}>è²¡æï¼éèå°æ¥­é¡
```

### Comparing `FindJobsTW-1.0.1/findJobs/url.py` & `FindJobsTW-1.0.2/findJobs/url.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.1/setup.py` & `FindJobsTW-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='1.0.1',      
+    version='1.0.2',      
     packages=find_packages(),    
     install_requires=requirements,
     package_data={
         'findJobs': ['templates/*', 'static/*']
     },  
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
```

