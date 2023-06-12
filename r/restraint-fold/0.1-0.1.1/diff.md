# Comparing `tmp/restraint-fold-0.1.tar.gz` & `tmp/restraint-fold-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restraint-fold-0.1.tar", last modified: Tue Jun  6 07:18:26 2023, max compression
+gzip compressed data, was "restraint-fold-0.1.1.tar", last modified: Mon Jun 12 02:06:39 2023, max compression
```

## Comparing `restraint-fold-0.1.tar` & `restraint-fold-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-06 07:18:26.348367 restraint-fold-0.1/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     1068 2023-06-06 06:19:40.000000 restraint-fold-0.1/LICENSE
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2635 2023-06-06 07:18:26.348367 restraint-fold-0.1/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2332 2023-06-06 07:12:17.000000 restraint-fold-0.1/README.md
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-06 07:18:26.348367 restraint-fold-0.1/fold/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     7708 2023-06-06 07:16:54.000000 restraint-fold-0.1/fold/__init__.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2967 2023-06-06 07:01:36.000000 restraint-fold-0.1/fold/__main__.py
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-06 07:18:26.348367 restraint-fold-0.1/restraint_fold.egg-info/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2635 2023-06-06 07:18:26.000000 restraint-fold-0.1/restraint_fold.egg-info/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)      249 2023-06-06 07:18:26.000000 restraint-fold-0.1/restraint_fold.egg-info/SOURCES.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-06-06 07:18:26.000000 restraint-fold-0.1/restraint_fold.egg-info/dependency_links.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        7 2023-06-06 07:18:26.000000 restraint-fold-0.1/restraint_fold.egg-info/requires.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        5 2023-06-06 07:18:26.000000 restraint-fold-0.1/restraint_fold.egg-info/top_level.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-06-06 07:18:26.348367 restraint-fold-0.1/setup.cfg
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     1981 2023-06-06 07:17:45.000000 restraint-fold-0.1/setup.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     1068 2023-06-06 06:19:40.000000 restraint-fold-0.1.1/LICENSE
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     2530 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     2226 2023-06-12 02:05:51.000000 restraint-fold-0.1.1/README.md
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/fold/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     7708 2023-06-12 01:57:29.000000 restraint-fold-0.1.1/fold/__init__.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     3009 2023-06-12 02:04:32.000000 restraint-fold-0.1.1/fold/__main__.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/restraint_fold.egg-info/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     2530 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)      249 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/SOURCES.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/dependency_links.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       13 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/requires.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        5 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/top_level.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/setup.cfg
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     1984 2023-06-12 01:59:32.000000 restraint-fold-0.1.1/setup.py
```

### Comparing `restraint-fold-0.1/LICENSE` & `restraint-fold-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `restraint-fold-0.1/PKG-INFO` & `restraint-fold-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,12 @@
-Metadata-Version: 2.1
-Name: restraint-fold
-Version: 0.1
-Summary: Simple Protein Structure Parser
-Home-page: https://gitee.com/dechin/restraint-fold/
-Author: Dechin CHEN
-Author-email: dechin.phy@gmail.com
-License: MIT License
-Platform: any
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## 简化版蛋白质二级结构分类器
 ### 使用方法
 - 首先通过pip进行安装：
 ```bash
-$ python3 -m pip install restraint-fold --upgrade
+$ python3 -m pip install restraint-fold --upgrade -i https://pypi.org/simple
 ```
 - 然后直接在命令行进行使用：
 ```bash
 $ python3 -m fold -h
 usage: __main__.py [-h] [-i I] [-o O] [--simplified SIMPLIFIED]
 
 optional arguments:
