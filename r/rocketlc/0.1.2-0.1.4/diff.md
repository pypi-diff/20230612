# Comparing `tmp/rocketlc-0.1.2-py3-none-any.whl.zip` & `tmp/rocketlc-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9346 bytes, number of entries: 10
+Zip file size: 9445 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      104 b- defN 22-Dec-31 06:29 rocketlc/__init__.py
 -rw-rw-r--  2.0 unx       79 b- defN 22-Dec-31 17:13 rocketlc/florida_review.py
 -rw-rw-r--  2.0 unx     4493 b- defN 22-Dec-31 15:30 rocketlc/rocket_launch_live.py
--rw-rw-r--  2.0 unx     2770 b- defN 23-Jun-11 16:43 rocketlc/space_schedulle_launch.py
--rw-rw-r--  2.0 unx      327 b- defN 23-Jun-11 16:41 rocketlc/tools_ssl.py
--rw-rw-r--  2.0 unx     1497 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21036 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      803 b- defN 23-Jun-11 16:44 rocketlc-0.1.2.dist-info/RECORD
-10 files, 31210 bytes uncompressed, 7974 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx     3007 b- defN 23-Jun-12 02:21 rocketlc/space_schedulle_launch.py
+-rw-rw-r--  2.0 unx      472 b- defN 23-Jun-12 02:25 rocketlc/tools_ssl.py
+-rw-rw-r--  2.0 unx     1497 b- defN 23-Jun-12 02:25 rocketlc-0.1.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21036 b- defN 23-Jun-12 02:25 rocketlc-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 02:25 rocketlc-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-12 02:25 rocketlc-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      803 b- defN 23-Jun-12 02:25 rocketlc-0.1.4.dist-info/RECORD
+10 files, 31592 bytes uncompressed, 8073 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: rocketlc/space_schedulle_launch.py
 Comment: 
 
 Filename: rocketlc/tools_ssl.py
 Comment: 
 
-Filename: rocketlc-0.1.2.dist-info/LICENSE
+Filename: rocketlc-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: rocketlc-0.1.2.dist-info/METADATA
+Filename: rocketlc-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: rocketlc-0.1.2.dist-info/WHEEL
+Filename: rocketlc-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: rocketlc-0.1.2.dist-info/top_level.txt
+Filename: rocketlc-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: rocketlc-0.1.2.dist-info/RECORD
+Filename: rocketlc-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rocketlc/space_schedulle_launch.py

```diff
@@ -27,18 +27,23 @@
         canaveral = bs(url_html,features="html.parser")
         div_mother = canaveral.find('div',{'class':'col-lg-8'})
         
         divs = div_mother.find_all('div')
         #print(divs)
         for dv in divs:
             if ('my-2' in dv['class']) and ('container' in dv['class']):
+                # print(dv)
                 name = dv.find('span',{'class':'mt-2'}).text
                 mission = dv.find('h2',{'class':'h4'}).text.replace('\n','')
                 mother = dv.find('h3',{'class':'h6'}).text
+                
                 time_lst = dv.find('time',{'class':"launchDateTime"})['datetime']
+                launch_time = dv.find('time',{'class':'launchDateTime'}).get('launch-window-end-utc',None)
+                time_lst = launch_time if launch_time else time_lst
+                
                 loc = dv.find('div',{'class':'mb-0'}).text.replace('\n','')
                 
                 style_a = dv.find('a',{'class':'launch-list-thumbnail'})['style']
                 a_img = dv.find('a',{'class':'ezlazyload'})
               
                 url_img = a_img['data-ezbg'] if a_img else style_a.split(':')[-1].split('url(')[-1].replace(')','').replace(';','').replace('//','')
                 url_img = url_img.split('?')[0]
```

## rocketlc/tools_ssl.py

