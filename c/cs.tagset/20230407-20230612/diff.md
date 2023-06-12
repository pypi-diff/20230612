# Comparing `tmp/cs.tagset-20230407.tar.gz` & `tmp/cs.tagset-20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.tagset-20230407.tar", last modified: Fri Apr  7 00:06:27 2023, max compression
+gzip compressed data, was "cs.tagset-20230612.tar", last modified: Mon Jun 12 04:26:19 2023, max compression
```

## Comparing `cs.tagset-20230407.tar` & `cs.tagset-20230612.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-07 00:06:27.871225 cs.tagset-20230407/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-04-07 00:05:56.000000 cs.tagset-20230407/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    31489 2023-04-07 00:06:27.871409 cs.tagset-20230407/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    64474 2023-04-07 00:06:02.000000 cs.tagset-20230407/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-07 00:06:27.866511 cs.tagset-20230407/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-07 00:06:27.866836 cs.tagset-20230407/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-07 00:06:27.868975 cs.tagset-20230407/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)   131222 2023-04-07 00:05:47.000000 cs.tagset-20230407/lib/python/cs/tagset.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-07 00:06:27.870932 cs.tagset-20230407/lib/python/cs.tagset.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    31489 2023-04-07 00:06:27.000000 cs.tagset-20230407/lib/python/cs.tagset.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      298 2023-04-07 00:06:27.000000 cs.tagset-20230407/lib/python/cs.tagset.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-04-07 00:06:27.000000 cs.tagset-20230407/lib/python/cs.tagset.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      298 2023-04-07 00:06:27.000000 cs.tagset-20230407/lib/python/cs.tagset.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-04-07 00:06:27.000000 cs.tagset-20230407/lib/python/cs.tagset.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    32134 2023-04-07 00:06:20.000000 cs.tagset-20230407/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1150 2023-04-07 00:06:27.872017 cs.tagset-20230407/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-04-07 00:06:02.000000 cs.tagset-20230407/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:26:19.526428 cs.tagset-20230612/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 04:25:43.000000 cs.tagset-20230612/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    31802 2023-06-12 04:26:19.526582 cs.tagset-20230612/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    64787 2023-06-12 04:25:50.000000 cs.tagset-20230612/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:26:19.519472 cs.tagset-20230612/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:26:19.519819 cs.tagset-20230612/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:26:19.523127 cs.tagset-20230612/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)   131556 2023-06-12 04:25:28.000000 cs.tagset-20230612/lib/python/cs/tagset.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:26:19.526159 cs.tagset-20230612/lib/python/cs.tagset.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    31802 2023-06-12 04:26:19.000000 cs.tagset-20230612/lib/python/cs.tagset.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      298 2023-06-12 04:26:19.000000 cs.tagset-20230612/lib/python/cs.tagset.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 04:26:19.000000 cs.tagset-20230612/lib/python/cs.tagset.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      296 2023-06-12 04:26:19.000000 cs.tagset-20230612/lib/python/cs.tagset.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 04:26:19.000000 cs.tagset-20230612/lib/python/cs.tagset.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    32445 2023-06-12 04:26:11.000000 cs.tagset-20230612/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1148 2023-06-12 04:26:19.527211 cs.tagset-20230612/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 04:25:50.000000 cs.tagset-20230612/setup.py
```

### Comparing `cs.tagset-20230407/PKG-INFO` & `cs.tagset-20230612/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.tagset
-Version: 20230407
+Version: 20230612
 Summary: Tags and sets of tags with __format__ support and optional ontology information.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -16,16 +16,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20230407*:
-Move the (optional) ORM open/close from FSTags.startup_shutdown to TagFile.save, greatly shortens the ORM lock.
+*Latest release 20230612*:
+* TagFile.save_tagsets: catch and warn about exceptions from update_mapping[key].update, something is wrong with my SQLTags usage.
+* TagFile.save_tagsets: update_mapping: do not swallow AttributeError.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no "name")
@@ -642,14 +643,18 @@
           type type_name + entity_name [tags...]
             Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* TagFile.save_tagsets: catch and warn about exceptions from update_mapping[key].update, something is wrong with my SQLTags usage.
