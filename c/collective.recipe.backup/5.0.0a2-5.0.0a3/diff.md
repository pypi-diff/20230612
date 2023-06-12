# Comparing `tmp/collective.recipe.backup-5.0.0a2.tar.gz` & `tmp/collective.recipe.backup-5.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.recipe.backup-5.0.0a2.tar", last modified: Wed Feb  1 22:35:52 2023, max compression
+gzip compressed data, was "collective.recipe.backup-5.0.0a3.tar", last modified: Wed Mar 15 14:20:59 2023, max compression
```

## Comparing `collective.recipe.backup-5.0.0a2.tar` & `collective.recipe.backup-5.0.0a3.tar`

### file list

```diff
@@ -1,53 +1,50 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-01 22:35:52.946955 collective.recipe.backup-5.0.0a2/
--rw-r--r--   0 maurits    (501) staff       (20)    21993 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)       84 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    54934 2023-02-01 22:35:52.947109 collective.recipe.backup-5.0.0a2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    30667 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1546 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       64 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)      170 2023-02-01 22:35:52.947616 collective.recipe.backup-5.0.0a2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-01 22:35:52.933380 collective.recipe.backup-5.0.0a2/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-01 22:35:52.936244 collective.recipe.backup-5.0.0a2/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)      245 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-01 22:35:52.938806 collective.recipe.backup-5.0.0a2/src/collective/recipe/
--rw-r--r--   0 maurits    (501) staff       (20)      245 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-01 22:35:52.940567 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/
--rw-r--r--   0 maurits    (501) staff       (20)    28770 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      137 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/config.py
--rw-r--r--   0 maurits    (501) staff       (20)    56802 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/copyblobs.py
--rw-r--r--   0 maurits    (501) staff       (20)    11383 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/main.py
--rw-r--r--   0 maurits    (501) staff       (20)    13371 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/repozorunner.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-01 22:35:52.946712 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       10 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    19402 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/altrestore.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8304 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/backup_blobs_archive.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6864 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/backup_blobs_dir.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7950 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/backup_blobs_dir_hard_links.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6028 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/base.rst
--rw-r--r--   0 maurits    (501) staff       (20)    33313 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/blob_timestamps.rst
--rw-r--r--   0 maurits    (501) staff       (20)    46902 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/blobs.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5815 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/cleanup_archives.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3777 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/cleanup_dir.rst
--rw-r--r--   0 maurits    (501) staff       (20)    12712 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/gzip.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9413 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/incremental_blobs.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2908 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/location.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9596 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/multiple.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5854 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/no_rsync.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6916 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/options.rst
--rw-r--r--   0 maurits    (501) staff       (20)    15147 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/prefix.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3972 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)    22882 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/test_unit.py
--rw-r--r--   0 maurits    (501) staff       (20)     6127 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/zipbackup.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4855 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/zope2instance.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6245 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-01 22:35:52.938535 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    54934 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1898 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       29 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       91 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-02-01 22:35:52.000000 collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-15 14:20:59.387684 collective.recipe.backup-5.0.0a3/
+-rw-r--r--   0 maurits    (501) staff       (20)    23580 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       84 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    52734 2023-03-15 14:20:59.387817 collective.recipe.backup-5.0.0a3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    26857 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1546 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       64 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2023-03-15 14:20:59.388263 collective.recipe.backup-5.0.0a3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2231 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-15 14:20:59.372455 collective.recipe.backup-5.0.0a3/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-15 14:20:59.375885 collective.recipe.backup-5.0.0a3/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-15 14:20:59.379396 collective.recipe.backup-5.0.0a3/src/collective/recipe/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-15 14:20:59.381701 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/
+-rw-r--r--   0 maurits    (501) staff       (20)    26191 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      137 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/config.py
+-rw-r--r--   0 maurits    (501) staff       (20)    56802 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/copyblobs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10696 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/main.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13153 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/repozorunner.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-15 14:20:59.387483 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       10 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14107 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/altrestore.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8304 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/backup_blobs_archive.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6864 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/backup_blobs_dir.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7950 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/backup_blobs_dir_hard_links.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6028 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/base.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16758 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/blob_timestamps.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    30069 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/blobs.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5815 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/cleanup_archives.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3777 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/cleanup_dir.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     9413 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/incremental_blobs.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2908 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/location.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5854 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/no_rsync.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5711 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/options.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    15147 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/prefix.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3540 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22882 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/test_unit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6107 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/zipbackup.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6139 2023-03-15 14:20:58.000000 collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-15 14:20:59.378921 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    52734 2023-03-15 14:20:59.000000 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1753 2023-03-15 14:20:59.000000 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-15 14:20:59.000000 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-15 14:20:59.000000 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       29 2023-03-15 14:20:59.000000 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-15 14:20:59.000000 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       91 2023-03-15 14:20:59.000000 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-03-15 14:20:59.000000 collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/top_level.txt
```

### Comparing `collective.recipe.backup-5.0.0a2/CHANGES.rst` & `collective.recipe.backup-5.0.0a3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,46 @@
          fix problems like typo corrections or such.
 
          To add a new change log entry, please see the notes from the ``pip`` project at
              https://pip.pypa.io/en/latest/development/#adding-a-news-entry
 
 .. towncrier release notes start
 
+5.0.0a3 (2023-03-15)
+====================
+
+Breaking changes:
+
+
+- Removed ``additional_filestorages`` option.
+  Removed support in ``alternative_restore_sources`` for multiple storages: only the standard single filestorage plus blobstorage is supported.
+  Renamed ``alternative_restore_sources`` to ``alternative_restore_source``, keeping the old alias for now.
+  [maurits] (`Issue #64 <https://github.com/collective/collective.recipe.backup/issues/64>`_)
+- Removed ``gzip`` option.
+  From now on, we always call repozo with the gzip option, you can no longer turn this off.
+  [maurits] (`Issue #67 <https://github.com/collective/collective.recipe.backup/issues/67>`_)
+- Removed option ``gzip_blob``.
+  This was a backwards compatibility alias for ``archive_blob``.
+  You should use that now it you want to create a tar archive.
+  Additionally use the ``compress_blob`` option if you are really sure you want to compress the archive.
+  [maurits] (`Issue #68 <https://github.com/collective/collective.recipe.backup/issues/68>`_)
+- Removed option ``quick``.
+  From now on, we always call repozo with the quick option for normal backups, you can no longer turn this off.
+  For full backups (snapshotbackups and zipbackups), the quick option is not used.
+  [maurits] (`Issue #69 <https://github.com/collective/collective.recipe.backup/issues/69>`_)
+
+
+Bug fixes:
+
+
+- Deprecate setting blob_timestamps to false.
+  See `issue 65 <https://github.com/collective/collective.recipe.backup/issues/65>`_.
+  [maurits] (`Issue #65 <https://github.com/collective/collective.recipe.backup/issues/65>`_)
+
+
 5.0.0a2 (2023-02-01)
 ====================
 
 Bug fixes:
 
 - Add missing changelog entries for release 5.0.0a1.  [maurits]
```

### Comparing `collective.recipe.backup-5.0.0a2/CONTRIBUTORS.rst` & `collective.recipe.backup-5.0.0a3/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/PKG-INFO` & `collective.recipe.backup-5.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.recipe.backup
-Version: 5.0.0a2
+Version: 5.0.0a3
 Summary: bin/backup script: sensible defaults around bin/repozo
 Home-page: https://github.com/collective/collective.recipe.backup
 Author: Reinout van Rees, Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL
 Keywords: buildout backup repozo zope
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Requires-Python: >=3.8
 Provides-Extra: tests
 
 Easy Zope backup/restore recipe for buildout
 ********************************************
 
 .. image:: https://github.com/collective/collective.recipe.backup/workflows/tests/badge.svg
     :target: https://github.com/collective/collective.recipe.backup/actions?query=workflow%3Atests
@@ -144,17 +145,14 @@
 ==============
 
 Which data does this recipe backup?
 
 - The Zope Object DataBase (ZODB) filestorage, by default located at
   ``var/filestorage/Data.fs``.
 
-- Possibly additional filestorages, see the
-  ``additional_filestorages`` option.
-
 - The blobstorage (since version 2.0) if your buildout uses it, by
   default located at ``var/blobstorage``.
 
 
 Data that is *not* backed up
 ============================
 
@@ -209,17 +207,14 @@
 do not want to use ``scp`` to recursively copy over all those blob
 files: downloading one tarball is faster.
 
 You can use the ``bin/zipbackup`` script for this.  This script
 overrides a few settings, ignoring whatever is set in the buildout
 config section:
 
-- ``gzip`` is explicitly turned on for the filestorage (this is
-  already the default, but we make sure).
-
 - ``archive_blob`` is turned on.
 
 - ``keep`` is set to 1 to avoid keeping lots of needless backups.
 
 - ``keep_blob_days`` is ignored because it is a full backup.
 
 The script places a full backup in, by default, ``var/zipbackups`` and
@@ -303,33 +298,31 @@
 default. The most common ones to change are ``location`` and
 ``blobbackuplocation``, as those allow you to place your backups in
 some system-wide directory like ``/var/zopebackups/instancename/`` and
 ``/var/zopebackups/instancename-blobs/``.
 
 .. Note: keep this in alphabetical order please.
 
-``additional_filestorages``
-    Advanced option, only needed when you have split for instance a
-    ``catalog.fs`` out of the regular ``Data.fs``.
-    Use it to specify the extra filestorages.
-    (See `Advanced usage: multiple Data.fs files`_).
-
 ``archive_blob``
     Use ``tar`` archiving functionality. ``false`` by default. Set it to ``true``
     and backup/restore will be done with ``tar`` command. Note that ``tar``
     command must be available on machine if this option is set to ``true``.
     This option also works with snapshot backup/restore commands. As this
     counts as a full backup ``keep_blob_days`` is ignored.
     See the ``compress_blob`` option if you want to compress the archive.
 
-``alternative_restore_sources``
+``alternative_restore_source``
     You can restore from an alternative source.  Use case: first make
     a backup of your production site, then go to the testing or
     staging server and restore the production data there.  See
-    `Alternative restore sources`_
+    `Alternative restore source`_
+
+``alternative_restore_sources``
+    Backwards compatibility spelling for ``alternative_restore_source``.
+    This will no longer work in version 7.
 
 ``backup_blobs``
     Backup the blob storage.  Default is ``True`` on Python 2.6 (Plone
     4) and higher, and ``False`` otherwise.  This requires the
     ``blob_storage`` location to be set.  If no ``blob_storage``
     location has been set and we cannot find one by looking in the
     other buildout parts, we quit with an error (since version 2.22).
@@ -414,24 +407,14 @@
     If ``backup_blobs`` is not on, these scripts are always disabled,
     because they are not useful then.
 
 ``full``
     By default, incremental backups are made. If this option is set to ``true``,
     ``bin/backup`` will always make a full backup.
 
-``gzip``
-    Use repozo's zipping functionality. ``true`` by default. Set it to ``false``
-    and repozo will not gzip its files. Note that gzipped databases are called
-    ``*.fsz``, not ``*.fs.gz``. **Changed in 0.8**: the default used to be
-    false, but it so totally makes sense to gzip your backups that we changed
-    the default.
-
-``gzip_blob``
-    Backwards compatibility alias for ``archive_blob`` option.
-
 ``incremental_blobs``
     New in version 4.0.  Default is false.
     When switched on, it will use the ``--listed-incremental`` option of ``tar``.
     Note: this only works with the GNU version of ``tar``.
     On Mac you may need to install this with ``brew install gnu-tar`` and change your ``PATH`` according to the instructions.
     It will create a metadata or `snapshot file <https://www.gnu.org/software/tar/manual/html_node/Incremental-Dumps.html>`_
     so that a second call to the backup script will create a second tarball with only the differences.
@@ -521,15 +504,15 @@
     a backup from a symlinked directory, in which case
     ``rsync_options = --no-l -k`` does the trick.
 
 ``rsync_hard_links_on_first_copy``
     When using ``rsync``, the blob files for the first backup are copied
     and then subsequent backups make use of hard links from this initial
     copy, to save time and disk space.
-    Enable this option to also use hard links for the initial copy to further reduce 
+    Enable this option to also use hard links for the initial copy to further reduce
     disk usage.
     This is safe for ZODB blobs, since they are not modified in place.
     The ``blob_storage`` and the backup folder ``blobbackuplocation``
     have to be in the same partition for hard links to be possible.
 
 ``snapshotlocation``
     Location where snapshot backups of the filestorage are stored. Defaults to
@@ -553,15 +536,14 @@
     recipe = collective.recipe.backup
     location = ${buildout:directory}/myproject
     keep = 2
     datafs = subfolder/myproject.fs
     full = true
     debug = true
     snapshotlocation = snap/my
-    gzip = false
     enable_snapshotrestore = true
     pre_command = echo 'Can I have a backup?'
     post_command =
         echo 'Thanks a lot for the backup.'
         echo 'We are done.'
 
 Paths in directories or files can use relative (``../``) paths, and
@@ -584,79 +566,14 @@
 
     [backupcronjob]
     recipe = z3c.recipe.usercrontab
     times = 0 12 * * *
     command = ${buildout:directory}/bin/backup
 
 
