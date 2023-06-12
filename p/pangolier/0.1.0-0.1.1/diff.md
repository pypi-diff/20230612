# Comparing `tmp/pangolier-0.1.0-py3-none-any.whl.zip` & `tmp/pangolier-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4720 bytes, number of entries: 10
+Zip file size: 5170 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 22-Aug-07 02:48 pangolier/__init__.py
--rw-rw-r--  2.0 unx       86 b- defN 22-Aug-06 10:19 pangolier/common.py
+-rw-rw-r--  2.0 unx      336 b- defN 23-Jun-12 03:36 pangolier/common.py
 -rw-rw-r--  2.0 unx      593 b- defN 22-Aug-06 08:53 pangolier/filters.py
 -rw-rw-r--  2.0 unx     2930 b- defN 23-Jan-16 03:51 pangolier/functions.py
--rw-rw-r--  2.0 unx     2161 b- defN 23-Jan-02 13:07 pangolier/metrics.py
+-rw-rw-r--  2.0 unx     3153 b- defN 23-Jun-12 03:36 pangolier/metrics.py
 -rw-rw-r--  2.0 unx     1121 b- defN 22-Aug-08 12:44 pangolier/prefixes.py
--rw-rw-r--  2.0 unx     3330 b- defN 23-Jan-16 03:51 pangolier-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-16 03:51 pangolier-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jan-16 03:51 pangolier-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      765 b- defN 23-Jan-16 03:51 pangolier-0.1.0.dist-info/RECORD
-10 files, 11088 bytes uncompressed, 3420 bytes compressed:  69.2%
+-rw-rw-r--  2.0 unx     3701 b- defN 23-Jun-12 03:36 pangolier-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 03:36 pangolier-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-12 03:36 pangolier-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      766 b- defN 23-Jun-12 03:36 pangolier-0.1.1.dist-info/RECORD
+10 files, 12702 bytes uncompressed, 3870 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: pangolier/metrics.py
 Comment: 
 
 Filename: pangolier/prefixes.py
 Comment: 
 
-Filename: pangolier-0.1.0.dist-info/METADATA
+Filename: pangolier-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pangolier-0.1.0.dist-info/WHEEL
+Filename: pangolier-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pangolier-0.1.0.dist-info/top_level.txt
+Filename: pangolier-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pangolier-0.1.0.dist-info/RECORD
+Filename: pangolier-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pangolier/common.py

```diff
@@ -1,5 +1,20 @@
 from textwrap import indent
 
 
 def indent_body(body):
     return indent(body, ' ' * 4)
+
+
+def format_modifier(name, args, pretty):
+    if not args:
+        return name
+
+    body = ', '.join(args)
+
+    if pretty:
+        return '%s(\n%s\n)' % (
+            name,
+            indent_body(body)
+        )
+
+    return '%s(%s)' % (name, body)
```

## pangolier/metrics.py

```diff
@@ -1,8 +1,8 @@
-from .common import indent_body
+from .common import indent_body, format_modifier
 from .filters import _make_filter
 
 
 class MetricBase:
     def to_str(self, pretty=False):
         raise NotImplementedError
 
@@ -72,19 +72,63 @@
 
         return FilteredMetric(
             self.origin_metric,
             self.filters + append_filters
         )
 
 
+class GroupBase(MetricBase):
+    modifier = ''
+
+    def __init__(self, *labels):
+        self.labels = labels
+
+    def to_str(self, pretty=False):
+        return format_modifier(self.modifier, self.labels, pretty=pretty)
+
+
+class GroupLeft(GroupBase):
+    modifier = 'group_left'
+
+
+class GroupRight(GroupBase):
+    modifier = 'group_right'
+
+
 class BinOp(MetricBase):
-    def __init__(self, op, first, second):
+    def __init__(
+        self, op, first, second,
+        *, on=None, ignoring=None, group=None,
+    ):
+        if on and ignoring:
+            raise ValueError('can not specific both `on` and `ignoring`')
+
         self.op = op
         self.first = first
         self.second = second
 
+        self.on = on
+        self.ignoring = ignoring
+        self.group = group
+
     def to_str(self, pretty=False):
-        return '%s %s %s' % (
-            self.first.to_str(pretty=pretty),
-            self.op,
-            self.second.to_str(pretty=pretty),
-        )
+        parts = []
+
+        parts.append(self.first.to_str(pretty=pretty))
+        parts.append(self.op)
+
+        if self.on:
+            parts.append(
+                format_modifier('on', self.on, pretty=pretty)
+            )
+
+        if self.ignoring:
+            parts.append(
+                format_modifier('ignoring', self.ignoring, pretty=pretty)
+            )
+
+        if self.group:
+            parts.append(self.group.to_str(pretty=pretty))
+
+        parts.append(self.second.to_str(pretty=pretty))
+
+        return ' '.join(parts)
```