+* TagFile.save_tagsets: update_mapping: do not swallow AttributeError.
+
 *Release 20230407*:
 Move the (optional) ORM open/close from FSTags.startup_shutdown to TagFile.save, greatly shortens the ORM lock.
 
 *Release 20230212*:
 Mark TagSetCriterion as Promotable.
 
 *Release 20230210*:
```

### Comparing `cs.tagset-20230407/README.md` & `cs.tagset-20230612/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20230407*:
-Move the (optional) ORM open/close from FSTags.startup_shutdown to TagFile.save, greatly shortens the ORM lock.
+*Latest release 20230612*:
+* TagFile.save_tagsets: catch and warn about exceptions from update_mapping[key].update, something is wrong with my SQLTags usage.
+* TagFile.save_tagsets: update_mapping: do not swallow AttributeError.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no "name")
@@ -1580,14 +1581,18 @@
 {cmd} type_name + entity_name [tags...]
   Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* TagFile.save_tagsets: catch and warn about exceptions from update_mapping[key].update, something is wrong with my SQLTags usage.
+* TagFile.save_tagsets: update_mapping: do not swallow AttributeError.
+
 *Release 20230407*:
 Move the (optional) ORM open/close from FSTags.startup_shutdown to TagFile.save, greatly shortens the ORM lock.
 
 *Release 20230212*:
 Mark TagSetCriterion as Promotable.
 
 *Release 20230210*:
```

### Comparing `cs.tagset-20230407/lib/python/cs/tagset.py` & `cs.tagset-20230612/lib/python/cs/tagset.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,28 +215,28 @@
 from cs.deco import decorator, fmtdoc, Promotable
 from cs.edit import edit_strings, edit as edit_lines
 from cs.fileutils import shortpath
 from cs.fs import FSPathBasedSingleton
 from cs.lex import (
     cropped_repr, cutprefix, cutsuffix, get_dotted_identifier, get_nonwhite,
     is_dotted_identifier, is_identifier, skipwhite, FormatableMixin,
-    has_format_attributes, format_attribute, FStr, r
+    has_format_attributes, format_attribute, FStr, r, s
 )
 from cs.logutils import setup_logging, debug, warning, error, ifverbose
 from cs.mappings import (
     AttrableMappingMixin, IndexedMapping, PrefixedMappingProxy,
     RemappedMappingProxy
 )
 from cs.obj import SingletonMixin
 from cs.pfx import Pfx, pfx, pfx_call, pfx_method
 from cs.py3 import date_fromisoformat, datetime_fromisoformat
 from cs.resources import MultiOpenMixin
 from cs.threads import locked_property
 