-Advanced usage: multiple Data.fs files
-======================================
-
-Sometimes, a filestorage is split into several files. Most common reason is to
-have a regular ``Data.fs`` and a ``catalog.fs`` which contains the
-``portal_catalog``. This is supported with the ``additional_filestorages``
-option::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        catalog
-        another
-
-This means that, with the standard ``Data.fs``, the ``bin/backup``
-script will now backup three filestorages::
-
-    var/filestorage/Data.fs
-    var/filestorage/catalog.fs
-    var/filestorage/another.fs
-
-The additional backups have to be stored separate from the ``Data.fs``
-backup. That's done by appending the file's name and creating extra backup
-directories named that way::
-
-    var/backups_catalog
-    var/snapshotbackups_catalog
-    var/backups_another
-    var/snapshotbackups_another
-
-The various backups are done one after the other. They cannot be done at the
-same time with ``repozo``. So they are not completely in sync. The "other"
-databases are backed up first as a small difference in the catalog is just
-mildly irritating, but the other way around users can get real errors.
-
-In the ``additional_filestorages`` option you can define different
-filestorages using this syntax::
-
-    additional_filestorages =
-        storagename1 [datafs1_path [blobdir1]]
-        storagename2 [datafs2_path [blobdir2]]
-        ...
-
-So if you want more control over the filestorage source path, you can
-explicitly set it, with or without the blobstorage path.  For
-example::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        foo ${buildout:directory}/var/filestorage/foo/foo.fs ${buildout:directory}/var/blobstorage-foo
-        bar ${buildout:directory}/var/filestorage/bar/bar.fs
-
-If the ``datafs_path`` is missing, then the default value will be used
-(``var/filestorage/storagename1.fs``).  If you do not specify a
-``blobdir``, then this means no blobs will be backed up for that
-storage.  Note that if you specify ``blobdir`` you must specify
-``datafs_path`` as well.
-
-Note that ``collective.recipe.filestorage`` creates additional
-filestorages in a slightly different location, but you can explictly define the
-paths of filestorage and blobstorage for all the ``parts`` defined in the recipe.
-Work is in progress to improve this.
-
-
 Blob storage
 ============
 
 Added in version 2.0.
 
 We can backup the blob storage.  Plone 4 uses a blob storage to store
 files (Binary Large OBjects) on the file system.  In Plone 3 this is
@@ -713,74 +630,60 @@
 http://www.mikerubel.org/computers/rsync_snapshots/
 
 We have not tried this on Windows.  Reports are welcome, but best is
 probably to set the ``use_rsync = false`` option in the backup part.
 Then we simply copy the blobstorage directory.
 
 
-Alternative restore sources
-===========================
+Alternative restore source
+==========================
 
 Added in version 2.17.
+Changed in version 5: only one source is supported.
 
 You can restore from an alternative source.  Use case: first make a
 backup of your production site, then go to the testing or staging
 server and restore the production data there.
 
-In the ``alternative_restore_sources`` option you can define different
+In the ``alternative_restore_source`` option you can define different
 filestorage and blobstorage backup source directories using this
 syntax::
 
-    alternative_restore_sources =
-        storagename1 datafs1_backup [blobdir1_backup]
-        storagename2 datafs2_backup [blobdir2_backup]
-        ...
+    alternative_restore_source =
+        storagename datafs1_backup [blobdir1_backup]
 
-The storagenames *must* be the same as in the additional_filestorages
-option, plus a key ``Data`` (or ``1``) for the standard ``Data.fs``
+The storagename must be ``Data`` (or ``1``) for the standard ``Data.fs``
 and optionally its blobstorage.
 
 The result is a ``bin/altrestore`` script.
 
 This will work for a standard buildout with a single filestorage and
 blobstorage::
 
     [backup]
     recipe = collective.recipe.backup
-    alternative_restore_sources =
+    alternative_restore_source =
         Data /path/to/production/var/backups /path/to/production/var/blobstoragebackups
 
 The above configuration uses ``repozo`` to restore the Data.fs from
 the ``/path/to/production/var/backups`` repository to the standard
 ``var/filestorage/Data.fs`` location.  It copies the most recent
 blobstorage backup from
 ``/path/to/production/var/blobstoragebackups/`` to the standard
 ``var/blobstorage`` location.
 
 Calling the script with a specific date is supported just like the
 normal restore script::
 
     bin/altrestore 2000-12-31-23-59
 
-If you have additional filestorages, it would be like this::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        foo ${buildout:directory}/var/filestorage/foo/foo.fs ${buildout:directory}/var/blobstorage-foo
-        bar ${buildout:directory}/var/filestorage/bar/bar.fs
-    alternative_restore_sources =
-        Data /path/to/production/var/backups /path/to/production/var/blobstoragebackups
-        foo /path/to/production/var/backups_foo /path/to/production/var/blobstoragebackups_foo
-        bar /path/to/production/var/backups_bar
-
-The recipe will fail if the alternative sources do not match the
-standard filestorage, blobstorage and additional storages.  For
-example, you get an error when the ``alternative_restore_sources`` is
-missing the ``Data`` key, when it has extra or missing keys, when a
+The recipe will fail if the alternative source does not match the
+standard filestorage and blobstorage.  For
+example, you get an error when the ``alternative_restore_source`` is
+missing the ``Data`` key, when it has an extra key, when a
 key has no paths, when a key has an extra or missing blobstorage.
 
 During install of the recipe, so during the ``bin/buildout`` run, it
 does not check if the sources exist: you might have the production
 backups on a different server and need to setup a remote shared
 directory, or you copy the data over manually.
 
@@ -838,14 +741,46 @@
          fix problems like typo corrections or such.
 
          To add a new change log entry, please see the notes from the ``pip`` project at
              https://pip.pypa.io/en/latest/development/#adding-a-news-entry
 
 .. towncrier release notes start
 
+5.0.0a3 (2023-03-15)
+====================
+
+Breaking changes:
+
+
+- Removed ``additional_filestorages`` option.
+  Removed support in ``alternative_restore_sources`` for multiple storages: only the standard single filestorage plus blobstorage is supported.
+  Renamed ``alternative_restore_sources`` to ``alternative_restore_source``, keeping the old alias for now.
+  [maurits] (`Issue #64 <https://github.com/collective/collective.recipe.backup/issues/64>`_)
+- Removed ``gzip`` option.
+  From now on, we always call repozo with the gzip option, you can no longer turn this off.
+  [maurits] (`Issue #67 <https://github.com/collective/collective.recipe.backup/issues/67>`_)
+- Removed option ``gzip_blob``.
+  This was a backwards compatibility alias for ``archive_blob``.
+  You should use that now it you want to create a tar archive.
+  Additionally use the ``compress_blob`` option if you are really sure you want to compress the archive.
+  [maurits] (`Issue #68 <https://github.com/collective/collective.recipe.backup/issues/68>`_)
+- Removed option ``quick``.
+  From now on, we always call repozo with the quick option for normal backups, you can no longer turn this off.
+  For full backups (snapshotbackups and zipbackups), the quick option is not used.
+  [maurits] (`Issue #69 <https://github.com/collective/collective.recipe.backup/issues/69>`_)
+
+
+Bug fixes:
+
+
+- Deprecate setting blob_timestamps to false.
+  See `issue 65 <https://github.com/collective/collective.recipe.backup/issues/65>`_.
+  [maurits] (`Issue #65 <https://github.com/collective/collective.recipe.backup/issues/65>`_)
+
+
 5.0.0a2 (2023-02-01)
 ====================
 
 Bug fixes:
 
 - Add missing changelog entries for release 5.0.0a1.  [maurits]
```

### Comparing `collective.recipe.backup-5.0.0a2/README.rst` & `collective.recipe.backup-5.0.0a3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -120,17 +120,14 @@
 ==============
 
 Which data does this recipe backup?
 
 - The Zope Object DataBase (ZODB) filestorage, by default located at
   ``var/filestorage/Data.fs``.
 
-- Possibly additional filestorages, see the
-  ``additional_filestorages`` option.
-
 - The blobstorage (since version 2.0) if your buildout uses it, by
   default located at ``var/blobstorage``.
 
 
 Data that is *not* backed up
 ============================
 
@@ -185,17 +182,14 @@
 do not want to use ``scp`` to recursively copy over all those blob
 files: downloading one tarball is faster.
 
 You can use the ``bin/zipbackup`` script for this.  This script
 overrides a few settings, ignoring whatever is set in the buildout
 config section:
 
-- ``gzip`` is explicitly turned on for the filestorage (this is
-  already the default, but we make sure).
-
 - ``archive_blob`` is turned on.
 
 - ``keep`` is set to 1 to avoid keeping lots of needless backups.
 
 - ``keep_blob_days`` is ignored because it is a full backup.
 
 The script places a full backup in, by default, ``var/zipbackups`` and
@@ -279,33 +273,31 @@
 default. The most common ones to change are ``location`` and
 ``blobbackuplocation``, as those allow you to place your backups in
 some system-wide directory like ``/var/zopebackups/instancename/`` and
 ``/var/zopebackups/instancename-blobs/``.
 
 .. Note: keep this in alphabetical order please.
 
-``additional_filestorages``
-    Advanced option, only needed when you have split for instance a
-    ``catalog.fs`` out of the regular ``Data.fs``.
-    Use it to specify the extra filestorages.
-    (See `Advanced usage: multiple Data.fs files`_).
-
 ``archive_blob``
     Use ``tar`` archiving functionality. ``false`` by default. Set it to ``true``
     and backup/restore will be done with ``tar`` command. Note that ``tar``
     command must be available on machine if this option is set to ``true``.
     This option also works with snapshot backup/restore commands. As this
     counts as a full backup ``keep_blob_days`` is ignored.
     See the ``compress_blob`` option if you want to compress the archive.
 
-``alternative_restore_sources``
+``alternative_restore_source``
     You can restore from an alternative source.  Use case: first make
     a backup of your production site, then go to the testing or
     staging server and restore the production data there.  See
-    `Alternative restore sources`_
+    `Alternative restore source`_
+
+``alternative_restore_sources``
+    Backwards compatibility spelling for ``alternative_restore_source``.
+    This will no longer work in version 7.
 
 ``backup_blobs``
     Backup the blob storage.  Default is ``True`` on Python 2.6 (Plone
     4) and higher, and ``False`` otherwise.  This requires the
     ``blob_storage`` location to be set.  If no ``blob_storage``
     location has been set and we cannot find one by looking in the
     other buildout parts, we quit with an error (since version 2.22).
@@ -390,24 +382,14 @@
     If ``backup_blobs`` is not on, these scripts are always disabled,
     because they are not useful then.
 
 ``full``
     By default, incremental backups are made. If this option is set to ``true``,
     ``bin/backup`` will always make a full backup.
 
-``gzip``
-    Use repozo's zipping functionality. ``true`` by default. Set it to ``false``
-    and repozo will not gzip its files. Note that gzipped databases are called
-    ``*.fsz``, not ``*.fs.gz``. **Changed in 0.8**: the default used to be
-    false, but it so totally makes sense to gzip your backups that we changed
-    the default.
-
-``gzip_blob``
-    Backwards compatibility alias for ``archive_blob`` option.
-
 ``incremental_blobs``
     New in version 4.0.  Default is false.
     When switched on, it will use the ``--listed-incremental`` option of ``tar``.
     Note: this only works with the GNU version of ``tar``.
     On Mac you may need to install this with ``brew install gnu-tar`` and change your ``PATH`` according to the instructions.
     It will create a metadata or `snapshot file <https://www.gnu.org/software/tar/manual/html_node/Incremental-Dumps.html>`_
     so that a second call to the backup script will create a second tarball with only the differences.
@@ -497,15 +479,15 @@
     a backup from a symlinked directory, in which case
     ``rsync_options = --no-l -k`` does the trick.
 
 ``rsync_hard_links_on_first_copy``
     When using ``rsync``, the blob files for the first backup are copied
     and then subsequent backups make use of hard links from this initial
     copy, to save time and disk space.
-    Enable this option to also use hard links for the initial copy to further reduce 
+    Enable this option to also use hard links for the initial copy to further reduce
     disk usage.
     This is safe for ZODB blobs, since they are not modified in place.
     The ``blob_storage`` and the backup folder ``blobbackuplocation``
     have to be in the same partition for hard links to be possible.
 
 ``snapshotlocation``
     Location where snapshot backups of the filestorage are stored. Defaults to
@@ -529,15 +511,14 @@
     recipe = collective.recipe.backup
     location = ${buildout:directory}/myproject
     keep = 2
     datafs = subfolder/myproject.fs
     full = true
     debug = true
     snapshotlocation = snap/my
-    gzip = false
     enable_snapshotrestore = true
     pre_command = echo 'Can I have a backup?'
     post_command =
         echo 'Thanks a lot for the backup.'
         echo 'We are done.'
 
 Paths in directories or files can use relative (``../``) paths, and
@@ -560,79 +541,14 @@
 
     [backupcronjob]
     recipe = z3c.recipe.usercrontab
     times = 0 12 * * *
     command = ${buildout:directory}/bin/backup
 
 
