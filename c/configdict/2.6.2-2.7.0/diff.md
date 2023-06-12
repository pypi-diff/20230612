# Comparing `tmp/configdict-2.6.2-py3-none-any.whl.zip` & `tmp/configdict-2.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 31515 bytes, number of entries: 9
+Zip file size: 31720 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       25 b- defN 21-Nov-25 01:23 configdict/__init__.py
--rw-rw-r--  2.0 unx    63032 b- defN 23-May-31 15:31 configdict/configdict.py
+-rw-rw-r--  2.0 unx    63756 b- defN 23-Jun-12 15:33 configdict/configdict.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Nov-25 01:23 configdict/py.typed
 -rw-rw-r--  2.0 unx    22699 b- defN 21-Nov-25 01:23 configdict/__pycache__/configdict.cpython-38.pyc
--rw-rw-r--  2.0 unx     1060 b- defN 23-May-31 15:33 configdict-2.6.2.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     3883 b- defN 23-May-31 15:33 configdict-2.6.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-31 15:33 configdict-2.6.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-31 15:33 configdict-2.6.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      742 b- defN 23-May-31 15:33 configdict-2.6.2.dist-info/RECORD
-9 files, 91544 bytes uncompressed, 30229 bytes compressed:  67.0%
+-rw-rw-r--  2.0 unx     1060 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     3883 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/RECORD
+9 files, 92268 bytes uncompressed, 30434 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: configdict/py.typed
 Comment: 
 
 Filename: configdict/__pycache__/configdict.cpython-38.pyc
 Comment: 
 
-Filename: configdict-2.6.2.dist-info/LICENSE.md
+Filename: configdict-2.7.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: configdict-2.6.2.dist-info/METADATA
+Filename: configdict-2.7.0.dist-info/METADATA
 Comment: 
 
-Filename: configdict-2.6.2.dist-info/WHEEL
+Filename: configdict-2.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: configdict-2.6.2.dist-info/top_level.txt
+Filename: configdict-2.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: configdict-2.6.2.dist-info/RECORD
+Filename: configdict-2.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## configdict/configdict.py

```diff
@@ -1365,26 +1365,30 @@
 
     def reset(self, save=True) -> None:
         """ Reset this dict to its default """
         super().reset()
         if save:
             self.save()
 
+    def resetKey(self, key: str) -> None:
+        """Reset the given key to its default value"""
+        self[key] = self.default[key]
+
     def save(self, path: str = None, header:str='') -> None:
         """
         Save this to its persistent path (or a custom path)
 
         If this config was created with the `persistent` flag on,
         it does not need to be saved manually, it is saved whenever it
         is modified. However if it was created with ``persistent=False``
         then this method can be used to write this dict so it will be
         loaded in a future session
 
         Args:
-            path (str): the path to save the config. If None and this
+            path: the path to save the config. If None and this
                 is a named config, it is saved to the path returned by
                 :meth:`~ConfigDict.getPath`
             header: if given, this string is written prior to the dict, as
                 a comment. This is only supported when saving to yaml
         """
         if not path:
             path = self.getPath()
@@ -1415,32 +1419,43 @@
         rows = []
         for key, value in self.items():
             infostr = self._infoStr(key)
             doc = self.getDoc(key)
             rows.append((key, str(value), infostr, doc if doc else ""))
         return rows
 
-    def generateRstDocumentation(self, maxwidth=80, withName=True, withDescription=True,
+    def generateRstDocumentation(self, maxWidth=80, withName=True, withDescription=True,
                                  withLink=True, linkPrefix=''
                                  ) -> str:
         """
         Generate ReST documentation for this dictionary
 
         The generated string can then be dumped to a file and included
         in documentation
+
+        Args:
+            maxWidth: the max. width of a line
+            withName: if True, add the name of the config (if it has a name)
+            withDescription: if True, add this dict's description (if it has any)
+            withLink: if True, for each key:value pair generate a RST link using the given linkPrefix
+                For example, for a key 'foo' and a linkPrefix='config' the generated link will be
+                ``.. _configfoo``. This link can be used within the documentation to link to this key
+
+        Returns:
+            the generated rst documentation, as str.
         """
         lines = []
         _ = lines.append
 
         if withName and self.name:
             _(self.name)
             _("-" * len(self.name))
             _('')
         if withDescription and self.description:
-            _(textwrap.wrap(self.description, width=maxwidth))
+            _(textwrap.wrap(self.description, width=maxWidth))
             _('\n------------------------\n')
         for key, value in self.default.items():
             if withLink:
                 linkkey = _asRstLinkKey(key)
                 if linkPrefix:
                     linkkey = linkPrefix + linkkey
                 _(f".. _{linkkey}:\n")
```

## Comparing `configdict-2.6.2.dist-info/LICENSE.md` & `configdict-2.7.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `configdict-2.6.2.dist-info/METADATA` & `configdict-2.7.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configdict
-Version: 2.6.2
+Version: 2.7.0
 Summary: A supercharged dict used as configuration
 Author-email: Eduardo Moguillansky <eduardo.moguillansky@gmail.com>
 License: Copyright (c) 2011-2017 GitHub Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

## Comparing `configdict-2.6.2.dist-info/RECORD` & `configdict-2.7.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 configdict/__init__.py,sha256=CI6gyI6isoSmOxiaMKQ1zJMLWzFYn6bOTnUcJtMAMRQ,25
-configdict/configdict.py,sha256=7PHxaDP9_CHchkQ33qrhEHGQ9wpcaLvUNGz1KpnqCwE,63032
+configdict/configdict.py,sha256=mZAF2AOJuxiKZG1DPSOizqlCCpe3Er2g8UJRIR0f3lA,63756
 configdict/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 configdict/__pycache__/configdict.cpython-38.pyc,sha256=pmenTOMg3mEukCVKrOf7lNx1TTPjNga5bTXY_VRnSFU,22699
-configdict-2.6.2.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
-configdict-2.6.2.dist-info/METADATA,sha256=l4UY0E_yNzH5BeJHXank0OPGV8SA8aOGLfWeEE3hCVA,3883
-configdict-2.6.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-configdict-2.6.2.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
-configdict-2.6.2.dist-info/RECORD,,
+configdict-2.7.0.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
+configdict-2.7.0.dist-info/METADATA,sha256=ArtjTXavlHB_r6gaApjmaXY7iJguBXDjkQ7jBthHmlg,3883
+configdict-2.7.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+configdict-2.7.0.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
+configdict-2.7.0.dist-info/RECORD,,
```