-__version__ = '20230407'
+__version__ = '20230612'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -2022,16 +2022,16 @@
           >>> sub.z = 5
           >>> sub
           TagSetPrefixView:sub.{'x': 3, 'y': 4, 'z': 5}
           >>> tags
           TagSet:{'a': 1, 'b': 2, 'sub.x': 3, 'sub.y': 4, 'sub.z': 5}
   '''
 
-  @typechecked
   @require(lambda prefix: len(prefix) > 0)
+  @typechecked
   def __init__(self, tags, prefix: str):
     self.__dict__.update(_tags=tags, _prefix=prefix, _prefix_=prefix + '.')
 
   def __str__(self):
     tag = self.tag
     if tag is None:
       return str(TagSet(self.as_dict()))
@@ -3492,15 +3492,23 @@
                     key = (
                         "%s.%s" %
                         (update_prefix, uuid_s) if update_prefix else uuid_s
                     )
                     d = tags.as_dict()
                     del d[update_uuid_tag_name]
                     d['fspath'] = joinpath(dirname(filepath), name)
-                    update_mapping[key].update(d)
+                    try:
+                      update_mapping[key].update(d)
+                    except AttributeError:
+                      raise
+                    except Exception as e:
+                      warning(
+                          "update_mapping:%s[%r].update(%s): %s",
+                          s(update_mapping), key, cropped_repr(d), e
+                      )
                 f.write(
                     cls.tags_line(
                         name, tags, extra_types=extra_types, prune=prune
                     )
                 )
                 f.write('\n')
         except OSError as e:
```

### Comparing `cs.tagset-20230407/lib/python/cs.tagset.egg-info/PKG-INFO` & `cs.tagset-20230612/lib/python/cs.tagset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.tagset
-Version: 20230407
+Version: 20230612
 Summary: Tags and sets of tags with __format__ support and optional ontology information.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -16,16 +16,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20230407*:
-Move the (optional) ORM open/close from FSTags.startup_shutdown to TagFile.save, greatly shortens the ORM lock.
+*Latest release 20230612*:
+* TagFile.save_tagsets: catch and warn about exceptions from update_mapping[key].update, something is wrong with my SQLTags usage.
+* TagFile.save_tagsets: update_mapping: do not swallow AttributeError.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no "name")
@@ -642,14 +643,18 @@
           type type_name + entity_name [tags...]
             Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* TagFile.save_tagsets: catch and warn about exceptions from update_mapping[key].update, something is wrong with my SQLTags usage.
+* TagFile.save_tagsets: update_mapping: do not swallow AttributeError.
+
 *Release 20230407*:
 Move the (optional) ORM open/close from FSTags.startup_shutdown to TagFile.save, greatly shortens the ORM lock.
 
 *Release 20230212*:
 Mark TagSetCriterion as Promotable.
 
 *Release 20230210*:
```

### Comparing `cs.tagset-20230407/pyproject.toml` & `cs.tagset-20230612/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,51 +8,52 @@
     "python3",
 ]
 dependencies = [
     "cs.cmdutils>=20210404",
     "cs.dateutils>=20230210",
     "cs.deco>=20230331",
     "cs.edit>=20220429",
-    "cs.fileutils>=20230401",
+    "cs.fileutils>=20230421",
     "cs.fs>=20220429",
     "cs.lex>=20230401",
     "cs.logutils>=20230212",
-    "cs.mappings>=20220912.4",
+    "cs.mappings>=20230612",
     "cs.obj>=20200716",
-    "cs.pfx>=20230331",
+    "cs.pfx>=20230604",
     "cs.py3>=20220523",
-    "cs.resources>=20230331",
+    "cs.resources>=20230503",
     "cs.threads>=20230331",
     "icontract",
     "typeguard",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230407"
+version = "20230612"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20230407*:
-Move the (optional) ORM open/close from FSTags.startup_shutdown to TagFile.save, greatly shortens the ORM lock.
+*Latest release 20230612*:
+* TagFile.save_tagsets: catch and warn about exceptions from update_mapping[key].update, something is wrong with my SQLTags usage.
+* TagFile.save_tagsets: update_mapping: do not swallow AttributeError.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no \"name\")
@@ -669,14 +670,18 @@
           type type_name + entity_name [tags...]
             Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* TagFile.save_tagsets: catch and warn about exceptions from update_mapping[key].update, something is wrong with my SQLTags usage.
+* TagFile.save_tagsets: update_mapping: do not swallow AttributeError.
+
 *Release 20230407*:
 Move the (optional) ORM open/close from FSTags.startup_shutdown to TagFile.save, greatly shortens the ORM lock.
 
 *Release 20230212*:
 Mark TagSetCriterion as Promotable.
 
 *Release 20230210*:
```

### Comparing `cs.tagset-20230407/setup.cfg` & `cs.tagset-20230612/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.tagset
-version = 20230407
+version = 20230612
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Tags and sets of tags with __format__ support and optional ontology information.
 keywords = python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -22,23 +22,23 @@
 package_dir = 
 	= lib/python
 install_requires = 
 	cs.cmdutils>=20210404
 	cs.dateutils>=20230210
 	cs.deco>=20230331
 	cs.edit>=20220429
-	cs.fileutils>=20230401
+	cs.fileutils>=20230421
 	cs.fs>=20220429
 	cs.lex>=20230401
 	cs.logutils>=20230212
-	cs.mappings>=20220912.4
+	cs.mappings>=20230612
 	cs.obj>=20200716
-	cs.pfx>=20230331
+	cs.pfx>=20230604
 	cs.py3>=20220523
-	cs.resources>=20230331
+	cs.resources>=20230503
 	cs.threads>=20230331
 	icontract
 	typeguard
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