-Advanced usage: multiple Data.fs files
-======================================
-
-Sometimes, a filestorage is split into several files. Most common reason is to
-have a regular ``Data.fs`` and a ``catalog.fs`` which contains the
-``portal_catalog``. This is supported with the ``additional_filestorages``
-option::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        catalog
-        another
-
-This means that, with the standard ``Data.fs``, the ``bin/backup``
-script will now backup three filestorages::
-
-    var/filestorage/Data.fs
-    var/filestorage/catalog.fs
-    var/filestorage/another.fs
-
-The additional backups have to be stored separate from the ``Data.fs``
-backup. That's done by appending the file's name and creating extra backup
-directories named that way::
-
-    var/backups_catalog
-    var/snapshotbackups_catalog
-    var/backups_another
-    var/snapshotbackups_another
-
-The various backups are done one after the other. They cannot be done at the
-same time with ``repozo``. So they are not completely in sync. The "other"
-databases are backed up first as a small difference in the catalog is just
-mildly irritating, but the other way around users can get real errors.
-
-In the ``additional_filestorages`` option you can define different
-filestorages using this syntax::
-
-    additional_filestorages =
-        storagename1 [datafs1_path [blobdir1]]
-        storagename2 [datafs2_path [blobdir2]]
-        ...
-
-So if you want more control over the filestorage source path, you can
-explicitly set it, with or without the blobstorage path.  For
-example::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        foo ${buildout:directory}/var/filestorage/foo/foo.fs ${buildout:directory}/var/blobstorage-foo
-        bar ${buildout:directory}/var/filestorage/bar/bar.fs
-
-If the ``datafs_path`` is missing, then the default value will be used
-(``var/filestorage/storagename1.fs``).  If you do not specify a
-``blobdir``, then this means no blobs will be backed up for that
-storage.  Note that if you specify ``blobdir`` you must specify
-``datafs_path`` as well.
-
-Note that ``collective.recipe.filestorage`` creates additional
-filestorages in a slightly different location, but you can explictly define the
-paths of filestorage and blobstorage for all the ``parts`` defined in the recipe.
-Work is in progress to improve this.
-
-
 Blob storage
 ============
 
 Added in version 2.0.
 
 We can backup the blob storage.  Plone 4 uses a blob storage to store
 files (Binary Large OBjects) on the file system.  In Plone 3 this is
@@ -689,74 +605,60 @@
 http://www.mikerubel.org/computers/rsync_snapshots/
 
 We have not tried this on Windows.  Reports are welcome, but best is
 probably to set the ``use_rsync = false`` option in the backup part.
 Then we simply copy the blobstorage directory.
 
 
-Alternative restore sources
-===========================
+Alternative restore source
+==========================
 
 Added in version 2.17.
+Changed in version 5: only one source is supported.
 
 You can restore from an alternative source.  Use case: first make a
 backup of your production site, then go to the testing or staging
 server and restore the production data there.
 
-In the ``alternative_restore_sources`` option you can define different
+In the ``alternative_restore_source`` option you can define different
 filestorage and blobstorage backup source directories using this
 syntax::
 
-    alternative_restore_sources =
-        storagename1 datafs1_backup [blobdir1_backup]
-        storagename2 datafs2_backup [blobdir2_backup]
-        ...
+    alternative_restore_source =
+        storagename datafs1_backup [blobdir1_backup]
 
-The storagenames *must* be the same as in the additional_filestorages
-option, plus a key ``Data`` (or ``1``) for the standard ``Data.fs``
+The storagename must be ``Data`` (or ``1``) for the standard ``Data.fs``
 and optionally its blobstorage.
 
 The result is a ``bin/altrestore`` script.
 
 This will work for a standard buildout with a single filestorage and
 blobstorage::
 
     [backup]
     recipe = collective.recipe.backup
-    alternative_restore_sources =
+    alternative_restore_source =
         Data /path/to/production/var/backups /path/to/production/var/blobstoragebackups
 
 The above configuration uses ``repozo`` to restore the Data.fs from
 the ``/path/to/production/var/backups`` repository to the standard
 ``var/filestorage/Data.fs`` location.  It copies the most recent
 blobstorage backup from
 ``/path/to/production/var/blobstoragebackups/`` to the standard
 ``var/blobstorage`` location.
 
 Calling the script with a specific date is supported just like the
 normal restore script::
 
     bin/altrestore 2000-12-31-23-59
 
-If you have additional filestorages, it would be like this::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        foo ${buildout:directory}/var/filestorage/foo/foo.fs ${buildout:directory}/var/blobstorage-foo
-        bar ${buildout:directory}/var/filestorage/bar/bar.fs
-    alternative_restore_sources =
-        Data /path/to/production/var/backups /path/to/production/var/blobstoragebackups
-        foo /path/to/production/var/backups_foo /path/to/production/var/blobstoragebackups_foo
-        bar /path/to/production/var/backups_bar
-
-The recipe will fail if the alternative sources do not match the
-standard filestorage, blobstorage and additional storages.  For
-example, you get an error when the ``alternative_restore_sources`` is
-missing the ``Data`` key, when it has extra or missing keys, when a
+The recipe will fail if the alternative source does not match the
+standard filestorage and blobstorage.  For
+example, you get an error when the ``alternative_restore_source`` is
+missing the ``Data`` key, when it has an extra key, when a
 key has no paths, when a key has an extra or missing blobstorage.
 
 During install of the recipe, so during the ``bin/buildout`` run, it
 does not check if the sources exist: you might have the production
 backups on a different server and need to setup a remote shared
 directory, or you copy the data over manually.
```

### Comparing `collective.recipe.backup-5.0.0a2/pyproject.toml` & `collective.recipe.backup-5.0.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/setup.py` & `collective.recipe.backup-5.0.0a3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 
 def read(*rnames):
     return open(os.path.join(*rnames)).read()
 
 
-version = "5.0.0a2"
+version = "5.0.0a3"
 
 long_description = (
     read("README.rst") + "\n" + "Contributors\n"
     "************\n" + "\n" + read("CONTRIBUTORS.rst") + "\n" + "Change history\n"
     "**************\n" + "\n" + read("CHANGES.rst")
 )
 entry_point = "collective.recipe.backup:Recipe"
