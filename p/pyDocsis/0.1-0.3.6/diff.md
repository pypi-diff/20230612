# Comparing `tmp/pyDocsis-0.1.tar.gz` & `tmp/pyDocsis-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDocsis-0.1.tar", last modified: Sun May 29 19:53:06 2022, max compression
+gzip compressed data, was "pyDocsis-0.3.6.tar", last modified: Mon Jun 12 16:43:39 2023, max compression
```

## Comparing `pyDocsis-0.1.tar` & `pyDocsis-0.3.6.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2022-05-29 19:53:06.712274 pyDocsis-0.1/
--rw-r--r--   0 tbalsley   (501) staff       (20)      272 2022-05-29 19:53:06.712137 pyDocsis-0.1/PKG-INFO
-drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2022-05-29 19:53:06.708003 pyDocsis-0.1/pyDocsis.egg-info/
--rw-r--r--   0 tbalsley   (501) staff       (20)      272 2022-05-29 19:53:06.000000 pyDocsis-0.1/pyDocsis.egg-info/PKG-INFO
--rw-r--r--   0 tbalsley   (501) staff       (20)      318 2022-05-29 19:53:06.000000 pyDocsis-0.1/pyDocsis.egg-info/SOURCES.txt
--rw-r--r--   0 tbalsley   (501) staff       (20)        1 2022-05-29 19:53:06.000000 pyDocsis-0.1/pyDocsis.egg-info/dependency_links.txt
--rw-r--r--   0 tbalsley   (501) staff       (20)        9 2022-05-29 19:53:06.000000 pyDocsis-0.1/pyDocsis.egg-info/top_level.txt
-drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2022-05-29 19:53:06.711786 pyDocsis-0.1/pydocsis/
--rw-r--r--   0 tbalsley   (501) staff       (20)     4562 2022-05-25 23:57:39.000000 pyDocsis-0.1/pydocsis/MTATlvs.py
--rw-r--r--   0 tbalsley   (501) staff       (20)     7842 2022-05-25 23:59:28.000000 pyDocsis-0.1/pydocsis/MtaConfig.py
--rw-r--r--   0 tbalsley   (501) staff       (20)     5154 2022-05-26 10:48:47.000000 pyDocsis-0.1/pydocsis/TLV.py
--rw-r--r--   0 tbalsley   (501) staff       (20)       43 2022-05-29 14:03:57.000000 pyDocsis-0.1/pydocsis/__init__.py
--rw-r--r--   0 tbalsley   (501) staff       (20)     6274 2022-05-29 14:28:36.000000 pyDocsis-0.1/pydocsis/cmConfig.py
--rw-r--r--   0 tbalsley   (501) staff       (20)     1456 2022-05-26 00:26:27.000000 pyDocsis-0.1/pydocsis/configFile.py
--rw-r--r--   0 tbalsley   (501) staff       (20)   620089 2022-05-26 00:00:46.000000 pyDocsis-0.1/pydocsis/docsisTlvs.py
--rw-r--r--   0 tbalsley   (501) staff       (20)    11777 2022-05-26 10:48:47.000000 pyDocsis-0.1/pydocsis/mib.py
--rw-r--r--   0 tbalsley   (501) staff       (20)    15401 2022-05-25 23:57:39.000000 pyDocsis-0.1/pydocsis/mtaMibs.py
--rw-r--r--   0 tbalsley   (501) staff       (20)       38 2022-05-29 19:53:06.712323 pyDocsis-0.1/setup.cfg
--rw-r--r--   0 tbalsley   (501) staff       (20)      316 2022-05-29 19:52:09.000000 pyDocsis-0.1/setup.py
+drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-12 16:43:39.789633 pyDocsis-0.3.6/
+-rw-r--r--   0 tbalsley   (501) staff       (20)      235 2023-06-12 16:43:39.789419 pyDocsis-0.3.6/PKG-INFO
+-rw-r--r--   0 tbalsley   (501) staff       (20)      329 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/README.md
+drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-12 16:43:39.785669 pyDocsis-0.3.6/Scripts/
+-rw-r--r--   0 tbalsley   (501) staff       (20)      319 2023-06-12 16:32:24.000000 pyDocsis-0.3.6/Scripts/cm_decode
+drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-12 16:43:39.786549 pyDocsis-0.3.6/pyDocsis.egg-info/
+-rw-r--r--   0 tbalsley   (501) staff       (20)      235 2023-06-12 16:43:39.000000 pyDocsis-0.3.6/pyDocsis.egg-info/PKG-INFO
+-rw-r--r--   0 tbalsley   (501) staff       (20)      346 2023-06-12 16:43:39.000000 pyDocsis-0.3.6/pyDocsis.egg-info/SOURCES.txt
+-rw-r--r--   0 tbalsley   (501) staff       (20)        1 2023-06-12 16:43:39.000000 pyDocsis-0.3.6/pyDocsis.egg-info/dependency_links.txt
+-rw-r--r--   0 tbalsley   (501) staff       (20)        9 2023-06-12 16:43:39.000000 pyDocsis-0.3.6/pyDocsis.egg-info/top_level.txt
+drwxr-xr-x   0 tbalsley   (501) staff       (20)        0 2023-06-12 16:43:39.789135 pyDocsis-0.3.6/pydocsis/
+-rw-r--r--   0 tbalsley   (501) staff       (20)     4562 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/MTATlvs.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)     7842 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/MtaConfig.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)     5294 2023-06-12 16:36:55.000000 pyDocsis-0.3.6/pydocsis/TLV.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)      111 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/__init__.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)     6664 2023-06-12 16:40:45.000000 pyDocsis-0.3.6/pydocsis/cmConfig.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)     1698 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/configFile.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)   620089 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/docsisTlvs.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)    11777 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/mib.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)    15401 2023-06-12 16:14:21.000000 pyDocsis-0.3.6/pydocsis/mtaMibs.py
+-rw-r--r--   0 tbalsley   (501) staff       (20)       38 2023-06-12 16:43:39.789693 pyDocsis-0.3.6/setup.cfg
+-rw-r--r--   0 tbalsley   (501) staff       (20)      431 2023-06-12 16:40:51.000000 pyDocsis-0.3.6/setup.py
```

### Comparing `pyDocsis-0.1/pydocsis/MTATlvs.py` & `pyDocsis-0.3.6/pydocsis/MTATlvs.py`

 * *Files identical despite different names*

### Comparing `pyDocsis-0.1/pydocsis/MtaConfig.py` & `pyDocsis-0.3.6/pydocsis/MtaConfig.py`

 * *Files identical despite different names*

### Comparing `pyDocsis-0.1/pydocsis/TLV.py` & `pyDocsis-0.3.6/pydocsis/TLV.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,18 @@
             self.value = args["value"]
         else:
             self.value = ""
         if "subTLVs" in args.keys():
             self.subTLVs = args["subTLVs"]
         else:
             self.subTLVs = []
