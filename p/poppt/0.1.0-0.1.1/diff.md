# Comparing `tmp/poppt-0.1.0.tar.gz` & `tmp/poppt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poppt-0.1.0.tar", last modified: Sat Jun 10 12:50:35 2023, max compression
+gzip compressed data, was "poppt-0.1.1.tar", last modified: Mon Jun 12 16:28:36 2023, max compression
```

## Comparing `poppt-0.1.0.tar` & `poppt-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:50:35.426512 poppt-0.1.0/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5248 2023-06-10 12:50:35.427483 poppt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:50:35.360529 poppt-0.1.0/poppt/
--rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.1.0/poppt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:50:35.397209 poppt-0.1.0/poppt/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.1.0/poppt/api/__init__.py
--rw-rw-rw-   0        0        0      974 2023-06-10 12:32:57.000000 poppt-0.1.0/poppt/api/ppt.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:50:35.404794 poppt-0.1.0/poppt/core/
--rw-rw-rw-   0        0        0     5475 2023-06-10 12:49:57.000000 poppt-0.1.0/poppt/core/PPTType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.1.0/poppt/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:50:35.407754 poppt-0.1.0/poppt/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.1.0/poppt/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:50:35.414763 poppt-0.1.0/poppt/lib/ppt/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.1.0/poppt/lib/ppt/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.1.0/poppt/lib/ppt/ppt2pdf_service.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:50:35.390128 poppt-0.1.0/poppt.egg-info/
--rw-rw-rw-   0        0        0     5248 2023-06-10 12:50:35.000000 poppt-0.1.0/poppt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-06-10 12:50:35.000000 poppt-0.1.0/poppt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:50:35.000000 poppt-0.1.0/poppt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 15:33:10.000000 poppt-0.1.0/poppt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-06-10 12:50:35.000000 poppt-0.1.0/poppt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-10 12:50:35.000000 poppt-0.1.0/poppt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      722 2023-06-10 12:50:35.430473 poppt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:50:35.422938 poppt-0.1.0/tests/
--rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      545 2023-06-08 15:25:23.000000 poppt-0.1.0/tests/test_ppt.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:28:36.635639 poppt-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5248 2023-06-12 16:28:36.635639 poppt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 16:28:36.470269 poppt-0.1.1/poppt/
+-rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.1.1/poppt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:28:36.583912 poppt-0.1.1/poppt/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.1.1/poppt/api/__init__.py
+-rw-rw-rw-   0        0        0      949 2023-06-10 14:53:03.000000 poppt-0.1.1/poppt/api/ppt.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:28:36.603037 poppt-0.1.1/poppt/core/
+-rw-rw-rw-   0        0        0     5259 2023-06-10 17:14:58.000000 poppt-0.1.1/poppt/core/PPTType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.1.1/poppt/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:28:36.613564 poppt-0.1.1/poppt/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.1.1/poppt/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:28:36.621085 poppt-0.1.1/poppt/lib/ppt/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.1.1/poppt/lib/ppt/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.1.1/poppt/lib/ppt/ppt2pdf_service.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:28:36.564806 poppt-0.1.1/poppt.egg-info/
+-rw-rw-rw-   0        0        0     5248 2023-06-12 16:28:35.000000 poppt-0.1.1/poppt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-06-12 16:28:35.000000 poppt-0.1.1/poppt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:28:35.000000 poppt-0.1.1/poppt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-10 17:15:12.000000 poppt-0.1.1/poppt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-06-12 16:28:35.000000 poppt-0.1.1/poppt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-12 16:28:35.000000 poppt-0.1.1/poppt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      729 2023-06-12 16:28:36.645977 poppt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:28:36.631697 poppt-0.1.1/tests/
+-rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      545 2023-06-08 15:25:23.000000 poppt-0.1.1/tests/test_ppt.py
```

### Comparing `poppt-0.1.0/LICENSE` & `poppt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poppt-0.1.0/PKG-INFO` & `poppt-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.1.0
+Version: 0.1.1
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
```

### Comparing `poppt-0.1.0/README.md` & `poppt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `poppt-0.1.0/poppt/api/ppt.py` & `poppt-0.1.1/poppt/api/ppt.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # @except_dec()
 def ppt2pdf(path: str, output_path='./'):
     mainPPT.ppt2pdf(path, output_path)
 
 
 # def ppt2img(intput_path, output_path=r'./', img_type='img'):
 #     mainPPT.ppt2img(intput_path, output_path, img_type)
-def ppt2img(input_path, output_path, img_type='jpg', merge=False):
+def ppt2img(input_path, output_path, merge=False):
     """
     :param intput_path:
     :param output_path:
     :param img_type:
     :return:
     """
-    mainPPT.ppt2img(input_path, output_path, img_type, merge)
+    mainPPT.ppt2img(input_path, output_path,  merge)
 
 
 def merge4ppt(input_path, output_path=r'./', output_name='merge4ppt.pptx'):
     mainPPT.merge4ppt(input_path, output_path, output_name)
```