@@ -55,14 +55,15 @@
     url="https://github.com/collective/collective.recipe.backup",
     license="GPL",
     package_dir={"": "src"},
     packages=find_packages("src"),
     namespace_packages=["collective", "collective.recipe"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
         "zc.buildout",
         "setuptools",
         "zc.recipe.egg",
     ],
     tests_require=tests_require,
     extras_require=dict(tests=tests_require),
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/__init__.py` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Recipe backup"""
 from collective.recipe.backup import utils
 
 import logging
 import os
 import pprint
 import re
-import sys
 import zc.buildout
 import zc.recipe.egg
 
 
 logger = logging.getLogger("backup")
 
+# Standard storage key for Data.fs.
+STORAGE_KEY = "1"
+
 
 class Recipe:
     """zc.buildout recipe"""
 
     def __init__(self, buildout, name, options):
         self.buildout, self.name, self.options = buildout, name, options
 
@@ -30,22 +32,15 @@
                 # Both options have been set explicitly, which is
                 # wrong.
                 raise zc.buildout.UserError(
                     "Both blob_storage and blob-storage have been set. "
                     "Please pick one."
                 )
 
-        # We usually want backup_blobs to be true.  If no blob_storage is
-        # found, we complain, unless backup_blobs has explicitly been disabled.
-        # Or when the Python version is lower than 2.6: we then expect Plone 3,
-        # so no blob storage.
-        if sys.version_info >= (2, 6):
-            options.setdefault("backup_blobs", "True")
-        else:
-            options.setdefault("backup_blobs", "False")
+        options.setdefault("backup_blobs", "True")
 
         # Validate options, checking for example that the locations are unique.
         self.validate()
 
     def install(self):
         """Installer"""
         options = self.options
@@ -121,33 +116,43 @@
         options.setdefault("snapshotlocation", snapshot_dir)
         options.setdefault("ziplocation", zip_backup_dir)
 
         # Validate options, checking that the locations are unique
         self.validate()
 
         # more options, alphabetical
-        options.setdefault("additional_filestorages", "")
-        options.setdefault("alternative_restore_sources", "")
-        # archive_blob used to be called gzip_blob.
-        options.setdefault("archive_blob", options.get("gzip_blob", "false"))
+        # options.setdefault(
+        #     "alternative_restore_source",
+        #     options.get("alternative_restore_sources", ""),
+        # )
+        options.setdefault("alternative_restore_source", "")
+        if not options["alternative_restore_source"]:
+            alt = options.get("alternative_restore_sources", "")
+            if alt:
+                options["alternative_restore_source"] = alt
+                logger.warning(
+                    "You should rename alternative_restore_sources "
+                    "to alternative_restore_source. In version 7 the "
+                    "old name will no longer work."
+                )
+
+        options.setdefault("archive_blob", "false")
         options.setdefault("blob_timestamps", "true")
         options.setdefault("compress_blob", "false")
         options.setdefault("datafs", datafs)
         options.setdefault("debug", "false")
         options.setdefault("enable_snapshotrestore", "true")
         options.setdefault("enable_zipbackup", "false")
         options.setdefault("full", "false")
-        options.setdefault("gzip", "true")
         options.setdefault("incremental_blobs", "false")
         options.setdefault("keep", "2")
         options.setdefault("keep_blob_days", "14")  # two weeks
         options.setdefault("only_blobs", "false")
         options.setdefault("post_command", "")
         options.setdefault("pre_command", "")
-        options.setdefault("quick", "true")
         options.setdefault("rsync_options", "")
         options.setdefault("use_rsync", "true")
         options.setdefault("rsync_hard_links_on_first_copy", "false")
 
         # Get the blob storage.
         blob_storage = options["blob_storage"]
         if not blob_storage:
@@ -202,96 +207,62 @@
         )
 
         # More locations.
         backup_location = construct_path(prefix, self.options["location"])
         snapshot_location = construct_path(prefix, self.options["snapshotlocation"])
         zip_location = construct_path(prefix, self.options["ziplocation"])
 
+        if not to_bool(options["blob_timestamps"]):
+            # blob_timestamps was explicitly set to false
+            logger.warning(
+                "You have disabled blob_timestamps. "
+                "Support for this may be dropped in version 6, "
+                "making it impossible to restore backups without timestamps. "
+                "See https://github.com/collective/collective.recipe.backup/issues/65"
+            )
+
         # Blob backup.
         if to_bool(self.options["backup_blobs"]):
             blob_backup_location = construct_path(
                 prefix, self.options["blobbackuplocation"]
             )
             blob_snapshot_location = construct_path(
                 prefix, self.options["blobsnapshotlocation"]
             )
             blob_zip_location = construct_path(prefix, self.options["blobziplocation"])
         else:
             blob_backup_location = ""
             blob_snapshot_location = ""
             blob_zip_location = ""
 
-        storages = self.compute_storages(
+        storage = self.compute_storage(
             buildout_dir,
             backup_location=backup_location,
             snapshot_location=snapshot_location,
             zip_location=zip_location,
             blob_backup_location=blob_backup_location,
             blob_snapshot_location=blob_snapshot_location,
             blob_zip_location=blob_zip_location,
         )
-        generated = self.generate_scripts(storages)
+        generated = self.generate_scripts(storage)
         return generated
 
-    def compute_storages(
+    def compute_storage(
         self,
         buildout_dir,
         backup_location,
         snapshot_location,
         zip_location,
         blob_backup_location,
         blob_snapshot_location,
         blob_zip_location,
     ):
-        storages = []
-        additional = self.options["additional_filestorages"]
+        # Note: we used to support additional storages,
+        # but that was dropped in version 5.
         datafs = construct_path(buildout_dir, self.options["datafs"])
-        filestorage_dir = os.path.split(datafs)[0]
-        if additional:
-            additional_regex = (
-                r"^\s*(?P<storage>[^\s]+)"
-                r"\s*(?P<datafs>[^\s]*)"
-                r"\s*(?P<blobdir>[^\s]*)\s*$"
-            )
-            for a in additional.split("\n"):
-                if not a:
-                    continue
-                storage = re.match(additional_regex, a).groupdict()
-                if storage["storage"] in [s["storage"] for s in storages]:
-                    logger.warning("storage {} duplicated".format(storage["storage"]))
-                if not storage["datafs"]:
-                    storage["datafs"] = os.path.join(
-                        filestorage_dir, "{}.fs".format(storage["storage"])
-                    )
-                storage["backup_location"] = "{}_{}".format(
-                    backup_location, storage["storage"]
-                )
-                storage["snapshot_location"] = "{}_{}".format(
-                    snapshot_location, storage["storage"]
-                )
-                storage["zip_location"] = "{}_{}".format(
-                    zip_location, storage["storage"]
-                )
-                if storage["blobdir"]:
-                    storage["blob_backup_location"] = (
-                        "{}_{}".format(blob_backup_location, storage["storage"])
-                        if blob_backup_location
-                        else None
-                    )
-                    storage["blob_snapshot_location"] = (
-                        "{}_{}".format(blob_snapshot_location, storage["storage"])
-                        if blob_snapshot_location
-                        else None
-                    )
-                    storage["blob_zip_location"] = (
-                        "{}_{}".format(blob_zip_location, storage["storage"])
-                        if blob_zip_location
-                        else None
-                    )
-                storages.append(storage)
 
         # '1' is the default root storagename for Zope. The property
         # ``storage`` on this recipe currently is used only for
         # logging.
         storage = dict(
             storage="1",
             datafs=datafs,
@@ -301,121 +272,102 @@
             zip_location=zip_location,
         )
 
         if storage["blobdir"]:
             storage["blob_backup_location"] = blob_backup_location
             storage["blob_snapshot_location"] = blob_snapshot_location
             storage["blob_zip_location"] = blob_zip_location
-        storages.append(storage)
 
         if not to_bool(self.options["only_blobs"]):
-            for s in storages:
-                backup_location = s["backup_location"]
-                snapshot_location = s["snapshot_location"]
-                utils.try_create_folder(backup_location)
-                utils.try_create_folder(snapshot_location)
+            backup_location = storage["backup_location"]
+            snapshot_location = storage["snapshot_location"]
+            utils.try_create_folder(backup_location)
+            utils.try_create_folder(snapshot_location)
 
         # Blob backup.
         if to_bool(self.options["backup_blobs"]):
-            blob_storage_found = False
-            for s in storages:
-                if s["blobdir"]:
-                    s["blobdir"] = s["blobdir"].rstrip(os.sep)
-                    blob_storage_found = True
-                    blob_backup_location = s["blob_backup_location"]
-                    blob_snapshot_location = s["blob_snapshot_location"]
-                    utils.try_create_folder(blob_backup_location)
-                    utils.try_create_folder(blob_snapshot_location)
-            if not blob_storage_found:
+            if not storage["blobdir"]:
                 raise zc.buildout.UserError(
-                    "backup_blobs is true, but no blob_storage could be " "found."
+                    "backup_blobs is true, but no blob_storage could be found."
                 )
+            storage["blobdir"] = storage["blobdir"].rstrip(os.sep)
+            blob_backup_location = storage["blob_backup_location"]
+            blob_snapshot_location = storage["blob_snapshot_location"]
+            utils.try_create_folder(blob_backup_location)
+            utils.try_create_folder(blob_snapshot_location)
 
         # Handle alternative restore sources.
-        storages = self.compute_alternative_restore_sources(buildout_dir, storages)
-        return storages
+        storage = self.compute_alternative_restore_source(buildout_dir, storage)
+        return storage
 
-    def compute_alternative_restore_sources(self, buildout_dir, storages):
-        """Compute alternative restore sources.
+    def compute_alternative_restore_source(self, buildout_dir, storage):
+        """Compute alternative restore source.
 
-        Return them in the storages list.
+        Return them in the storage.
+        Support for multiple sources for additional storages was dropped
+        in version 5.
         """
-        alt_sources = self.options["alternative_restore_sources"]
+        alt_sources = self.options["alternative_restore_source"]
         if not alt_sources:
-            return storages
-        storage_keys = [s["storage"] for s in storages]
-        alt_keys = []
+            return storage
+        found = False
         alt_regex = (
             r"^\s*(?P<storage>[^\s]+)"
             r"\s+(?P<datafs>[^\s]+)"
             r"\s*(?P<blobdir>[^\s]*)\s*$"
         )
         for a in alt_sources.split("\n"):
+            a = a.strip()
             if not a:
                 continue
+            if a.startswith("#"):
+                continue
+            if found:
+                raise zc.buildout.UserError(
+                    "Only one alternative_restore_source line is supported."
+                )
+            found = True
             match = re.match(alt_regex, a)
             if match is None:
                 raise zc.buildout.UserError(
-                    "alternative_restore_sources line {!r} has a wrong "
+                    "alternative_restore_source line {!r} has a wrong "
                     "format. Should be: 'storage-name "
                     "filestorage-backup-path', optionally followed by "
                     "a blobstorage-backup-path.".format(a)
                 )
             source = match.groupdict()
             key = orig_key = source["storage"]
             if key == "Data":
                 key = "1"  # Data.fs is called storage '1'.
-            if key not in storage_keys:
+            if key != STORAGE_KEY:
                 raise zc.buildout.UserError(
-                    "alternative_restore_sources key {!r} unknown in "
-                    "storages.".format(orig_key)
-                )
-            alt_keys.append(key)
-            storage = [s for s in storages if key == s["storage"]][0]
-            if storage.get("alt_location"):
-                # Duplicate key.
-                if key == "1":
-                    raise zc.buildout.UserError(
-                        "alternative_restore_sources key {!r} is used. "
-                        "Are you using both '1' and 'Data'? They are "
-                        "alternative keys for the same Data.fs.".format(orig_key)
-                    )
-                raise zc.buildout.UserError(
-                    "alternative_restore_sources key {!r} "
-                    "is used twice.".format(orig_key)
+                    "alternative_restore_source key {!r} unknown. "
+                    "Expected 1 or Data.".format(orig_key)
                 )
             storage["alt_location"] = construct_path(buildout_dir, source["datafs"])
             blobdir = source["blobdir"]
             if storage["blobdir"]:
                 if not blobdir:
                     raise zc.buildout.UserError(
-                        "alternative_restore_sources key {!r} is "
+                        "alternative_restore_source key {!r} is "
                         "missing a blobdir.".format(orig_key)
                     )
                 storage["blob_alt_location"] = construct_path(buildout_dir, blobdir)
             elif blobdir:
                 raise zc.buildout.UserError(
-                    "alternative_restore_sources key {!r} specifies "
+                    "alternative_restore_source key {!r} specifies "
                     "blobdir {!r} but the original storage has no "
                     "blobstorage.".format(orig_key, blobdir)
                 )
             else:
                 storage["blob_alt_location"] = ""
-        # Check that all original storages have an alternative.
-        for key in storage_keys:
-            if key not in alt_keys:
-                if key == "1":
-                    key = "Data"  # canonical spelling
-                raise zc.buildout.UserError(
-                    f"alternative_restore_sources is missing key {key!r}."
-                )
 
-        return storages
+        return storage
 
-    def generate_scripts(self, storages):
+    def generate_scripts(self, storage):
         """Generate scripts and return their names."""
         if to_bool(self.options["debug"]):
             loglevel = "DEBUG"
         else:
             loglevel = "INFO"
         initialization_template = """
 import logging
@@ -440,21 +392,19 @@
 if loglevel < logging.INFO:
     log_format = '%(asctime)s ' + log_format
 logging.basicConfig(level=loglevel,
     format=log_format)
 """
         arguments_template = """
         bin_dir={bin-directory!r},
-        storages={storages},
+        storage={storage},
         keep={keep},
         keep_blob_days={keep_blob_days},
         full={full},
         verbose={debug},
-        gzip={gzip},
-        quick={quick},
         only_blobs={only_blobs},
         backup_blobs={backup_blobs},
         use_rsync={use_rsync},
         rsync_options={rsync_options!r},
         archive_blob={archive_blob},
         compress_blob={compress_blob},
         pre_command={pre_command!r},
@@ -463,15 +413,15 @@
         blob_timestamps={blob_timestamps},
         incremental_blobs={incremental_blobs},
         rsync_hard_links_on_first_copy={rsync_hard_links_on_first_copy},
         """
         # Work with a copy of the options, for safety.
         opts = self.options.copy()
         opts["loglevel"] = loglevel
-        opts["storages"] = pprint.pformat(storages)
+        opts["storage"] = pprint.pformat(storage)
 
         # Keep list of generated files/directories/scripts
         generated = []
 
         # Handle a few alternative spellings:
         opts["bin_dir"] = opts["bin-directory"]
         opts["verbose"] = opts["debug"]
@@ -560,15 +510,15 @@
                     "snapshot_restore_main",
                 )
             ]
             creation_args["reqs"] = reqs
             generated += create_script(**creation_args)
 
         # Create alternative sources restore script
-        if self.options["alternative_restore_sources"]:
+        if self.options["alternative_restore_source"]:
             reqs = [
                 (
                     self.options["altrestore_name"],
                     "collective.recipe.backup.main",
                     "alt_restore_main",
                 )
             ]
@@ -589,20 +539,18 @@
     def validate(self):
         options = self.options
         check_for_true(
             options,
             [
                 "full",
                 "debug",
-                "gzip",
                 "only_blobs",
                 "backup_blobs",
                 "use_rsync",
                 "archive_blob",
-                "quick",
                 "enable_snapshotrestore",
                 "enable_zipbackup",
                 "compress_blob",
                 "blob_timestamps",
                 "incremental_blobs",
                 "rsync_hard_links_on_first_copy",
             ],
@@ -637,15 +585,15 @@
                     "Cannot have backup_blobs false and enable_zipbackup "
                     "true. zipbackup is useless without blobs."
                 )
         if not to_bool(options.get("blob_timestamps", True)):
             # blob_timestamps was explicitly set to false
             if to_bool(options.get("incremental_blobs")):
                 raise zc.buildout.UserError(
-                    "Cannot have blob_timestamps false and " "incremental_blobs true."
+                    "Cannot have blob_timestamps false and incremental_blobs true."
                 )
 
 
 def check_for_true(options, keys):
     """Set the truth options right.
 
     Default value is False, set it to True only if we're passed the string
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/copyblobs.py` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/copyblobs.py`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/main.py` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,109 +10,106 @@
 
 
 logger = logging.getLogger("backup")
 
 
 def backup_main(
     bin_dir,
-    storages,
+    storage,
     keep,
     full,
     verbose,
-    gzip,
     backup_blobs,
     only_blobs,
     use_rsync,
     keep_blob_days=0,
     pre_command="",
     post_command="",
     archive_blob=False,
     compress_blob=False,
     rsync_options="",
-    quick=True,
     blob_timestamps=False,
     backup_method=config.STANDARD_BACKUP,
     incremental_blobs=False,
     rsync_hard_links_on_first_copy=False,
     **kwargs,
 ):
     """Main method, gets called by generated bin/backup."""
     if backup_method not in config.BACKUP_METHODS:
         raise RuntimeError(f"Unknown backup method {backup_method}.")
     utils.execute_or_fail(pre_command)
     utils.check_folders(
-        storages,
+        storage,
         backup_blobs=backup_blobs,
         only_blobs=only_blobs,
         backup_method=backup_method,
     )
     if not only_blobs:
         result = repozorunner.backup_main(
-            bin_dir, storages, keep, full, verbose, gzip, quick, backup_method
+            bin_dir, storage, keep, full, verbose, backup_method
         )
         if result:
             if backup_blobs:
                 logger.error("Halting execution due to error; not backing up blobs.")
             else:
                 logger.error("Halting execution due to error.")
             sys.exit(1)
 
     if not backup_blobs:
         utils.execute_or_fail(post_command)
         return