+        if "description" in args.keys():
+            self.description = args["description"]
+        else:
+            self.description = ""
 
     def encode_for_file(self, tags=None):
         if tags is None:
             tags = {}
         if tags == {}:
             tags = DocsisTlvs
         tlv_string = ''
```

### Comparing `pyDocsis-0.1/pydocsis/cmConfig.py` & `pyDocsis-0.3.6/pydocsis/cmConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 stack up a bunch of TLVs and send it to a cable modem
 """
 import binascii
 from pydocsis.TLV import TLV
 from pydocsis.docsisTlvs import DocsisTlvs
 import hashlib
+import hmac
 
 
 class CmConfig(object):
     """
 A config file for a cable modem.
     """
 
@@ -31,21 +32,29 @@
             f = open(self.configFilePath, "rb")
             content = f.read()
             self.tlv_string = binascii.hexlify(content).decode('UTF-8')[:]
         else:
             raise ValueError("Cannot turn a file into a string if there is no file.")
 
     def parse(self, tlv_string="", tags=None):
-        """stolen from https://github.com/timgabets/pytlv and modified"""
+        """
+        stolen from https://github.com/timgabets/pytlv and modified
+
+        :param tv_string: A string of the hex in the file
+        :type tlvs: basestring
+        :param tags: the tlv disctionary thing, as a dict
+        :type tags: dict
+
+        """
         if tags is None:
             tags = {}
         tlvs = []
         if len(tlv_string) == 0:
             tlv_string = self.tlv_string
-            print(tlv_string)
+            # print(tlv_string)
         i = 0
         if len(tags.keys()) == 0:
             print("Loading keys from docsis file")
             tags = self.tags
         while i < len(tlv_string):
             tag_found = False
             tag_length = 2