### Comparing `poppt-0.1.0/poppt/core/PPTType.py` & `poppt-0.1.1/poppt/core/PPTType.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,16 @@
 
 
 class MainPPT():
     def __init__(self):
         self.app = 'PowerPoint.Application'
         self.suffix_list = ["ppt", "pptx"]
         self.default_img_type = ".jpg"
-        # JPG是17
-        self.img_type_jpg = 17
-        # PNG是18
-        self.img_type_png = 18
+        # JPG是17，PNG是18
+        self.ppt2img_type = 17
 
     def ppt2pdf(self, path, output_path):
         """
         @Author & Date  : CoderWanFeng 2022/5/9 23:34
         @Desc  : path:存放ppt的路径
         """
         filenames = get_files(path)
@@ -36,15 +34,14 @@
                 # time.sleep(3)
 
     def merge4ppt(self, input_path: str, output_path: str, output_name: str):
         """
         :param path: ppt所在文件路径
         :return: None
         """
-
         abs_input_path = Path(input_path).absolute()  # 相对路径→绝对路径
         exsit, abs_output_path = mkdir(output_path)
         ppt_file_list = get_files(abs_input_path)
         save_path = Path(abs_output_path) / output_name
 
         Application = win32com.client.gencache.EnsureDispatch(self.app)
 
@@ -56,72 +53,66 @@
             print('正在操作的文件：', ppt_file)
             page_num = exit_ppt.Slides.Count
             exit_ppt.Close()
             new_ppt.Slides.InsertFromFile(ppt_file, new_ppt.Slides.Count, 1, page_num)
         new_ppt.Save()  # 括号内为保存位置：如C:\Users\Administrator\Documents\下
         Application.Quit()
 
-    def ppt2img(self, input_path, output_path, img_type, merge=False):
+    def ppt2img(self, input_path, output_path, merge=False):
         '''将PPT另存为图片格式
           arguments:
               pptFullName: 要转换的ppt文件，
               pptName：转换后的存放JPG文件的目录
-              imgType: 图片类型
         '''
 
         filenames = get_files(input_path)
         # 启动PPT
         pptClient = win32com.client.Dispatch(self.app)
         # 设置为0表示后台运行，不显示，1则显示
         pptClient.Visible = True
         for ppt_file in filenames:
             if check_suffix(ppt_file, self.suffix_list):
                 # Python路径操作模块pathlib，看这篇就够了！ https://zhuanlan.zhihu.com/p/475661402
                 output_dir = Path(output_path).absolute() / str(Path(ppt_file).stem)
                 exsit, output_dir = mkdir(output_dir)
-
                 # 打开PPT文件
                 ppt = pptClient.Presentations.Open(ppt_file, WithWindow=False, ReadOnly=1)
                 # 另存为图片
-                if img_type in self.default_img_type:
-                    ppt.SaveAs(output_dir, self.img_type_jpg)
-                else:
-                    ppt.SaveAs(output_dir, self.img_type_png)
+                ppt.SaveAs(output_dir, self.ppt2img_type)
 
         # 退出
         pptClient.Quit()
         if merge:
             merge_dir = Path(output_path).absolute()
             for dirpath, dirnames, filenames in os.walk(merge_dir):
                 # print(dirpath, dirnames, filenames)
                 for dirname in dirnames:
-                    current_img_path=os.path.join(dirpath, dirname)
+                    current_img_path = os.path.join(dirpath, dirname)
                     self.generate_long_image(input_path=current_img_path,
                                              current_ppt_name=dirname,
                                              output_path=merge_dir,
                                              img_name=dirname + self.default_img_type)
-                    shutil.rmtree(current_img_path)
+                    shutil.rmtree(current_img_path)  # 删除暂存图片
 