-    for storage in storages:
-        blobdir = storage["blobdir"]
-        if not blobdir:
-            logger.info("No blob dir defined for %s storage", storage["storage"])
-            continue
-        blob_backup_location = None
-        if backup_method == config.STANDARD_BACKUP:
-            blob_backup_location = storage["blob_backup_location"]
-            logger.info(
-                "Please wait while backing up blobs from %s to %s",
-                blobdir,
-                blob_backup_location,
-            )
-        elif backup_method == config.SNAPSHOT_BACKUP:
-            blob_backup_location = storage["blob_snapshot_location"]
-            logger.info(
-                "Please wait while making snapshot of blobs from %s to %s",
-                blobdir,
-                blob_backup_location,
-            )
-        elif backup_method == config.ZIP_BACKUP:
-            blob_backup_location = storage["blob_zip_location"]
-            logger.info(
-                "Please wait while backing up blobs from %s to %s",
-                blobdir,
-                blob_backup_location,
-            )
-        if only_blobs:
-            fs_backup_location = None
-        elif backup_method == config.STANDARD_BACKUP:
-            fs_backup_location = storage["backup_location"]
-        elif backup_method == config.SNAPSHOT_BACKUP:
-            fs_backup_location = storage["snapshot_location"]
-        elif backup_method == config.ZIP_BACKUP:
-            fs_backup_location = storage["zip_location"]
-        copyblobs.backup_blobs(
+    blobdir = storage["blobdir"]
+    if not blobdir:
+        logger.info("No blob dir defined for %s storage", storage["storage"])
+        return
+    blob_backup_location = None
+    if backup_method == config.STANDARD_BACKUP:
+        blob_backup_location = storage["blob_backup_location"]
+        logger.info(
+            "Please wait while backing up blobs from %s to %s",
+            blobdir,
+            blob_backup_location,
+        )
+    elif backup_method == config.SNAPSHOT_BACKUP:
+        blob_backup_location = storage["blob_snapshot_location"]
+        logger.info(
+            "Please wait while making snapshot of blobs from %s to %s",
+            blobdir,
+            blob_backup_location,
+        )
+    elif backup_method == config.ZIP_BACKUP:
+        blob_backup_location = storage["blob_zip_location"]
+        logger.info(
+            "Please wait while backing up blobs from %s to %s",
             blobdir,
             blob_backup_location,
-            full,
-            use_rsync,
-            keep=keep,
-            keep_blob_days=keep_blob_days,
-            archive_blob=archive_blob,
-            compress_blob=compress_blob,
-            rsync_options=rsync_options,
-            timestamps=blob_timestamps,
-            fs_backup_location=fs_backup_location,
-            incremental_blobs=incremental_blobs,
-            rsync_hard_links_on_first_copy=rsync_hard_links_on_first_copy,
         )
+    if only_blobs:
+        fs_backup_location = None
+    elif backup_method == config.STANDARD_BACKUP:
+        fs_backup_location = storage["backup_location"]
+    elif backup_method == config.SNAPSHOT_BACKUP:
+        fs_backup_location = storage["snapshot_location"]
+    elif backup_method == config.ZIP_BACKUP:
+        fs_backup_location = storage["zip_location"]
+    copyblobs.backup_blobs(
+        blobdir,
+        blob_backup_location,
+        full,
+        use_rsync,
+        keep=keep,
+        keep_blob_days=keep_blob_days,
+        archive_blob=archive_blob,
+        compress_blob=compress_blob,
+        rsync_options=rsync_options,
+        timestamps=blob_timestamps,
+        fs_backup_location=fs_backup_location,
+        incremental_blobs=incremental_blobs,
+        rsync_hard_links_on_first_copy=rsync_hard_links_on_first_copy,
+    )
     utils.execute_or_fail(post_command)
 
 
 def snapshot_main(*args, **kwargs):
     """Main method, gets called by generated bin/snapshotbackup."""
     kwargs["full"] = True
     kwargs["incremental_blobs"] = False
@@ -120,24 +117,23 @@
     return backup_main(*args, **kwargs)
 
 
 def zipbackup_main(*args, **kwargs):
     """Main method, gets called by generated bin/zipbackup."""
     kwargs["backup_method"] = config.ZIP_BACKUP
     kwargs["full"] = True
-    kwargs["gzip"] = True
     kwargs["archive_blob"] = True
     kwargs["incremental_blobs"] = False
     kwargs["blob_timestamps"] = False
     kwargs["keep"] = 1
     return backup_main(*args, **kwargs)
 
 
 def check_blobs(
-    storages,
+    storage,
     use_rsync,
     restore_snapshot=False,
     archive_blob=False,
     alt_restore=False,
     rsync_options="",
     zip_restore=False,
     blob_timestamps=False,
@@ -145,60 +141,58 @@
 ):
     """Check that blobs can be restored.
 
     In this check run, we check what the blob backup location is,
     and set this as blob_backup_location, so we have to do this
     only once.
     """
-    for storage in storages:
-        blobdir = storage["blobdir"]
-        if not blobdir:
-            logger.info("No blob dir defined for %s storage", storage["storage"])
-            continue
-        if restore_snapshot:
-            blob_backup_location = storage["blob_snapshot_location"]
-        elif alt_restore:
-            blob_backup_location = storage["blob_alt_location"]
-        elif zip_restore:
-            blob_backup_location = storage["blob_zip_location"]
-        else:
-            blob_backup_location = storage["blob_backup_location"]
-        if not blob_backup_location:
-            logger.error("No blob storage source specified")
-            sys.exit(1)
-        storage["blob_backup_location"] = blob_backup_location
-        result = copyblobs.restore_blobs(
-            blob_backup_location,
-            blobdir,
-            use_rsync=use_rsync,
-            date=date,
-            archive_blob=archive_blob,
-            rsync_options=rsync_options,
-            timestamps=blob_timestamps,
-            only_check=True,
-        )
-        if result:
-            logger.error("Halting execution: " "restoring blobstorages would fail.")
-            sys.exit(1)
+    blobdir = storage["blobdir"]
+    if not blobdir:
+        logger.info("No blob dir defined for %s storage", storage["storage"])
+        return
+    if restore_snapshot:
+        blob_backup_location = storage["blob_snapshot_location"]
+    elif alt_restore:
+        blob_backup_location = storage["blob_alt_location"]
+    elif zip_restore:
+        blob_backup_location = storage["blob_zip_location"]
+    else:
+        blob_backup_location = storage["blob_backup_location"]
+    if not blob_backup_location:
+        logger.error("No blob storage source specified")
+        sys.exit(1)
+    storage["blob_backup_location"] = blob_backup_location
+    result = copyblobs.restore_blobs(
+        blob_backup_location,
+        blobdir,
+        use_rsync=use_rsync,
+        date=date,
+        archive_blob=archive_blob,
+        rsync_options=rsync_options,
+        timestamps=blob_timestamps,
+        only_check=True,
+    )
+    if result:
+        logger.error("Halting execution: " "restoring blobstorages would fail.")
+        sys.exit(1)
 
 
 def restore_check(
     bin_dir,
-    storages,
+    storage,
     verbose,
     backup_blobs,
     only_blobs,
     use_rsync,
     restore_snapshot=False,
     pre_command="",
     post_command="",
     archive_blob=False,
     alt_restore=False,
     rsync_options="",
-    quick=True,
     zip_restore=False,
     blob_timestamps=False,
     **kwargs,
 ):
     """Method to check that a restore will work.
 
     Returns the chosen date, if any.
@@ -213,132 +207,127 @@
     # Try to find a date in the command line arguments
     date = utils.get_date_from_args()
 
     if not kwargs.get("no_prompt"):
         question = "\n"
         if not only_blobs:
             question += "This will replace the filestorage:\n"
-            for storage in storages:
-                question += "    {}\n".format(storage.get("datafs"))
+            question += "    {}\n".format(storage.get("datafs"))
         if backup_blobs:
             question += "This will replace the blobstorage:\n"
-            for storage in storages:
-                if storage.get("blobdir"):
-                    question += "    {}\n".format(storage.get("blobdir"))
+            if storage.get("blobdir"):
+                question += "    {}\n".format(storage.get("blobdir"))
         question += "Are you sure?"
         if not utils.ask(question, default=False, exact=True):
             logger.info("Not restoring.")
             sys.exit(0)
 
     utils.execute_or_fail(pre_command)
 
     # First run some checks.
     if not only_blobs:
         result = repozorunner.restore_main(
             bin_dir,
-            storages,
+            storage,
             verbose,
             date,
             restore_snapshot,
             alt_restore,
             zip_restore,
             only_check=True,
         )
         if result:
             logger.error("Halting execution: " "restoring filestorages would fail.")
             sys.exit(1)
     if backup_blobs:
         check_blobs(
-            storages,
+            storage,
             use_rsync,
             restore_snapshot=restore_snapshot,
             archive_blob=archive_blob,
             alt_restore=alt_restore,
             rsync_options=rsync_options,
             zip_restore=zip_restore,
             blob_timestamps=blob_timestamps,
             date=date,
         )
     return date
 
 
 def restore_main(
     bin_dir,
-    storages,
+    storage,
     verbose,
     backup_blobs,
     only_blobs,
     use_rsync,
     restore_snapshot=False,
     pre_command="",
     post_command="",
     archive_blob=False,
     alt_restore=False,
     rsync_options="",
-    quick=True,
     zip_restore=False,
     blob_timestamps=False,
     incremental_blobs=False,
     **kwargs,
 ):
 
     """Main method, gets called by generated bin/restore."""
     # First run several checks, and get the date that should be restored.
     date = restore_check(
         bin_dir,
-        storages,
+        storage,
         verbose,
         backup_blobs,
         only_blobs,
         use_rsync,
         restore_snapshot=restore_snapshot,
         pre_command=pre_command,
         post_command=post_command,
         archive_blob=archive_blob,
         alt_restore=alt_restore,
         rsync_options=rsync_options,
-        quick=quick,
         zip_restore=zip_restore,
         blob_timestamps=blob_timestamps,
         incremental_blobs=incremental_blobs,
         **kwargs,
     )
     # Checks have passed, now do the real restore.
     if not only_blobs:
         result = repozorunner.restore_main(
-            bin_dir, storages, verbose, date, restore_snapshot, alt_restore, zip_restore
+            bin_dir, storage, verbose, date, restore_snapshot, alt_restore, zip_restore
         )
         if result:
             if backup_blobs:
                 logger.error("Halting execution due to error; not restoring " "blobs.")
             else:
                 logger.error("Halting execution due to error.")
             sys.exit(1)
 
     if not backup_blobs:
         utils.execute_or_fail(post_command)
         return
-    for storage in storages:
-        blobdir = storage["blobdir"]
-        if not blobdir:
-            continue
-        blob_backup_location = storage["blob_backup_location"]
-        logger.info("Restoring blobs from %s to %s", blob_backup_location, blobdir)
-        result = copyblobs.restore_blobs(
-            blob_backup_location,
-            blobdir,
-            use_rsync=use_rsync,
-            date=date,
-            archive_blob=archive_blob,
-            rsync_options=rsync_options,
-            timestamps=blob_timestamps,
-        )
-        if result:
-            logger.error("Halting execution due to error.")
-            sys.exit(1)
+    blobdir = storage["blobdir"]
+    if not blobdir:
+        return
+    blob_backup_location = storage["blob_backup_location"]
+    logger.info("Restoring blobs from %s to %s", blob_backup_location, blobdir)
+    result = copyblobs.restore_blobs(
+        blob_backup_location,
+        blobdir,
+        use_rsync=use_rsync,
+        date=date,
+        archive_blob=archive_blob,
+        rsync_options=rsync_options,
+        timestamps=blob_timestamps,
+    )
+    if result:
+        logger.error("Halting execution due to error.")
+        sys.exit(1)
     utils.execute_or_fail(post_command)
 
 
 def snapshot_restore_main(*args, **kwargs):
     """Main method, gets called by generated bin/snapshotrestore.
 
     Difference with restore_main is that we use the
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/repozorunner.py` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/repozorunner.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,62 +31,51 @@
         # whole line.
         command = f'"{command}"'
     return command
 
 
 def backup_main(
     bin_dir,
-    storages,
+    storage,
     keep,
     full,
     verbose,
-    gzip,
-    quick,
     backup_method=config.STANDARD_BACKUP,
 ):
     """Main method, gets called by generated bin/backup."""
     repozo = os.path.join(bin_dir, "repozo")
-    if full:
-        quick = False
-
-    for storage in storages:
-        fs = storage["datafs"]
-        if backup_method == config.STANDARD_BACKUP:
-            location = storage["backup_location"]
-            logger.info(
-                "Please wait while backing up database file: %s to %s", fs, location
-            )
-        elif backup_method == config.SNAPSHOT_BACKUP:
-            location = storage["snapshot_location"]
-            logger.info(
-                "Please wait while making snapshot backup: %s to %s", fs, location
-            )
-        elif backup_method == config.ZIP_BACKUP:
-            location = storage["zip_location"]
-            logger.info(
-                "Please wait while backing up database file: %s to %s", fs, location
-            )
-        result = os.system(
-            quote_command(
-                [repozo]
-                + backup_arguments(
-                    fs, location, full, verbose, gzip, quick, as_list=True
-                )
-            )
+    fs = storage["datafs"]
+    if backup_method == config.STANDARD_BACKUP:
+        location = storage["backup_location"]
+        logger.info(
+            "Please wait while backing up database file: %s to %s", fs, location
+        )
+    elif backup_method == config.SNAPSHOT_BACKUP:
+        location = storage["snapshot_location"]
+        logger.info("Please wait while making snapshot backup: %s to %s", fs, location)
+    elif backup_method == config.ZIP_BACKUP:
+        location = storage["zip_location"]
+        logger.info(
+            "Please wait while backing up database file: %s to %s", fs, location
+        )
+    result = os.system(
+        quote_command(
+            [repozo] + backup_arguments(fs, location, full, verbose, as_list=True)
         )
-        logger.debug("Repozo command executed.")
-        if result:
-            logger.error("Repozo command failed. See message above.")
-            return result
-        cleanup(location, keep)
+    )
+    logger.debug("Repozo command executed.")
+    if result:
+        logger.error("Repozo command failed. See message above.")
+        return result
+    cleanup(location, keep)
 
 
 def restore_main(
     bin_dir,
-    storages,
+    storage,
     verbose,
     date=None,
     restore_snapshot=False,
     alt_restore=False,
     zip_restore=False,
     only_check=False,
 ):
@@ -105,92 +94,91 @@
         logger.error(
             "Must use at most one option of restore_snapshot, "
             "alt_restore and zip_restore."
         )
         sys.exit(1)
     repozo = os.path.join(bin_dir, "repozo")
     logger.debug("If things break: did you stop zope?")
-    for storage in storages:
-        if restore_snapshot:
-            backup_location = storage["snapshot_location"]
-        elif alt_restore:
-            backup_location = storage["alt_location"]
-        elif zip_restore:
-            backup_location = storage["zip_location"]
-        else:
-            backup_location = storage["backup_location"]
-        fs = storage["datafs"].rstrip(os.sep)
-        fs_dir = os.path.dirname(fs)
-        if not os.path.exists(fs_dir):
-            os.makedirs(fs_dir)
-            logger.info("Created directory %s", fs_dir)
-        arguments = restore_arguments(fs, backup_location, date, verbose, as_list=True)
-        if only_check:
-            continue
-        logger.info(
-            "Please wait while restoring database file: %s to %s", backup_location, fs
-        )
-        result = os.system(quote_command([repozo] + arguments))
-        if result:
-            logger.error("Repozo command failed. See message above.")
-            return result
+    if restore_snapshot:
+        backup_location = storage["snapshot_location"]
+    elif alt_restore:
+        backup_location = storage["alt_location"]
+    elif zip_restore:
+        backup_location = storage["zip_location"]
+    else:
+        backup_location = storage["backup_location"]
+    fs = storage["datafs"].rstrip(os.sep)
+    fs_dir = os.path.dirname(fs)
+    if not os.path.exists(fs_dir):
+        os.makedirs(fs_dir)
+        logger.info("Created directory %s", fs_dir)
+    arguments = restore_arguments(fs, backup_location, date, verbose, as_list=True)
+    if only_check:
+        return
+    logger.info(
+        "Please wait while restoring database file: %s to %s", backup_location, fs
+    )
+    result = os.system(quote_command([repozo] + arguments))
+    if result:
+        logger.error("Repozo command failed. See message above.")
+        return result
 
 
 def backup_arguments(
     datafs=None,
     backup_location=None,
     full=False,
     verbose=False,
-    gzip=False,
-    quick=False,
     as_list=False,
 ):
     """
     >>> backup_arguments()
     Traceback (most recent call last):
     ...
     RuntimeError: Missing locations.
     >>> backup_arguments(datafs='in/Data.fs', backup_location='out')
-    '--backup -f in/Data.fs -r out'
+    '--backup -f in/Data.fs -r out --quick --gzip'
     >>> backup_arguments(datafs='in/Data.fs', backup_location='out',
-    ...                  full=True)
-    '--backup -f in/Data.fs -r out -F'
+    ...                  verbose=True)
+    '--backup -f in/Data.fs -r out --quick --verbose --gzip'
     >>> backup_arguments(datafs='in/Data.fs', backup_location='out',
-    ...                  quick=True)
-    '--backup -f in/Data.fs -r out --quick'
+    ...                  full=True)
+    '--backup -f in/Data.fs -r out -F --gzip'
 
     """
     if datafs is None or backup_location is None:
         raise RuntimeError("Missing locations.")
     arguments = []
     arguments.append("--backup")
     arguments.append("-f")
     arguments.append(datafs)
     arguments.append("-r")
     arguments.append(backup_location)
-    if quick:
-        # From the repozo help text:
-        # Verify via md5 checksum only the last incremental written.
-        # This significantly reduces the disk i/o at the (theoretical)
-        # cost of inconsistency.  This is a probabilistic way of
-        # determining whether a full backup is necessary.
-        arguments.append("--quick")
     if full:
         # By default, there's an incremental backup, if possible.
         arguments.append("-F")
     else:
         logger.debug(
             "You are not making a full backup. Note that if there "
             "are no changes since the last backup, there will not "
             "be a new incremental backup file."
         )
+        # 'quick' was optional before collective.recipe.backup 5.
+        # Now we always set it for non-full backups.
+        # From the repozo help text:
+        # Verify via md5 checksum only the last incremental written.
+        # This significantly reduces the disk i/o at the (theoretical)
+        # cost of inconsistency.  This is a probabilistic way of
+        # determining whether a full backup is necessary.
+        arguments.append("--quick")
     if verbose:
         arguments.append("--verbose")
-    if gzip:
-        arguments.append("--gzip")
+    # Before collective.recipe.backup 5, this was an option.
+    # Now it is always true.
+    arguments.append("--gzip")
 
     logger.debug("Repozo arguments used: %s", " ".join(arguments))
     if as_list:
         return arguments
     return " ".join(arguments)
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/altrestore.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/altrestore.rst`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,26 @@
     >>> mkdir('alt')
     >>> mkdir('alt', 'data')
     >>> mkdir('alt', 'blobs')
 
 You can restore from an alternative source.  Use case: first make a
 backup of your production site, then go to the testing or staging
 server and restore the production data there.  This is supported with
-the ``alternative_restore_sources`` option::
+the ``alternative_restore_source`` option::
 
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... backup_blobs = false
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     Data ${buildout:directory}/alt/data
     ... """)
     >>> print(system(buildout))
     Installing backup.
     Generated script '/sample-buildout/bin/backup'.
     Generated script '/sample-buildout/bin/snapshotbackup'.
     Generated script '/sample-buildout/bin/restore'.
@@ -56,58 +56,58 @@
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... blob_storage = ${buildout:directory}/var/blobstorage
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     Data ${buildout:directory}/alt/data
     ... """)
     >>> print(system(buildout))
     Uninstalling backup.
     Installing backup.
     While:
       Installing backup.
