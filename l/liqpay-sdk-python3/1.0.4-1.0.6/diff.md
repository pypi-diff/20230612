# Comparing `tmp/liqpay-sdk-python3-1.0.4.tar.gz` & `tmp/liqpay-sdk-python3-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liqpay-sdk-python3-1.0.4.tar", last modified: Mon Jun 12 15:49:15 2023, max compression
+gzip compressed data, was "liqpay-sdk-python3-1.0.6.tar", last modified: Mon Jun 12 16:23:19 2023, max compression
```

## Comparing `liqpay-sdk-python3-1.0.4.tar` & `liqpay-sdk-python3-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 15:49:15.424590 liqpay-sdk-python3-1.0.4/
--rw-rw-rw-   0        0        0     5561 2023-06-12 15:49:15.424590 liqpay-sdk-python3-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5368 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 15:49:15.414590 liqpay-sdk-python3-1.0.4/liqpay/
--rw-rw-rw-   0        0        0       24 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/liqpay/__init__.py
--rw-rw-rw-   0        0        0     6790 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/liqpay/liqpay3.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:49:15.416589 liqpay-sdk-python3-1.0.4/liqpay/tests/
--rw-rw-rw-   0        0        0        0 2023-06-12 10:46:25.000000 liqpay-sdk-python3-1.0.4/liqpay/tests/__init__.py
--rw-rw-rw-   0        0        0     1137 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/liqpay/tests/test_pay_simple.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:49:15.422590 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/
--rw-rw-rw-   0        0        0     5561 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 15:49:15.425593 liqpay-sdk-python3-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      493 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:23:19.148472 liqpay-sdk-python3-1.0.6/
+-rw-rw-rw-   0        0        0     5888 2023-06-12 16:23:19.147472 liqpay-sdk-python3-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5695 2023-06-12 16:22:30.000000 liqpay-sdk-python3-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 16:23:19.137476 liqpay-sdk-python3-1.0.6/liqpay/
+-rw-rw-rw-   0        0        0       24 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.6/liqpay/__init__.py
+-rw-rw-rw-   0        0        0     6790 2023-06-12 16:19:16.000000 liqpay-sdk-python3-1.0.6/liqpay/liqpay3.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:23:19.139468 liqpay-sdk-python3-1.0.6/liqpay/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-12 10:46:25.000000 liqpay-sdk-python3-1.0.6/liqpay/tests/__init__.py
+-rw-rw-rw-   0        0        0     1137 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.6/liqpay/tests/test_pay_simple.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:23:19.146475 liqpay-sdk-python3-1.0.6/liqpay_sdk_python3.egg-info/
+-rw-rw-rw-   0        0        0     5888 2023-06-12 16:23:19.000000 liqpay-sdk-python3-1.0.6/liqpay_sdk_python3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-12 16:23:19.000000 liqpay-sdk-python3-1.0.6/liqpay_sdk_python3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:23:19.000000 liqpay-sdk-python3-1.0.6/liqpay_sdk_python3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 16:23:19.000000 liqpay-sdk-python3-1.0.6/liqpay_sdk_python3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 16:23:19.000000 liqpay-sdk-python3-1.0.6/liqpay_sdk_python3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 16:23:19.148472 liqpay-sdk-python3-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      493 2023-06-12 16:19:16.000000 liqpay-sdk-python3-1.0.6/setup.py
```

### Comparing `liqpay-sdk-python3-1.0.4/PKG-INFO` & `liqpay-sdk-python3-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: liqpay-sdk-python3
-Version: 1.0.4
+Version: 1.0.6
 Summary: LiqPay Python3 SDK
 Home-page: https://github.com/aorzh/liqpay-sdk-python3
 Description-Content-Type: text/markdown
 
 [![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 
 [![SDK-Python3](https://www.liqpay.ua/logo_liqpay_main.svg)](https://www.liqpay.ua/documentation/api/home)
 
-* Version: 1.0.3
 * Web: https://www.liqpay.ua/
 * Download: https://pypi.org/project/liqpay-sdk-python3/
 * Source: https://github.com/aorzh/liqpay-sdk-python3
 * Documentation: https://www.liqpay.ua/documentation/en/
 * Keywords: liqpay, privat24, privatbank, python, internet acquiring, P2P payments, two-step payments
 
 
@@ -33,15 +32,15 @@
 From pip
 ```pip install liqpay-sdk-python3```
 
 Working with LiqPay Callback locally
 ============
 If you need debugging API Callback on local environment use https://localtunnel.github.io/www/
 
-How it use?
+How it uses?
 ============
 
 Example 1: Basic
 -------
 
 **Backend**
 Get payment button (html response)
@@ -80,21 +79,20 @@
 
 
 **Frontend**
 
 Variable ``html`` will contain next html form
 
 ```
-    <form method="POST" action="https://www.liqpay.ua/api/3/checkout" accept-charset="utf-8">
-        <input type="hidden" name="data" value="eyAidmVyc2lvbiIgOiAzLCAicHVibGljX2tleSIgOiAieW91cl9wdWJsaWNfa2V5IiwgImFjdGlv
-        biIgOiAicGF5IiwgImFtb3VudCIgOiAxLCAiY3VycmVuY3kiIDogIlVTRCIsICJkZXNjcmlwdGlv
-        biIgOiAiZGVzY3JpcHRpb24gdGV4dCIsICJvcmRlcl9pZCIgOiAib3JkZXJfaWRfMSIgfQ=="/>
-        <input type="hidden" name="signature" value="QvJD5u9Fg55PCx/Hdz6lzWtYwcI="/>
-        <input type="image"
-        src="//static.liqpay.ua/buttons/p1ru.radius.png"/>
+    <form method="POST" action="https://www.liqpay.ua/api/3/checkout/" accept-charset="utf-8">
+         <input type='hidden' name='data' value='eyJhbW91bnQiOi...='/>
+         <input type='hidden' name='signature' value='edUs4...='/>
+         <button style="border: none !important;display:inline-block !important;text-align: center !important; padding: 7px 20px !important; color: #fff !important;font-size:16px !important; font-weight: 600 !important; font-family:OpenSans, sans-serif;cursor: pointer !important;border-radius: 2px !important;background: rgba(122,183,43,1) !important;"onmouseover="this.style.opacity=0.5;" onmouseout="this.style.opacity=1;"> <img src="https://static.liqpay.ua/buttons/logo-small.png" name="btn_text" style="margin-right: 7px !important; vertical-align: middle !important;"/> 
+         <span style="vertical-align:middle;!important">PAY 100 UAH</span>
+         </button>
     </form>
 ```
 
 Example 2: Integrate Payment widget to Django
 -------
 `Payment widget documentation` 
 https://www.liqpay.ua/documentation/en/api/aquiring/widget/
```

### Comparing `liqpay-sdk-python3-1.0.4/README.md` & `liqpay-sdk-python3-1.0.6/liqpay_sdk_python3.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,336 +1,368 @@
-00000000: 5b21 5b50 7974 686f 6e20 332e 362b 5d28  [![Python 3.6+](
-00000010: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000020: 6c64 732e 696f 2f62 6164 6765 2f70 7974  lds.io/badge/pyt
-00000030: 686f 6e2d 332e 362b 2d62 6c75 652e 7376  hon-3.6+-blue.sv
-00000040: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
-00000050: 7079 7468 6f6e 2e6f 7267 2f64 6f77 6e6c  python.org/downl
-00000060: 6f61 6473 2f72 656c 6561 7365 2f70 7974  oads/release/pyt
-00000070: 686f 6e2d 3336 302f 290d 0a0d 0a5b 215b  hon-360/)....[![
-00000080: 5344 4b2d 5079 7468 6f6e 335d 2868 7474  SDK-Python3](htt
-00000090: 7073 3a2f 2f77 7777 2e6c 6971 7061 792e  ps://www.liqpay.
-000000a0: 7561 2f6c 6f67 6f5f 6c69 7170 6179 5f6d  ua/logo_liqpay_m
-000000b0: 6169 6e2e 7376 6729 5d28 6874 7470 733a  ain.svg)](https:
-000000c0: 2f2f 7777 772e 6c69 7170 6179 2e75 612f  //www.liqpay.ua/
-000000d0: 646f 6375 6d65 6e74 6174 696f 6e2f 6170  documentation/ap
-000000e0: 692f 686f 6d65 290d 0a0d 0a2a 2056 6572  i/home)....* Ver
-000000f0: 7369 6f6e 3a20 312e 302e 330d 0a2a 2057  sion: 1.0.3..* W
-00000100: 6562 3a20 6874 7470 733a 2f2f 7777 772e  eb: https://www.
-00000110: 6c69 7170 6179 2e75 612f 0d0a 2a20 446f  liqpay.ua/..* Do
-00000120: 776e 6c6f 6164 3a20 6874 7470 733a 2f2f  wnload: https://
-00000130: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000140: 2f6c 6971 7061 792d 7364 6b2d 7079 7468  /liqpay-sdk-pyth
-00000150: 6f6e 332f 0d0a 2a20 536f 7572 6365 3a20  on3/..* Source: 
-00000160: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000170: 6f6d 2f61 6f72 7a68 2f6c 6971 7061 792d  om/aorzh/liqpay-
-00000180: 7364 6b2d 7079 7468 6f6e 330d 0a2a 2044  sdk-python3..* D
-00000190: 6f63 756d 656e 7461 7469 6f6e 3a20 6874  ocumentation: ht
-000001a0: 7470 733a 2f2f 7777 772e 6c69 7170 6179  tps://www.liqpay
-000001b0: 2e75 612f 646f 6375 6d65 6e74 6174 696f  .ua/documentatio
-000001c0: 6e2f 656e 2f0d 0a2a 204b 6579 776f 7264  n/en/..* Keyword
-000001d0: 733a 206c 6971 7061 792c 2070 7269 7661  s: liqpay, priva
-000001e0: 7432 342c 2070 7269 7661 7462 616e 6b2c  t24, privatbank,
-000001f0: 2070 7974 686f 6e2c 2069 6e74 6572 6e65   python, interne
-00000200: 7420 6163 7175 6972 696e 672c 2050 3250  t acquiring, P2P
-00000210: 2070 6179 6d65 6e74 732c 2074 776f 2d73   payments, two-s
-00000220: 7465 7020 7061 796d 656e 7473 0d0a 0d0a  tep payments....
-00000230: 0d0a 5768 6174 2070 7974 686f 6e20 7665  ..What python ve
-00000240: 7273 696f 6e20 6973 2073 7570 706f 7274  rsion is support
-00000250: 6564 3f0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  ed?..===========
-00000260: 3d0d 0a2d 2050 7974 686f 6e20 332e 342b  =..- Python 3.4+
-00000270: 0d0a 0d0a 4765 7420 5374 6172 7465 640d  ....Get Started.
-00000280: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a31  .============..1
-00000290: 2e20 5369 676e 2075 7020 696e 2068 7474  . Sign up in htt
-000002a0: 7073 3a2f 2f77 7777 2e6c 6971 7061 792e  ps://www.liqpay.
-000002b0: 7561 2f65 6e2f 6175 7468 6f72 697a 6174  ua/en/authorizat
-000002c0: 696f 6e2e 0d0a 322e 2043 7265 6174 6520  ion...2. Create 
-000002d0: 6120 636f 6d70 616e 792e 0d0a 332e 2049  a company...3. I
-000002e0: 6e20 636f 6d70 616e 7920 7365 7474 696e  n company settin
-000002f0: 6773 2c20 6f6e 2041 5049 2074 6162 2c20  gs, on API tab, 
-00000300: 6765 7420 2a2a 5075 626c 6963 206b 6579  get **Public key
-00000310: 2a2a 2061 6e64 202a 2a50 7269 7661 7465  ** and **Private
-00000320: 206b 6579 2a2a 2e0d 0a34 2e20 446f 6e65   key**...4. Done
-00000330: 2e0d 0a0d 0a49 6e73 7461 6c6c 6174 696f  .....Installatio
-00000340: 6e0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  n..============.
-00000350: 0a46 726f 6d20 7069 700d 0a60 6060 7069  .From pip..```pi
-00000360: 7020 696e 7374 616c 6c20 6c69 7170 6179  p install liqpay
-00000370: 2d73 646b 2d70 7974 686f 6e33 6060 600d  -sdk-python3```.
-00000380: 0a0d 0a57 6f72 6b69 6e67 2077 6974 6820  ...Working with 
-00000390: 4c69 7150 6179 2043 616c 6c62 6163 6b20  LiqPay Callback 
-000003a0: 6c6f 6361 6c6c 790d 0a3d 3d3d 3d3d 3d3d  locally..=======
-000003b0: 3d3d 3d3d 3d0d 0a49 6620 796f 7520 6e65  =====..If you ne
-000003c0: 6564 2064 6562 7567 6769 6e67 2041 5049  ed debugging API
-000003d0: 2043 616c 6c62 6163 6b20 6f6e 206c 6f63   Callback on loc
-000003e0: 616c 2065 6e76 6972 6f6e 6d65 6e74 2075  al environment u
-000003f0: 7365 2068 7474 7073 3a2f 2f6c 6f63 616c  se https://local
-00000400: 7475 6e6e 656c 2e67 6974 6875 622e 696f  tunnel.github.io
-00000410: 2f77 7777 2f0d 0a0d 0a48 6f77 2069 7420  /www/....How it 
-00000420: 7573 653f 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d  use?..==========
-00000430: 3d3d 0d0a 0d0a 4578 616d 706c 6520 313a  ==....Example 1:
-00000440: 2042 6173 6963 0d0a 2d2d 2d2d 2d2d 2d0d   Basic..-------.
-00000450: 0a0d 0a2a 2a42 6163 6b65 6e64 2a2a 0d0a  ...**Backend**..
-00000460: 4765 7420 7061 796d 656e 7420 6275 7474  Get payment butt
-00000470: 6f6e 2028 6874 6d6c 2072 6573 706f 6e73  on (html respons
-00000480: 6529 0d0a 6060 600d 0a6c 6971 7061 7920  e)..```..liqpay 
-00000490: 3d20 4c69 7150 6179 2870 7562 6c69 635f  = LiqPay(public_
-000004a0: 6b65 792c 2070 7269 7661 7465 5f6b 6579  key, private_key
-000004b0: 290d 0a68 746d 6c20 3d20 6c69 7170 6179  )..html = liqpay
-000004c0: 2e63 6e62 5f66 6f72 6d28 7b0d 0a20 2020  .cnb_form({..   
-000004d0: 2027 6163 7469 6f6e 273a 2027 7061 7927   'action': 'pay'
-000004e0: 2c0d 0a20 2020 2027 616d 6f75 6e74 273a  ,..    'amount':
-000004f0: 2027 3127 2c0d 0a20 2020 2027 6375 7272   '1',..    'curr
-00000500: 656e 6379 273a 2027 5553 4427 2c0d 0a20  ency': 'USD',.. 
-00000510: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
-00000520: 3a20 2764 6573 6372 6970 7469 6f6e 2074  : 'description t
-00000530: 6578 7427 2c0d 0a20 2020 2027 6f72 6465  ext',..    'orde
-00000540: 725f 6964 273a 2027 6f72 6465 725f 6964  r_id': 'order_id
-00000550: 5f31 272c 0d0a 2020 2020 2776 6572 7369  _1',..    'versi
-00000560: 6f6e 273a 2027 3327 2c0d 0a20 2020 2027  on': '3',..    '
-00000570: 6c61 6e67 7561 6765 273a 2027 7275 7c75  language': 'ru|u
-00000580: 6b7c 656e 270d 0a7d 290d 0a60 6060 0d0a  k|en'..})..```..
-00000590: 0d0a 4765 7420 706c 6169 6e20 6368 6563  ..Get plain chec
-000005a0: 6b6f 7574 2075 726c 3a0d 0a0d 0a60 6060  kout url:....```
-000005b0: 0d0a 6c69 7170 6179 203d 204c 6971 5061  ..liqpay = LiqPa
-000005c0: 7928 7075 626c 6963 5f6b 6579 2c20 7072  y(public_key, pr
-000005d0: 6976 6174 655f 6b65 7929 0d0a 6874 6d6c  ivate_key)..html
-000005e0: 203d 206c 6971 7061 792e 6368 6563 6b6f   = liqpay.checko
-000005f0: 7574 5f75 726c 287b 0d0a 2020 2020 2761  ut_url({..    'a
-00000600: 6374 696f 6e27 3a20 2761 7574 6827 2c0d  ction': 'auth',.
-00000610: 0a20 2020 2027 616d 6f75 6e74 273a 2027  .    'amount': '
-00000620: 3127 2c0d 0a20 2020 2027 6375 7272 656e  1',..    'curren
-00000630: 6379 273a 2027 5553 4427 2c0d 0a20 2020  cy': 'USD',..   
-00000640: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
-00000650: 2764 6573 6372 6970 7469 6f6e 2074 6578  'description tex
-00000660: 7427 2c0d 0a20 2020 2027 6f72 6465 725f  t',..    'order_
-00000670: 6964 273a 2027 6f72 6465 725f 6964 5f31  id': 'order_id_1
-00000680: 272c 0d0a 2020 2020 2776 6572 7369 6f6e  ',..    'version
-00000690: 273a 2027 3327 2c0d 0a20 2020 2027 6c61  ': '3',..    'la
-000006a0: 6e67 7561 6765 273a 2027 7275 7c75 6b7c  nguage': 'ru|uk|
-000006b0: 656e 272c 0d0a 2020 2020 2772 6563 7572  en',..    'recur
-000006c0: 7269 6e67 6279 746f 6b65 6e27 3a20 2731  ringbytoken': '1
-000006d0: 270d 0a7d 290d 0a23 2052 6573 706f 6e73  '..})..# Respons
-000006e0: 653a 0d0a 0d0a 7374 723a 2068 7474 7073  e:....str: https
-000006f0: 3a2f 2f77 7777 2e6c 6971 7061 792e 7561  ://www.liqpay.ua
-00000700: 2f61 7069 2f33 2f63 6865 636b 6f75 742f  /api/3/checkout/
-00000710: 3f64 6174 613d 3c64 6563 6f64 6564 2064  ?data=<decoded d
-00000720: 6174 613e 2673 6967 6e61 7475 7265 3d3c  ata>&signature=<
-00000730: 6465 636f 6465 6420 7369 676e 6174 7572  decoded signatur
-00000740: 653e 0d0a 0d0a 6060 600d 0a0d 0a0d 0a2a  e>....```......*
-00000750: 2a46 726f 6e74 656e 642a 2a0d 0a0d 0a56  *Frontend**....V
-00000760: 6172 6961 626c 6520 6060 6874 6d6c 6060  ariable ``html``
-00000770: 2077 696c 6c20 636f 6e74 6169 6e20 6e65   will contain ne
-00000780: 7874 2068 746d 6c20 666f 726d 0d0a 0d0a  xt html form....
-00000790: 6060 600d 0a20 2020 203c 666f 726d 206d  ```..    <form m
-000007a0: 6574 686f 643d 2250 4f53 5422 2061 6374  ethod="POST" act
-000007b0: 696f 6e3d 2268 7474 7073 3a2f 2f77 7777  ion="https://www
-000007c0: 2e6c 6971 7061 792e 7561 2f61 7069 2f33  .liqpay.ua/api/3
-000007d0: 2f63 6865 636b 6f75 7422 2061 6363 6570  /checkout" accep
-000007e0: 742d 6368 6172 7365 743d 2275 7466 2d38  t-charset="utf-8
-000007f0: 223e 0d0a 2020 2020 2020 2020 3c69 6e70  ">..        <inp
-00000800: 7574 2074 7970 653d 2268 6964 6465 6e22  ut type="hidden"
-00000810: 206e 616d 653d 2264 6174 6122 2076 616c   name="data" val
-00000820: 7565 3d22 6579 4169 646d 5679 6332 6c76  ue="eyAidmVyc2lv
-00000830: 6269 4967 4f69 417a 4c43 4169 6348 5669  biIgOiAzLCAicHVi
-00000840: 6247 6c6a 5832 746c 6553 4967 4f69 4169  bGljX2tleSIgOiAi
-00000850: 6557 3931 636c 3977 6457 4a73 6157 4e66  eW91cl9wdWJsaWNf
-00000860: 6132 5635 4969 7767 496d 466a 6447 6c76  a2V5IiwgImFjdGlv
-00000870: 0d0a 2020 2020 2020 2020 6269 4967 4f69  ..        biIgOi
-00000880: 4169 6347 4635 4969 7767 496d 4674 6233  AicGF5IiwgImFtb3
-00000890: 5675 6443 4967 4f69 4178 4c43 4169 5933  VudCIgOiAxLCAiY3
-000008a0: 5679 636d 5675 5933 6b69 4944 6f67 496c  VycmVuY3kiIDogIl
-000008b0: 5654 5243 4973 4943 4a6b 5a58 4e6a 636d  VTRCIsICJkZXNjcm
-000008c0: 6c77 6447 6c76 0d0a 2020 2020 2020 2020  lwdGlv..        
-000008d0: 6269 4967 4f69 4169 5a47 567a 5933 4a70  biIgOiAiZGVzY3Jp
-000008e0: 6348 5270 6232 3467 6447 5634 6443 4973  cHRpb24gdGV4dCIs
-000008f0: 4943 4a76 636d 526c 636c 3970 5a43 4967  ICJvcmRlcl9pZCIg
-00000900: 4f69 4169 6233 4a6b 5a58 4a66 6157 5266  OiAib3JkZXJfaWRf
-00000910: 4d53 4967 6651 3d3d 222f 3e0d 0a20 2020  MSIgfQ=="/>..   
-00000920: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
-00000930: 3d22 6869 6464 656e 2220 6e61 6d65 3d22  ="hidden" name="
-00000940: 7369 676e 6174 7572 6522 2076 616c 7565  signature" value
-00000950: 3d22 5176 4a44 3575 3946 6735 3550 4378  ="QvJD5u9Fg55PCx
-00000960: 2f48 647a 366c 7a57 7459 7763 493d 222f  /Hdz6lzWtYwcI="/
-00000970: 3e0d 0a20 2020 2020 2020 203c 696e 7075  >..        <inpu
-00000980: 7420 7479 7065 3d22 696d 6167 6522 0d0a  t type="image"..
-00000990: 2020 2020 2020 2020 7372 633d 222f 2f73          src="//s
-000009a0: 7461 7469 632e 6c69 7170 6179 2e75 612f  tatic.liqpay.ua/
-000009b0: 6275 7474 6f6e 732f 7031 7275 2e72 6164  buttons/p1ru.rad
-000009c0: 6975 732e 706e 6722 2f3e 0d0a 2020 2020  ius.png"/>..    
-000009d0: 3c2f 666f 726d 3e0d 0a60 6060 0d0a 0d0a  </form>..```....
-000009e0: 4578 616d 706c 6520 323a 2049 6e74 6567  Example 2: Integ
-000009f0: 7261 7465 2050 6179 6d65 6e74 2077 6964  rate Payment wid
-00000a00: 6765 7420 746f 2044 6a61 6e67 6f0d 0a2d  get to Django..-
-00000a10: 2d2d 2d2d 2d2d 0d0a 6050 6179 6d65 6e74  ------..`Payment
-00000a20: 2077 6964 6765 7420 646f 6375 6d65 6e74   widget document
-00000a30: 6174 696f 6e60 200d 0a68 7474 7073 3a2f  ation` ..https:/
-00000a40: 2f77 7777 2e6c 6971 7061 792e 7561 2f64  /www.liqpay.ua/d
-00000a50: 6f63 756d 656e 7461 7469 6f6e 2f65 6e2f  ocumentation/en/
-00000a60: 6170 692f 6171 7569 7269 6e67 2f77 6964  api/aquiring/wid
-00000a70: 6765 742f 0d0a 0d0a 2a42 6163 6b65 6e64  get/....*Backend
-00000a80: 2a0d 0a0d 0a60 7669 6577 732e 7079 600d  *....`views.py`.
-00000a90: 0a0d 0a60 6060 0d0a 0d0a 2020 2020 6672  ...```....    fr
-00000aa0: 6f6d 206c 6971 7061 7920 696d 706f 7274  om liqpay import
-00000ab0: 204c 6971 5061 790d 0a0d 0a20 2020 2066   LiqPay....    f
-00000ac0: 726f 6d20 646a 616e 676f 2e76 6965 7773  rom django.views
-00000ad0: 2e67 656e 6572 6963 2069 6d70 6f72 7420  .generic import 
-00000ae0: 5465 6d70 6c61 7465 5669 6577 0d0a 2020  TemplateView..  
-00000af0: 2020 6672 6f6d 2064 6a61 6e67 6f2e 7368    from django.sh
-00000b00: 6f72 7463 7574 7320 696d 706f 7274 2072  ortcuts import r
-00000b10: 656e 6465 720d 0a20 2020 2066 726f 6d20  ender..    from 
-00000b20: 646a 616e 676f 2e68 7474 7020 696d 706f  django.http impo
-00000b30: 7274 2048 7474 7052 6573 706f 6e73 650d  rt HttpResponse.
-00000b40: 0a0d 0a20 2020 2063 6c61 7373 2050 6179  ...    class Pay
-00000b50: 5669 6577 2854 656d 706c 6174 6556 6965  View(TemplateVie
-00000b60: 7729 3a0d 0a20 2020 2074 656d 706c 6174  w):..    templat
-00000b70: 655f 6e61 6d65 203d 2027 6269 6c6c 696e  e_name = 'billin
-00000b80: 672f 7061 792e 6874 6d6c 270d 0a0d 0a20  g/pay.html'.... 
-00000b90: 2020 2064 6566 2067 6574 2873 656c 662c     def get(self,
-00000ba0: 2072 6571 7565 7374 2c20 2a61 7267 732c   request, *args,
-00000bb0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00000bc0: 2020 2020 206c 6971 7061 7920 3d20 4c69       liqpay = Li
-00000bd0: 7150 6179 2873 6574 7469 6e67 732e 4c49  qPay(settings.LI
-00000be0: 5150 4159 5f50 5542 4c49 435f 4b45 592c  QPAY_PUBLIC_KEY,
-00000bf0: 2073 6574 7469 6e67 732e 4c49 5150 4159   settings.LIQPAY
-00000c00: 5f50 5249 5641 5445 5f4b 4559 290d 0a20  _PRIVATE_KEY).. 
-00000c10: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
-00000c20: 7b0d 0a20 2020 2020 2020 2020 2020 2027  {..            '
-00000c30: 6163 7469 6f6e 273a 2027 7061 7927 2c0d  action': 'pay',.
-00000c40: 0a20 2020 2020 2020 2020 2020 2027 616d  .            'am
-00000c50: 6f75 6e74 273a 2027 3130 3027 2c0d 0a20  ount': '100',.. 
-00000c60: 2020 2020 2020 2020 2020 2027 6375 7272             'curr
-00000c70: 656e 6379 273a 2027 5553 4427 2c0d 0a20  ency': 'USD',.. 
-00000c80: 2020 2020 2020 2020 2020 2027 6465 7363             'desc
-00000c90: 7269 7074 696f 6e27 3a20 2750 6179 6d65  ription': 'Payme
-00000ca0: 6e74 2066 6f72 2063 6c6f 7468 6573 272c  nt for clothes',
-00000cb0: 0d0a 2020 2020 2020 2020 2020 2020 276f  ..            'o
-00000cc0: 7264 6572 5f69 6427 3a20 276f 7264 6572  rder_id': 'order
-00000cd0: 5f69 645f 3127 2c0d 0a20 2020 2020 2020  _id_1',..       
-00000ce0: 2020 2020 2027 7665 7273 696f 6e27 3a20       'version': 
-00000cf0: 2733 272c 0d0a 2020 2020 2020 2020 2020  '3',..          
-00000d00: 2020 2773 616e 6462 6f78 273a 2030 2c20    'sandbox': 0, 
-00000d10: 2320 7361 6e64 626f 7820 6d6f 6465 2c20  # sandbox mode, 
-00000d20: 7365 7420 746f 2031 2074 6f20 656e 6162  set to 1 to enab
-00000d30: 6c65 2069 740d 0a20 2020 2020 2020 2020  le it..         
-00000d40: 2020 2027 7365 7276 6572 5f75 726c 273a     'server_url':
-00000d50: 2027 6874 7470 733a 2f2f 7465 7374 2e63   'https://test.c
-00000d60: 6f6d 2f62 696c 6c69 6e67 2f70 6179 2d63  om/billing/pay-c
-00000d70: 616c 6c62 6163 6b2f 272c 2023 2075 726c  allback/', # url
-00000d80: 2074 6f20 6361 6c6c 6261 636b 2076 6965   to callback vie
-00000d90: 770d 0a20 2020 2020 2020 207d 0d0a 2020  w..        }..  
-00000da0: 2020 2020 2020 7369 676e 6174 7572 6520        signature 
-00000db0: 3d20 6c69 7170 6179 2e63 6e62 5f73 6967  = liqpay.cnb_sig
-00000dc0: 6e61 7475 7265 2870 6172 616d 7329 0d0a  nature(params)..
-00000dd0: 2020 2020 2020 2020 6461 7461 203d 206c          data = l
-00000de0: 6971 7061 792e 636e 625f 6461 7461 2870  iqpay.cnb_data(p
-00000df0: 6172 616d 7329 0d0a 2020 2020 2020 2020  arams)..        
-00000e00: 7265 7475 726e 2072 656e 6465 7228 7265  return render(re
-00000e10: 7175 6573 742c 2073 656c 662e 7465 6d70  quest, self.temp
-00000e20: 6c61 7465 5f6e 616d 652c 207b 2773 6967  late_name, {'sig
-00000e30: 6e61 7475 7265 273a 2073 6967 6e61 7475  nature': signatu
-00000e40: 7265 2c20 2764 6174 6127 3a20 6461 7461  re, 'data': data
-00000e50: 7d29 0d0a 0d0a 2020 2020 406d 6574 686f  })....    @metho
-00000e60: 645f 6465 636f 7261 746f 7228 6373 7266  d_decorator(csrf
-00000e70: 5f65 7865 6d70 742c 206e 616d 653d 2764  _exempt, name='d
-00000e80: 6973 7061 7463 6827 290d 0a20 2020 2063  ispatch')..    c
-00000e90: 6c61 7373 2050 6179 4361 6c6c 6261 636b  lass PayCallback
-00000ea0: 5669 6577 2856 6965 7729 3a0d 0a20 2020  View(View):..   
-00000eb0: 2020 2020 2064 6566 2070 6f73 7428 7365       def post(se
-00000ec0: 6c66 2c20 7265 7175 6573 742c 202a 6172  lf, request, *ar
-00000ed0: 6773 2c20 2a2a 6b77 6172 6773 293a 0d0a  gs, **kwargs):..
-00000ee0: 2020 2020 2020 2020 2020 2020 6c69 7170              liqp
-00000ef0: 6179 203d 204c 6971 5061 7928 7365 7474  ay = LiqPay(sett
-00000f00: 696e 6773 2e4c 4951 5041 595f 5055 424c  ings.LIQPAY_PUBL
-00000f10: 4943 5f4b 4559 2c20 7365 7474 696e 6773  IC_KEY, settings
-00000f20: 2e4c 4951 5041 595f 5052 4956 4154 455f  .LIQPAY_PRIVATE_
-00000f30: 4b45 5929 0d0a 2020 2020 2020 2020 2020  KEY)..          
-00000f40: 2020 6461 7461 203d 2072 6571 7565 7374    data = request
-00000f50: 2e50 4f53 542e 6765 7428 2764 6174 6127  .POST.get('data'
-00000f60: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00000f70: 6967 6e61 7475 7265 203d 2072 6571 7565  ignature = reque
-00000f80: 7374 2e50 4f53 542e 6765 7428 2773 6967  st.POST.get('sig
-00000f90: 6e61 7475 7265 2729 0d0a 2020 2020 2020  nature')..      
-00000fa0: 2020 2020 2020 7369 676e 203d 206c 6971        sign = liq
-00000fb0: 7061 792e 7374 725f 746f 5f73 6967 6e28  pay.str_to_sign(
-00000fc0: 7365 7474 696e 6773 2e4c 4951 5041 595f  settings.LIQPAY_
-00000fd0: 5052 4956 4154 455f 4b45 5920 2b20 6461  PRIVATE_KEY + da
-00000fe0: 7461 202b 2073 6574 7469 6e67 732e 4c49  ta + settings.LI
-00000ff0: 5150 4159 5f50 5249 5641 5445 5f4b 4559  QPAY_PRIVATE_KEY
-00001000: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00001010: 6620 7369 676e 203d 3d20 7369 676e 6174  f sign == signat
-00001020: 7572 653a 0d0a 2020 2020 2020 2020 2020  ure:..          
-00001030: 2020 2020 2020 7072 696e 7428 2763 616c        print('cal
-00001040: 6c62 6163 6b20 6973 2076 616c 6964 2729  lback is valid')
-00001050: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00001060: 7370 6f6e 7365 203d 206c 6971 7061 792e  sponse = liqpay.
-00001070: 6465 636f 6465 5f64 6174 615f 6672 6f6d  decode_data_from
-00001080: 5f73 7472 2864 6174 6129 0d0a 2020 2020  _str(data)..    
-00001090: 2020 2020 2020 2020 7072 696e 7428 2763          print('c
-000010a0: 616c 6c62 6163 6b20 6461 7461 272c 2072  allback data', r
-000010b0: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
-000010c0: 2020 2020 2020 7265 7475 726e 2048 7474        return Htt
-000010d0: 7052 6573 706f 6e73 6528 290d 0a60 6060  pResponse()..```
-000010e0: 0d0a 6075 726c 732e 7079 600d 0a0d 0a60  ..`urls.py`....`
-000010f0: 6060 0d0a 0d0a 2020 2020 6672 6f6d 2064  ``....    from d
-00001100: 6a61 6e67 6f2e 636f 6e66 2e75 726c 7320  jango.conf.urls 
-00001110: 696d 706f 7274 2075 726c 0d0a 0d0a 2020  import url....  
-00001120: 2020 6672 6f6d 2062 696c 6c69 6e67 2e76    from billing.v
-00001130: 6965 7773 2069 6d70 6f72 7420 5061 7956  iews import PayV
-00001140: 6965 772c 2050 6179 4361 6c6c 6261 636b  iew, PayCallback
-00001150: 5669 6577 0d0a 0d0a 0d0a 2020 2020 7572  View......    ur
-00001160: 6c70 6174 7465 726e 7320 3d20 5b0d 0a20  lpatterns = [.. 
-00001170: 2020 2020 2020 2075 726c 2872 275e 7061         url(r'^pa
-00001180: 792f 2427 2c20 5061 7956 6965 772e 6173  y/$', PayView.as
-00001190: 5f76 6965 7728 292c 206e 616d 653d 2770  _view(), name='p
-000011a0: 6179 5f76 6965 7727 292c 0d0a 2020 2020  ay_view'),..    
-000011b0: 2020 2020 7572 6c28 7227 5e70 6179 2d63      url(r'^pay-c
-000011c0: 616c 6c62 6163 6b2f 2427 2c20 5061 7943  allback/$', PayC
-000011d0: 616c 6c62 6163 6b56 6965 772e 6173 5f76  allbackView.as_v
-000011e0: 6965 7728 292c 206e 616d 653d 2770 6179  iew(), name='pay
-000011f0: 5f63 616c 6c62 6163 6b27 292c 0d0a 2020  _callback'),..  
-00001200: 2020 5d0d 0a60 6060 0d0a 2a46 726f 6e74    ]..```..*Front
-00001210: 656e 642a 0d0a 0d0a 6060 600d 0a0d 0a20  end*....```.... 
-00001220: 2020 203c 6469 7620 6964 3d22 6c69 7170     <div id="liqp
-00001230: 6179 5f63 6865 636b 6f75 7422 3e3c 2f64  ay_checkout"></d
-00001240: 6976 3e0d 0a20 2020 203c 7363 7269 7074  iv>..    <script
-00001250: 3e0d 0a20 2020 2020 2020 2077 696e 646f  >..        windo
-00001260: 772e 4c69 7150 6179 4368 6563 6b6f 7574  w.LiqPayCheckout
-00001270: 4361 6c6c 6261 636b 203d 2066 756e 6374  Callback = funct
-00001280: 696f 6e28 2920 7b0d 0a20 2020 2020 2020  ion() {..       
-00001290: 2020 2020 204c 6971 5061 7943 6865 636b       LiqPayCheck
-000012a0: 6f75 742e 696e 6974 287b 0d0a 2020 2020  out.init({..    
-000012b0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000012c0: 3a20 227b 7b20 6461 7461 207d 7d22 2c0d  : "{{ data }}",.
-000012d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000012e0: 2073 6967 6e61 7475 7265 3a20 227b 7b20   signature: "{{ 
-000012f0: 7369 676e 6174 7572 6520 7d7d 222c 0d0a  signature }}",..
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 656d 6265 6454 6f3a 2022 236c 6971 7061  embedTo: "#liqpa
-00001320: 795f 6368 6563 6b6f 7574 222c 0d0a 2020  y_checkout",..  
-00001330: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-00001340: 6465 3a20 2265 6d62 6564 2220 2f2f 2065  de: "embed" // e
-00001350: 6d62 6564 207c 7c20 706f 7075 702c 0d0a  mbed || popup,..
-00001360: 2020 2020 2020 2020 2020 2020 7d29 2e6f              }).o
-00001370: 6e28 226c 6971 7061 792e 6361 6c6c 6261  n("liqpay.callba
-00001380: 636b 222c 2066 756e 6374 696f 6e28 6461  ck", function(da
-00001390: 7461 297b 0d0a 2020 2020 2020 2020 2020  ta){..          
-000013a0: 2020 2020 2020 636f 6e73 6f6c 652e 6c6f        console.lo
-000013b0: 6728 6461 7461 2e73 7461 7475 7329 3b0d  g(data.status);.
-000013c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013d0: 2063 6f6e 736f 6c65 2e6c 6f67 2864 6174   console.log(dat
-000013e0: 6129 3b0d 0a20 2020 2020 2020 2020 2020  a);..           
-000013f0: 207d 292e 6f6e 2822 6c69 7170 6179 2e72   }).on("liqpay.r
-00001400: 6561 6479 222c 2066 756e 6374 696f 6e28  eady", function(
-00001410: 6461 7461 297b 0d0a 2020 2020 2020 2020  data){..        
-00001420: 2020 2020 2020 2020 2f2f 2072 6561 6479          // ready
-00001430: 0d0a 2020 2020 2020 2020 2020 2020 7d29  ..            })
-00001440: 2e6f 6e28 226c 6971 7061 792e 636c 6f73  .on("liqpay.clos
-00001450: 6522 2c20 6675 6e63 7469 6f6e 2864 6174  e", function(dat
-00001460: 6129 7b0d 0a20 2020 2020 2020 2020 2020  a){..           
-00001470: 2020 2020 202f 2f20 636c 6f73 650d 0a20       // close.. 
-00001480: 2020 2020 2020 2020 2020 207d 293b 0d0a             });..
-00001490: 2020 2020 2020 2020 7d3b 0d0a 2020 2020          };..    
-000014a0: 3c2f 7363 7269 7074 3e0d 0a20 2020 203c  </script>..    <
-000014b0: 7363 7269 7074 2073 7263 3d22 2f2f 7374  script src="//st
-000014c0: 6174 6963 2e6c 6971 7061 792e 7561 2f6c  atic.liqpay.ua/l
-000014d0: 6962 6a73 2f63 6865 636b 6f75 742e 6a73  ibjs/checkout.js
-000014e0: 2220 6173 796e 633e 3c2f 7363 7269 7074  " async></script
-000014f0: 3e0d 0a60 6060 0d0a                      >..```..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 206c 6971  : 2.1..Name: liq
+00000020: 7061 792d 7364 6b2d 7079 7468 6f6e 330d  pay-sdk-python3.
+00000030: 0a56 6572 7369 6f6e 3a20 312e 302e 360d  .Version: 1.0.6.
+00000040: 0a53 756d 6d61 7279 3a20 4c69 7150 6179  .Summary: LiqPay
+00000050: 2050 7974 686f 6e33 2053 444b 0d0a 486f   Python3 SDK..Ho
+00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000070: 2f67 6974 6875 622e 636f 6d2f 616f 727a  /github.com/aorz
+00000080: 682f 6c69 7170 6179 2d73 646b 2d70 7974  h/liqpay-sdk-pyt
+00000090: 686f 6e33 0d0a 4465 7363 7269 7074 696f  hon3..Descriptio
+000000a0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+000000b0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a0d  text/markdown...
+000000c0: 0a5b 215b 5079 7468 6f6e 2033 2e36 2b5d  .[![Python 3.6+]
+000000d0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000000e0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+000000f0: 7468 6f6e 2d33 2e36 2b2d 626c 7565 2e73  thon-3.6+-blue.s
+00000100: 7667 295d 2868 7474 7073 3a2f 2f77 7777  vg)](https://www
+00000110: 2e70 7974 686f 6e2e 6f72 672f 646f 776e  .python.org/down
+00000120: 6c6f 6164 732f 7265 6c65 6173 652f 7079  loads/release/py
+00000130: 7468 6f6e 2d33 3630 2f29 0d0a 0d0a 5b21  thon-360/)....[!
+00000140: 5b53 444b 2d50 7974 686f 6e33 5d28 6874  [SDK-Python3](ht
+00000150: 7470 733a 2f2f 7777 772e 6c69 7170 6179  tps://www.liqpay
+00000160: 2e75 612f 6c6f 676f 5f6c 6971 7061 795f  .ua/logo_liqpay_
+00000170: 6d61 696e 2e73 7667 295d 2868 7474 7073  main.svg)](https
+00000180: 3a2f 2f77 7777 2e6c 6971 7061 792e 7561  ://www.liqpay.ua
+00000190: 2f64 6f63 756d 656e 7461 7469 6f6e 2f61  /documentation/a
+000001a0: 7069 2f68 6f6d 6529 0d0a 0d0a 2a20 5765  pi/home)....* We
+000001b0: 623a 2068 7474 7073 3a2f 2f77 7777 2e6c  b: https://www.l
+000001c0: 6971 7061 792e 7561 2f0d 0a2a 2044 6f77  iqpay.ua/..* Dow
+000001d0: 6e6c 6f61 643a 2068 7474 7073 3a2f 2f70  nload: https://p
+000001e0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000001f0: 6c69 7170 6179 2d73 646b 2d70 7974 686f  liqpay-sdk-pytho
+00000200: 6e33 2f0d 0a2a 2053 6f75 7263 653a 2068  n3/..* Source: h
+00000210: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000220: 6d2f 616f 727a 682f 6c69 7170 6179 2d73  m/aorzh/liqpay-s
+00000230: 646b 2d70 7974 686f 6e33 0d0a 2a20 446f  dk-python3..* Do
+00000240: 6375 6d65 6e74 6174 696f 6e3a 2068 7474  cumentation: htt
+00000250: 7073 3a2f 2f77 7777 2e6c 6971 7061 792e  ps://www.liqpay.
+00000260: 7561 2f64 6f63 756d 656e 7461 7469 6f6e  ua/documentation
+00000270: 2f65 6e2f 0d0a 2a20 4b65 7977 6f72 6473  /en/..* Keywords
+00000280: 3a20 6c69 7170 6179 2c20 7072 6976 6174  : liqpay, privat
+00000290: 3234 2c20 7072 6976 6174 6261 6e6b 2c20  24, privatbank, 
+000002a0: 7079 7468 6f6e 2c20 696e 7465 726e 6574  python, internet
+000002b0: 2061 6371 7569 7269 6e67 2c20 5032 5020   acquiring, P2P 
+000002c0: 7061 796d 656e 7473 2c20 7477 6f2d 7374  payments, two-st
+000002d0: 6570 2070 6179 6d65 6e74 730d 0a0d 0a0d  ep payments.....
+000002e0: 0a57 6861 7420 7079 7468 6f6e 2076 6572  .What python ver
+000002f0: 7369 6f6e 2069 7320 7375 7070 6f72 7465  sion is supporte
+00000300: 643f 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  d?..============
+00000310: 0d0a 2d20 5079 7468 6f6e 2033 2e34 2b0d  ..- Python 3.4+.
+00000320: 0a0d 0a47 6574 2053 7461 7274 6564 0d0a  ...Get Started..
+00000330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 312e  ============..1.
+00000340: 2053 6967 6e20 7570 2069 6e20 6874 7470   Sign up in http
+00000350: 733a 2f2f 7777 772e 6c69 7170 6179 2e75  s://www.liqpay.u
+00000360: 612f 656e 2f61 7574 686f 7269 7a61 7469  a/en/authorizati
+00000370: 6f6e 2e0d 0a32 2e20 4372 6561 7465 2061  on...2. Create a
+00000380: 2063 6f6d 7061 6e79 2e0d 0a33 2e20 496e   company...3. In
+00000390: 2063 6f6d 7061 6e79 2073 6574 7469 6e67   company setting
+000003a0: 732c 206f 6e20 4150 4920 7461 622c 2067  s, on API tab, g
+000003b0: 6574 202a 2a50 7562 6c69 6320 6b65 792a  et **Public key*
+000003c0: 2a20 616e 6420 2a2a 5072 6976 6174 6520  * and **Private 
+000003d0: 6b65 792a 2a2e 0d0a 342e 2044 6f6e 652e  key**...4. Done.
+000003e0: 0d0a 0d0a 496e 7374 616c 6c61 7469 6f6e  ....Installation
+000003f0: 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ..============..
+00000400: 4672 6f6d 2070 6970 0d0a 6060 6070 6970  From pip..```pip
+00000410: 2069 6e73 7461 6c6c 206c 6971 7061 792d   install liqpay-
+00000420: 7364 6b2d 7079 7468 6f6e 3360 6060 0d0a  sdk-python3```..
+00000430: 0d0a 576f 726b 696e 6720 7769 7468 204c  ..Working with L
+00000440: 6971 5061 7920 4361 6c6c 6261 636b 206c  iqPay Callback l
+00000450: 6f63 616c 6c79 0d0a 3d3d 3d3d 3d3d 3d3d  ocally..========
+00000460: 3d3d 3d3d 0d0a 4966 2079 6f75 206e 6565  ====..If you nee
+00000470: 6420 6465 6275 6767 696e 6720 4150 4920  d debugging API 
+00000480: 4361 6c6c 6261 636b 206f 6e20 6c6f 6361  Callback on loca
+00000490: 6c20 656e 7669 726f 6e6d 656e 7420 7573  l environment us
+000004a0: 6520 6874 7470 733a 2f2f 6c6f 6361 6c74  e https://localt
+000004b0: 756e 6e65 6c2e 6769 7468 7562 2e69 6f2f  unnel.github.io/
+000004c0: 7777 772f 0d0a 0d0a 486f 7720 6974 2075  www/....How it u
+000004d0: 7365 733f 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d  ses?..==========
+000004e0: 3d3d 0d0a 0d0a 4578 616d 706c 6520 313a  ==....Example 1:
+000004f0: 2042 6173 6963 0d0a 2d2d 2d2d 2d2d 2d0d   Basic..-------.
+00000500: 0a0d 0a2a 2a42 6163 6b65 6e64 2a2a 0d0a  ...**Backend**..
+00000510: 4765 7420 7061 796d 656e 7420 6275 7474  Get payment butt
+00000520: 6f6e 2028 6874 6d6c 2072 6573 706f 6e73  on (html respons
+00000530: 6529 0d0a 6060 600d 0a6c 6971 7061 7920  e)..```..liqpay 
+00000540: 3d20 4c69 7150 6179 2870 7562 6c69 635f  = LiqPay(public_
+00000550: 6b65 792c 2070 7269 7661 7465 5f6b 6579  key, private_key
+00000560: 290d 0a68 746d 6c20 3d20 6c69 7170 6179  )..html = liqpay
+00000570: 2e63 6e62 5f66 6f72 6d28 7b0d 0a20 2020  .cnb_form({..   
+00000580: 2027 6163 7469 6f6e 273a 2027 7061 7927   'action': 'pay'
+00000590: 2c0d 0a20 2020 2027 616d 6f75 6e74 273a  ,..    'amount':
+000005a0: 2027 3127 2c0d 0a20 2020 2027 6375 7272   '1',..    'curr
+000005b0: 656e 6379 273a 2027 5553 4427 2c0d 0a20  ency': 'USD',.. 
+000005c0: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
+000005d0: 3a20 2764 6573 6372 6970 7469 6f6e 2074  : 'description t
+000005e0: 6578 7427 2c0d 0a20 2020 2027 6f72 6465  ext',..    'orde
+000005f0: 725f 6964 273a 2027 6f72 6465 725f 6964  r_id': 'order_id
+00000600: 5f31 272c 0d0a 2020 2020 2776 6572 7369  _1',..    'versi
+00000610: 6f6e 273a 2027 3327 2c0d 0a20 2020 2027  on': '3',..    '
+00000620: 6c61 6e67 7561 6765 273a 2027 7275 7c75  language': 'ru|u
+00000630: 6b7c 656e 270d 0a7d 290d 0a60 6060 0d0a  k|en'..})..```..
+00000640: 0d0a 4765 7420 706c 6169 6e20 6368 6563  ..Get plain chec
+00000650: 6b6f 7574 2075 726c 3a0d 0a0d 0a60 6060  kout url:....```
+00000660: 0d0a 6c69 7170 6179 203d 204c 6971 5061  ..liqpay = LiqPa
+00000670: 7928 7075 626c 6963 5f6b 6579 2c20 7072  y(public_key, pr
+00000680: 6976 6174 655f 6b65 7929 0d0a 6874 6d6c  ivate_key)..html
+00000690: 203d 206c 6971 7061 792e 6368 6563 6b6f   = liqpay.checko
+000006a0: 7574 5f75 726c 287b 0d0a 2020 2020 2761  ut_url({..    'a
+000006b0: 6374 696f 6e27 3a20 2761 7574 6827 2c0d  ction': 'auth',.
+000006c0: 0a20 2020 2027 616d 6f75 6e74 273a 2027  .    'amount': '
+000006d0: 3127 2c0d 0a20 2020 2027 6375 7272 656e  1',..    'curren
+000006e0: 6379 273a 2027 5553 4427 2c0d 0a20 2020  cy': 'USD',..   
+000006f0: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
+00000700: 2764 6573 6372 6970 7469 6f6e 2074 6578  'description tex
+00000710: 7427 2c0d 0a20 2020 2027 6f72 6465 725f  t',..    'order_
+00000720: 6964 273a 2027 6f72 6465 725f 6964 5f31  id': 'order_id_1
+00000730: 272c 0d0a 2020 2020 2776 6572 7369 6f6e  ',..    'version
+00000740: 273a 2027 3327 2c0d 0a20 2020 2027 6c61  ': '3',..    'la
+00000750: 6e67 7561 6765 273a 2027 7275 7c75 6b7c  nguage': 'ru|uk|
+00000760: 656e 272c 0d0a 2020 2020 2772 6563 7572  en',..    'recur
+00000770: 7269 6e67 6279 746f 6b65 6e27 3a20 2731  ringbytoken': '1
+00000780: 270d 0a7d 290d 0a23 2052 6573 706f 6e73  '..})..# Respons
+00000790: 653a 0d0a 0d0a 7374 723a 2068 7474 7073  e:....str: https
+000007a0: 3a2f 2f77 7777 2e6c 6971 7061 792e 7561  ://www.liqpay.ua
+000007b0: 2f61 7069 2f33 2f63 6865 636b 6f75 742f  /api/3/checkout/
+000007c0: 3f64 6174 613d 3c64 6563 6f64 6564 2064  ?data=<decoded d
+000007d0: 6174 613e 2673 6967 6e61 7475 7265 3d3c  ata>&signature=<
+000007e0: 6465 636f 6465 6420 7369 676e 6174 7572  decoded signatur
+000007f0: 653e 0d0a 0d0a 6060 600d 0a0d 0a0d 0a2a  e>....```......*
+00000800: 2a46 726f 6e74 656e 642a 2a0d 0a0d 0a56  *Frontend**....V
+00000810: 6172 6961 626c 6520 6060 6874 6d6c 6060  ariable ``html``
+00000820: 2077 696c 6c20 636f 6e74 6169 6e20 6e65   will contain ne
+00000830: 7874 2068 746d 6c20 666f 726d 0d0a 0d0a  xt html form....
+00000840: 6060 600d 0a20 2020 203c 666f 726d 206d  ```..    <form m
+00000850: 6574 686f 643d 2250 4f53 5422 2061 6374  ethod="POST" act
+00000860: 696f 6e3d 2268 7474 7073 3a2f 2f77 7777  ion="https://www
+00000870: 2e6c 6971 7061 792e 7561 2f61 7069 2f33  .liqpay.ua/api/3
+00000880: 2f63 6865 636b 6f75 742f 2220 6163 6365  /checkout/" acce
+00000890: 7074 2d63 6861 7273 6574 3d22 7574 662d  pt-charset="utf-
+000008a0: 3822 3e0d 0a20 2020 2020 2020 2020 3c69  8">..         <i
+000008b0: 6e70 7574 2074 7970 653d 2768 6964 6465  nput type='hidde
+000008c0: 6e27 206e 616d 653d 2764 6174 6127 2076  n' name='data' v
+000008d0: 616c 7565 3d27 6579 4a68 6257 3931 626e  alue='eyJhbW91bn
+000008e0: 5169 4f69 2e2e 2e3d 272f 3e0d 0a20 2020  QiOi...='/>..   
+000008f0: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
+00000900: 653d 2768 6964 6465 6e27 206e 616d 653d  e='hidden' name=
+00000910: 2773 6967 6e61 7475 7265 2720 7661 6c75  'signature' valu
+00000920: 653d 2765 6455 7334 2e2e 2e3d 272f 3e0d  e='edUs4...='/>.
+00000930: 0a20 2020 2020 2020 2020 3c62 7574 746f  .         <butto
+00000940: 6e20 7374 796c 653d 2262 6f72 6465 723a  n style="border:
+00000950: 206e 6f6e 6520 2169 6d70 6f72 7461 6e74   none !important
+00000960: 3b64 6973 706c 6179 3a69 6e6c 696e 652d  ;display:inline-
+00000970: 626c 6f63 6b20 2169 6d70 6f72 7461 6e74  block !important
+00000980: 3b74 6578 742d 616c 6967 6e3a 2063 656e  ;text-align: cen
+00000990: 7465 7220 2169 6d70 6f72 7461 6e74 3b20  ter !important; 
+000009a0: 7061 6464 696e 673a 2037 7078 2032 3070  padding: 7px 20p
+000009b0: 7820 2169 6d70 6f72 7461 6e74 3b20 636f  x !important; co
+000009c0: 6c6f 723a 2023 6666 6620 2169 6d70 6f72  lor: #fff !impor
+000009d0: 7461 6e74 3b66 6f6e 742d 7369 7a65 3a31  tant;font-size:1
+000009e0: 3670 7820 2169 6d70 6f72 7461 6e74 3b20  6px !important; 
+000009f0: 666f 6e74 2d77 6569 6768 743a 2036 3030  font-weight: 600
+00000a00: 2021 696d 706f 7274 616e 743b 2066 6f6e   !important; fon
+00000a10: 742d 6661 6d69 6c79 3a4f 7065 6e53 616e  t-family:OpenSan
+00000a20: 732c 2073 616e 732d 7365 7269 663b 6375  s, sans-serif;cu
+00000a30: 7273 6f72 3a20 706f 696e 7465 7220 2169  rsor: pointer !i
+00000a40: 6d70 6f72 7461 6e74 3b62 6f72 6465 722d  mportant;border-
+00000a50: 7261 6469 7573 3a20 3270 7820 2169 6d70  radius: 2px !imp
+00000a60: 6f72 7461 6e74 3b62 6163 6b67 726f 756e  ortant;backgroun
+00000a70: 643a 2072 6762 6128 3132 322c 3138 332c  d: rgba(122,183,
+00000a80: 3433 2c31 2920 2169 6d70 6f72 7461 6e74  43,1) !important
+00000a90: 3b22 6f6e 6d6f 7573 656f 7665 723d 2274  ;"onmouseover="t
+00000aa0: 6869 732e 7374 796c 652e 6f70 6163 6974  his.style.opacit
+00000ab0: 793d 302e 353b 2220 6f6e 6d6f 7573 656f  y=0.5;" onmouseo
+00000ac0: 7574 3d22 7468 6973 2e73 7479 6c65 2e6f  ut="this.style.o
+00000ad0: 7061 6369 7479 3d31 3b22 3e20 3c69 6d67  pacity=1;"> <img
+00000ae0: 2073 7263 3d22 6874 7470 733a 2f2f 7374   src="https://st
+00000af0: 6174 6963 2e6c 6971 7061 792e 7561 2f62  atic.liqpay.ua/b
+00000b00: 7574 746f 6e73 2f6c 6f67 6f2d 736d 616c  uttons/logo-smal
+00000b10: 6c2e 706e 6722 206e 616d 653d 2262 746e  l.png" name="btn
+00000b20: 5f74 6578 7422 2073 7479 6c65 3d22 6d61  _text" style="ma
+00000b30: 7267 696e 2d72 6967 6874 3a20 3770 7820  rgin-right: 7px 
+00000b40: 2169 6d70 6f72 7461 6e74 3b20 7665 7274  !important; vert
+00000b50: 6963 616c 2d61 6c69 676e 3a20 6d69 6464  ical-align: midd
+00000b60: 6c65 2021 696d 706f 7274 616e 743b 222f  le !important;"/
+00000b70: 3e20 0d0a 2020 2020 2020 2020 203c 7370  > ..         <sp
+00000b80: 616e 2073 7479 6c65 3d22 7665 7274 6963  an style="vertic
+00000b90: 616c 2d61 6c69 676e 3a6d 6964 646c 653b  al-align:middle;
+00000ba0: 2169 6d70 6f72 7461 6e74 223e 5041 5920  !important">PAY 
+00000bb0: 3130 3020 5541 483c 2f73 7061 6e3e 0d0a  100 UAH</span>..
+00000bc0: 2020 2020 2020 2020 203c 2f62 7574 746f           </butto
+00000bd0: 6e3e 0d0a 2020 2020 3c2f 666f 726d 3e0d  n>..    </form>.
+00000be0: 0a60 6060 0d0a 0d0a 4578 616d 706c 6520  .```....Example 
+00000bf0: 323a 2049 6e74 6567 7261 7465 2050 6179  2: Integrate Pay
+00000c00: 6d65 6e74 2077 6964 6765 7420 746f 2044  ment widget to D
+00000c10: 6a61 6e67 6f0d 0a2d 2d2d 2d2d 2d2d 0d0a  jango..-------..
+00000c20: 6050 6179 6d65 6e74 2077 6964 6765 7420  `Payment widget 
+00000c30: 646f 6375 6d65 6e74 6174 696f 6e60 200d  documentation` .
+00000c40: 0a68 7474 7073 3a2f 2f77 7777 2e6c 6971  .https://www.liq
+00000c50: 7061 792e 7561 2f64 6f63 756d 656e 7461  pay.ua/documenta
+00000c60: 7469 6f6e 2f65 6e2f 6170 692f 6171 7569  tion/en/api/aqui
+00000c70: 7269 6e67 2f77 6964 6765 742f 0d0a 0d0a  ring/widget/....
+00000c80: 2a42 6163 6b65 6e64 2a0d 0a0d 0a60 7669  *Backend*....`vi
+00000c90: 6577 732e 7079 600d 0a0d 0a60 6060 0d0a  ews.py`....```..
+00000ca0: 0d0a 2020 2020 6672 6f6d 206c 6971 7061  ..    from liqpa
+00000cb0: 7920 696d 706f 7274 204c 6971 5061 790d  y import LiqPay.
+00000cc0: 0a0d 0a20 2020 2066 726f 6d20 646a 616e  ...    from djan
+00000cd0: 676f 2e76 6965 7773 2e67 656e 6572 6963  go.views.generic
+00000ce0: 2069 6d70 6f72 7420 5465 6d70 6c61 7465   import Template
+00000cf0: 5669 6577 0d0a 2020 2020 6672 6f6d 2064  View..    from d
+00000d00: 6a61 6e67 6f2e 7368 6f72 7463 7574 7320  jango.shortcuts 
+00000d10: 696d 706f 7274 2072 656e 6465 720d 0a20  import render.. 
+00000d20: 2020 2066 726f 6d20 646a 616e 676f 2e68     from django.h
+00000d30: 7474 7020 696d 706f 7274 2048 7474 7052  ttp import HttpR
+00000d40: 6573 706f 6e73 650d 0a0d 0a20 2020 2063  esponse....    c
+00000d50: 6c61 7373 2050 6179 5669 6577 2854 656d  lass PayView(Tem
+00000d60: 706c 6174 6556 6965 7729 3a0d 0a20 2020  plateView):..   
+00000d70: 2074 656d 706c 6174 655f 6e61 6d65 203d   template_name =
+00000d80: 2027 6269 6c6c 696e 672f 7061 792e 6874   'billing/pay.ht
+00000d90: 6d6c 270d 0a0d 0a20 2020 2064 6566 2067  ml'....    def g
+00000da0: 6574 2873 656c 662c 2072 6571 7565 7374  et(self, request
+00000db0: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+00000dc0: 7329 3a0d 0a20 2020 2020 2020 206c 6971  s):..        liq
+00000dd0: 7061 7920 3d20 4c69 7150 6179 2873 6574  pay = LiqPay(set
+00000de0: 7469 6e67 732e 4c49 5150 4159 5f50 5542  tings.LIQPAY_PUB
+00000df0: 4c49 435f 4b45 592c 2073 6574 7469 6e67  LIC_KEY, setting
+00000e00: 732e 4c49 5150 4159 5f50 5249 5641 5445  s.LIQPAY_PRIVATE
+00000e10: 5f4b 4559 290d 0a20 2020 2020 2020 2070  _KEY)..        p
+00000e20: 6172 616d 7320 3d20 7b0d 0a20 2020 2020  arams = {..     
+00000e30: 2020 2020 2020 2027 6163 7469 6f6e 273a         'action':
+00000e40: 2027 7061 7927 2c0d 0a20 2020 2020 2020   'pay',..       
+00000e50: 2020 2020 2027 616d 6f75 6e74 273a 2027       'amount': '
+00000e60: 3130 3027 2c0d 0a20 2020 2020 2020 2020  100',..         
+00000e70: 2020 2027 6375 7272 656e 6379 273a 2027     'currency': '
+00000e80: 5553 4427 2c0d 0a20 2020 2020 2020 2020  USD',..         
+00000e90: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
+00000ea0: 3a20 2750 6179 6d65 6e74 2066 6f72 2063  : 'Payment for c
+00000eb0: 6c6f 7468 6573 272c 0d0a 2020 2020 2020  lothes',..      
+00000ec0: 2020 2020 2020 276f 7264 6572 5f69 6427        'order_id'
+00000ed0: 3a20 276f 7264 6572 5f69 645f 3127 2c0d  : 'order_id_1',.
+00000ee0: 0a20 2020 2020 2020 2020 2020 2027 7665  .            've
+00000ef0: 7273 696f 6e27 3a20 2733 272c 0d0a 2020  rsion': '3',..  
+00000f00: 2020 2020 2020 2020 2020 2773 616e 6462            'sandb
+00000f10: 6f78 273a 2030 2c20 2320 7361 6e64 626f  ox': 0, # sandbo
+00000f20: 7820 6d6f 6465 2c20 7365 7420 746f 2031  x mode, set to 1
+00000f30: 2074 6f20 656e 6162 6c65 2069 740d 0a20   to enable it.. 
+00000f40: 2020 2020 2020 2020 2020 2027 7365 7276             'serv
+00000f50: 6572 5f75 726c 273a 2027 6874 7470 733a  er_url': 'https:
+00000f60: 2f2f 7465 7374 2e63 6f6d 2f62 696c 6c69  //test.com/billi
+00000f70: 6e67 2f70 6179 2d63 616c 6c62 6163 6b2f  ng/pay-callback/
+00000f80: 272c 2023 2075 726c 2074 6f20 6361 6c6c  ', # url to call
+00000f90: 6261 636b 2076 6965 770d 0a20 2020 2020  back view..     
+00000fa0: 2020 207d 0d0a 2020 2020 2020 2020 7369     }..        si
+00000fb0: 676e 6174 7572 6520 3d20 6c69 7170 6179  gnature = liqpay
+00000fc0: 2e63 6e62 5f73 6967 6e61 7475 7265 2870  .cnb_signature(p
+00000fd0: 6172 616d 7329 0d0a 2020 2020 2020 2020  arams)..        
+00000fe0: 6461 7461 203d 206c 6971 7061 792e 636e  data = liqpay.cn
+00000ff0: 625f 6461 7461 2870 6172 616d 7329 0d0a  b_data(params)..
+00001000: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00001010: 656e 6465 7228 7265 7175 6573 742c 2073  ender(request, s
+00001020: 656c 662e 7465 6d70 6c61 7465 5f6e 616d  elf.template_nam
+00001030: 652c 207b 2773 6967 6e61 7475 7265 273a  e, {'signature':
+00001040: 2073 6967 6e61 7475 7265 2c20 2764 6174   signature, 'dat
+00001050: 6127 3a20 6461 7461 7d29 0d0a 0d0a 2020  a': data})....  
+00001060: 2020 406d 6574 686f 645f 6465 636f 7261    @method_decora
+00001070: 746f 7228 6373 7266 5f65 7865 6d70 742c  tor(csrf_exempt,
+00001080: 206e 616d 653d 2764 6973 7061 7463 6827   name='dispatch'
+00001090: 290d 0a20 2020 2063 6c61 7373 2050 6179  )..    class Pay
+000010a0: 4361 6c6c 6261 636b 5669 6577 2856 6965  CallbackView(Vie
+000010b0: 7729 3a0d 0a20 2020 2020 2020 2064 6566  w):..        def
+000010c0: 2070 6f73 7428 7365 6c66 2c20 7265 7175   post(self, requ
+000010d0: 6573 742c 202a 6172 6773 2c20 2a2a 6b77  est, *args, **kw
+000010e0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+000010f0: 2020 2020 6c69 7170 6179 203d 204c 6971      liqpay = Liq
+00001100: 5061 7928 7365 7474 696e 6773 2e4c 4951  Pay(settings.LIQ
+00001110: 5041 595f 5055 424c 4943 5f4b 4559 2c20  PAY_PUBLIC_KEY, 
+00001120: 7365 7474 696e 6773 2e4c 4951 5041 595f  settings.LIQPAY_
+00001130: 5052 4956 4154 455f 4b45 5929 0d0a 2020  PRIVATE_KEY)..  
+00001140: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00001150: 2072 6571 7565 7374 2e50 4f53 542e 6765   request.POST.ge
+00001160: 7428 2764 6174 6127 290d 0a20 2020 2020  t('data')..     
+00001170: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
+00001180: 203d 2072 6571 7565 7374 2e50 4f53 542e   = request.POST.
+00001190: 6765 7428 2773 6967 6e61 7475 7265 2729  get('signature')
+000011a0: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
+000011b0: 676e 203d 206c 6971 7061 792e 7374 725f  gn = liqpay.str_
+000011c0: 746f 5f73 6967 6e28 7365 7474 696e 6773  to_sign(settings
+000011d0: 2e4c 4951 5041 595f 5052 4956 4154 455f  .LIQPAY_PRIVATE_
+000011e0: 4b45 5920 2b20 6461 7461 202b 2073 6574  KEY + data + set
+000011f0: 7469 6e67 732e 4c49 5150 4159 5f50 5249  tings.LIQPAY_PRI
+00001200: 5641 5445 5f4b 4559 290d 0a20 2020 2020  VATE_KEY)..     
+00001210: 2020 2020 2020 2069 6620 7369 676e 203d         if sign =
+00001220: 3d20 7369 676e 6174 7572 653a 0d0a 2020  = signature:..  
+00001230: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001240: 696e 7428 2763 616c 6c62 6163 6b20 6973  int('callback is
+00001250: 2076 616c 6964 2729 0d0a 2020 2020 2020   valid')..      
+00001260: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00001270: 206c 6971 7061 792e 6465 636f 6465 5f64   liqpay.decode_d
+00001280: 6174 615f 6672 6f6d 5f73 7472 2864 6174  ata_from_str(dat
+00001290: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
+000012a0: 7072 696e 7428 2763 616c 6c62 6163 6b20  print('callback 
+000012b0: 6461 7461 272c 2072 6573 706f 6e73 6529  data', response)
+000012c0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000012d0: 7475 726e 2048 7474 7052 6573 706f 6e73  turn HttpRespons
+000012e0: 6528 290d 0a60 6060 0d0a 6075 726c 732e  e()..```..`urls.
+000012f0: 7079 600d 0a0d 0a60 6060 0d0a 0d0a 2020  py`....```....  
+00001300: 2020 6672 6f6d 2064 6a61 6e67 6f2e 636f    from django.co
+00001310: 6e66 2e75 726c 7320 696d 706f 7274 2075  nf.urls import u
+00001320: 726c 0d0a 0d0a 2020 2020 6672 6f6d 2062  rl....    from b
+00001330: 696c 6c69 6e67 2e76 6965 7773 2069 6d70  illing.views imp
+00001340: 6f72 7420 5061 7956 6965 772c 2050 6179  ort PayView, Pay
+00001350: 4361 6c6c 6261 636b 5669 6577 0d0a 0d0a  CallbackView....
+00001360: 0d0a 2020 2020 7572 6c70 6174 7465 726e  ..    urlpattern
+00001370: 7320 3d20 5b0d 0a20 2020 2020 2020 2075  s = [..        u
+00001380: 726c 2872 275e 7061 792f 2427 2c20 5061  rl(r'^pay/$', Pa
+00001390: 7956 6965 772e 6173 5f76 6965 7728 292c  yView.as_view(),
+000013a0: 206e 616d 653d 2770 6179 5f76 6965 7727   name='pay_view'
+000013b0: 292c 0d0a 2020 2020 2020 2020 7572 6c28  ),..        url(
+000013c0: 7227 5e70 6179 2d63 616c 6c62 6163 6b2f  r'^pay-callback/
+000013d0: 2427 2c20 5061 7943 616c 6c62 6163 6b56  $', PayCallbackV
+000013e0: 6965 772e 6173 5f76 6965 7728 292c 206e  iew.as_view(), n
+000013f0: 616d 653d 2770 6179 5f63 616c 6c62 6163  ame='pay_callbac
+00001400: 6b27 292c 0d0a 2020 2020 5d0d 0a60 6060  k'),..    ]..```
+00001410: 0d0a 2a46 726f 6e74 656e 642a 0d0a 0d0a  ..*Frontend*....
+00001420: 6060 600d 0a0d 0a20 2020 203c 6469 7620  ```....    <div 
+00001430: 6964 3d22 6c69 7170 6179 5f63 6865 636b  id="liqpay_check
+00001440: 6f75 7422 3e3c 2f64 6976 3e0d 0a20 2020  out"></div>..   
+00001450: 203c 7363 7269 7074 3e0d 0a20 2020 2020   <script>..     
+00001460: 2020 2077 696e 646f 772e 4c69 7150 6179     window.LiqPay
+00001470: 4368 6563 6b6f 7574 4361 6c6c 6261 636b  CheckoutCallback
+00001480: 203d 2066 756e 6374 696f 6e28 2920 7b0d   = function() {.
+00001490: 0a20 2020 2020 2020 2020 2020 204c 6971  .            Liq
+000014a0: 5061 7943 6865 636b 6f75 742e 696e 6974  PayCheckout.init
+000014b0: 287b 0d0a 2020 2020 2020 2020 2020 2020  ({..            
+000014c0: 2020 2020 6461 7461 3a20 227b 7b20 6461      data: "{{ da
+000014d0: 7461 207d 7d22 2c0d 0a20 2020 2020 2020  ta }}",..       
+000014e0: 2020 2020 2020 2020 2073 6967 6e61 7475           signatu
+000014f0: 7265 3a20 227b 7b20 7369 676e 6174 7572  re: "{{ signatur
+00001500: 6520 7d7d 222c 0d0a 2020 2020 2020 2020  e }}",..        
+00001510: 2020 2020 2020 2020 656d 6265 6454 6f3a          embedTo:
+00001520: 2022 236c 6971 7061 795f 6368 6563 6b6f   "#liqpay_checko
+00001530: 7574 222c 0d0a 2020 2020 2020 2020 2020  ut",..          
+00001540: 2020 2020 2020 6d6f 6465 3a20 2265 6d62        mode: "emb
+00001550: 6564 2220 2f2f 2065 6d62 6564 207c 7c20  ed" // embed || 
+00001560: 706f 7075 702c 0d0a 2020 2020 2020 2020  popup,..        
+00001570: 2020 2020 7d29 2e6f 6e28 226c 6971 7061      }).on("liqpa
+00001580: 792e 6361 6c6c 6261 636b 222c 2066 756e  y.callback", fun
+00001590: 6374 696f 6e28 6461 7461 297b 0d0a 2020  ction(data){..  
+000015a0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000015b0: 6e73 6f6c 652e 6c6f 6728 6461 7461 2e73  nsole.log(data.s
+000015c0: 7461 7475 7329 3b0d 0a20 2020 2020 2020  tatus);..       
+000015d0: 2020 2020 2020 2020 2063 6f6e 736f 6c65           console
+000015e0: 2e6c 6f67 2864 6174 6129 3b0d 0a20 2020  .log(data);..   
+000015f0: 2020 2020 2020 2020 207d 292e 6f6e 2822           }).on("
+00001600: 6c69 7170 6179 2e72 6561 6479 222c 2066  liqpay.ready", f
+00001610: 756e 6374 696f 6e28 6461 7461 297b 0d0a  unction(data){..
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2f2f 2072 6561 6479 0d0a 2020 2020 2020  // ready..      
+00001640: 2020 2020 2020 7d29 2e6f 6e28 226c 6971        }).on("liq
+00001650: 7061 792e 636c 6f73 6522 2c20 6675 6e63  pay.close", func
+00001660: 7469 6f6e 2864 6174 6129 7b0d 0a20 2020  tion(data){..   
+00001670: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
+00001680: 636c 6f73 650d 0a20 2020 2020 2020 2020  close..         
+00001690: 2020 207d 293b 0d0a 2020 2020 2020 2020     });..        
+000016a0: 7d3b 0d0a 2020 2020 3c2f 7363 7269 7074  };..    </script
+000016b0: 3e0d 0a20 2020 203c 7363 7269 7074 2073  >..    <script s
+000016c0: 7263 3d22 2f2f 7374 6174 6963 2e6c 6971  rc="//static.liq
+000016d0: 7061 792e 7561 2f6c 6962 6a73 2f63 6865  pay.ua/libjs/che
+000016e0: 636b 6f75 742e 6a73 2220 6173 796e 633e  ckout.js" async>
+000016f0: 3c2f 7363 7269 7074 3e0d 0a60 6060 0d0a  </script>..```..
```

### Comparing `liqpay-sdk-python3-1.0.4/liqpay/liqpay3.py` & `liqpay-sdk-python3-1.0.6/liqpay/liqpay3.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 LiqPay Python SDK
 ~~~~~~~~~~~~~~~~~
 supports python 3 version
 requires requests module
 """
 
 __title__ = "LiqPay Python3 SDK"
-__version__ = "1.0.4"
+__version__ = "1.0.6"
 
 import base64
 from copy import deepcopy
 import hashlib
 import json
 from urllib.parse import urljoin
```

### Comparing `liqpay-sdk-python3-1.0.4/liqpay/tests/test_pay_simple.py` & `liqpay-sdk-python3-1.0.6/liqpay/tests/test_pay_simple.py`

 * *Files identical despite different names*

### Comparing `liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/PKG-INFO` & `liqpay-sdk-python3-1.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,348 +1,356 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 206c 6971  : 2.1..Name: liq
-00000020: 7061 792d 7364 6b2d 7079 7468 6f6e 330d  pay-sdk-python3.
-00000030: 0a56 6572 7369 6f6e 3a20 312e 302e 340d  .Version: 1.0.4.
-00000040: 0a53 756d 6d61 7279 3a20 4c69 7150 6179  .Summary: LiqPay
-00000050: 2050 7974 686f 6e33 2053 444b 0d0a 486f   Python3 SDK..Ho
-00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-00000070: 2f67 6974 6875 622e 636f 6d2f 616f 727a  /github.com/aorz
-00000080: 682f 6c69 7170 6179 2d73 646b 2d70 7974  h/liqpay-sdk-pyt
-00000090: 686f 6e33 0d0a 4465 7363 7269 7074 696f  hon3..Descriptio
-000000a0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000000b0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a0d  text/markdown...
-000000c0: 0a5b 215b 5079 7468 6f6e 2033 2e36 2b5d  .[![Python 3.6+]
-000000d0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000000e0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
-000000f0: 7468 6f6e 2d33 2e36 2b2d 626c 7565 2e73  thon-3.6+-blue.s
-00000100: 7667 295d 2868 7474 7073 3a2f 2f77 7777  vg)](https://www
-00000110: 2e70 7974 686f 6e2e 6f72 672f 646f 776e  .python.org/down
-00000120: 6c6f 6164 732f 7265 6c65 6173 652f 7079  loads/release/py
-00000130: 7468 6f6e 2d33 3630 2f29 0d0a 0d0a 5b21  thon-360/)....[!
-00000140: 5b53 444b 2d50 7974 686f 6e33 5d28 6874  [SDK-Python3](ht
-00000150: 7470 733a 2f2f 7777 772e 6c69 7170 6179  tps://www.liqpay
-00000160: 2e75 612f 6c6f 676f 5f6c 6971 7061 795f  .ua/logo_liqpay_
-00000170: 6d61 696e 2e73 7667 295d 2868 7474 7073  main.svg)](https
-00000180: 3a2f 2f77 7777 2e6c 6971 7061 792e 7561  ://www.liqpay.ua
-00000190: 2f64 6f63 756d 656e 7461 7469 6f6e 2f61  /documentation/a
-000001a0: 7069 2f68 6f6d 6529 0d0a 0d0a 2a20 5665  pi/home)....* Ve
-000001b0: 7273 696f 6e3a 2031 2e30 2e33 0d0a 2a20  rsion: 1.0.3..* 
-000001c0: 5765 623a 2068 7474 7073 3a2f 2f77 7777  Web: https://www
-000001d0: 2e6c 6971 7061 792e 7561 2f0d 0a2a 2044  .liqpay.ua/..* D
-000001e0: 6f77 6e6c 6f61 643a 2068 7474 7073 3a2f  ownload: https:/
-000001f0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000200: 742f 6c69 7170 6179 2d73 646b 2d70 7974  t/liqpay-sdk-pyt
-00000210: 686f 6e33 2f0d 0a2a 2053 6f75 7263 653a  hon3/..* Source:
-00000220: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000230: 636f 6d2f 616f 727a 682f 6c69 7170 6179  com/aorzh/liqpay
-00000240: 2d73 646b 2d70 7974 686f 6e33 0d0a 2a20  -sdk-python3..* 
-00000250: 446f 6375 6d65 6e74 6174 696f 6e3a 2068  Documentation: h
-00000260: 7474 7073 3a2f 2f77 7777 2e6c 6971 7061  ttps://www.liqpa
-00000270: 792e 7561 2f64 6f63 756d 656e 7461 7469  y.ua/documentati
-00000280: 6f6e 2f65 6e2f 0d0a 2a20 4b65 7977 6f72  on/en/..* Keywor
-00000290: 6473 3a20 6c69 7170 6179 2c20 7072 6976  ds: liqpay, priv
-000002a0: 6174 3234 2c20 7072 6976 6174 6261 6e6b  at24, privatbank
-000002b0: 2c20 7079 7468 6f6e 2c20 696e 7465 726e  , python, intern
-000002c0: 6574 2061 6371 7569 7269 6e67 2c20 5032  et acquiring, P2
-000002d0: 5020 7061 796d 656e 7473 2c20 7477 6f2d  P payments, two-
-000002e0: 7374 6570 2070 6179 6d65 6e74 730d 0a0d  step payments...
-000002f0: 0a0d 0a57 6861 7420 7079 7468 6f6e 2076  ...What python v
-00000300: 6572 7369 6f6e 2069 7320 7375 7070 6f72  ersion is suppor
-00000310: 7465 643f 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d  ted?..==========
-00000320: 3d3d 0d0a 2d20 5079 7468 6f6e 2033 2e34  ==..- Python 3.4
-00000330: 2b0d 0a0d 0a47 6574 2053 7461 7274 6564  +....Get Started
-00000340: 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ..============..
-00000350: 312e 2053 6967 6e20 7570 2069 6e20 6874  1. Sign up in ht
-00000360: 7470 733a 2f2f 7777 772e 6c69 7170 6179  tps://www.liqpay
-00000370: 2e75 612f 656e 2f61 7574 686f 7269 7a61  .ua/en/authoriza
-00000380: 7469 6f6e 2e0d 0a32 2e20 4372 6561 7465  tion...2. Create
-00000390: 2061 2063 6f6d 7061 6e79 2e0d 0a33 2e20   a company...3. 
-000003a0: 496e 2063 6f6d 7061 6e79 2073 6574 7469  In company setti
-000003b0: 6e67 732c 206f 6e20 4150 4920 7461 622c  ngs, on API tab,
-000003c0: 2067 6574 202a 2a50 7562 6c69 6320 6b65   get **Public ke
-000003d0: 792a 2a20 616e 6420 2a2a 5072 6976 6174  y** and **Privat
-000003e0: 6520 6b65 792a 2a2e 0d0a 342e 2044 6f6e  e key**...4. Don
-000003f0: 652e 0d0a 0d0a 496e 7374 616c 6c61 7469  e.....Installati
-00000400: 6f6e 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  on..============
-00000410: 0d0a 4672 6f6d 2070 6970 0d0a 6060 6070  ..From pip..```p
-00000420: 6970 2069 6e73 7461 6c6c 206c 6971 7061  ip install liqpa
-00000430: 792d 7364 6b2d 7079 7468 6f6e 3360 6060  y-sdk-python3```
-00000440: 0d0a 0d0a 576f 726b 696e 6720 7769 7468  ....Working with
-00000450: 204c 6971 5061 7920 4361 6c6c 6261 636b   LiqPay Callback
-00000460: 206c 6f63 616c 6c79 0d0a 3d3d 3d3d 3d3d   locally..======
-00000470: 3d3d 3d3d 3d3d 0d0a 4966 2079 6f75 206e  ======..If you n
-00000480: 6565 6420 6465 6275 6767 696e 6720 4150  eed debugging AP
-00000490: 4920 4361 6c6c 6261 636b 206f 6e20 6c6f  I Callback on lo
-000004a0: 6361 6c20 656e 7669 726f 6e6d 656e 7420  cal environment 
-000004b0: 7573 6520 6874 7470 733a 2f2f 6c6f 6361  use https://loca
-000004c0: 6c74 756e 6e65 6c2e 6769 7468 7562 2e69  ltunnel.github.i
-000004d0: 6f2f 7777 772f 0d0a 0d0a 486f 7720 6974  o/www/....How it
-000004e0: 2075 7365 3f0d 0a3d 3d3d 3d3d 3d3d 3d3d   use?..=========
-000004f0: 3d3d 3d0d 0a0d 0a45 7861 6d70 6c65 2031  ===....Example 1
-00000500: 3a20 4261 7369 630d 0a2d 2d2d 2d2d 2d2d  : Basic..-------
-00000510: 0d0a 0d0a 2a2a 4261 636b 656e 642a 2a0d  ....**Backend**.
-00000520: 0a47 6574 2070 6179 6d65 6e74 2062 7574  .Get payment but
-00000530: 746f 6e20 2868 746d 6c20 7265 7370 6f6e  ton (html respon
-00000540: 7365 290d 0a60 6060 0d0a 6c69 7170 6179  se)..```..liqpay
-00000550: 203d 204c 6971 5061 7928 7075 626c 6963   = LiqPay(public
-00000560: 5f6b 6579 2c20 7072 6976 6174 655f 6b65  _key, private_ke
-00000570: 7929 0d0a 6874 6d6c 203d 206c 6971 7061  y)..html = liqpa
-00000580: 792e 636e 625f 666f 726d 287b 0d0a 2020  y.cnb_form({..  
-00000590: 2020 2761 6374 696f 6e27 3a20 2770 6179    'action': 'pay
-000005a0: 272c 0d0a 2020 2020 2761 6d6f 756e 7427  ',..    'amount'
-000005b0: 3a20 2731 272c 0d0a 2020 2020 2763 7572  : '1',..    'cur
-000005c0: 7265 6e63 7927 3a20 2755 5344 272c 0d0a  rency': 'USD',..
-000005d0: 2020 2020 2764 6573 6372 6970 7469 6f6e      'description
-000005e0: 273a 2027 6465 7363 7269 7074 696f 6e20  ': 'description 
-000005f0: 7465 7874 272c 0d0a 2020 2020 276f 7264  text',..    'ord
-00000600: 6572 5f69 6427 3a20 276f 7264 6572 5f69  er_id': 'order_i
-00000610: 645f 3127 2c0d 0a20 2020 2027 7665 7273  d_1',..    'vers
-00000620: 696f 6e27 3a20 2733 272c 0d0a 2020 2020  ion': '3',..    
-00000630: 276c 616e 6775 6167 6527 3a20 2772 757c  'language': 'ru|
-00000640: 756b 7c65 6e27 0d0a 7d29 0d0a 6060 600d  uk|en'..})..```.
-00000650: 0a0d 0a47 6574 2070 6c61 696e 2063 6865  ...Get plain che
-00000660: 636b 6f75 7420 7572 6c3a 0d0a 0d0a 6060  ckout url:....``
-00000670: 600d 0a6c 6971 7061 7920 3d20 4c69 7150  `..liqpay = LiqP
-00000680: 6179 2870 7562 6c69 635f 6b65 792c 2070  ay(public_key, p
-00000690: 7269 7661 7465 5f6b 6579 290d 0a68 746d  rivate_key)..htm
-000006a0: 6c20 3d20 6c69 7170 6179 2e63 6865 636b  l = liqpay.check
-000006b0: 6f75 745f 7572 6c28 7b0d 0a20 2020 2027  out_url({..    '
-000006c0: 6163 7469 6f6e 273a 2027 6175 7468 272c  action': 'auth',
-000006d0: 0d0a 2020 2020 2761 6d6f 756e 7427 3a20  ..    'amount': 
-000006e0: 2731 272c 0d0a 2020 2020 2763 7572 7265  '1',..    'curre
-000006f0: 6e63 7927 3a20 2755 5344 272c 0d0a 2020  ncy': 'USD',..  
-00000700: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
-00000710: 2027 6465 7363 7269 7074 696f 6e20 7465   'description te
-00000720: 7874 272c 0d0a 2020 2020 276f 7264 6572  xt',..    'order
-00000730: 5f69 6427 3a20 276f 7264 6572 5f69 645f  _id': 'order_id_
-00000740: 3127 2c0d 0a20 2020 2027 7665 7273 696f  1',..    'versio
-00000750: 6e27 3a20 2733 272c 0d0a 2020 2020 276c  n': '3',..    'l
-00000760: 616e 6775 6167 6527 3a20 2772 757c 756b  anguage': 'ru|uk
-00000770: 7c65 6e27 2c0d 0a20 2020 2027 7265 6375  |en',..    'recu
-00000780: 7272 696e 6762 7974 6f6b 656e 273a 2027  rringbytoken': '
-00000790: 3127 0d0a 7d29 0d0a 2320 5265 7370 6f6e  1'..})..# Respon
-000007a0: 7365 3a0d 0a0d 0a73 7472 3a20 6874 7470  se:....str: http
-000007b0: 733a 2f2f 7777 772e 6c69 7170 6179 2e75  s://www.liqpay.u
-000007c0: 612f 6170 692f 332f 6368 6563 6b6f 7574  a/api/3/checkout
-000007d0: 2f3f 6461 7461 3d3c 6465 636f 6465 6420  /?data=<decoded 
-000007e0: 6461 7461 3e26 7369 676e 6174 7572 653d  data>&signature=
-000007f0: 3c64 6563 6f64 6564 2073 6967 6e61 7475  <decoded signatu
-00000800: 7265 3e0d 0a0d 0a60 6060 0d0a 0d0a 0d0a  re>....```......
-00000810: 2a2a 4672 6f6e 7465 6e64 2a2a 0d0a 0d0a  **Frontend**....
-00000820: 5661 7269 6162 6c65 2060 6068 746d 6c60  Variable ``html`
-00000830: 6020 7769 6c6c 2063 6f6e 7461 696e 206e  ` will contain n
-00000840: 6578 7420 6874 6d6c 2066 6f72 6d0d 0a0d  ext html form...
-00000850: 0a60 6060 0d0a 2020 2020 3c66 6f72 6d20  .```..    <form 
-00000860: 6d65 7468 6f64 3d22 504f 5354 2220 6163  method="POST" ac
-00000870: 7469 6f6e 3d22 6874 7470 733a 2f2f 7777  tion="https://ww
-00000880: 772e 6c69 7170 6179 2e75 612f 6170 692f  w.liqpay.ua/api/
-00000890: 332f 6368 6563 6b6f 7574 2220 6163 6365  3/checkout" acce
-000008a0: 7074 2d63 6861 7273 6574 3d22 7574 662d  pt-charset="utf-
-000008b0: 3822 3e0d 0a20 2020 2020 2020 203c 696e  8">..        <in
-000008c0: 7075 7420 7479 7065 3d22 6869 6464 656e  put type="hidden
-000008d0: 2220 6e61 6d65 3d22 6461 7461 2220 7661  " name="data" va
-000008e0: 6c75 653d 2265 7941 6964 6d56 7963 326c  lue="eyAidmVyc2l
-000008f0: 7662 6949 674f 6941 7a4c 4341 6963 4856  vbiIgOiAzLCAicHV
-00000900: 6962 476c 6a58 3274 6c65 5349 674f 6941  ibGljX2tleSIgOiA
-00000910: 6965 5739 3163 6c39 7764 574a 7361 574e  ieW91cl9wdWJsaWN
-00000920: 6661 3256 3549 6977 6749 6d46 6a64 476c  fa2V5IiwgImFjdGl
-00000930: 760d 0a20 2020 2020 2020 2062 6949 674f  v..        biIgO
-00000940: 6941 6963 4746 3549 6977 6749 6d46 7462  iAicGF5IiwgImFtb
-00000950: 3356 7564 4349 674f 6941 784c 4341 6959  3VudCIgOiAxLCAiY
-00000960: 3356 7963 6d56 7559 336b 6949 446f 6749  3VycmVuY3kiIDogI
-00000970: 6c56 5452 4349 7349 434a 6b5a 584e 6a63  lVTRCIsICJkZXNjc
-00000980: 6d6c 7764 476c 760d 0a20 2020 2020 2020  mlwdGlv..       
-00000990: 2062 6949 674f 6941 695a 4756 7a59 334a   biIgOiAiZGVzY3J
-000009a0: 7063 4852 7062 3234 6764 4756 3464 4349  pcHRpb24gdGV4dCI
-000009b0: 7349 434a 7663 6d52 6c63 6c39 705a 4349  sICJvcmRlcl9pZCI
-000009c0: 674f 6941 6962 334a 6b5a 584a 6661 5752  gOiAib3JkZXJfaWR
-000009d0: 664d 5349 6766 513d 3d22 2f3e 0d0a 2020  fMSIgfQ=="/>..  
-000009e0: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-000009f0: 653d 2268 6964 6465 6e22 206e 616d 653d  e="hidden" name=
-00000a00: 2273 6967 6e61 7475 7265 2220 7661 6c75  "signature" valu
-00000a10: 653d 2251 764a 4435 7539 4667 3535 5043  e="QvJD5u9Fg55PC
-00000a20: 782f 4864 7a36 6c7a 5774 5977 6349 3d22  x/Hdz6lzWtYwcI="
-00000a30: 2f3e 0d0a 2020 2020 2020 2020 3c69 6e70  />..        <inp
-00000a40: 7574 2074 7970 653d 2269 6d61 6765 220d  ut type="image".
-00000a50: 0a20 2020 2020 2020 2073 7263 3d22 2f2f  .        src="//
-00000a60: 7374 6174 6963 2e6c 6971 7061 792e 7561  static.liqpay.ua
-00000a70: 2f62 7574 746f 6e73 2f70 3172 752e 7261  /buttons/p1ru.ra
-00000a80: 6469 7573 2e70 6e67 222f 3e0d 0a20 2020  dius.png"/>..   
-00000a90: 203c 2f66 6f72 6d3e 0d0a 6060 600d 0a0d   </form>..```...
-00000aa0: 0a45 7861 6d70 6c65 2032 3a20 496e 7465  .Example 2: Inte
-00000ab0: 6772 6174 6520 5061 796d 656e 7420 7769  grate Payment wi
-00000ac0: 6467 6574 2074 6f20 446a 616e 676f 0d0a  dget to Django..
-00000ad0: 2d2d 2d2d 2d2d 2d0d 0a60 5061 796d 656e  -------..`Paymen
-00000ae0: 7420 7769 6467 6574 2064 6f63 756d 656e  t widget documen
-00000af0: 7461 7469 6f6e 6020 0d0a 6874 7470 733a  tation` ..https:
-00000b00: 2f2f 7777 772e 6c69 7170 6179 2e75 612f  //www.liqpay.ua/
-00000b10: 646f 6375 6d65 6e74 6174 696f 6e2f 656e  documentation/en
-00000b20: 2f61 7069 2f61 7175 6972 696e 672f 7769  /api/aquiring/wi
-00000b30: 6467 6574 2f0d 0a0d 0a2a 4261 636b 656e  dget/....*Backen
-00000b40: 642a 0d0a 0d0a 6076 6965 7773 2e70 7960  d*....`views.py`
-00000b50: 0d0a 0d0a 6060 600d 0a0d 0a20 2020 2066  ....```....    f
-00000b60: 726f 6d20 6c69 7170 6179 2069 6d70 6f72  rom liqpay impor
-00000b70: 7420 4c69 7150 6179 0d0a 0d0a 2020 2020  t LiqPay....    
-00000b80: 6672 6f6d 2064 6a61 6e67 6f2e 7669 6577  from django.view
-00000b90: 732e 6765 6e65 7269 6320 696d 706f 7274  s.generic import
-00000ba0: 2054 656d 706c 6174 6556 6965 770d 0a20   TemplateView.. 
-00000bb0: 2020 2066 726f 6d20 646a 616e 676f 2e73     from django.s
-00000bc0: 686f 7274 6375 7473 2069 6d70 6f72 7420  hortcuts import 
-00000bd0: 7265 6e64 6572 0d0a 2020 2020 6672 6f6d  render..    from
-00000be0: 2064 6a61 6e67 6f2e 6874 7470 2069 6d70   django.http imp
-00000bf0: 6f72 7420 4874 7470 5265 7370 6f6e 7365  ort HttpResponse
-00000c00: 0d0a 0d0a 2020 2020 636c 6173 7320 5061  ....    class Pa
-00000c10: 7956 6965 7728 5465 6d70 6c61 7465 5669  yView(TemplateVi
-00000c20: 6577 293a 0d0a 2020 2020 7465 6d70 6c61  ew):..    templa
-00000c30: 7465 5f6e 616d 6520 3d20 2762 696c 6c69  te_name = 'billi
-00000c40: 6e67 2f70 6179 2e68 746d 6c27 0d0a 0d0a  ng/pay.html'....
-00000c50: 2020 2020 6465 6620 6765 7428 7365 6c66      def get(self
-00000c60: 2c20 7265 7175 6573 742c 202a 6172 6773  , request, *args
-00000c70: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
-00000c80: 2020 2020 2020 6c69 7170 6179 203d 204c        liqpay = L
-00000c90: 6971 5061 7928 7365 7474 696e 6773 2e4c  iqPay(settings.L
-00000ca0: 4951 5041 595f 5055 424c 4943 5f4b 4559  IQPAY_PUBLIC_KEY
-00000cb0: 2c20 7365 7474 696e 6773 2e4c 4951 5041  , settings.LIQPA
-00000cc0: 595f 5052 4956 4154 455f 4b45 5929 0d0a  Y_PRIVATE_KEY)..
-00000cd0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-00000ce0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00000cf0: 2761 6374 696f 6e27 3a20 2770 6179 272c  'action': 'pay',
-00000d00: 0d0a 2020 2020 2020 2020 2020 2020 2761  ..            'a
-00000d10: 6d6f 756e 7427 3a20 2731 3030 272c 0d0a  mount': '100',..
-00000d20: 2020 2020 2020 2020 2020 2020 2763 7572              'cur
-00000d30: 7265 6e63 7927 3a20 2755 5344 272c 0d0a  rency': 'USD',..
-00000d40: 2020 2020 2020 2020 2020 2020 2764 6573              'des
-00000d50: 6372 6970 7469 6f6e 273a 2027 5061 796d  cription': 'Paym
-00000d60: 656e 7420 666f 7220 636c 6f74 6865 7327  ent for clothes'
-00000d70: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00000d80: 6f72 6465 725f 6964 273a 2027 6f72 6465  order_id': 'orde
-00000d90: 725f 6964 5f31 272c 0d0a 2020 2020 2020  r_id_1',..      
-00000da0: 2020 2020 2020 2776 6572 7369 6f6e 273a        'version':
-00000db0: 2027 3327 2c0d 0a20 2020 2020 2020 2020   '3',..         
-00000dc0: 2020 2027 7361 6e64 626f 7827 3a20 302c     'sandbox': 0,
-00000dd0: 2023 2073 616e 6462 6f78 206d 6f64 652c   # sandbox mode,
-00000de0: 2073 6574 2074 6f20 3120 746f 2065 6e61   set to 1 to ena
-00000df0: 626c 6520 6974 0d0a 2020 2020 2020 2020  ble it..        
-00000e00: 2020 2020 2773 6572 7665 725f 7572 6c27      'server_url'
-00000e10: 3a20 2768 7474 7073 3a2f 2f74 6573 742e  : 'https://test.
-00000e20: 636f 6d2f 6269 6c6c 696e 672f 7061 792d  com/billing/pay-
-00000e30: 6361 6c6c 6261 636b 2f27 2c20 2320 7572  callback/', # ur
-00000e40: 6c20 746f 2063 616c 6c62 6163 6b20 7669  l to callback vi
-00000e50: 6577 0d0a 2020 2020 2020 2020 7d0d 0a20  ew..        }.. 
-00000e60: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-00000e70: 203d 206c 6971 7061 792e 636e 625f 7369   = liqpay.cnb_si
-00000e80: 676e 6174 7572 6528 7061 7261 6d73 290d  gnature(params).
-00000e90: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00000ea0: 6c69 7170 6179 2e63 6e62 5f64 6174 6128  liqpay.cnb_data(
-00000eb0: 7061 7261 6d73 290d 0a20 2020 2020 2020  params)..       
-00000ec0: 2072 6574 7572 6e20 7265 6e64 6572 2872   return render(r
-00000ed0: 6571 7565 7374 2c20 7365 6c66 2e74 656d  equest, self.tem
-00000ee0: 706c 6174 655f 6e61 6d65 2c20 7b27 7369  plate_name, {'si
-00000ef0: 676e 6174 7572 6527 3a20 7369 676e 6174  gnature': signat
-00000f00: 7572 652c 2027 6461 7461 273a 2064 6174  ure, 'data': dat
-00000f10: 617d 290d 0a0d 0a20 2020 2040 6d65 7468  a})....    @meth
-00000f20: 6f64 5f64 6563 6f72 6174 6f72 2863 7372  od_decorator(csr
-00000f30: 665f 6578 656d 7074 2c20 6e61 6d65 3d27  f_exempt, name='
-00000f40: 6469 7370 6174 6368 2729 0d0a 2020 2020  dispatch')..    
-00000f50: 636c 6173 7320 5061 7943 616c 6c62 6163  class PayCallbac
-00000f60: 6b56 6965 7728 5669 6577 293a 0d0a 2020  kView(View):..  
-00000f70: 2020 2020 2020 6465 6620 706f 7374 2873        def post(s
-00000f80: 656c 662c 2072 6571 7565 7374 2c20 2a61  elf, request, *a
-00000f90: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
-00000fa0: 0a20 2020 2020 2020 2020 2020 206c 6971  .            liq
-00000fb0: 7061 7920 3d20 4c69 7150 6179 2873 6574  pay = LiqPay(set
-00000fc0: 7469 6e67 732e 4c49 5150 4159 5f50 5542  tings.LIQPAY_PUB
-00000fd0: 4c49 435f 4b45 592c 2073 6574 7469 6e67  LIC_KEY, setting
-00000fe0: 732e 4c49 5150 4159 5f50 5249 5641 5445  s.LIQPAY_PRIVATE
-00000ff0: 5f4b 4559 290d 0a20 2020 2020 2020 2020  _KEY)..         
-00001000: 2020 2064 6174 6120 3d20 7265 7175 6573     data = reques
-00001010: 742e 504f 5354 2e67 6574 2827 6461 7461  t.POST.get('data
-00001020: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00001030: 7369 676e 6174 7572 6520 3d20 7265 7175  signature = requ
-00001040: 6573 742e 504f 5354 2e67 6574 2827 7369  est.POST.get('si
-00001050: 676e 6174 7572 6527 290d 0a20 2020 2020  gnature')..     
-00001060: 2020 2020 2020 2073 6967 6e20 3d20 6c69         sign = li
-00001070: 7170 6179 2e73 7472 5f74 6f5f 7369 676e  qpay.str_to_sign
-00001080: 2873 6574 7469 6e67 732e 4c49 5150 4159  (settings.LIQPAY
-00001090: 5f50 5249 5641 5445 5f4b 4559 202b 2064  _PRIVATE_KEY + d
-000010a0: 6174 6120 2b20 7365 7474 696e 6773 2e4c  ata + settings.L
-000010b0: 4951 5041 595f 5052 4956 4154 455f 4b45  IQPAY_PRIVATE_KE
-000010c0: 5929 0d0a 2020 2020 2020 2020 2020 2020  Y)..            
-000010d0: 6966 2073 6967 6e20 3d3d 2073 6967 6e61  if sign == signa
-000010e0: 7475 7265 3a0d 0a20 2020 2020 2020 2020  ture:..         
-000010f0: 2020 2020 2020 2070 7269 6e74 2827 6361         print('ca
-00001100: 6c6c 6261 636b 2069 7320 7661 6c69 6427  llback is valid'
-00001110: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00001120: 6573 706f 6e73 6520 3d20 6c69 7170 6179  esponse = liqpay
-00001130: 2e64 6563 6f64 655f 6461 7461 5f66 726f  .decode_data_fro
-00001140: 6d5f 7374 7228 6461 7461 290d 0a20 2020  m_str(data)..   
-00001150: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00001160: 6361 6c6c 6261 636b 2064 6174 6127 2c20  callback data', 
-00001170: 7265 7370 6f6e 7365 290d 0a20 2020 2020  response)..     
-00001180: 2020 2020 2020 2072 6574 7572 6e20 4874         return Ht
-00001190: 7470 5265 7370 6f6e 7365 2829 0d0a 6060  tpResponse()..``
-000011a0: 600d 0a60 7572 6c73 2e70 7960 0d0a 0d0a  `..`urls.py`....
-000011b0: 6060 600d 0a0d 0a20 2020 2066 726f 6d20  ```....    from 
-000011c0: 646a 616e 676f 2e63 6f6e 662e 7572 6c73  django.conf.urls
-000011d0: 2069 6d70 6f72 7420 7572 6c0d 0a0d 0a20   import url.... 
-000011e0: 2020 2066 726f 6d20 6269 6c6c 696e 672e     from billing.
-000011f0: 7669 6577 7320 696d 706f 7274 2050 6179  views import Pay
-00001200: 5669 6577 2c20 5061 7943 616c 6c62 6163  View, PayCallbac
-00001210: 6b56 6965 770d 0a0d 0a0d 0a20 2020 2075  kView......    u
-00001220: 726c 7061 7474 6572 6e73 203d 205b 0d0a  rlpatterns = [..
-00001230: 2020 2020 2020 2020 7572 6c28 7227 5e70          url(r'^p
-00001240: 6179 2f24 272c 2050 6179 5669 6577 2e61  ay/$', PayView.a
-00001250: 735f 7669 6577 2829 2c20 6e61 6d65 3d27  s_view(), name='
-00001260: 7061 795f 7669 6577 2729 2c0d 0a20 2020  pay_view'),..   
-00001270: 2020 2020 2075 726c 2872 275e 7061 792d       url(r'^pay-
-00001280: 6361 6c6c 6261 636b 2f24 272c 2050 6179  callback/$', Pay
-00001290: 4361 6c6c 6261 636b 5669 6577 2e61 735f  CallbackView.as_
-000012a0: 7669 6577 2829 2c20 6e61 6d65 3d27 7061  view(), name='pa
-000012b0: 795f 6361 6c6c 6261 636b 2729 2c0d 0a20  y_callback'),.. 
-000012c0: 2020 205d 0d0a 6060 600d 0a2a 4672 6f6e     ]..```..*Fron
-000012d0: 7465 6e64 2a0d 0a0d 0a60 6060 0d0a 0d0a  tend*....```....
-000012e0: 2020 2020 3c64 6976 2069 643d 226c 6971      <div id="liq
-000012f0: 7061 795f 6368 6563 6b6f 7574 223e 3c2f  pay_checkout"></
-00001300: 6469 763e 0d0a 2020 2020 3c73 6372 6970  div>..    <scrip
-00001310: 743e 0d0a 2020 2020 2020 2020 7769 6e64  t>..        wind
-00001320: 6f77 2e4c 6971 5061 7943 6865 636b 6f75  ow.LiqPayCheckou
-00001330: 7443 616c 6c62 6163 6b20 3d20 6675 6e63  tCallback = func
-00001340: 7469 6f6e 2829 207b 0d0a 2020 2020 2020  tion() {..      
-00001350: 2020 2020 2020 4c69 7150 6179 4368 6563        LiqPayChec
-00001360: 6b6f 7574 2e69 6e69 7428 7b0d 0a20 2020  kout.init({..   
-00001370: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00001380: 613a 2022 7b7b 2064 6174 6120 7d7d 222c  a: "{{ data }}",
-00001390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000013a0: 2020 7369 676e 6174 7572 653a 2022 7b7b    signature: "{{
-000013b0: 2073 6967 6e61 7475 7265 207d 7d22 2c0d   signature }}",.
-000013c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013d0: 2065 6d62 6564 546f 3a20 2223 6c69 7170   embedTo: "#liqp
-000013e0: 6179 5f63 6865 636b 6f75 7422 2c0d 0a20  ay_checkout",.. 
-000013f0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00001400: 6f64 653a 2022 656d 6265 6422 202f 2f20  ode: "embed" // 
-00001410: 656d 6265 6420 7c7c 2070 6f70 7570 2c0d  embed || popup,.
-00001420: 0a20 2020 2020 2020 2020 2020 207d 292e  .            }).
-00001430: 6f6e 2822 6c69 7170 6179 2e63 616c 6c62  on("liqpay.callb
-00001440: 6163 6b22 2c20 6675 6e63 7469 6f6e 2864  ack", function(d
-00001450: 6174 6129 7b0d 0a20 2020 2020 2020 2020  ata){..         
-00001460: 2020 2020 2020 2063 6f6e 736f 6c65 2e6c         console.l
-00001470: 6f67 2864 6174 612e 7374 6174 7573 293b  og(data.status);
-00001480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001490: 2020 636f 6e73 6f6c 652e 6c6f 6728 6461    console.log(da
-000014a0: 7461 293b 0d0a 2020 2020 2020 2020 2020  ta);..          
-000014b0: 2020 7d29 2e6f 6e28 226c 6971 7061 792e    }).on("liqpay.
-000014c0: 7265 6164 7922 2c20 6675 6e63 7469 6f6e  ready", function
-000014d0: 2864 6174 6129 7b0d 0a20 2020 2020 2020  (data){..       
-000014e0: 2020 2020 2020 2020 202f 2f20 7265 6164           // read
-000014f0: 790d 0a20 2020 2020 2020 2020 2020 207d  y..            }
-00001500: 292e 6f6e 2822 6c69 7170 6179 2e63 6c6f  ).on("liqpay.clo
-00001510: 7365 222c 2066 756e 6374 696f 6e28 6461  se", function(da
-00001520: 7461 297b 0d0a 2020 2020 2020 2020 2020  ta){..          
-00001530: 2020 2020 2020 2f2f 2063 6c6f 7365 0d0a        // close..
-00001540: 2020 2020 2020 2020 2020 2020 7d29 3b0d              });.
-00001550: 0a20 2020 2020 2020 207d 3b0d 0a20 2020  .        };..   
-00001560: 203c 2f73 6372 6970 743e 0d0a 2020 2020   </script>..    
-00001570: 3c73 6372 6970 7420 7372 633d 222f 2f73  <script src="//s
-00001580: 7461 7469 632e 6c69 7170 6179 2e75 612f  tatic.liqpay.ua/
-00001590: 6c69 626a 732f 6368 6563 6b6f 7574 2e6a  libjs/checkout.j
-000015a0: 7322 2061 7379 6e63 3e3c 2f73 6372 6970  s" async></scrip
-000015b0: 743e 0d0a 6060 600d 0a                   t>..```..
+00000000: 5b21 5b50 7974 686f 6e20 332e 362b 5d28  [![Python 3.6+](
+00000010: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000020: 6c64 732e 696f 2f62 6164 6765 2f70 7974  lds.io/badge/pyt
+00000030: 686f 6e2d 332e 362b 2d62 6c75 652e 7376  hon-3.6+-blue.sv
+00000040: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
+00000050: 7079 7468 6f6e 2e6f 7267 2f64 6f77 6e6c  python.org/downl
+00000060: 6f61 6473 2f72 656c 6561 7365 2f70 7974  oads/release/pyt
+00000070: 686f 6e2d 3336 302f 290d 0a0d 0a5b 215b  hon-360/)....[![
+00000080: 5344 4b2d 5079 7468 6f6e 335d 2868 7474  SDK-Python3](htt
+00000090: 7073 3a2f 2f77 7777 2e6c 6971 7061 792e  ps://www.liqpay.
+000000a0: 7561 2f6c 6f67 6f5f 6c69 7170 6179 5f6d  ua/logo_liqpay_m
+000000b0: 6169 6e2e 7376 6729 5d28 6874 7470 733a  ain.svg)](https:
+000000c0: 2f2f 7777 772e 6c69 7170 6179 2e75 612f  //www.liqpay.ua/
+000000d0: 646f 6375 6d65 6e74 6174 696f 6e2f 6170  documentation/ap
+000000e0: 692f 686f 6d65 290d 0a0d 0a2a 2057 6562  i/home)....* Web
+000000f0: 3a20 6874 7470 733a 2f2f 7777 772e 6c69  : https://www.li
+00000100: 7170 6179 2e75 612f 0d0a 2a20 446f 776e  qpay.ua/..* Down
+00000110: 6c6f 6164 3a20 6874 7470 733a 2f2f 7079  load: https://py
+00000120: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6c  pi.org/project/l
+00000130: 6971 7061 792d 7364 6b2d 7079 7468 6f6e  iqpay-sdk-python
+00000140: 332f 0d0a 2a20 536f 7572 6365 3a20 6874  3/..* Source: ht
+00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000160: 2f61 6f72 7a68 2f6c 6971 7061 792d 7364  /aorzh/liqpay-sd
+00000170: 6b2d 7079 7468 6f6e 330d 0a2a 2044 6f63  k-python3..* Doc
+00000180: 756d 656e 7461 7469 6f6e 3a20 6874 7470  umentation: http
+00000190: 733a 2f2f 7777 772e 6c69 7170 6179 2e75  s://www.liqpay.u
+000001a0: 612f 646f 6375 6d65 6e74 6174 696f 6e2f  a/documentation/
+000001b0: 656e 2f0d 0a2a 204b 6579 776f 7264 733a  en/..* Keywords:
+000001c0: 206c 6971 7061 792c 2070 7269 7661 7432   liqpay, privat2
+000001d0: 342c 2070 7269 7661 7462 616e 6b2c 2070  4, privatbank, p
+000001e0: 7974 686f 6e2c 2069 6e74 6572 6e65 7420  ython, internet 
+000001f0: 6163 7175 6972 696e 672c 2050 3250 2070  acquiring, P2P p
+00000200: 6179 6d65 6e74 732c 2074 776f 2d73 7465  ayments, two-ste
+00000210: 7020 7061 796d 656e 7473 0d0a 0d0a 0d0a  p payments......
+00000220: 5768 6174 2070 7974 686f 6e20 7665 7273  What python vers
+00000230: 696f 6e20 6973 2073 7570 706f 7274 6564  ion is supported
+00000240: 3f0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  ?..============.
+00000250: 0a2d 2050 7974 686f 6e20 332e 342b 0d0a  .- Python 3.4+..
+00000260: 0d0a 4765 7420 5374 6172 7465 640d 0a3d  ..Get Started..=
+00000270: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a31 2e20  ===========..1. 
+00000280: 5369 676e 2075 7020 696e 2068 7474 7073  Sign up in https
+00000290: 3a2f 2f77 7777 2e6c 6971 7061 792e 7561  ://www.liqpay.ua
+000002a0: 2f65 6e2f 6175 7468 6f72 697a 6174 696f  /en/authorizatio
+000002b0: 6e2e 0d0a 322e 2043 7265 6174 6520 6120  n...2. Create a 
+000002c0: 636f 6d70 616e 792e 0d0a 332e 2049 6e20  company...3. In 
+000002d0: 636f 6d70 616e 7920 7365 7474 696e 6773  company settings
+000002e0: 2c20 6f6e 2041 5049 2074 6162 2c20 6765  , on API tab, ge
+000002f0: 7420 2a2a 5075 626c 6963 206b 6579 2a2a  t **Public key**
+00000300: 2061 6e64 202a 2a50 7269 7661 7465 206b   and **Private k
+00000310: 6579 2a2a 2e0d 0a34 2e20 446f 6e65 2e0d  ey**...4. Done..
+00000320: 0a0d 0a49 6e73 7461 6c6c 6174 696f 6e0d  ...Installation.
+00000330: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a46  .============..F
+00000340: 726f 6d20 7069 700d 0a60 6060 7069 7020  rom pip..```pip 
+00000350: 696e 7374 616c 6c20 6c69 7170 6179 2d73  install liqpay-s
+00000360: 646b 2d70 7974 686f 6e33 6060 600d 0a0d  dk-python3```...
+00000370: 0a57 6f72 6b69 6e67 2077 6974 6820 4c69  .Working with Li
+00000380: 7150 6179 2043 616c 6c62 6163 6b20 6c6f  qPay Callback lo
+00000390: 6361 6c6c 790d 0a3d 3d3d 3d3d 3d3d 3d3d  cally..=========
+000003a0: 3d3d 3d0d 0a49 6620 796f 7520 6e65 6564  ===..If you need
+000003b0: 2064 6562 7567 6769 6e67 2041 5049 2043   debugging API C
+000003c0: 616c 6c62 6163 6b20 6f6e 206c 6f63 616c  allback on local
+000003d0: 2065 6e76 6972 6f6e 6d65 6e74 2075 7365   environment use
+000003e0: 2068 7474 7073 3a2f 2f6c 6f63 616c 7475   https://localtu
+000003f0: 6e6e 656c 2e67 6974 6875 622e 696f 2f77  nnel.github.io/w
+00000400: 7777 2f0d 0a0d 0a48 6f77 2069 7420 7573  ww/....How it us
+00000410: 6573 3f0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  es?..===========
+00000420: 3d0d 0a0d 0a45 7861 6d70 6c65 2031 3a20  =....Example 1: 
+00000430: 4261 7369 630d 0a2d 2d2d 2d2d 2d2d 0d0a  Basic..-------..
+00000440: 0d0a 2a2a 4261 636b 656e 642a 2a0d 0a47  ..**Backend**..G
+00000450: 6574 2070 6179 6d65 6e74 2062 7574 746f  et payment butto
+00000460: 6e20 2868 746d 6c20 7265 7370 6f6e 7365  n (html response
+00000470: 290d 0a60 6060 0d0a 6c69 7170 6179 203d  )..```..liqpay =
+00000480: 204c 6971 5061 7928 7075 626c 6963 5f6b   LiqPay(public_k
+00000490: 6579 2c20 7072 6976 6174 655f 6b65 7929  ey, private_key)
+000004a0: 0d0a 6874 6d6c 203d 206c 6971 7061 792e  ..html = liqpay.
+000004b0: 636e 625f 666f 726d 287b 0d0a 2020 2020  cnb_form({..    
+000004c0: 2761 6374 696f 6e27 3a20 2770 6179 272c  'action': 'pay',
+000004d0: 0d0a 2020 2020 2761 6d6f 756e 7427 3a20  ..    'amount': 
+000004e0: 2731 272c 0d0a 2020 2020 2763 7572 7265  '1',..    'curre
+000004f0: 6e63 7927 3a20 2755 5344 272c 0d0a 2020  ncy': 'USD',..  
+00000500: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
+00000510: 2027 6465 7363 7269 7074 696f 6e20 7465   'description te
+00000520: 7874 272c 0d0a 2020 2020 276f 7264 6572  xt',..    'order
+00000530: 5f69 6427 3a20 276f 7264 6572 5f69 645f  _id': 'order_id_
+00000540: 3127 2c0d 0a20 2020 2027 7665 7273 696f  1',..    'versio
+00000550: 6e27 3a20 2733 272c 0d0a 2020 2020 276c  n': '3',..    'l
+00000560: 616e 6775 6167 6527 3a20 2772 757c 756b  anguage': 'ru|uk
+00000570: 7c65 6e27 0d0a 7d29 0d0a 6060 600d 0a0d  |en'..})..```...
+00000580: 0a47 6574 2070 6c61 696e 2063 6865 636b  .Get plain check
+00000590: 6f75 7420 7572 6c3a 0d0a 0d0a 6060 600d  out url:....```.
+000005a0: 0a6c 6971 7061 7920 3d20 4c69 7150 6179  .liqpay = LiqPay
+000005b0: 2870 7562 6c69 635f 6b65 792c 2070 7269  (public_key, pri
+000005c0: 7661 7465 5f6b 6579 290d 0a68 746d 6c20  vate_key)..html 
+000005d0: 3d20 6c69 7170 6179 2e63 6865 636b 6f75  = liqpay.checkou
+000005e0: 745f 7572 6c28 7b0d 0a20 2020 2027 6163  t_url({..    'ac
+000005f0: 7469 6f6e 273a 2027 6175 7468 272c 0d0a  tion': 'auth',..
+00000600: 2020 2020 2761 6d6f 756e 7427 3a20 2731      'amount': '1
+00000610: 272c 0d0a 2020 2020 2763 7572 7265 6e63  ',..    'currenc
+00000620: 7927 3a20 2755 5344 272c 0d0a 2020 2020  y': 'USD',..    
+00000630: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
+00000640: 6465 7363 7269 7074 696f 6e20 7465 7874  description text
+00000650: 272c 0d0a 2020 2020 276f 7264 6572 5f69  ',..    'order_i
+00000660: 6427 3a20 276f 7264 6572 5f69 645f 3127  d': 'order_id_1'
+00000670: 2c0d 0a20 2020 2027 7665 7273 696f 6e27  ,..    'version'
+00000680: 3a20 2733 272c 0d0a 2020 2020 276c 616e  : '3',..    'lan
+00000690: 6775 6167 6527 3a20 2772 757c 756b 7c65  guage': 'ru|uk|e
+000006a0: 6e27 2c0d 0a20 2020 2027 7265 6375 7272  n',..    'recurr
+000006b0: 696e 6762 7974 6f6b 656e 273a 2027 3127  ingbytoken': '1'
+000006c0: 0d0a 7d29 0d0a 2320 5265 7370 6f6e 7365  ..})..# Response
+000006d0: 3a0d 0a0d 0a73 7472 3a20 6874 7470 733a  :....str: https:
+000006e0: 2f2f 7777 772e 6c69 7170 6179 2e75 612f  //www.liqpay.ua/
+000006f0: 6170 692f 332f 6368 6563 6b6f 7574 2f3f  api/3/checkout/?
+00000700: 6461 7461 3d3c 6465 636f 6465 6420 6461  data=<decoded da
+00000710: 7461 3e26 7369 676e 6174 7572 653d 3c64  ta>&signature=<d
+00000720: 6563 6f64 6564 2073 6967 6e61 7475 7265  ecoded signature
+00000730: 3e0d 0a0d 0a60 6060 0d0a 0d0a 0d0a 2a2a  >....```......**
+00000740: 4672 6f6e 7465 6e64 2a2a 0d0a 0d0a 5661  Frontend**....Va
+00000750: 7269 6162 6c65 2060 6068 746d 6c60 6020  riable ``html`` 
+00000760: 7769 6c6c 2063 6f6e 7461 696e 206e 6578  will contain nex
+00000770: 7420 6874 6d6c 2066 6f72 6d0d 0a0d 0a60  t html form....`
+00000780: 6060 0d0a 2020 2020 3c66 6f72 6d20 6d65  ``..    <form me
+00000790: 7468 6f64 3d22 504f 5354 2220 6163 7469  thod="POST" acti
+000007a0: 6f6e 3d22 6874 7470 733a 2f2f 7777 772e  on="https://www.
+000007b0: 6c69 7170 6179 2e75 612f 6170 692f 332f  liqpay.ua/api/3/
+000007c0: 6368 6563 6b6f 7574 2f22 2061 6363 6570  checkout/" accep
+000007d0: 742d 6368 6172 7365 743d 2275 7466 2d38  t-charset="utf-8
+000007e0: 223e 0d0a 2020 2020 2020 2020 203c 696e  ">..         <in
+000007f0: 7075 7420 7479 7065 3d27 6869 6464 656e  put type='hidden
+00000800: 2720 6e61 6d65 3d27 6461 7461 2720 7661  ' name='data' va
+00000810: 6c75 653d 2765 794a 6862 5739 3162 6e51  lue='eyJhbW91bnQ
+00000820: 694f 692e 2e2e 3d27 2f3e 0d0a 2020 2020  iOi...='/>..    
+00000830: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
+00000840: 3d27 6869 6464 656e 2720 6e61 6d65 3d27  ='hidden' name='
+00000850: 7369 676e 6174 7572 6527 2076 616c 7565  signature' value
+00000860: 3d27 6564 5573 342e 2e2e 3d27 2f3e 0d0a  ='edUs4...='/>..
+00000870: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
+00000880: 2073 7479 6c65 3d22 626f 7264 6572 3a20   style="border: 
+00000890: 6e6f 6e65 2021 696d 706f 7274 616e 743b  none !important;
+000008a0: 6469 7370 6c61 793a 696e 6c69 6e65 2d62  display:inline-b
+000008b0: 6c6f 636b 2021 696d 706f 7274 616e 743b  lock !important;
+000008c0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000008d0: 6572 2021 696d 706f 7274 616e 743b 2070  er !important; p
+000008e0: 6164 6469 6e67 3a20 3770 7820 3230 7078  adding: 7px 20px
+000008f0: 2021 696d 706f 7274 616e 743b 2063 6f6c   !important; col
+00000900: 6f72 3a20 2366 6666 2021 696d 706f 7274  or: #fff !import
+00000910: 616e 743b 666f 6e74 2d73 697a 653a 3136  ant;font-size:16
+00000920: 7078 2021 696d 706f 7274 616e 743b 2066  px !important; f
+00000930: 6f6e 742d 7765 6967 6874 3a20 3630 3020  ont-weight: 600 
+00000940: 2169 6d70 6f72 7461 6e74 3b20 666f 6e74  !important; font
+00000950: 2d66 616d 696c 793a 4f70 656e 5361 6e73  -family:OpenSans
+00000960: 2c20 7361 6e73 2d73 6572 6966 3b63 7572  , sans-serif;cur
+00000970: 736f 723a 2070 6f69 6e74 6572 2021 696d  sor: pointer !im
+00000980: 706f 7274 616e 743b 626f 7264 6572 2d72  portant;border-r
+00000990: 6164 6975 733a 2032 7078 2021 696d 706f  adius: 2px !impo
+000009a0: 7274 616e 743b 6261 636b 6772 6f75 6e64  rtant;background
+000009b0: 3a20 7267 6261 2831 3232 2c31 3833 2c34  : rgba(122,183,4
+000009c0: 332c 3129 2021 696d 706f 7274 616e 743b  3,1) !important;
+000009d0: 226f 6e6d 6f75 7365 6f76 6572 3d22 7468  "onmouseover="th
+000009e0: 6973 2e73 7479 6c65 2e6f 7061 6369 7479  is.style.opacity
+000009f0: 3d30 2e35 3b22 206f 6e6d 6f75 7365 6f75  =0.5;" onmouseou
+00000a00: 743d 2274 6869 732e 7374 796c 652e 6f70  t="this.style.op
+00000a10: 6163 6974 793d 313b 223e 203c 696d 6720  acity=1;"> <img 
+00000a20: 7372 633d 2268 7474 7073 3a2f 2f73 7461  src="https://sta
+00000a30: 7469 632e 6c69 7170 6179 2e75 612f 6275  tic.liqpay.ua/bu
+00000a40: 7474 6f6e 732f 6c6f 676f 2d73 6d61 6c6c  ttons/logo-small
+00000a50: 2e70 6e67 2220 6e61 6d65 3d22 6274 6e5f  .png" name="btn_
+00000a60: 7465 7874 2220 7374 796c 653d 226d 6172  text" style="mar
+00000a70: 6769 6e2d 7269 6768 743a 2037 7078 2021  gin-right: 7px !
+00000a80: 696d 706f 7274 616e 743b 2076 6572 7469  important; verti
+00000a90: 6361 6c2d 616c 6967 6e3a 206d 6964 646c  cal-align: middl
+00000aa0: 6520 2169 6d70 6f72 7461 6e74 3b22 2f3e  e !important;"/>
+00000ab0: 200d 0a20 2020 2020 2020 2020 3c73 7061   ..         <spa
+00000ac0: 6e20 7374 796c 653d 2276 6572 7469 6361  n style="vertica
+00000ad0: 6c2d 616c 6967 6e3a 6d69 6464 6c65 3b21  l-align:middle;!
+00000ae0: 696d 706f 7274 616e 7422 3e50 4159 2031  important">PAY 1
+00000af0: 3030 2055 4148 3c2f 7370 616e 3e0d 0a20  00 UAH</span>.. 
+00000b00: 2020 2020 2020 2020 3c2f 6275 7474 6f6e          </button
+00000b10: 3e0d 0a20 2020 203c 2f66 6f72 6d3e 0d0a  >..    </form>..
+00000b20: 6060 600d 0a0d 0a45 7861 6d70 6c65 2032  ```....Example 2
+00000b30: 3a20 496e 7465 6772 6174 6520 5061 796d  : Integrate Paym
+00000b40: 656e 7420 7769 6467 6574 2074 6f20 446a  ent widget to Dj
+00000b50: 616e 676f 0d0a 2d2d 2d2d 2d2d 2d0d 0a60  ango..-------..`
+00000b60: 5061 796d 656e 7420 7769 6467 6574 2064  Payment widget d
+00000b70: 6f63 756d 656e 7461 7469 6f6e 6020 0d0a  ocumentation` ..
+00000b80: 6874 7470 733a 2f2f 7777 772e 6c69 7170  https://www.liqp
+00000b90: 6179 2e75 612f 646f 6375 6d65 6e74 6174  ay.ua/documentat
+00000ba0: 696f 6e2f 656e 2f61 7069 2f61 7175 6972  ion/en/api/aquir
+00000bb0: 696e 672f 7769 6467 6574 2f0d 0a0d 0a2a  ing/widget/....*
+00000bc0: 4261 636b 656e 642a 0d0a 0d0a 6076 6965  Backend*....`vie
+00000bd0: 7773 2e70 7960 0d0a 0d0a 6060 600d 0a0d  ws.py`....```...
+00000be0: 0a20 2020 2066 726f 6d20 6c69 7170 6179  .    from liqpay
+00000bf0: 2069 6d70 6f72 7420 4c69 7150 6179 0d0a   import LiqPay..
+00000c00: 0d0a 2020 2020 6672 6f6d 2064 6a61 6e67  ..    from djang
+00000c10: 6f2e 7669 6577 732e 6765 6e65 7269 6320  o.views.generic 
+00000c20: 696d 706f 7274 2054 656d 706c 6174 6556  import TemplateV
+00000c30: 6965 770d 0a20 2020 2066 726f 6d20 646a  iew..    from dj
+00000c40: 616e 676f 2e73 686f 7274 6375 7473 2069  ango.shortcuts i
+00000c50: 6d70 6f72 7420 7265 6e64 6572 0d0a 2020  mport render..  
+00000c60: 2020 6672 6f6d 2064 6a61 6e67 6f2e 6874    from django.ht
+00000c70: 7470 2069 6d70 6f72 7420 4874 7470 5265  tp import HttpRe
+00000c80: 7370 6f6e 7365 0d0a 0d0a 2020 2020 636c  sponse....    cl
+00000c90: 6173 7320 5061 7956 6965 7728 5465 6d70  ass PayView(Temp
+00000ca0: 6c61 7465 5669 6577 293a 0d0a 2020 2020  lateView):..    
+00000cb0: 7465 6d70 6c61 7465 5f6e 616d 6520 3d20  template_name = 
+00000cc0: 2762 696c 6c69 6e67 2f70 6179 2e68 746d  'billing/pay.htm
+00000cd0: 6c27 0d0a 0d0a 2020 2020 6465 6620 6765  l'....    def ge
+00000ce0: 7428 7365 6c66 2c20 7265 7175 6573 742c  t(self, request,
+00000cf0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00000d00: 293a 0d0a 2020 2020 2020 2020 6c69 7170  ):..        liqp
+00000d10: 6179 203d 204c 6971 5061 7928 7365 7474  ay = LiqPay(sett
+00000d20: 696e 6773 2e4c 4951 5041 595f 5055 424c  ings.LIQPAY_PUBL
+00000d30: 4943 5f4b 4559 2c20 7365 7474 696e 6773  IC_KEY, settings
+00000d40: 2e4c 4951 5041 595f 5052 4956 4154 455f  .LIQPAY_PRIVATE_
+00000d50: 4b45 5929 0d0a 2020 2020 2020 2020 7061  KEY)..        pa
+00000d60: 7261 6d73 203d 207b 0d0a 2020 2020 2020  rams = {..      
+00000d70: 2020 2020 2020 2761 6374 696f 6e27 3a20        'action': 
+00000d80: 2770 6179 272c 0d0a 2020 2020 2020 2020  'pay',..        
+00000d90: 2020 2020 2761 6d6f 756e 7427 3a20 2731      'amount': '1
+00000da0: 3030 272c 0d0a 2020 2020 2020 2020 2020  00',..          
+00000db0: 2020 2763 7572 7265 6e63 7927 3a20 2755    'currency': 'U
+00000dc0: 5344 272c 0d0a 2020 2020 2020 2020 2020  SD',..          
+00000dd0: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
+00000de0: 2027 5061 796d 656e 7420 666f 7220 636c   'Payment for cl
+00000df0: 6f74 6865 7327 2c0d 0a20 2020 2020 2020  othes',..       
+00000e00: 2020 2020 2027 6f72 6465 725f 6964 273a       'order_id':
+00000e10: 2027 6f72 6465 725f 6964 5f31 272c 0d0a   'order_id_1',..
+00000e20: 2020 2020 2020 2020 2020 2020 2776 6572              'ver
+00000e30: 7369 6f6e 273a 2027 3327 2c0d 0a20 2020  sion': '3',..   
+00000e40: 2020 2020 2020 2020 2027 7361 6e64 626f           'sandbo
+00000e50: 7827 3a20 302c 2023 2073 616e 6462 6f78  x': 0, # sandbox
+00000e60: 206d 6f64 652c 2073 6574 2074 6f20 3120   mode, set to 1 
+00000e70: 746f 2065 6e61 626c 6520 6974 0d0a 2020  to enable it..  
+00000e80: 2020 2020 2020 2020 2020 2773 6572 7665            'serve
+00000e90: 725f 7572 6c27 3a20 2768 7474 7073 3a2f  r_url': 'https:/
+00000ea0: 2f74 6573 742e 636f 6d2f 6269 6c6c 696e  /test.com/billin
+00000eb0: 672f 7061 792d 6361 6c6c 6261 636b 2f27  g/pay-callback/'
+00000ec0: 2c20 2320 7572 6c20 746f 2063 616c 6c62  , # url to callb
+00000ed0: 6163 6b20 7669 6577 0d0a 2020 2020 2020  ack view..      
+00000ee0: 2020 7d0d 0a20 2020 2020 2020 2073 6967    }..        sig
+00000ef0: 6e61 7475 7265 203d 206c 6971 7061 792e  nature = liqpay.
+00000f00: 636e 625f 7369 676e 6174 7572 6528 7061  cnb_signature(pa
+00000f10: 7261 6d73 290d 0a20 2020 2020 2020 2064  rams)..        d
+00000f20: 6174 6120 3d20 6c69 7170 6179 2e63 6e62  ata = liqpay.cnb
+00000f30: 5f64 6174 6128 7061 7261 6d73 290d 0a20  _data(params).. 
+00000f40: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00000f50: 6e64 6572 2872 6571 7565 7374 2c20 7365  nder(request, se
+00000f60: 6c66 2e74 656d 706c 6174 655f 6e61 6d65  lf.template_name
+00000f70: 2c20 7b27 7369 676e 6174 7572 6527 3a20  , {'signature': 
+00000f80: 7369 676e 6174 7572 652c 2027 6461 7461  signature, 'data
+00000f90: 273a 2064 6174 617d 290d 0a0d 0a20 2020  ': data})....   
+00000fa0: 2040 6d65 7468 6f64 5f64 6563 6f72 6174   @method_decorat
+00000fb0: 6f72 2863 7372 665f 6578 656d 7074 2c20  or(csrf_exempt, 
+00000fc0: 6e61 6d65 3d27 6469 7370 6174 6368 2729  name='dispatch')
+00000fd0: 0d0a 2020 2020 636c 6173 7320 5061 7943  ..    class PayC
+00000fe0: 616c 6c62 6163 6b56 6965 7728 5669 6577  allbackView(View
+00000ff0: 293a 0d0a 2020 2020 2020 2020 6465 6620  ):..        def 
+00001000: 706f 7374 2873 656c 662c 2072 6571 7565  post(self, reque
+00001010: 7374 2c20 2a61 7267 732c 202a 2a6b 7761  st, *args, **kwa
+00001020: 7267 7329 3a0d 0a20 2020 2020 2020 2020  rgs):..         
+00001030: 2020 206c 6971 7061 7920 3d20 4c69 7150     liqpay = LiqP
+00001040: 6179 2873 6574 7469 6e67 732e 4c49 5150  ay(settings.LIQP
+00001050: 4159 5f50 5542 4c49 435f 4b45 592c 2073  AY_PUBLIC_KEY, s
+00001060: 6574 7469 6e67 732e 4c49 5150 4159 5f50  ettings.LIQPAY_P
+00001070: 5249 5641 5445 5f4b 4559 290d 0a20 2020  RIVATE_KEY)..   
+00001080: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+00001090: 7265 7175 6573 742e 504f 5354 2e67 6574  request.POST.get
+000010a0: 2827 6461 7461 2729 0d0a 2020 2020 2020  ('data')..      
+000010b0: 2020 2020 2020 7369 676e 6174 7572 6520        signature 
+000010c0: 3d20 7265 7175 6573 742e 504f 5354 2e67  = request.POST.g
+000010d0: 6574 2827 7369 676e 6174 7572 6527 290d  et('signature').
+000010e0: 0a20 2020 2020 2020 2020 2020 2073 6967  .            sig
+000010f0: 6e20 3d20 6c69 7170 6179 2e73 7472 5f74  n = liqpay.str_t
+00001100: 6f5f 7369 676e 2873 6574 7469 6e67 732e  o_sign(settings.
+00001110: 4c49 5150 4159 5f50 5249 5641 5445 5f4b  LIQPAY_PRIVATE_K
+00001120: 4559 202b 2064 6174 6120 2b20 7365 7474  EY + data + sett
+00001130: 696e 6773 2e4c 4951 5041 595f 5052 4956  ings.LIQPAY_PRIV
+00001140: 4154 455f 4b45 5929 0d0a 2020 2020 2020  ATE_KEY)..      
+00001150: 2020 2020 2020 6966 2073 6967 6e20 3d3d        if sign ==
+00001160: 2073 6967 6e61 7475 7265 3a0d 0a20 2020   signature:..   
+00001170: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00001180: 6e74 2827 6361 6c6c 6261 636b 2069 7320  nt('callback is 
+00001190: 7661 6c69 6427 290d 0a20 2020 2020 2020  valid')..       
+000011a0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+000011b0: 6c69 7170 6179 2e64 6563 6f64 655f 6461  liqpay.decode_da
+000011c0: 7461 5f66 726f 6d5f 7374 7228 6461 7461  ta_from_str(data
+000011d0: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+000011e0: 7269 6e74 2827 6361 6c6c 6261 636b 2064  rint('callback d
+000011f0: 6174 6127 2c20 7265 7370 6f6e 7365 290d  ata', response).
+00001200: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00001210: 7572 6e20 4874 7470 5265 7370 6f6e 7365  urn HttpResponse
+00001220: 2829 0d0a 6060 600d 0a60 7572 6c73 2e70  ()..```..`urls.p
+00001230: 7960 0d0a 0d0a 6060 600d 0a0d 0a20 2020  y`....```....   
+00001240: 2066 726f 6d20 646a 616e 676f 2e63 6f6e   from django.con
+00001250: 662e 7572 6c73 2069 6d70 6f72 7420 7572  f.urls import ur
+00001260: 6c0d 0a0d 0a20 2020 2066 726f 6d20 6269  l....    from bi
+00001270: 6c6c 696e 672e 7669 6577 7320 696d 706f  lling.views impo
+00001280: 7274 2050 6179 5669 6577 2c20 5061 7943  rt PayView, PayC
+00001290: 616c 6c62 6163 6b56 6965 770d 0a0d 0a0d  allbackView.....
+000012a0: 0a20 2020 2075 726c 7061 7474 6572 6e73  .    urlpatterns
+000012b0: 203d 205b 0d0a 2020 2020 2020 2020 7572   = [..        ur
+000012c0: 6c28 7227 5e70 6179 2f24 272c 2050 6179  l(r'^pay/$', Pay
+000012d0: 5669 6577 2e61 735f 7669 6577 2829 2c20  View.as_view(), 
+000012e0: 6e61 6d65 3d27 7061 795f 7669 6577 2729  name='pay_view')
+000012f0: 2c0d 0a20 2020 2020 2020 2075 726c 2872  ,..        url(r
+00001300: 275e 7061 792d 6361 6c6c 6261 636b 2f24  '^pay-callback/$
+00001310: 272c 2050 6179 4361 6c6c 6261 636b 5669  ', PayCallbackVi
+00001320: 6577 2e61 735f 7669 6577 2829 2c20 6e61  ew.as_view(), na
+00001330: 6d65 3d27 7061 795f 6361 6c6c 6261 636b  me='pay_callback
+00001340: 2729 2c0d 0a20 2020 205d 0d0a 6060 600d  '),..    ]..```.
+00001350: 0a2a 4672 6f6e 7465 6e64 2a0d 0a0d 0a60  .*Frontend*....`
+00001360: 6060 0d0a 0d0a 2020 2020 3c64 6976 2069  ``....    <div i
+00001370: 643d 226c 6971 7061 795f 6368 6563 6b6f  d="liqpay_checko
+00001380: 7574 223e 3c2f 6469 763e 0d0a 2020 2020  ut"></div>..    
+00001390: 3c73 6372 6970 743e 0d0a 2020 2020 2020  <script>..      
+000013a0: 2020 7769 6e64 6f77 2e4c 6971 5061 7943    window.LiqPayC
+000013b0: 6865 636b 6f75 7443 616c 6c62 6163 6b20  heckoutCallback 
+000013c0: 3d20 6675 6e63 7469 6f6e 2829 207b 0d0a  = function() {..
+000013d0: 2020 2020 2020 2020 2020 2020 4c69 7150              LiqP
+000013e0: 6179 4368 6563 6b6f 7574 2e69 6e69 7428  ayCheckout.init(
+000013f0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00001400: 2020 2064 6174 613a 2022 7b7b 2064 6174     data: "{{ dat
+00001410: 6120 7d7d 222c 0d0a 2020 2020 2020 2020  a }}",..        
+00001420: 2020 2020 2020 2020 7369 676e 6174 7572          signatur
+00001430: 653a 2022 7b7b 2073 6967 6e61 7475 7265  e: "{{ signature
+00001440: 207d 7d22 2c0d 0a20 2020 2020 2020 2020   }}",..         
+00001450: 2020 2020 2020 2065 6d62 6564 546f 3a20         embedTo: 
+00001460: 2223 6c69 7170 6179 5f63 6865 636b 6f75  "#liqpay_checkou
+00001470: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
+00001480: 2020 2020 206d 6f64 653a 2022 656d 6265       mode: "embe
+00001490: 6422 202f 2f20 656d 6265 6420 7c7c 2070  d" // embed || p
+000014a0: 6f70 7570 2c0d 0a20 2020 2020 2020 2020  opup,..         
+000014b0: 2020 207d 292e 6f6e 2822 6c69 7170 6179     }).on("liqpay
+000014c0: 2e63 616c 6c62 6163 6b22 2c20 6675 6e63  .callback", func
+000014d0: 7469 6f6e 2864 6174 6129 7b0d 0a20 2020  tion(data){..   
+000014e0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000014f0: 736f 6c65 2e6c 6f67 2864 6174 612e 7374  sole.log(data.st
+00001500: 6174 7573 293b 0d0a 2020 2020 2020 2020  atus);..        
+00001510: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
+00001520: 6c6f 6728 6461 7461 293b 0d0a 2020 2020  log(data);..    
+00001530: 2020 2020 2020 2020 7d29 2e6f 6e28 226c          }).on("l
+00001540: 6971 7061 792e 7265 6164 7922 2c20 6675  iqpay.ready", fu
+00001550: 6e63 7469 6f6e 2864 6174 6129 7b0d 0a20  nction(data){.. 
+00001560: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+00001570: 2f20 7265 6164 790d 0a20 2020 2020 2020  / ready..       
+00001580: 2020 2020 207d 292e 6f6e 2822 6c69 7170       }).on("liqp
+00001590: 6179 2e63 6c6f 7365 222c 2066 756e 6374  ay.close", funct
+000015a0: 696f 6e28 6461 7461 297b 0d0a 2020 2020  ion(data){..    
+000015b0: 2020 2020 2020 2020 2020 2020 2f2f 2063              // c
+000015c0: 6c6f 7365 0d0a 2020 2020 2020 2020 2020  lose..          
+000015d0: 2020 7d29 3b0d 0a20 2020 2020 2020 207d    });..        }
+000015e0: 3b0d 0a20 2020 203c 2f73 6372 6970 743e  ;..    </script>
+000015f0: 0d0a 2020 2020 3c73 6372 6970 7420 7372  ..    <script sr
+00001600: 633d 222f 2f73 7461 7469 632e 6c69 7170  c="//static.liqp
+00001610: 6179 2e75 612f 6c69 626a 732f 6368 6563  ay.ua/libjs/chec
+00001620: 6b6f 7574 2e6a 7322 2061 7379 6e63 3e3c  kout.js" async><
+00001630: 2f73 6372 6970 743e 0d0a 6060 600d 0a    /script>..```..
```