```diff
@@ -1,9 +1,14 @@
 from datetime import datetime as dt
 
 def get_time(launch_datetime_str):
-    launch = dt.strptime(launch_datetime_str,'%Y-%m-%d %H:%M')
+
+    if 'T' in launch_datetime_str:
+        launch = dt.strptime(rf'{launch_datetime_str}','%Y-%m-%dT%H:%M:%SZ')
+    else:
+        launch = dt.strptime(rf'{launch_datetime_str}','%Y-%m-%d %H:%M:%S')
+
     date = launch.strftime('%d/%m/%Y')
     hour = launch.strftime('%H:%M')
-    res_seconds = (launch - dt.utcnow()).seconds
+    res_seconds = (launch - dt.utcnow()).total_seconds()
     return {'hour':hour,'date':date,'res_seconds':res_seconds}
```

## Comparing `rocketlc-0.1.2.dist-info/LICENSE` & `rocketlc-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rocketlc-0.1.2.dist-info/METADATA` & `rocketlc-0.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketlc
-Version: 0.1.2
+Version: 0.1.4
 Summary: Library for getting schedule launch rocket
 Home-page: https://github.com/reinanbr/rocketlc
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: BSD v3
 Keywords: rocket launch schedule
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rocketlc Version: 0.1.2 Summary: Library for
+Metadata-Version: 2.1 Name: rocketlc Version: 0.1.4 Summary: Library for
 getting schedule launch rocket Home-page: https://github.com/reinanbr/rocketlc
 Author: Reinan Br Author-email: slimchatuba@gmail.com License: BSD v3 Keywords:
 rocket launch schedule Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: mechanicalsoup Requires-Dist:
 cssutils Requires-Dist: bs4
                              ***** Rocketlc *****
                         getting schedule launch rocket
```

## Comparing `rocketlc-0.1.2.dist-info/RECORD` & `rocketlc-0.1.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 rocketlc/__init__.py,sha256=X4yCGNqYQKnsdbrnMPaxXE6zc-gg_HW6WdplGIXrzkQ,104
 rocketlc/florida_review.py,sha256=K8rpaPEDBKNY_ueV0TMHrvQGxspFNOzDktgOMI6o6vk,79
 rocketlc/rocket_launch_live.py,sha256=u0YDTen1YAE3KWeFtiGkNzW5paXPnIttVMbjFIUv9Cg,4493
-rocketlc/space_schedulle_launch.py,sha256=bEyfqDMV0h2NltaixklRiudnVcD3EU-Sgax8pLKFAd0,2770
-rocketlc/tools_ssl.py,sha256=nfyvHM44F49EfRvo0zpaRoDzSxRT7H0_B7N7AWANKo4,327
-rocketlc-0.1.2.dist-info/LICENSE,sha256=Tl-V6VQEtfTkxCWsZ6J-i_-1-revwfdkfy6hz45P8bM,1497
-rocketlc-0.1.2.dist-info/METADATA,sha256=zDg-7sDqbQx2Mr_PDxh9gyAU-wFNm2jSeEwucXy9Mg0,21036
-rocketlc-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rocketlc-0.1.2.dist-info/top_level.txt,sha256=02sCqeNCLTHdHZouYwEtsyGPHh828Lji7RhrEXY1eu4,9
-rocketlc-0.1.2.dist-info/RECORD,,
+rocketlc/space_schedulle_launch.py,sha256=WiHmXVc6P-CwyCydpfugtnma_M-QvNbSfBSjuNSeuAo,3007
+rocketlc/tools_ssl.py,sha256=ZXWOL3icVgj4Va9zlFCZRYJ_WQ2osoHd-zT149uxin4,472
+rocketlc-0.1.4.dist-info/LICENSE,sha256=Tl-V6VQEtfTkxCWsZ6J-i_-1-revwfdkfy6hz45P8bM,1497
+rocketlc-0.1.4.dist-info/METADATA,sha256=baQGpDz07i_FvFW92zboRcb7AoDU4sJKnyDKjF_Wpb0,21036
+rocketlc-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rocketlc-0.1.4.dist-info/top_level.txt,sha256=02sCqeNCLTHdHZouYwEtsyGPHh828Lji7RhrEXY1eu4,9
+rocketlc-0.1.4.dist-info/RECORD,,
```