-    Error: alternative_restore_sources key 'Data' is missing a blobdir.
+    Error: alternative_restore_source key 'Data' is missing a blobdir.
     <BLANKLINE>
 
 Add blobstorage to the alternative, but not the original::
 
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... backup_blobs = false
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     Data ${buildout:directory}/alt/data ${buildout:directory}/alt/blobs
     ... """)
     >>> print(system(buildout))
     Installing backup.
     While:
       Installing backup.
-    Error: alternative_restore_sources key 'Data' specifies blobdir '/sample-buildout/alt/blobs' but the original storage has no blobstorage.
+    Error: alternative_restore_source key 'Data' specifies blobdir '/sample-buildout/alt/blobs' but the original storage has no blobstorage.
     <BLANKLINE>
 
 Add blobstorage to original and alternative::
 
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... blob_storage = ${buildout:directory}/var/blobstorage
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     Data ${buildout:directory}/alt/data ${buildout:directory}/alt/blobs
     ... """)
     >>> print(system(buildout))
     Installing backup.
     Generated script '/sample-buildout/bin/backup'.
     Generated script '/sample-buildout/bin/snapshotbackup'.
     Generated script '/sample-buildout/bin/restore'.
@@ -189,101 +189,27 @@
     INFO: Please wait while restoring database file: /sample-buildout/alt/data to /sample-buildout/var/filestorage/Data.fs
     INFO: Restoring blobs from /sample-buildout/alt/blobs to /sample-buildout/var/blobstorage
     INFO: rsync -a  --delete /sample-buildout/alt/blobs/blobstorage.0/blobstorage /sample-buildout/var
     <BLANKLINE>
     >>> check_repozo_output()
     --recover -o /sample-buildout/var/filestorage/Data.fs -r /sample-buildout/alt/data -D 2100-12-31-23-59
 
-Test in combination with additional filestorage::
-
-    >>> write('buildout.cfg',
-    ... """
-    ... [buildout]
-    ... newest = false
-    ... parts = backup
-    ...
-    ... [backup]
-    ... recipe = collective.recipe.backup
-    ... blob_storage = ${buildout:directory}/var/blobstorage
-    ... additional_filestorages =
-    ...     foo ${buildout:directory}/var/filestorage/foo/foo.fs ${buildout:directory}/var/blobstorage-foo
-    ...     bar ${buildout:directory}/var/filestorage/bar/bar.fs
-    ... alternative_restore_sources =
-    ...     Data ${buildout:directory}/alt/data ${buildout:directory}/alt/blobs
-    ...     foo ${buildout:directory}/alt/foo ${buildout:directory}/alt/fooblobs
-    ...     bar ${buildout:directory}/alt/bar
-    ... """)
-    >>> remove('var')
-    >>> mkdir('var')
-    >>> mkdir('alt', 'foo')
-    >>> mkdir('alt', 'bar')
-    >>> mkdir('alt', 'fooblobs')
-    >>> mkdir('alt', 'fooblobs', 'blobstorage-foo.0')
-    >>> mkdir('alt', 'fooblobs', 'blobstorage-foo.0', 'blobstorage-foo')
-    >>> write('alt', 'fooblobs', 'blobstorage-foo.0', 'blobstorage-foo', 'fooblobfile.txt', 'Hello fooblob.')
-    >>> print(system(buildout))
-    Uninstalling backup.
-    Installing backup.
-    Generated script '/sample-buildout/bin/backup'.
-    Generated script '/sample-buildout/bin/snapshotbackup'.
-    Generated script '/sample-buildout/bin/restore'.
-    Generated script '/sample-buildout/bin/snapshotrestore'.
-    Generated script '/sample-buildout/bin/altrestore'.
-    <BLANKLINE>
-    >>> print(system('bin/altrestore', input='yes\n'))
-    <BLANKLINE>
-    This will replace the filestorage:
-        /sample-buildout/var/filestorage/foo/foo.fs
-        /sample-buildout/var/filestorage/bar/bar.fs
-        /sample-buildout/var/filestorage/Data.fs
-    This will replace the blobstorage:
-        /sample-buildout/var/blobstorage-foo
-        /sample-buildout/var/blobstorage
-    Are you sure? (yes/No)?
-    INFO: Created directory /sample-buildout/var/filestorage/foo
-    INFO: Created directory /sample-buildout/var/filestorage/bar
-    INFO: No blob dir defined for bar storage
-    INFO: Please wait while restoring database file: /sample-buildout/alt/foo to /sample-buildout/var/filestorage/foo/foo.fs
-    INFO: Please wait while restoring database file: /sample-buildout/alt/bar to /sample-buildout/var/filestorage/bar/bar.fs
-    INFO: Please wait while restoring database file: /sample-buildout/alt/data to /sample-buildout/var/filestorage/Data.fs
-    INFO: Restoring blobs from /sample-buildout/alt/fooblobs to /sample-buildout/var/blobstorage-foo
-    INFO: rsync -a  --delete /sample-buildout/alt/fooblobs/blobstorage-foo.0/blobstorage-foo /sample-buildout/var
-    INFO: Restoring blobs from /sample-buildout/alt/blobs to /sample-buildout/var/blobstorage
-    INFO: rsync -a  --delete /sample-buildout/alt/blobs/blobstorage.0/blobstorage /sample-buildout/var
-    <BLANKLINE>
-    >>> check_repozo_output()
-    --recover -o /sample-buildout/var/filestorage/foo/foo.fs -r /sample-buildout/alt/foo
-    --recover -o /sample-buildout/var/filestorage/bar/bar.fs -r /sample-buildout/alt/bar
-    --recover -o /sample-buildout/var/filestorage/Data.fs -r /sample-buildout/alt/data
-    >>> ls('var')
-    d  blobstorage
-    d  blobstorage-foo
-    d  filestorage
-    >>> ls('var', 'blobstorage')
-    -   blobfile.txt
-    >>> cat('var', 'blobstorage', 'blobfile.txt')
-    Hello blob.
-    >>> ls('var', 'blobstorage-foo')
-    -   fooblobfile.txt
-    >>> cat('var', 'blobstorage-foo', 'fooblobfile.txt')
-    Hello fooblob.
-
 When archive_blob is true, we use it::
 
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... blob_storage = ${buildout:directory}/var/blobstorage
     ... archive_blob = true
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     Data ${buildout:directory}/alt/data ${buildout:directory}/alt/blobs
     ... """)
     >>> print(system(buildout))
     Uninstalling backup.
     Installing backup.
     Generated script '/sample-buildout/bin/backup'.
     Generated script '/sample-buildout/bin/snapshotbackup'.
@@ -332,21 +258,21 @@
     ... parts =
     ...     secondbackup
     ...     firstbackup
     ...
     ... [firstbackup]
     ... recipe = collective.recipe.backup
     ... backup_blobs = false
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     Data ${buildout:directory}/alt/data
     ...
     ... [secondbackup]
     ... recipe = collective.recipe.backup
     ... backup_blobs = false
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     Data ${buildout:directory}/alt/data
     ... """)
     >>> print(system(buildout))
     Uninstalling backup.
     Installing secondbackup.
     Generated script '/sample-buildout/bin/secondbackup'.
     Generated script '/sample-buildout/bin/secondbackup-snapshot'.
@@ -372,15 +298,15 @@
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... backup_blobs = false
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     1 ${buildout:directory}/alt/data
     ... """)
     >>> print(system(buildout))
     Uninstalling firstbackup.
     Uninstalling secondbackup.
     Installing backup.
     Generated script '/sample-buildout/bin/backup'.
@@ -394,130 +320,69 @@
     This will replace the filestorage:
         /sample-buildout/var/filestorage/Data.fs
     Are you sure? (yes/No)?
     INFO: Please wait while restoring database file: /sample-buildout/alt/data to /sample-buildout/var/filestorage/Data.fs
     >>> check_repozo_output()
     --recover -o /sample-buildout/var/filestorage/Data.fs -r /sample-buildout/alt/data
 
-Specifying both ``1`` and ``Data`` is bad::
+Specifying both ``1`` and ``Data`` is bad.
+But since version 5, only one line is supported anyway::
 
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... backup_blobs = false
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     1 ${buildout:directory}/alt/one
     ...     Data ${buildout:directory}/alt/data
     ... """)
     >>> print(system(buildout))
     Uninstalling backup.
     Installing backup.
     While:
       Installing backup.
-    Error: alternative_restore_sources key 'Data' is used. Are you using both '1' and 'Data'? They are alternative keys for the same Data.fs.
-
-Switching them around also fails::
-
-    >>> write('buildout.cfg',
-    ... """
-    ... [buildout]
-    ... newest = false
-    ... parts = backup
-    ...
-    ... [backup]
-    ... recipe = collective.recipe.backup
-    ... backup_blobs = false
-    ... alternative_restore_sources =
-    ...     Data ${buildout:directory}/alt/data
-    ...     1 ${buildout:directory}/alt/one
-    ... """)
-    >>> print(system(buildout))
-    Installing backup.
-    While:
-      Installing backup.
-    Error: alternative_restore_sources key '1' is used. Are you using both '1' and 'Data'? They are alternative keys for the same Data.fs.
-
-Missing keys is bad::
-
-    >>> write('buildout.cfg',
-    ... """
-    ... [buildout]
-    ... newest = false
-    ... parts = backup
-    ...
-    ... [backup]
-    ... recipe = collective.recipe.backup
-    ... backup_blobs = false
-    ... additional_filestorages =
-    ...     foo ${buildout:directory}/var/filestorage/foo/foo.fs
-    ... alternative_restore_sources =
-    ...     Data ${buildout:directory}/alt/data
-    ... """)
-    >>> print(system(buildout))
-    Installing backup.
-    While:
-      Installing backup.
-    Error: alternative_restore_sources is missing key 'foo'.
-    >>> write('buildout.cfg',
-    ... """
-    ... [buildout]
-    ... newest = false
-    ... parts = backup
-    ...
-    ... [backup]
-    ... recipe = collective.recipe.backup
-    ... backup_blobs = false
-    ... additional_filestorages =
-    ...     foo ${buildout:directory}/var/filestorage/foo/foo.fs
-    ... alternative_restore_sources =
-    ...     foo ${buildout:directory}/alt/foo
-    ... """)
-    >>> print(system(buildout))
-    Installing backup.
-    While:
-      Installing backup.
-    Error: alternative_restore_sources is missing key 'Data'.
+    Error: Only one alternative_restore_source line is supported.
 