## Comparing `pangolier-0.1.0.dist-info/METADATA` & `pangolier-0.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangolier
-Version: 0.1.0
+Version: 0.1.1
 Summary: prometheus query builder
 Home-page: https://github.com/lexdene/pangolier
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
 
 # Pangolier
 
@@ -166,10 +166,31 @@
         }[5m]
     ) / rate(
         bar{
             group="canary"
         }[5m]
     )
 
+For operation with modifier:
+
+    from pangolier.metrics import Metric, BinOp, GroupLeft
+
+    print(BinOp(
+        '*',
+        Metric('foo'),
+        Metric('bar'),
+        on=('interface', 'job'),
+        group=GroupLeft('node', 'resource'),
+    ).to_str(pretty=True))
+
+output:
+
+    foo * on(
+        interface, job
+    ) group_left(
+        node, resource
+    ) bar
+
+
 ## about name
 
 [Pangolier](https://dota2.fandom.com/wiki/Pangolier)
```

## Comparing `pangolier-0.1.0.dist-info/RECORD` & `pangolier-0.1.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pangolier/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pangolier/common.py,sha256=h-vJ8l4Bk6Y8h5U5GSDsfYaxfNkFLeM-GD1E0UqVYo4,86
+pangolier/common.py,sha256=6CiIILgtgsnSlYkreEOirY1Ox85e_iNBUqTnAmawxgM,336
 pangolier/filters.py,sha256=0rEzH9BsJ_Lka9JcnNLNK9-52V9G7NQ2DCKWXaKxvjM,593
 pangolier/functions.py,sha256=wLnItRKEoCT5tnKX0ZgIbl6gPGB-_qosCz4v0qba8fI,2930
-pangolier/metrics.py,sha256=cXJuWHaWrSxMm--SNRbPLSv7tY_LLmrMmXCgWJQxw2w,2161
+pangolier/metrics.py,sha256=D47ly81aVF1jEKZPFtzhdP_Dyg7Ukh18QqvfCztwBzw,3153
 pangolier/prefixes.py,sha256=5lgLpoRUF2oP3eT5BEzWyOOxTb_dGdl6LR8YBvtWKtU,1121
-pangolier-0.1.0.dist-info/METADATA,sha256=qmm2EguMu2lfJqgpu2gOyNeYP30CnpodK5L4LMm1Bpc,3330
-pangolier-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pangolier-0.1.0.dist-info/top_level.txt,sha256=oVjXI9K4K47ZzdvnhAwezlDWfgBGevyp1bX99_TSZlk,10
-pangolier-0.1.0.dist-info/RECORD,,
+pangolier-0.1.1.dist-info/METADATA,sha256=VmNmmuHAaCvDcjRezF3mMxLIJ0k6DCqfBToTHYH0BQ4,3701
+pangolier-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pangolier-0.1.1.dist-info/top_level.txt,sha256=oVjXI9K4K47ZzdvnhAwezlDWfgBGevyp1bX99_TSZlk,10
+pangolier-0.1.1.dist-info/RECORD,,
```

