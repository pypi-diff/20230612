# Comparing `tmp/natalify-3.0.tar.gz` & `tmp/natalify-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natalify-3.0.tar", last modified: Wed Jun  7 14:52:04 2023, max compression
+gzip compressed data, was "natalify-3.2.tar", last modified: Mon Jun 12 09:01:11 2023, max compression
```

## Comparing `natalify-3.0.tar` & `natalify-3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:52:04.549696 natalify-3.0/
--rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-3.0/LICENSE
--rw-rw-rw-   0        0        0     2184 2023-06-07 14:52:04.549696 natalify-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1664 2023-05-22 11:28:41.000000 natalify-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 14:52:04.534072 natalify-3.0/natalify/
--rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-3.0/natalify/__init__.py
--rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-3.0/natalify/__main__.py
--rw-rw-rw-   0        0        0    64049 2023-06-07 14:51:01.000000 natalify-3.0/natalify/natalify.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:52:04.534072 natalify-3.0/natalify.egg-info/
--rw-rw-rw-   0        0        0     2184 2023-06-07 14:52:02.000000 natalify-3.0/natalify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-07 14:52:04.000000 natalify-3.0/natalify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:52:03.000000 natalify-3.0/natalify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-07 14:52:03.000000 natalify-3.0/natalify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 14:52:03.000000 natalify-3.0/natalify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:52:04.549696 natalify-3.0/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-06-07 14:51:55.000000 natalify-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:01:11.678819 natalify-3.2/
+-rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-3.2/LICENSE
+-rw-rw-rw-   0        0        0     2184 2023-06-12 09:01:11.678819 natalify-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1664 2023-05-22 11:28:41.000000 natalify-3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 09:01:11.654823 natalify-3.2/natalify/
+-rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-3.2/natalify/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-3.2/natalify/__main__.py
+-rw-rw-rw-   0        0        0    64162 2023-06-12 08:59:42.000000 natalify-3.2/natalify/natalify.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:01:11.670820 natalify-3.2/natalify.egg-info/
+-rw-rw-rw-   0        0        0     2184 2023-06-12 09:01:09.000000 natalify-3.2/natalify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-12 09:01:11.000000 natalify-3.2/natalify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:01:09.000000 natalify-3.2/natalify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-12 09:01:09.000000 natalify-3.2/natalify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 09:01:10.000000 natalify-3.2/natalify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 09:01:11.678819 natalify-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-06-12 08:59:56.000000 natalify-3.2/setup.py
```

### Comparing `natalify-3.0/LICENSE` & `natalify-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `natalify-3.0/PKG-INFO` & `natalify-3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 3.0
+Version: 3.2
 Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `natalify-3.0/README.md` & `natalify-3.2/README.md`

 * *Files identical despite different names*

### Comparing `natalify-3.0/natalify/natalify.py` & `natalify-3.2/natalify/natalify.py`

 * *Files 0% similar despite different names*

```diff
@@ -858,37 +858,39 @@
     async def main_window(self,search_key):
 
         win_handle = self.driver.window_handles
         self.driver.switch_to.window(win_handle[0])
 
         await self.search(search_key,0)
 
+
         self.driver.switch_to.window(win_handle[0])
+        self.driver.refresh()
 
         try:
 
-            hashtags_posts=random.randrange(12,20)
+            hashtags_posts=random.randrange(10,40)
 
             for row in range(0,hashtags_posts):
             
                 
-                wait = WebDriverWait(self.driver, 50)  
+                wait = WebDriverWait(self.driver, 70)  
 
                 post = wait.until(EC.presence_of_all_elements_located((By.CLASS_NAME, '_aabd')))
 
                
 
                     # Scroll the page to the element using JavaScript
                 self.driver.execute_script("arguments[0].scrollIntoView();", post[row])
 
                 post[row].click()
 
 
                                     # Wait for the presence of the div element
-                wait = WebDriverWait(self.driver, 10)
+                wait = WebDriverWait(self.driver, 50)
                 div_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "div._aaqt")))
 
                 # Get the text of the div element
                 username = div_element.text
 
 
                 self.sleep_ = random.randrange(15,25)
@@ -897,15 +899,15 @@
                 self.status = f" {str(datetime.datetime.now())}  Getting [ {username} ] post"
 
                 await asyncio.sleep(self.sleep_)
                 self.driver.switch_to.window(win_handle[0])
 
                 
 
-                post_buttons = WebDriverWait(self.driver, 20).until(
+                post_buttons = WebDriverWait(self.driver, 50).until(
                         EC.presence_of_all_elements_located((By.CSS_SELECTOR, "button[class='_abl-']")))
 
                 
 
                 for element in post_buttons:
 
                     if "Unlike" in element.get_attribute("innerHTML") or "Like" in element.get_attribute("innerHTML"):
@@ -946,15 +948,15 @@
 
                                     break
 
                             # Perform the desired action on the element
                             comment_button.click()
 
 
-                            comment_field = WebDriverWait(self.driver, 20).until(
+                            comment_field = WebDriverWait(self.driver, 50).until(
                                 EC.presence_of_element_located(
                                     (By.CSS_SELECTOR, 'textarea[aria-label="Add a comment…"]')))
 
                             comment_field.send_keys(self.comments[random.randrange(len(self.comments))])
 
                             time.sleep(random.randrange(1, 4))
 
@@ -1222,15 +1224,15 @@
 
         attempts = 0
 
         while True:
             try:
                                      
                                 # Wait for the elements to be present
-                elements = WebDriverWait(self.driver, 10).until(
+                elements = WebDriverWait(self.driver, 50).until(
                     EC.presence_of_all_elements_located((By.XPATH, f"//div[@role='none']//span[contains(text(), '{search_key}')]"))
                 )
 
                 # Click on the first element
                 element=elements[0]
                 
 
@@ -1513,18 +1515,21 @@
             print(colored(f"\nStarting .... \n\nTo logout of {user()} run the following command and reset your settings \n\npython3 -m natalify -logout","cyan"))
             run_target_accounts = settings[0].get("run_target_accounts")
             run_hashtags = settings[0].get("run_hashtags")
             comment = settings[0].get("comment")
             window = settings[0].get("window")
             components_path = settings[0].get("components_path")
 
+           
             credentials=db.search(User.credentials == 'true')
 
             if credentials:
                 # print(credentials)
+                encrypted_creds=credentials[0].get("encrypted")
+
                 decrypt_credentials=credentials[0].get("encrypted").encode()
 
                 encrypted = encrypt_creds.decrypt(decrypt_credentials)
                 decrypt_pickle2 = pickle.loads(encrypted)
                 username = decrypt_pickle2.get("username", "specify a username")
                 password = decrypt_pickle2.get("password", "specify a password")
             time.sleep(5)
```

### Comparing `natalify-3.0/natalify.egg-info/PKG-INFO` & `natalify-3.2/natalify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 3.0
+Version: 3.2
 Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `natalify-3.0/setup.py` & `natalify-3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='natalify',
-    version='3.0',
+    version='3.2',
     packages=setuptools.find_packages(),
     license='GPL-3.0',
     author='jack',
     author_email='kinginjack@gmail.com',
     description='A simple automation software for various tasks',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

