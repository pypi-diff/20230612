# Comparing `tmp/FindJobsTW-0.3.1.tar.gz` & `tmp/FindJobsTW-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-0.3.1.tar", last modified: Tue Jun  6 16:31:28 2023, max compression
+gzip compressed data, was "FindJobsTW-1.0.0.tar", last modified: Mon Jun 12 09:25:51 2023, max compression
```

## Comparing `FindJobsTW-0.3.1.tar` & `FindJobsTW-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:31:28.924555 FindJobsTW-0.3.1/
-drwxrwxrwx   0        0        0        0 2023-06-06 16:31:28.922562 FindJobsTW-0.3.1/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-06 16:31:28.000000 FindJobsTW-0.3.1/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-06 16:31:28.000000 FindJobsTW-0.3.1/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:31:28.000000 FindJobsTW-0.3.1/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-06-06 16:31:28.000000 FindJobsTW-0.3.1/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 16:31:28.000000 FindJobsTW-0.3.1/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 16:16:15.000000 FindJobsTW-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      591 2023-06-06 16:31:28.924555 FindJobsTW-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 16:16:15.000000 FindJobsTW-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:31:28.923558 FindJobsTW-0.3.1/findJobs/
--rw-rw-rw-   0        0        0    17377 2023-06-06 16:23:15.000000 FindJobsTW-0.3.1/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0        0 2023-06-06 16:16:15.000000 FindJobsTW-0.3.1/findJobs/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-06 16:31:28.924555 FindJobsTW-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-06-06 16:31:10.000000 FindJobsTW-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:25:51.899273 FindJobsTW-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-12 09:25:51.885274 FindJobsTW-1.0.0/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      591 2023-06-12 09:25:51.898290 FindJobsTW-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 09:25:51.894290 FindJobsTW-1.0.0/findJobs/
+-rw-rw-rw-   0        0        0    17529 2023-06-12 09:09:07.000000 FindJobsTW-1.0.0/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0      133 2023-06-12 09:19:48.000000 FindJobsTW-1.0.0/findJobs/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-06-12 09:15:10.000000 FindJobsTW-1.0.0/findJobs/app.py
+-rw-rw-rw-   0        0        0     4908 2023-06-12 04:00:23.000000 FindJobsTW-1.0.0/findJobs/url.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 09:25:51.901276 FindJobsTW-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-06-12 09:25:08.000000 FindJobsTW-1.0.0/setup.py
```

### Comparing `FindJobsTW-0.3.1/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-1.0.0/FindJobsTW.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.3.1
+Version: 1.0.0
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-0.3.1/LICENSE` & `FindJobsTW-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-0.3.1/PKG-INFO` & `FindJobsTW-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.3.1
+Version: 1.0.0
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-0.3.1/findJobs/FindJobs.py` & `FindJobsTW-1.0.0/findJobs/FindJobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,24 +42,26 @@
              "工作技能" : f"/html/body/div[2]/div/div[2]/div/div[1]/div[2]/div[2]/div[{index}]/div[2]/div//*/a/u",
              "具備證照" : f"/html/body/div[2]/div/div[2]/div/div[1]/div[2]/div[2]/div[{index}]/div[2]/div//*/p/a/u",
              "其他條件" : f"/html/body/div[2]/div/div[2]/div/div[1]/div[2]/div[3]/div/div[2]/div/div/p",
              "具備駕照" : f"/html/body/div[2]/div/div[2]/div/div[1]/div[2]/div[2]/div[{index}]/div[2]/div",
             }
         return match.get(col_name)
 
-    def search_links(self, max_pages = 3):
+    def search_links(self, max_pages = 3, ori_url = None):
         page = 1
         data = []
+        if ori_url == None:
+            ori_url = f'https://www.104.com.tw/jobs/search/?ro=0&kwop=7&keyword={self.keyword}&expansionType=area%2Cspec%2Ccom%2Cjob%2Cwf%2Cwktm&order=15&asc=0&mode=s&jobsource=2018indexpoc&langFlag=0&langStatus=0&recommendJob=1&hotJob=1'
         print(f"開始搜尋關鍵字: {self.keyword}")
         while True:
-            url = f'https://www.104.com.tw/jobs/search/?ro=0&kwop=7&keyword={self.keyword}&expansionType=area%2Cspec%2Ccom%2Cjob%2Cwf%2Cwktm&order=15&asc=0&page={page}&mode=s&jobsource=2018indexpoc&langFlag=0&langStatus=0&recommendJob=1&hotJob=1'
+            url = ori_url + f"&page={page}"
             res = requests.get(url, timeout=10)
             soup = BeautifulSoup(res.text, features="lxml")
             jobs = soup.find_all('article', class_='b-block--top-bord job-list-item b-clearfix js-job-item')
-            if not jobs:
+            if not jobs:#找不到內容就中斷
                 break
             print("現在正在讀取第" + str(page) + "頁")
             for job in jobs:
                 title = job['data-job-name'].strip()
                 company = job('li')[1].text.strip()
                 URL = 'https:' + job.find("a", class_='js-job-link')['href']
                 dict1 = {"公司名稱": company, "職缺名稱": title, "職缺連結": URL}
@@ -70,14 +72,15 @@
         if data:
             self.job_links = pd.DataFrame(columns = data[0].keys(), data = data)
             print("-"*20)
             print("已完成搜尋，請使用find_jobs爬取工作資料")
             print("-"*20)
         else:
             print("查詢失敗")
+            self.job_links = pd.DataFrame()
         return self.job_links
         
     def save_jobs_link(self):
         if not self.job_links:
             print("無資料可儲存")
             return
         path = self.keyword + r"-職缺連結.xlsx" #定義檔案路徑 #當檔案名稱有中文要加r
@@ -349,14 +352,14 @@
         plt.ylabel('密度')
         plt.legend()
         plt.show()
 
 if __name__ == "__main__":
     keyword = "數據分析師"
     jobs = Jobs(keyword)
-    jobs.search_links(max_pages = 1)#一頁是20個職缺
+    jobs.search_links(max_pages = 3)#一頁是20個職缺
     jobs.find_jobs()
     jobs.save_jobs()
     jobs.draw_box()
     jobs.draw_density()
     #jobs.show("all") #一次秀出全部
     jobs.show("職務類別")
```

### Comparing `FindJobsTW-0.3.1/setup.py` & `FindJobsTW-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='0.3.1',      
+    version='1.0.0',      
     packages=find_packages(),    
     install_requires=requirements,
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
     description="A Python package to find jobs on 104.com.tw based on specific keywords.",
     long_description=open('README.md', 'r', encoding='utf-8').read(),# 若Discription.md中有中文 須加上 encoding="utf-8"
     long_description_content_type="text/markdown",
```