@@ -75,30 +84,30 @@
                         #    print(value)
                         if len(tags[tag]["subTlvs"].keys()) > 0:
                             # print(tag)
                             # print("down")
                             subts = self.parse(value, tags[tag]["subTlvs"])
                             # print("up")
                             parsed_data = [tag, subts]
-                            tlvs.append(TLV(tag=tag, subTLVs=subts, datatype=tags[tag]["datatype"]))
+                            tlvs.append(TLV(tag=tag, subTLVs=subts, datatype=tags[tag]["datatype"], description=tags[tag]["description"]))
                         # tlvs.append(parsed_data)
                         else:
                             # if tag == "11":
                             #    print(value)
                             # if "str" in tags[tag]["datatype"]:
                             #    if "encode_strzero" in tags[tag]["datatype"]:
                             #        value = value[:-2]
                             #    value = codecs.decode(value, "hex")
                             # parsed_data = [tag,  tags[tag]["description"], tags[tag]["datatype"] , value]
-                            tlvs.append(TLV(tag=tag, value=value, datatype=tags[tag]["datatype"]))
+                            tlvs.append(TLV(tag=tag, value=value, datatype=tags[tag]["datatype"], description=tags[tag]["description"]))
                         i = value_end_position
                     tag_found = True
             if not tag_found:
                 # print(i)
-                print(tlvs)
+                # print(tlvs)
                 msg = 'Unknown tag found: ' + tlv_string[i:i + 10]
                 raise ValueError(msg)
         self.tlvs = tlvs
         return tlvs
 
     def encode(self):
         """
@@ -122,18 +131,20 @@
         exts = ""
         if '06' in self.hashme:
             newval = hashlib.md5(binascii.unhexlify(stuff))
             # print(newval.hexdigest())
             nextTLV = TLV(tag="06", datatype="md5", value=newval.hexdigest())
             exts += nextTLV.encode_for_file()
         if '07' in self.hashme:
+            ekey = 0xdeadbeef
             newval = hashlib.md5(binascii.unhexlify(stuff))
-            nextTLV = TLV(tag="07", datatype="md5", value=newval.hexdigest())
-            #exts += nextTLV.encode_for_file()
-            exts += oldTLV7.encode_for_file()
+            enc_res = hmac.new(ekey, newval, hashlib.md5)
+            nextTLV = TLV(tag="07", datatype="md5", value=enc_res.hexdigest())
+            exts += nextTLV.encode_for_file()
+            #exts += oldTLV7.encode_for_file()
 
         stuff += exts
         stuff += lastTLV.encode_for_file()
 
         while (len(stuff) / 2) % 4 != 0:
             stuff += "00"
         # print(stuff)
@@ -150,11 +161,11 @@
     :type tlvs: [TLV]
     :return: a disct that can be easily converted to json
     :rtype: {}
     """
     outs = {}
     for t in tlvs:
         if len(t.subTLVs) == 0:
-            outs[t.tag] = str(t.get_value()) + " (" + t.datatype + ")"
+            outs[t.tag] = str(t.get_value()) + " (" + t.datatype + ") " + t.description
         else:
             outs[t.tag] = json_this(t.subTLVs)
     return outs
```

### Comparing `pyDocsis-0.1/pydocsis/configFile.py` & `pyDocsis-0.3.6/pydocsis/configFile.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,19 @@
 
     def get_config(self):
         """
 
         :return: either an MTA config or a CmConfig
         :rtype: an object!
         """
+        if self.tlv_string == "":
+            if self.configFilePath == "":
+                raise ValueError("Cannot turn a file into a string if there is no file.")
+                # return False
+            self.generate_string_from_file()
         if self.tlv_string.startswith("fe0101"):
             bob = MtaConfig()
             bob.configFilePath = self.configFilePath
             bob.tlv_string = self.tlv_string
             return bob
         else:
             bob = CmConfig()
```

### Comparing `pyDocsis-0.1/pydocsis/docsisTlvs.py` & `pyDocsis-0.3.6/pydocsis/docsisTlvs.py`

 * *Files identical despite different names*

### Comparing `pyDocsis-0.1/pydocsis/mib.py` & `pyDocsis-0.3.6/pydocsis/mib.py`

 * *Files identical despite different names*

### Comparing `pyDocsis-0.1/pydocsis/mtaMibs.py` & `pyDocsis-0.3.6/pydocsis/mtaMibs.py`

 * *Files identical despite different names*