@@ -34,27 +22,19 @@
 ```bash
 $ python3 -m fold -i fold/pdb/case2-optimized.pdb -o case2-secondary.txt
 ```
 得到的结果如下所示：
 ```txt
 # case2-secondary.txt
 alpha:
-[  1   2   3   4   5   6   7   8   9  10  11  12  13  14  15  16  17  18
-  19  20  21  22  23  24  31  32  33  34  35  36  39  40  41  42  43  44
-  45  78  79  80  81  82  83  84  85  94  95  96  97  99 100 101 102 103
- 104 105 106 107 108]
+1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 31 32 33 34 35 36 37 39 40 41 42 43 44 45 46 78 79 80 81 82 83 84 85 86 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109
 beta:
-[ 23  24  25  26  27  28  46  47  48  49  50  51  52  53  54  55  56  57
-  58  59  60  61  62  63  64  65  66  67  68  69  70  71  72  73  74  75
-  76  86  87  88  89  90  91  92  93  94  95  96  97  98 117 118 119 120
- 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138
- 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156
- 157]
+23 24 25 26 27 28 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 86 87 88 89 90 91 92 93 94 95 96 97 98 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157
 ```
-- 执行一个生成简化版alpha和beta片段的命令：
+
 ```bash
 $ python3 -m fold -i fold/pdb/case2-optimized.pdb -o case2-secondary.txt --simplified 1
 ```
 得到的结果如下所示：
 ```txt
 # case2-secondary.txt
 alpha:
@@ -70,15 +50,15 @@
 46~76
 86~98
 117~157
 ```
 ### 提示
 如果输入的pdb文件中氢原子有缺失，需要先通过Xponge或者Hadder等工具进行补氢，然后再对结构进行解析：
 ```bash
-$ python3 -m pip install hadder --upgrade
+$ python3 -m pip install hadder --upgrade -i https://pypi.org/simple
 $ python3 -m hadder -h
 usage: __main__.py [-h] [-i I] [-o O]
 
 optional arguments:
   -h, --help  show this help message and exit
   -i I        Set the input pdb file path.
   -o O        Set the output pdb file path.
```

### Comparing `restraint-fold-0.1/fold/__init__.py` & `restraint-fold-0.1.1/fold/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         tmp_bond_4 = np.array([index, index + 3])
         if np.sum(np.isin(res_bonds, tmp_bond_1).sum(axis=-1) == 2) > 0:
             counter += 1
             continue
         elif np.sum(np.isin(res_bonds, tmp_bond_4).sum(axis=-1) == 2) > 0:
             counter += 1
             continue
-        elif counter > 0 and np.sum(np.isin(res_bonds, tmp_bond_2).sum(axis=-1) == 2) > 0:
+        elif counter > 2 and np.sum(np.isin(res_bonds, tmp_bond_2).sum(axis=-1) == 2) > 0:
             counter += 1
             continue
         # elif counter>0 and np.sum(np.isin(res_bonds, tmp_bond_3).sum(axis=-1)==2)>0:
         #     counter += 1
         #     continue
         elif counter < min_alpha:
             counter = 0
```

### Comparing `restraint-fold-0.1/fold/__main__.py` & `restraint-fold-0.1.1/fold/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,31 +22,31 @@
 
 import argparse
 from fold import get_alpha, get_beta, get_residue_type
 
 parser = argparse.ArgumentParser()
 parser.add_argument("-i", help="Set the input pdb file path.")
 parser.add_argument("-o", help="Set the output txt file path.")
-parser.add_argument("--simplified", help="Return the simplified information, default to be 0.", default=0)
+parser.add_argument("--simplified", help="Return the simplified information, default to be 0.", default='0')
 
 args = parser.parse_args()
 pdb_name = args.i
 save_txt_name = args.o
 use_simplified = args.simplified
 
 alphas = get_alpha(pdb_name, hbond_length=3.5)
 betas = get_beta(pdb_name, hbond_length=4.0)
 
 if use_simplified == '0':
     with open(save_txt_name, 'w') as file:
         file.write('alpha:\n')
