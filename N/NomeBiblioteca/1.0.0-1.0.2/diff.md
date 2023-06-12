# Comparing `tmp/NomeBiblioteca-1.0.0.tar.gz` & `tmp/NomeBiblioteca-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NomeBiblioteca-1.0.0.tar", last modified: Mon Jun 12 21:12:11 2023, max compression
+gzip compressed data, was "NomeBiblioteca-1.0.2.tar", last modified: Mon Jun 12 21:40:27 2023, max compression
```

## Comparing `NomeBiblioteca-1.0.0.tar` & `NomeBiblioteca-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 21:12:11.944008 NomeBiblioteca-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-12 21:12:11.936021 NomeBiblioteca-1.0.0/NomeBiblioteca.egg-info/
--rw-rw-rw-   0        0        0      160 2023-06-12 21:12:11.000000 NomeBiblioteca-1.0.0/NomeBiblioteca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-06-12 21:12:11.000000 NomeBiblioteca-1.0.0/NomeBiblioteca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 21:12:11.000000 NomeBiblioteca-1.0.0/NomeBiblioteca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 21:12:11.000000 NomeBiblioteca-1.0.0/NomeBiblioteca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      160 2023-06-12 21:12:11.944008 NomeBiblioteca-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-12 21:12:11.944008 NomeBiblioteca-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      205 2023-06-12 21:12:07.000000 NomeBiblioteca-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 21:40:27.071361 NomeBiblioteca-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-12 21:40:27.063362 NomeBiblioteca-1.0.2/NomeBiblioteca.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-06-12 21:40:26.000000 NomeBiblioteca-1.0.2/NomeBiblioteca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-06-12 21:40:26.000000 NomeBiblioteca-1.0.2/NomeBiblioteca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 21:40:26.000000 NomeBiblioteca-1.0.2/NomeBiblioteca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-12 21:40:26.000000 NomeBiblioteca-1.0.2/NomeBiblioteca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 21:40:26.000000 NomeBiblioteca-1.0.2/NomeBiblioteca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      160 2023-06-12 21:40:27.063362 NomeBiblioteca-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-12 21:40:27.071361 NomeBiblioteca-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      274 2023-06-12 21:40:17.000000 NomeBiblioteca-1.0.2/setup.py
```