-Extra keys are also bad::
+Unknown keys are bad::
 
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... backup_blobs = false
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     foo ${buildout:directory}/alt/foo
     ... """)
     >>> print(system(buildout))
     Installing backup.
     While:
       Installing backup.
-    Error: alternative_restore_sources key 'foo' unknown in storages.
+    Error: alternative_restore_source key 'foo' unknown. Expected 1 or Data.
 
 A filestorage source path is required::
 
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
     ... [backup]
     ... recipe = collective.recipe.backup
     ... backup_blobs = false
-    ... alternative_restore_sources =
+    ... alternative_restore_source =
     ...     Data
     ... """)
     >>> print(system(buildout))
     Installing backup.
     While:
       Installing backup.
-    Error: alternative_restore_sources line 'Data' has a wrong format. Should be: 'storage-name filestorage-backup-path', optionally followed by a blobstorage-backup-path.
+    Error: alternative_restore_source line 'Data' has a wrong format. Should be: 'storage-name filestorage-backup-path', optionally followed by a blobstorage-backup-path.
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/backup_blobs_archive.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/backup_blobs_archive.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/backup_blobs_dir.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/backup_blobs_dir.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/backup_blobs_dir_hard_links.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/backup_blobs_dir_hard_links.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/base.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/base.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/cleanup_archives.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/cleanup_archives.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/cleanup_dir.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/cleanup_dir.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/incremental_blobs.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/incremental_blobs.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/location.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/location.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/no_rsync.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/no_rsync.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/options.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/options.rst`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     ... backup_blobs = false
     ... location = ${buildout:directory}/myproject
     ... keep = 2
     ... datafs = subfolder/myproject.fs
     ... full = true
     ... debug = true
     ... snapshotlocation = snap/my
-    ... gzip = false
     ... enable_snapshotrestore = true
     ... pre_command = echo 'Can I have a backup?' > pre
     ... post_command =
     ...     echo 'Thanks a lot for the backup.' > post
     ...     echo 'We are done.' >> post
     ... """)
     >>> print(system(buildout))
@@ -47,15 +46,15 @@
     >>> output = system('bin/backup')
     >>> print(output)
     <BLANKLINE>
     20...-...-... INFO: Created /sample-buildout/myproject
     20...-...-... INFO: Please wait while backing up database file: /sample-buildout/subfolder/myproject.fs to /sample-buildout/myproject
     20...-...-...
     >>> check_repozo_output()
-    --backup -f /sample-buildout/subfolder/myproject.fs -r /sample-buildout/myproject -F --verbose
+    --backup -f /sample-buildout/subfolder/myproject.fs -r /sample-buildout/myproject -F --verbose --gzip
 
 We do not check that the pre and post output appear in the correct order.
 In the tests the output order can differ between Python 2 and 3.
 
     >>> cat('pre')
     Can I have a backup?
     >>> cat('post')
@@ -73,15 +72,15 @@
     >>> output = system('bin/snapshotbackup')
     >>> print(output)
     20...-...-... INFO: Created /sample-buildout/var/snap/my
     20...-...-... INFO: Please wait while making snapshot backup: /sample-buildout/subfolder/myproject.fs to /sample-buildout/var/snap/my
     20...-...-...
     >>> if 'ERROR' in output: print(output)
     >>> check_repozo_output()
-    --backup -f /sample-buildout/subfolder/myproject.fs -r /sample-buildout/var/snap/my -F --verbose
+    --backup -f /sample-buildout/subfolder/myproject.fs -r /sample-buildout/var/snap/my -F --verbose --gzip
     >>> cat('pre')
     Can I have a backup?
     >>> cat('post')
     Thanks a lot for the backup.
     We are done.
     >>> remove('pre')
     >>> remove('post')
@@ -108,25 +107,25 @@
     Can I have a backup?
     >>> cat('post')
     Thanks a lot for the backup.
     We are done.
     >>> remove('pre')
     >>> remove('post')
     >>> check_repozo_output()
-    --backup -f /sample-buildout/subfolder/myproject.fs -r /sample-buildout/myproject -F --verbose
+    --backup -f /sample-buildout/subfolder/myproject.fs -r /sample-buildout/myproject -F --verbose --gzip
     >>> print(system('bin/backup --quiet'))
     >>> cat('pre')
     Can I have a backup?
     >>> cat('post')
     Thanks a lot for the backup.
     We are done.
     >>> remove('pre')
     >>> remove('post')
     >>> check_repozo_output()
-    --backup -f /sample-buildout/subfolder/myproject.fs -r /sample-buildout/myproject -F --verbose
+    --backup -f /sample-buildout/subfolder/myproject.fs -r /sample-buildout/myproject -F --verbose --gzip
 
 In our case the ``--backup ...`` lines above are just the mock repozo script
 that still prints something. So it proves that the command is executed, but it
 won't end up in the output.
 
 Speaking of cron jobs?  Take a look at `zc.recipe.usercrontab
 <http://pypi.python.org/pypi/z3c.recipe.usercrontab>`_ if you want to handle
@@ -167,44 +166,7 @@
     <BLANKLINE>
     >>> ls('bin')
     -  backup
     -  buildout
     -  repozo
     -  restore
     -  snapshotbackup
-
-
-Not quick
----------
-
-The repozo script has the quick option set the false by default.
-Usually it makes sense to set it to true, as this can be a *lot*
-quicker.  So version 2.19 introduced the quick option for the backup
-script and has set the default to true.  You can set it to false if
-wanted.
-
-    >>> write('buildout.cfg',
-    ... """
-    ... [buildout]
-    ... newest = false
-    ... parts = backup
-    ...
-    ... [backup]
-    ... recipe = collective.recipe.backup
-    ... backup_blobs = false
-    ... quick = false
-    ... """)
-
-    >>> print(system(buildout))
-    Uninstalling backup.
-    Installing backup.
-    Generated script '/sample-buildout/bin/backup'.
-    Generated script '/sample-buildout/bin/snapshotbackup'.
-    Generated script '/sample-buildout/bin/restore'.
-    Generated script '/sample-buildout/bin/snapshotrestore'.
-    <BLANKLINE>
-    >>> print(system('bin/backup'))
-    INFO: Created /sample-buildout/var/backups
-    INFO: Please wait while backing up database file: /sample-buildout/var/filestorage/Data.fs to /sample-buildout/var/backups
-    <BLANKLINE>
-    >>> check_repozo_output()
-    --backup -f /sample-buildout/var/filestorage/Data.fs -r /sample-buildout/var/backups --gzip
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/prefix.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/prefix.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/test_docs.py` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/test_docs.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from collective.recipe.backup import utils
 from zope.testing import renormalizing
 
 # Importing modules so that we can install their eggs in the test buildout.
 import collective.recipe.backup
 import doctest
 import re
-import sys
 import tempfile
 import unittest
 import zc.buildout.testing
 import zc.buildout.tests
 import zc.recipe.egg
 
 
@@ -98,32 +97,21 @@
         "backup_blobs_dir.rst",
         "backup_blobs_dir_hard_links.rst",
         "base.rst",
         "blobs.rst",
         "blob_timestamps.rst",
         "cleanup_archives.rst",
         "cleanup_dir.rst",
-        "gzip.rst",
         "incremental_blobs.rst",
         "location.rst",
-        "multiple.rst",
         "no_rsync.rst",
         "options.rst",
         "prefix.rst",
         "zipbackup.rst",
     ]
-    test_file = "zope2instance.rst"
-    if sys.version_info[0] > 2:
-        print(f"INFO: ignoring {test_file} tests on Python 3.")
-        print(
-            "It would pull in Zope and ZODB, which is too much for what we try to test."
-        )
-        print("See https://github.com/collective/collective.recipe.backup/issues/31")
-    else:
-        docfiles.append(test_file)
     for docfile in docfiles:
         suite.addTest(
             doctest.DocFileSuite(
                 docfile,
                 setUp=setUp,
                 tearDown=zc.buildout.testing.buildoutTearDown,
                 optionflags=optionflags,
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/test_unit.py` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/tests/zipbackup.rst` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/tests/zipbackup.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*-doctest-*-
 
 zipbackup and ziprestore
 ========================
 
 Since version 2.20, we can create a zipbackup and ziprestore
 script.  These use a different backup location and have a few options
-hardcoded: gzip and archive_blob are True, keep is 1, regardless of what
+hardcoded: archive_blob is True, keep is 1, regardless of what
 the options in the buildout recipe section are.  You can always create
 a separate buildout section where you explicitly change this using
 options for the standard bin/backup script.
 
 By default the scripts are not created.  You can ensable the them by
 setting the enable_zipbackup option to true.
 
 Create directories and content::
 
     >>> mkdir('var', 'blobstorage')
     >>> write('var', 'blobstorage', 'blob1.txt', 'Sample blob 1.')
 
-Create some archived (gzipped) and not-archived separate backup scripts::
+Create some archived and not-archived separate backup scripts::
 
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... newest = false
     ... parts = backup
     ...
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective/recipe/backup/utils.py` & `collective.recipe.backup-5.0.0a3/src/collective/recipe/backup/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,41 +101,40 @@
         print(output)
     if failed:
         logger.error("command %r failed. See message above.", command)
         sys.exit(1)
 
 
 def check_folders(
-    storages, backup_blobs=True, only_blobs=False, backup_method=config.STANDARD_BACKUP
+    storage, backup_blobs=True, only_blobs=False, backup_method=config.STANDARD_BACKUP
 ):
     """Check that folders exist, and create them if not."""
     backup = backup_method == config.STANDARD_BACKUP
     snapshot = backup_method == config.SNAPSHOT_BACKUP
     zipbackup = backup_method == config.ZIP_BACKUP
-    for storage in storages:
-        pathdirs = []
-        if not only_blobs:
-            if backup:
-                pathdirs.append(storage.get("backup_location"))
-            if snapshot:
-                pathdirs.append(storage.get("snapshot_location"))
-            if zipbackup:
-                pathdirs.append(storage.get("zip_location"))
-        if backup_blobs:
-            if backup:
-                pathdirs.append(storage.get("blob_backup_location"))
-            if snapshot:
-                pathdirs.append(storage.get("blob_snapshot_location"))
-            if zipbackup:
-                pathdirs.append(storage.get("blob_zip_location"))
-
-        for pathdir in pathdirs:
-            if pathdir and not os.path.isdir(pathdir):
-                os.makedirs(pathdir)
-                logger.info("Created %s", pathdir)
+    pathdirs = []
+    if not only_blobs:
+        if backup:
+            pathdirs.append(storage.get("backup_location"))
+        if snapshot:
+            pathdirs.append(storage.get("snapshot_location"))
+        if zipbackup:
+            pathdirs.append(storage.get("zip_location"))
+    if backup_blobs:
+        if backup:
+            pathdirs.append(storage.get("blob_backup_location"))
+        if snapshot:
+            pathdirs.append(storage.get("blob_snapshot_location"))
+        if zipbackup:
+            pathdirs.append(storage.get("blob_zip_location"))
+
+    for pathdir in pathdirs:
+        if pathdir and not os.path.isdir(pathdir):
+            os.makedirs(pathdir)
+            logger.info("Created %s", pathdir)
 
 
 def try_create_folder(pathdir):
     """Try to create a folder, but remove it again.
 
     >>> try_create_folder('mytest')
     >>> mkdir('mytest')
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/PKG-INFO` & `collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.recipe.backup
-Version: 5.0.0a2
+Version: 5.0.0a3
 Summary: bin/backup script: sensible defaults around bin/repozo
 Home-page: https://github.com/collective/collective.recipe.backup
 Author: Reinout van Rees, Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL
 Keywords: buildout backup repozo zope
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Requires-Python: >=3.8
 Provides-Extra: tests
 
 Easy Zope backup/restore recipe for buildout
 ********************************************
 
 .. image:: https://github.com/collective/collective.recipe.backup/workflows/tests/badge.svg
     :target: https://github.com/collective/collective.recipe.backup/actions?query=workflow%3Atests
@@ -144,17 +145,14 @@
 ==============
 
 Which data does this recipe backup?
 
 - The Zope Object DataBase (ZODB) filestorage, by default located at
   ``var/filestorage/Data.fs``.
 
-- Possibly additional filestorages, see the
-  ``additional_filestorages`` option.
-
 - The blobstorage (since version 2.0) if your buildout uses it, by
   default located at ``var/blobstorage``.
 
 
 Data that is *not* backed up
 ============================
 
@@ -209,17 +207,14 @@
 do not want to use ``scp`` to recursively copy over all those blob
 files: downloading one tarball is faster.
 
 You can use the ``bin/zipbackup`` script for this.  This script
 overrides a few settings, ignoring whatever is set in the buildout
 config section:
 
-- ``gzip`` is explicitly turned on for the filestorage (this is
-  already the default, but we make sure).
-
 - ``archive_blob`` is turned on.
 
 - ``keep`` is set to 1 to avoid keeping lots of needless backups.
 
 - ``keep_blob_days`` is ignored because it is a full backup.
 
 The script places a full backup in, by default, ``var/zipbackups`` and
@@ -303,33 +298,31 @@
 default. The most common ones to change are ``location`` and
 ``blobbackuplocation``, as those allow you to place your backups in
 some system-wide directory like ``/var/zopebackups/instancename/`` and
 ``/var/zopebackups/instancename-blobs/``.
 
 .. Note: keep this in alphabetical order please.
 
-``additional_filestorages``
-    Advanced option, only needed when you have split for instance a
-    ``catalog.fs`` out of the regular ``Data.fs``.
-    Use it to specify the extra filestorages.
-    (See `Advanced usage: multiple Data.fs files`_).
-
 ``archive_blob``
     Use ``tar`` archiving functionality. ``false`` by default. Set it to ``true``
     and backup/restore will be done with ``tar`` command. Note that ``tar``
     command must be available on machine if this option is set to ``true``.
     This option also works with snapshot backup/restore commands. As this
     counts as a full backup ``keep_blob_days`` is ignored.
     See the ``compress_blob`` option if you want to compress the archive.
 
-``alternative_restore_sources``
+``alternative_restore_source``
     You can restore from an alternative source.  Use case: first make
     a backup of your production site, then go to the testing or
     staging server and restore the production data there.  See
-    `Alternative restore sources`_
+    `Alternative restore source`_
+
+``alternative_restore_sources``
+    Backwards compatibility spelling for ``alternative_restore_source``.
+    This will no longer work in version 7.
 
 ``backup_blobs``
     Backup the blob storage.  Default is ``True`` on Python 2.6 (Plone
     4) and higher, and ``False`` otherwise.  This requires the
     ``blob_storage`` location to be set.  If no ``blob_storage``
     location has been set and we cannot find one by looking in the
     other buildout parts, we quit with an error (since version 2.22).
@@ -414,24 +407,14 @@
     If ``backup_blobs`` is not on, these scripts are always disabled,
     because they are not useful then.
 
 ``full``
     By default, incremental backups are made. If this option is set to ``true``,
     ``bin/backup`` will always make a full backup.
 
-``gzip``
-    Use repozo's zipping functionality. ``true`` by default. Set it to ``false``
-    and repozo will not gzip its files. Note that gzipped databases are called
-    ``*.fsz``, not ``*.fs.gz``. **Changed in 0.8**: the default used to be
-    false, but it so totally makes sense to gzip your backups that we changed
-    the default.
-
-``gzip_blob``
-    Backwards compatibility alias for ``archive_blob`` option.
-
 ``incremental_blobs``
     New in version 4.0.  Default is false.
     When switched on, it will use the ``--listed-incremental`` option of ``tar``.
     Note: this only works with the GNU version of ``tar``.
     On Mac you may need to install this with ``brew install gnu-tar`` and change your ``PATH`` according to the instructions.
     It will create a metadata or `snapshot file <https://www.gnu.org/software/tar/manual/html_node/Incremental-Dumps.html>`_
     so that a second call to the backup script will create a second tarball with only the differences.