-        file.write(str(alphas))
+        file.write(' '.join(list(map(str,alphas))))
         file.write('\n')
         file.write('beta:\n')
-        file.write(str(betas))
+        file.write(' '.join(list(map(str,betas))))
 else:
     with open(save_txt_name, 'w') as file:
         file.write('alpha:\n')
         for i in range(len(alphas)):
             if i == 0:
                 file.write(str(alphas[i]))
                 file.write('~')
```

### Comparing `restraint-fold-0.1/restraint_fold.egg-info/PKG-INFO` & `restraint-fold-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: restraint-fold
-Version: 0.1
+Version: 0.1.1
 Summary: Simple Protein Structure Parser
 Home-page: https://gitee.com/dechin/restraint-fold/
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## 简化版蛋白质二级结构分类器
 ### 使用方法
 - 首先通过pip进行安装：
 ```bash
-$ python3 -m pip install restraint-fold --upgrade
+$ python3 -m pip install restraint-fold --upgrade -i https://pypi.org/simple
 ```
 - 然后直接在命令行进行使用：
 ```bash
 $ python3 -m fold -h
 usage: __main__.py [-h] [-i I] [-o O] [--simplified SIMPLIFIED]
 
 optional arguments:
@@ -34,27 +34,19 @@
 ```bash
 $ python3 -m fold -i fold/pdb/case2-optimized.pdb -o case2-secondary.txt
 ```
 得到的结果如下所示：
 ```txt
 # case2-secondary.txt
 alpha:
-[  1   2   3   4   5   6   7   8   9  10  11  12  13  14  15  16  17  18
-  19  20  21  22  23  24  31  32  33  34  35  36  39  40  41  42  43  44
-  45  78  79  80  81  82  83  84  85  94  95  96  97  99 100 101 102 103
- 104 105 106 107 108]
+1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 31 32 33 34 35 36 37 39 40 41 42 43 44 45 46 78 79 80 81 82 83 84 85 86 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109
 beta:
-[ 23  24  25  26  27  28  46  47  48  49  50  51  52  53  54  55  56  57
-  58  59  60  61  62  63  64  65  66  67  68  69  70  71  72  73  74  75
-  76  86  87  88  89  90  91  92  93  94  95  96  97  98 117 118 119 120
- 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138
- 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156
- 157]
+23 24 25 26 27 28 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 86 87 88 89 90 91 92 93 94 95 96 97 98 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157
 ```
-- 执行一个生成简化版alpha和beta片段的命令：
+
 ```bash
 $ python3 -m fold -i fold/pdb/case2-optimized.pdb -o case2-secondary.txt --simplified 1
 ```
 得到的结果如下所示：
 ```txt
 # case2-secondary.txt
 alpha:
@@ -70,15 +62,15 @@
 46~76
 86~98
 117~157
 ```
 ### 提示
 如果输入的pdb文件中氢原子有缺失，需要先通过Xponge或者Hadder等工具进行补氢，然后再对结构进行解析：
 ```bash
-$ python3 -m pip install hadder --upgrade
+$ python3 -m pip install hadder --upgrade -i https://pypi.org/simple
 $ python3 -m hadder -h
 usage: __main__.py [-h] [-i I] [-o O]
 
 optional arguments:
   -h, --help  show this help message and exit
   -i I        Set the input pdb file path.
   -o O        Set the output pdb file path.
```

### Comparing `restraint-fold-0.1/setup.py` & `restraint-fold-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="restraint-fold",
-    version="0.1",
+    version="0.1.1",
     description="Simple Protein Structure Parser",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT License",
 
     url="https://gitee.com/dechin/restraint-fold/",
     author="Dechin CHEN",
     author_email="dechin.phy@gmail.com",
     packages=find_packages(exclude=["tests", "examples"]),
     install_requires=open('requirements.txt', 'r').readlines(),
     platforms="any",
     scripts=[],
     include_package_data=True
-)
+)
```