-    def generate_long_image(self, input_path: str, current_ppt_name,output_path, img_name='merge.jpg'):
+    def generate_long_image(self, input_path: str, current_ppt_name, output_path, img_name='merge.jpg'):
         """
         将ppt的各个页面拼接成长图：https://blog.csdn.net/m0_51777056/article/details/130262561
         :param input_path:
         :param output_path:
         :param img_name:
         :return:
         """
         # 获取图片列表
         img_list = []
         for imgs in os.listdir(input_path):
             img_list.append(os.path.join(input_path, imgs))
 
-        # print(ims)
         # 将获取到ppt的页面进行排序
         ims_sort = sorted(img_list, key=lambda jpg: len(jpg))
-        print(f"正在生成《{current_ppt_name}》的图片")
+        print(f"正在生成【PPT文件名为：{current_ppt_name}】的图片")
 
         width, height = Image.open(img_list[0]).size  # 取第一个图片尺寸
         img_mode = Image.open(img_list[0]).mode
         long_canvas = Image.new(img_mode, (width, height * len(img_list)))  # 创建同宽，n倍高的空白图片
 
         # 拼接图片
         for i, image in enumerate(ims_sort):
```

### Comparing `poppt-0.1.0/poppt/lib/ppt/ppt2pdf_service.py` & `poppt-0.1.1/poppt/lib/ppt/ppt2pdf_service.py`

 * *Files identical despite different names*

### Comparing `poppt-0.1.0/poppt.egg-info/PKG-INFO` & `poppt-0.1.1/poppt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.1.0
+Version: 0.1.1
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
```

### Comparing `poppt-0.1.0/setup.cfg` & `poppt-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f70 7074 0d0a 7665 7273 696f   = poppt..versio
-00000020: 6e20 3d20 302e 312e 300d 0a64 6573 6372  n = 0.1.0..descr
+00000020: 6e20 3d20 302e 312e 310d 0a64 6573 6372  n = 0.1.1..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f70 7074 0d0a 6c6f 6e67  tall poppt..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
@@ -29,18 +29,18 @@
 000001c0: 6d61 7374 6572 2f52 4541 444d 452e 6d64  master/README.md
 000001d0: 0d0a 0953 6f75 7263 6520 436f 6465 203d  ...Source Code =
 000001e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 000001f0: 636f 6d2f 436f 6465 7257 616e 4665 6e67  com/CoderWanFeng
 00000200: 2f70 6f70 7074 0d0a 0d0a 5b6f 7074 696f  /poppt....[optio
 00000210: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
 00000220: 6669 6e64 3a0d 0a69 6e73 7461 6c6c 5f72  find:..install_r
-00000230: 6571 7569 7265 7320 3d20 0d0a 0970 7970  equires = ...pyp
-00000240: 6977 696e 3332 0d0a 0970 6f70 726f 6772  iwin32...poprogr
-00000250: 6573 730d 0a09 706f 6669 6c65 0d0a 7079  ess...pofile..py
-00000260: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000270: 3e3d 332e 370d 0a69 6e63 6c75 6465 5f70  >=3.7..include_p
-00000280: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
-00000290: 7565 0d0a 7a69 705f 7361 6665 203d 2046  ue..zip_safe = F
-000002a0: 616c 7365 0d0a 0d0a 5b65 6767 5f69 6e66  alse....[egg_inf
-000002b0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000002c0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000002d0: 0d0a                                     ..
+00000230: 6571 7569 7265 7320 3d20 0d0a 0970 7977  equires = ...pyw
+00000240: 696e 3332 0d0a 0970 6f70 726f 6772 6573  in32...poprogres
+00000250: 730d 0a09 706f 6669 6c65 0d0a 0970 696c  s...pofile...pil
+00000260: 6c6f 770d 0a70 7974 686f 6e5f 7265 7175  low..python_requ
+00000270: 6972 6573 203d 203e 3d33 2e37 0d0a 696e  ires = >=3.7..in
+00000280: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000290: 7461 203d 2054 7275 650d 0a7a 6970 5f73  ta = True..zip_s
+000002a0: 6166 6520 3d20 4661 6c73 650d 0a0d 0a5b  afe = False....[
+000002b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000002c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000002d0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `poppt-0.1.0/tests/test_ppt.py` & `poppt-0.1.1/tests/test_ppt.py`

 * *Files identical despite different names*