@@ -521,15 +504,15 @@
     a backup from a symlinked directory, in which case
     ``rsync_options = --no-l -k`` does the trick.
 
 ``rsync_hard_links_on_first_copy``
     When using ``rsync``, the blob files for the first backup are copied
     and then subsequent backups make use of hard links from this initial
     copy, to save time and disk space.
-    Enable this option to also use hard links for the initial copy to further reduce 
+    Enable this option to also use hard links for the initial copy to further reduce
     disk usage.
     This is safe for ZODB blobs, since they are not modified in place.
     The ``blob_storage`` and the backup folder ``blobbackuplocation``
     have to be in the same partition for hard links to be possible.
 
 ``snapshotlocation``
     Location where snapshot backups of the filestorage are stored. Defaults to
@@ -553,15 +536,14 @@
     recipe = collective.recipe.backup
     location = ${buildout:directory}/myproject
     keep = 2
     datafs = subfolder/myproject.fs
     full = true
     debug = true
     snapshotlocation = snap/my
-    gzip = false
     enable_snapshotrestore = true
     pre_command = echo 'Can I have a backup?'
     post_command =
         echo 'Thanks a lot for the backup.'
         echo 'We are done.'
 
 Paths in directories or files can use relative (``../``) paths, and
@@ -584,79 +566,14 @@
 
     [backupcronjob]
     recipe = z3c.recipe.usercrontab
     times = 0 12 * * *
     command = ${buildout:directory}/bin/backup
 
 
-Advanced usage: multiple Data.fs files
-======================================
-
-Sometimes, a filestorage is split into several files. Most common reason is to
-have a regular ``Data.fs`` and a ``catalog.fs`` which contains the
-``portal_catalog``. This is supported with the ``additional_filestorages``
-option::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        catalog
-        another
-
-This means that, with the standard ``Data.fs``, the ``bin/backup``
-script will now backup three filestorages::
-
-    var/filestorage/Data.fs
-    var/filestorage/catalog.fs
-    var/filestorage/another.fs
-
-The additional backups have to be stored separate from the ``Data.fs``
-backup. That's done by appending the file's name and creating extra backup
-directories named that way::
-
-    var/backups_catalog
-    var/snapshotbackups_catalog
-    var/backups_another
-    var/snapshotbackups_another
-
-The various backups are done one after the other. They cannot be done at the
-same time with ``repozo``. So they are not completely in sync. The "other"
-databases are backed up first as a small difference in the catalog is just
-mildly irritating, but the other way around users can get real errors.
-
-In the ``additional_filestorages`` option you can define different
-filestorages using this syntax::
-
-    additional_filestorages =
-        storagename1 [datafs1_path [blobdir1]]
-        storagename2 [datafs2_path [blobdir2]]
-        ...
-
-So if you want more control over the filestorage source path, you can
-explicitly set it, with or without the blobstorage path.  For
-example::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        foo ${buildout:directory}/var/filestorage/foo/foo.fs ${buildout:directory}/var/blobstorage-foo
-        bar ${buildout:directory}/var/filestorage/bar/bar.fs
-
-If the ``datafs_path`` is missing, then the default value will be used
-(``var/filestorage/storagename1.fs``).  If you do not specify a
-``blobdir``, then this means no blobs will be backed up for that
-storage.  Note that if you specify ``blobdir`` you must specify
-``datafs_path`` as well.
-
-Note that ``collective.recipe.filestorage`` creates additional
-filestorages in a slightly different location, but you can explictly define the
-paths of filestorage and blobstorage for all the ``parts`` defined in the recipe.
-Work is in progress to improve this.
-
-
 Blob storage
 ============
 
 Added in version 2.0.
 
 We can backup the blob storage.  Plone 4 uses a blob storage to store
 files (Binary Large OBjects) on the file system.  In Plone 3 this is
@@ -713,74 +630,60 @@
 http://www.mikerubel.org/computers/rsync_snapshots/
 
 We have not tried this on Windows.  Reports are welcome, but best is
 probably to set the ``use_rsync = false`` option in the backup part.
 Then we simply copy the blobstorage directory.
 
 
-Alternative restore sources
-===========================
+Alternative restore source
+==========================
 
 Added in version 2.17.
+Changed in version 5: only one source is supported.
 
 You can restore from an alternative source.  Use case: first make a
 backup of your production site, then go to the testing or staging
 server and restore the production data there.
 
-In the ``alternative_restore_sources`` option you can define different
+In the ``alternative_restore_source`` option you can define different
 filestorage and blobstorage backup source directories using this
 syntax::
 
-    alternative_restore_sources =
-        storagename1 datafs1_backup [blobdir1_backup]
-        storagename2 datafs2_backup [blobdir2_backup]
-        ...
+    alternative_restore_source =
+        storagename datafs1_backup [blobdir1_backup]
 
-The storagenames *must* be the same as in the additional_filestorages
-option, plus a key ``Data`` (or ``1``) for the standard ``Data.fs``
+The storagename must be ``Data`` (or ``1``) for the standard ``Data.fs``
 and optionally its blobstorage.
 
 The result is a ``bin/altrestore`` script.
 
 This will work for a standard buildout with a single filestorage and
 blobstorage::
 
     [backup]
     recipe = collective.recipe.backup
-    alternative_restore_sources =
+    alternative_restore_source =
         Data /path/to/production/var/backups /path/to/production/var/blobstoragebackups
 
 The above configuration uses ``repozo`` to restore the Data.fs from
 the ``/path/to/production/var/backups`` repository to the standard
 ``var/filestorage/Data.fs`` location.  It copies the most recent
 blobstorage backup from
 ``/path/to/production/var/blobstoragebackups/`` to the standard
 ``var/blobstorage`` location.
 
 Calling the script with a specific date is supported just like the
 normal restore script::
 
     bin/altrestore 2000-12-31-23-59
 
-If you have additional filestorages, it would be like this::
-
-    [backup]
-    recipe = collective.recipe.backup
-    additional_filestorages =
-        foo ${buildout:directory}/var/filestorage/foo/foo.fs ${buildout:directory}/var/blobstorage-foo
-        bar ${buildout:directory}/var/filestorage/bar/bar.fs
-    alternative_restore_sources =
-        Data /path/to/production/var/backups /path/to/production/var/blobstoragebackups
-        foo /path/to/production/var/backups_foo /path/to/production/var/blobstoragebackups_foo
-        bar /path/to/production/var/backups_bar
-
-The recipe will fail if the alternative sources do not match the
-standard filestorage, blobstorage and additional storages.  For
-example, you get an error when the ``alternative_restore_sources`` is
-missing the ``Data`` key, when it has extra or missing keys, when a
+The recipe will fail if the alternative source does not match the
+standard filestorage and blobstorage.  For
+example, you get an error when the ``alternative_restore_source`` is
+missing the ``Data`` key, when it has an extra key, when a
 key has no paths, when a key has an extra or missing blobstorage.
 
 During install of the recipe, so during the ``bin/buildout`` run, it
 does not check if the sources exist: you might have the production
 backups on a different server and need to setup a remote shared
 directory, or you copy the data over manually.
 
@@ -838,14 +741,46 @@
          fix problems like typo corrections or such.
 
          To add a new change log entry, please see the notes from the ``pip`` project at
              https://pip.pypa.io/en/latest/development/#adding-a-news-entry
 
 .. towncrier release notes start
 
+5.0.0a3 (2023-03-15)
+====================
+
+Breaking changes:
+
+
+- Removed ``additional_filestorages`` option.
+  Removed support in ``alternative_restore_sources`` for multiple storages: only the standard single filestorage plus blobstorage is supported.
+  Renamed ``alternative_restore_sources`` to ``alternative_restore_source``, keeping the old alias for now.
+  [maurits] (`Issue #64 <https://github.com/collective/collective.recipe.backup/issues/64>`_)
+- Removed ``gzip`` option.
+  From now on, we always call repozo with the gzip option, you can no longer turn this off.
+  [maurits] (`Issue #67 <https://github.com/collective/collective.recipe.backup/issues/67>`_)
+- Removed option ``gzip_blob``.
+  This was a backwards compatibility alias for ``archive_blob``.
+  You should use that now it you want to create a tar archive.
+  Additionally use the ``compress_blob`` option if you are really sure you want to compress the archive.
+  [maurits] (`Issue #68 <https://github.com/collective/collective.recipe.backup/issues/68>`_)
+- Removed option ``quick``.
+  From now on, we always call repozo with the quick option for normal backups, you can no longer turn this off.
+  For full backups (snapshotbackups and zipbackups), the quick option is not used.
+  [maurits] (`Issue #69 <https://github.com/collective/collective.recipe.backup/issues/69>`_)
+
+
+Bug fixes:
+
+
+- Deprecate setting blob_timestamps to false.
+  See `issue 65 <https://github.com/collective/collective.recipe.backup/issues/65>`_.
+  [maurits] (`Issue #65 <https://github.com/collective/collective.recipe.backup/issues/65>`_)
+
+
 5.0.0a2 (2023-02-01)
 ====================
 
 Bug fixes:
 
 - Add missing changelog entries for release 5.0.0a1.  [maurits]
```

### Comparing `collective.recipe.backup-5.0.0a2/src/collective.recipe.backup.egg-info/SOURCES.txt` & `collective.recipe.backup-5.0.0a3/src/collective.recipe.backup.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -28,18 +28,15 @@
 src/collective/recipe/backup/tests/backup_blobs_dir.rst
 src/collective/recipe/backup/tests/backup_blobs_dir_hard_links.rst
 src/collective/recipe/backup/tests/base.rst
 src/collective/recipe/backup/tests/blob_timestamps.rst
 src/collective/recipe/backup/tests/blobs.rst
 src/collective/recipe/backup/tests/cleanup_archives.rst
 src/collective/recipe/backup/tests/cleanup_dir.rst
-src/collective/recipe/backup/tests/gzip.rst
 src/collective/recipe/backup/tests/incremental_blobs.rst
 src/collective/recipe/backup/tests/location.rst
-src/collective/recipe/backup/tests/multiple.rst
 src/collective/recipe/backup/tests/no_rsync.rst
 src/collective/recipe/backup/tests/options.rst
 src/collective/recipe/backup/tests/prefix.rst
 src/collective/recipe/backup/tests/test_docs.py
 src/collective/recipe/backup/tests/test_unit.py
-src/collective/recipe/backup/tests/zipbackup.rst
-src/collective/recipe/backup/tests/zope2instance.rst
+src/collective/recipe/backup/tests/zipbackup.rst
```

