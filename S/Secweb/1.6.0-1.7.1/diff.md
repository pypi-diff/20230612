# Comparing `tmp/Secweb-1.6.0.tar.gz` & `tmp/Secweb-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Secweb-1.6.0.tar", last modified: Tue Oct 18 12:01:54 2022, max compression
+gzip compressed data, was "Secweb-1.7.1.tar", last modified: Mon Jun 12 14:19:55 2023, max compression
```

## Comparing `Secweb-1.6.0.tar` & `Secweb-1.7.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.835878 Secweb-1.6.0/
--rw-rw-rw-   0        0        0    17154 2022-04-11 14:18:33.000000 Secweb-1.6.0/LICENSE
--rw-rw-rw-   0        0        0    18026 2022-10-18 12:01:54.836878 Secweb-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    17296 2022-10-18 07:52:46.000000 Secweb-1.6.0/README.md
--rw-rw-rw-   0        0        0       88 2022-10-18 09:42:21.000000 Secweb-1.6.0/pyproject.toml
--rw-rw-rw-   0        0        0      845 2022-10-18 12:01:54.838877 Secweb-1.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.699175 Secweb-1.6.0/src/
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.738756 Secweb-1.6.0/src/Secweb/
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.751754 Secweb-1.6.0/src/Secweb/CacheControl/
--rw-rw-rw-   0        0        0     4533 2022-10-18 09:38:24.000000 Secweb-1.6.0/src/Secweb/CacheControl/CacheControlMiddleware.py
--rw-rw-rw-   0        0        0       48 2022-04-09 06:01:04.000000 Secweb-1.6.0/src/Secweb/CacheControl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.763780 Secweb-1.6.0/src/Secweb/ClearSiteData/
--rw-rw-rw-   0        0        0     3899 2022-10-18 09:38:25.000000 Secweb-1.6.0/src/Secweb/ClearSiteData/ClearSiteDataMiddleware.py
--rw-rw-rw-   0        0        0       50 2022-04-09 06:01:25.000000 Secweb-1.6.0/src/Secweb/ClearSiteData/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.780896 Secweb-1.6.0/src/Secweb/ContentSecurityPolicy/
--rw-rw-rw-   0        0        0     5242 2022-10-18 09:38:25.000000 Secweb-1.6.0/src/Secweb/ContentSecurityPolicy/ContentSecurityPolicyMiddleware.py
--rw-rw-rw-   0        0        0      130 2021-07-11 12:29:16.000000 Secweb-1.6.0/src/Secweb/ContentSecurityPolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.783895 Secweb-1.6.0/src/Secweb/CrossOriginEmbedderPolicy/
--rw-rw-rw-   0        0        0     1497 2022-10-18 09:38:26.000000 Secweb-1.6.0/src/Secweb/CrossOriginEmbedderPolicy/CrossOriginEmbedderPolicyMiddleware.py
--rw-rw-rw-   0        0        0       74 2021-07-11 12:30:08.000000 Secweb-1.6.0/src/Secweb/CrossOriginEmbedderPolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.787893 Secweb-1.6.0/src/Secweb/CrossOriginOpenerPolicy/
--rw-rw-rw-   0        0        0     1561 2022-10-18 09:38:26.000000 Secweb-1.6.0/src/Secweb/CrossOriginOpenerPolicy/CrossOriginOpenerPolicyMiddleware.py
--rw-rw-rw-   0        0        0       70 2021-07-11 12:30:45.000000 Secweb-1.6.0/src/Secweb/CrossOriginOpenerPolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.790892 Secweb-1.6.0/src/Secweb/CrossOriginResourcePolicy/
--rw-rw-rw-   0        0        0     1526 2022-10-18 09:38:27.000000 Secweb-1.6.0/src/Secweb/CrossOriginResourcePolicy/CrossOriginResourcePolicyMiddleware.py
--rw-rw-rw-   0        0        0       74 2021-07-11 12:31:17.000000 Secweb-1.6.0/src/Secweb/CrossOriginResourcePolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.805887 Secweb-1.6.0/src/Secweb/ExpectCt/
--rw-rw-rw-   0        0        0     2203 2022-10-18 09:38:28.000000 Secweb-1.6.0/src/Secweb/ExpectCt/ExpectCtMiddleware.py
--rw-rw-rw-   0        0        0       42 2021-04-11 15:30:17.000000 Secweb-1.6.0/src/Secweb/ExpectCt/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.808886 Secweb-1.6.0/src/Secweb/OriginAgentCluster/
--rw-rw-rw-   0        0        0      992 2022-10-18 09:38:28.000000 Secweb-1.6.0/src/Secweb/OriginAgentCluster/OriginAgentClusterMiddleware.py
--rw-rw-rw-   0        0        0       62 2021-04-11 15:30:42.000000 Secweb-1.6.0/src/Secweb/OriginAgentCluster/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.812887 Secweb-1.6.0/src/Secweb/ReferrerPolicy/
--rw-rw-rw-   0        0        0     1990 2022-10-18 09:38:29.000000 Secweb-1.6.0/src/Secweb/ReferrerPolicy/ReferrerPolicyMiddleware.py
--rw-rw-rw-   0        0        0       54 2021-04-11 15:31:16.000000 Secweb-1.6.0/src/Secweb/ReferrerPolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.816885 Secweb-1.6.0/src/Secweb/StrictTransportSecurity/
--rw-rw-rw-   0        0        0     2075 2022-10-18 09:38:29.000000 Secweb-1.6.0/src/Secweb/StrictTransportSecurity/StrictTransportSecurityMiddleware.py
--rw-rw-rw-   0        0        0       51 2021-04-11 15:31:34.000000 Secweb-1.6.0/src/Secweb/StrictTransportSecurity/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.819885 Secweb-1.6.0/src/Secweb/XContentTypeOptions/
--rw-rw-rw-   0        0        0     1004 2022-10-18 09:38:30.000000 Secweb-1.6.0/src/Secweb/XContentTypeOptions/XContentTypeOptionsMiddleware.py
--rw-rw-rw-   0        0        0       64 2021-04-11 15:31:57.000000 Secweb-1.6.0/src/Secweb/XContentTypeOptions/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.822883 Secweb-1.6.0/src/Secweb/XDNSPrefetchControl/
--rw-rw-rw-   0        0        0     1407 2022-10-18 09:38:30.000000 Secweb-1.6.0/src/Secweb/XDNSPrefetchControl/XDNSPrefetchControlMiddleware.py
--rw-rw-rw-   0        0        0       64 2021-04-11 15:32:10.000000 Secweb-1.6.0/src/Secweb/XDNSPrefetchControl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.825883 Secweb-1.6.0/src/Secweb/XDownloadOptions/
--rw-rw-rw-   0        0        0      986 2022-10-18 09:38:31.000000 Secweb-1.6.0/src/Secweb/XDownloadOptions/XDownloadOptionsMiddleware.py
--rw-rw-rw-   0        0        0       58 2021-04-11 15:32:26.000000 Secweb-1.6.0/src/Secweb/XDownloadOptions/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.828880 Secweb-1.6.0/src/Secweb/XFrameOptions/
--rw-rw-rw-   0        0        0     1338 2022-10-18 09:38:31.000000 Secweb-1.6.0/src/Secweb/XFrameOptions/XFrameOptionsMiddleware.py
--rw-rw-rw-   0        0        0       45 2021-04-11 15:32:44.000000 Secweb-1.6.0/src/Secweb/XFrameOptions/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.831879 Secweb-1.6.0/src/Secweb/XPermittedCrossDomainPolicies/
--rw-rw-rw-   0        0        0     1574 2022-10-18 09:38:32.000000 Secweb-1.6.0/src/Secweb/XPermittedCrossDomainPolicies/XPermittedCrossDomainPoliciesMiddleware.py
--rw-rw-rw-   0        0        0       84 2021-04-11 15:33:27.000000 Secweb-1.6.0/src/Secweb/XPermittedCrossDomainPolicies/__init__.py
--rw-rw-rw-   0        0        0       25 2021-07-11 16:07:32.000000 Secweb-1.6.0/src/Secweb/__init__.py
--rw-rw-rw-   0        0        0     6877 2022-10-18 09:38:23.000000 Secweb-1.6.0/src/Secweb/index.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.834879 Secweb-1.6.0/src/Secweb/xXSSProtection/
--rw-rw-rw-   0        0        0       54 2021-04-11 15:33:44.000000 Secweb-1.6.0/src/Secweb/xXSSProtection/__init__.py
--rw-rw-rw-   0        0        0     1496 2022-10-18 09:38:33.000000 Secweb-1.6.0/src/Secweb/xXSSProtection/xXSSProtectionMiddleware.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:01:54.743757 Secweb-1.6.0/src/Secweb.egg-info/
--rw-rw-rw-   0        0        0    18026 2022-10-18 12:01:54.000000 Secweb-1.6.0/src/Secweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1897 2022-10-18 12:01:54.000000 Secweb-1.6.0/src/Secweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-18 12:01:54.000000 Secweb-1.6.0/src/Secweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-10-18 12:01:54.000000 Secweb-1.6.0/src/Secweb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.874220 Secweb-1.7.1/
+-rw-rw-rw-   0        0        0    17154 2023-06-11 15:32:03.000000 Secweb-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0    18130 2023-06-12 14:19:55.873223 Secweb-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    17396 2023-06-11 15:31:47.000000 Secweb-1.7.1/README.md
+-rw-rw-rw-   0        0        0      800 2023-06-11 15:24:00.000000 Secweb-1.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:19:55.874220 Secweb-1.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.763217 Secweb-1.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.781219 Secweb-1.7.1/src/Secweb/
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.791220 Secweb-1.7.1/src/Secweb/CacheControl/
+-rw-rw-rw-   0        0        0     4392 2023-06-10 14:44:58.000000 Secweb-1.7.1/src/Secweb/CacheControl/CacheControlMiddleware.py
+-rw-rw-rw-   0        0        0       48 2022-04-09 06:01:04.000000 Secweb-1.7.1/src/Secweb/CacheControl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.796220 Secweb-1.7.1/src/Secweb/ClearSiteData/
+-rw-rw-rw-   0        0        0     3768 2023-06-11 06:37:05.000000 Secweb-1.7.1/src/Secweb/ClearSiteData/ClearSiteDataMiddleware.py
+-rw-rw-rw-   0        0        0       50 2022-04-09 06:01:25.000000 Secweb-1.7.1/src/Secweb/ClearSiteData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.801219 Secweb-1.7.1/src/Secweb/ContentSecurityPolicy/
+-rw-rw-rw-   0        0        0     6144 2023-06-11 14:16:25.000000 Secweb-1.7.1/src/Secweb/ContentSecurityPolicy/ContentSecurityPolicyMiddleware.py
+-rw-rw-rw-   0        0        0      130 2021-07-11 12:29:16.000000 Secweb-1.7.1/src/Secweb/ContentSecurityPolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.806220 Secweb-1.7.1/src/Secweb/CrossOriginEmbedderPolicy/
+-rw-rw-rw-   0        0        0     1686 2023-06-10 06:05:41.000000 Secweb-1.7.1/src/Secweb/CrossOriginEmbedderPolicy/CrossOriginEmbedderPolicyMiddleware.py
+-rw-rw-rw-   0        0        0       74 2021-07-11 12:30:08.000000 Secweb-1.7.1/src/Secweb/CrossOriginEmbedderPolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.811220 Secweb-1.7.1/src/Secweb/CrossOriginOpenerPolicy/
+-rw-rw-rw-   0        0        0     1682 2023-06-10 05:46:33.000000 Secweb-1.7.1/src/Secweb/CrossOriginOpenerPolicy/CrossOriginOpenerPolicyMiddleware.py
+-rw-rw-rw-   0        0        0       70 2021-07-11 12:30:45.000000 Secweb-1.7.1/src/Secweb/CrossOriginOpenerPolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.815219 Secweb-1.7.1/src/Secweb/CrossOriginResourcePolicy/
+-rw-rw-rw-   0        0        0     1677 2023-06-10 05:32:12.000000 Secweb-1.7.1/src/Secweb/CrossOriginResourcePolicy/CrossOriginResourcePolicyMiddleware.py
+-rw-rw-rw-   0        0        0       74 2021-07-11 12:31:17.000000 Secweb-1.7.1/src/Secweb/CrossOriginResourcePolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.819218 Secweb-1.7.1/src/Secweb/ExpectCt/
+-rw-rw-rw-   0        0        0     2210 2023-06-10 05:21:43.000000 Secweb-1.7.1/src/Secweb/ExpectCt/ExpectCtMiddleware.py
+-rw-rw-rw-   0        0        0       42 2021-04-11 15:30:17.000000 Secweb-1.7.1/src/Secweb/ExpectCt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.823218 Secweb-1.7.1/src/Secweb/OriginAgentCluster/
+-rw-rw-rw-   0        0        0     1146 2023-06-09 15:21:23.000000 Secweb-1.7.1/src/Secweb/OriginAgentCluster/OriginAgentClusterMiddleware.py
+-rw-rw-rw-   0        0        0       62 2021-04-11 15:30:42.000000 Secweb-1.7.1/src/Secweb/OriginAgentCluster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.831221 Secweb-1.7.1/src/Secweb/ReferrerPolicy/
+-rw-rw-rw-   0        0        0     2345 2023-06-09 14:21:28.000000 Secweb-1.7.1/src/Secweb/ReferrerPolicy/ReferrerPolicyMiddleware.py
+-rw-rw-rw-   0        0        0       54 2021-04-11 15:31:16.000000 Secweb-1.7.1/src/Secweb/ReferrerPolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.841220 Secweb-1.7.1/src/Secweb/StrictTransportSecurity/
+-rw-rw-rw-   0        0        0     2155 2023-06-10 05:21:05.000000 Secweb-1.7.1/src/Secweb/StrictTransportSecurity/StrictTransportSecurityMiddleware.py
+-rw-rw-rw-   0        0        0       51 2021-04-11 15:31:34.000000 Secweb-1.7.1/src/Secweb/StrictTransportSecurity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.848220 Secweb-1.7.1/src/Secweb/XContentTypeOptions/
+-rw-rw-rw-   0        0        0     1162 2023-06-08 12:41:33.000000 Secweb-1.7.1/src/Secweb/XContentTypeOptions/XContentTypeOptionsMiddleware.py
+-rw-rw-rw-   0        0        0       64 2021-04-11 15:31:57.000000 Secweb-1.7.1/src/Secweb/XContentTypeOptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.853220 Secweb-1.7.1/src/Secweb/XDNSPrefetchControl/
+-rw-rw-rw-   0        0        0     1553 2023-06-09 10:34:53.000000 Secweb-1.7.1/src/Secweb/XDNSPrefetchControl/XDNSPrefetchControlMiddleware.py
+-rw-rw-rw-   0        0        0       64 2021-04-11 15:32:10.000000 Secweb-1.7.1/src/Secweb/XDNSPrefetchControl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.858219 Secweb-1.7.1/src/Secweb/XDownloadOptions/
+-rw-rw-rw-   0        0        0     1136 2023-06-08 12:32:50.000000 Secweb-1.7.1/src/Secweb/XDownloadOptions/XDownloadOptionsMiddleware.py
+-rw-rw-rw-   0        0        0       58 2021-04-11 15:32:26.000000 Secweb-1.7.1/src/Secweb/XDownloadOptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.862222 Secweb-1.7.1/src/Secweb/XFrameOptions/
+-rw-rw-rw-   0        0        0     1470 2023-06-09 10:32:42.000000 Secweb-1.7.1/src/Secweb/XFrameOptions/XFrameOptionsMiddleware.py
+-rw-rw-rw-   0        0        0       45 2021-04-11 15:32:44.000000 Secweb-1.7.1/src/Secweb/XFrameOptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.866219 Secweb-1.7.1/src/Secweb/XPermittedCrossDomainPolicies/
+-rw-rw-rw-   0        0        0     1735 2023-06-09 10:30:43.000000 Secweb-1.7.1/src/Secweb/XPermittedCrossDomainPolicies/XPermittedCrossDomainPoliciesMiddleware.py
+-rw-rw-rw-   0        0        0       84 2021-04-11 15:33:27.000000 Secweb-1.7.1/src/Secweb/XPermittedCrossDomainPolicies/__init__.py
+-rw-rw-rw-   0        0        0       25 2021-07-11 16:07:32.000000 Secweb-1.7.1/src/Secweb/__init__.py
+-rw-rw-rw-   0        0        0     6764 2023-06-11 14:40:50.000000 Secweb-1.7.1/src/Secweb/index.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.871218 Secweb-1.7.1/src/Secweb/xXSSProtection/
+-rw-rw-rw-   0        0        0       54 2021-04-11 15:33:44.000000 Secweb-1.7.1/src/Secweb/xXSSProtection/__init__.py
+-rw-rw-rw-   0        0        0     1636 2023-06-11 04:52:15.000000 Secweb-1.7.1/src/Secweb/xXSSProtection/xXSSProtectionMiddleware.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.786220 Secweb-1.7.1/src/Secweb.egg-info/
+-rw-rw-rw-   0        0        0    18130 2023-06-12 14:19:55.000000 Secweb-1.7.1/src/Secweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1887 2023-06-12 14:19:55.000000 Secweb-1.7.1/src/Secweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:19:55.000000 Secweb-1.7.1/src/Secweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 14:19:55.000000 Secweb-1.7.1/src/Secweb.egg-info/top_level.txt
```

### Comparing `Secweb-1.6.0/LICENSE` & `Secweb-1.7.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 Exhibit A - Source Code Form License Notice
 -------------------------------------------
 
   This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
   
-  Copyright 2021-2022, Motagamwala Taha Arif Ali
+  Copyright 2021-2023, Motagamwala Taha Arif Ali
 
 If it is not possible or desirable to put the notice in a particular
 file, then You may include the notice in a location (such as a LICENSE
 file in a relevant directory) where a recipient would be likely to look
 for such a notice.
 
 You may add additional accurate notices of copyright ownership.
```

### Comparing `Secweb-1.6.0/PKG-INFO` & `Secweb-1.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,17 @@
-Metadata-Version: 2.1
-Name: Secweb
-Version: 1.6.0
-Summary: Secweb is a pack of security middlewares for fastApi and starlette servers it includes CSP, HSTS, and many more
-Home-page: https://github.com/tmotagam/Secweb
-Author: Motagamwala Taha Arif Ali
-Author-email: tahaar5321@gmail.com
-Project-URL: Bug Tracker, https://github.com/tmotagam/Secweb/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align = "center"><img alt="Secweb logo" src="https://raw.githubusercontent.com/tmotagam/Secweb/main/Secweb.jpg"></p>
 
 <p align="center"><em>Secweb helps in setting security headers for FastApi and Starlette</em></p>
 
 ---
 <br>
 
-Secweb is the pack of middlewares for setting security headers for fastapi and can also be used for any framework created on starlette it has 16 middlewares for setting headers of your website and also for your api`s
+Secweb is the pack of middlewares for setting security headers for fastapi and can also be used for any framework created on starlette it has 16 middlewares for setting headers of your website and also for your api(s)
+
+Now all the middlewares are pure ASGI implemented middlewares and from now on all the release will have sigstore signatures you can get them from the github release for both dev and production Secweb.
 
 #### The PermissionsPolicy middleware lies in development branch [here](https://github.com/tmotagam/Secweb/tree/Secweb-Beta#readme)
 
 The list of middleware is as follows:
 
 1. Content Security Policy (CSP)
 
@@ -164,15 +149,15 @@
 12. `'clearSiteData'` for calling ClearSiteData class to set the user-defined values
 <br>
 
 13. `'cacheControl'` for calling CacheControl class to set the user-defined values
 
 ```python
 # Example of the values
-SecWeb(app=app, Option={'csp': {'default-src': ["'self'"]}, 'xframe': {'X-Frame-Options': 'SAMEORIGIN'}, 'xss': {'X-XSS-Protection': '1; mode=block'}, 'hsts': {'max-age': 4, 'preload': True}, 'xcdp': {'X-Permitted-Cross-Domain-Policies': 'all'}, 'xdns': {'X-DNS-Prefetch-Control': 'on'}, 'referrer': {'Referrer-Policy': 'no-referrer'}, 'expectCt': {'max-age': 128, 'enforce': True, 'report-uri': "https://example.com/example"}, 'coep': {'Cross-Origin-Embedder-Policy': 'require-corp'}, 'coop': {'Cross-Origin-Opener-Policy': 'same-origin-allow-popups'}, 'corp': {'Cross-Origin-Resource-Policy': 'same-site'}, 'clearSiteData': {'cache': True, 'storage': True}, 'cacheControl': {'public': True, 's-maxage': 600}}, Routes=['/login', '/logout/{id}'])
+SecWeb(app=app, Option={'csp': {'default-src': ["'self'"]}, 'xframe': {'X-Frame-Options': 'SAMEORIGIN'}, 'xss': {'X-XSS-Protection': '1; mode=block'}, 'hsts': {'max-age': 4, 'preload': True}, 'xcdp': {'X-Permitted-Cross-Domain-Policies': 'all'}, 'xdns': {'X-DNS-Prefetch-Control': 'on'}, 'referrer': {'Referrer-Policy': 'no-referrer'}, 'expectCt': {'max-age': 128, 'enforce': True, 'report-uri': "https://example.com/example"}, 'coep': {'Cross-Origin-Embedder-Policy': 'require-corp'}, 'coop': {'Cross-Origin-Opener-Policy': 'same-origin-allow-popups'}, 'corp': {'Cross-Origin-Resource-Policy': 'same-site'}, 'clearSiteData': {'cache': True, 'storage': True}, 'cacheControl': {'public': True, 's-maxage': 600}}, Routes=['/login/{id}', '/logout/{id:uuid}/username/{username:string}'])
 ```
 ### Middleware Classes
 
 #### Content Security Policy (CSP)
 
 ContentSecurityPolicy class sets the csp header
 
@@ -384,15 +369,14 @@
 from starlette.applications import Starlette
 from Secweb.XDownloadOptions import XDownloadOptions
 
 app = Starlette()
 
 app.add_middleware(XDownloadOptions)
 ```
-For more detail on X-Download-Options header go to this [NWebsec Site](https://www.nwebsec.com/HttpHeaders/SecurityHeaders/XDownloadOptions)
 
 #### X-Frame
 
 XFrame class sets the X-Frame-Options header
 
 ```python
 from fastapi import FastAPI
@@ -582,8 +566,8 @@
 [Github](https://github.com/tmotagam/Secweb)
 
 ## License
 [MLP 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
 
 ## Secweb Icon
 
-[Secweb Icon](https://github.com/tmotagam/Secweb/blob/main/Secweb.jpg) © 2021 - 2022 by [Motagamwala Taha Arif Ali](https://github.com/tmotagam) is licensed under [Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1)
+[Secweb Icon](https://github.com/tmotagam/Secweb/blob/main/Secweb.jpg) © 2021 - 2023 by [Motagamwala Taha Arif Ali](https://github.com/tmotagam) is licensed under [Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1)
```

### Comparing `Secweb-1.6.0/README.md` & `Secweb-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,33 @@
+Metadata-Version: 2.1
+Name: Secweb
+Version: 1.7.1
+Summary: Secweb is a pack of security middlewares for fastApi and starlette server it includes CSP, HSTS, and many more
+Author-email: Motagamwala Taha Arif Ali <tahaar5321@gmail.com>
+Project-URL: Homepage, https://github.com/tmotagam/Secweb
+Project-URL: Bug Tracker, https://github.com/tmotagam/Secweb/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align = "center"><img alt="Secweb logo" src="https://raw.githubusercontent.com/tmotagam/Secweb/main/Secweb.jpg"></p>
 
 <p align="center"><em>Secweb helps in setting security headers for FastApi and Starlette</em></p>
 
 ---
 <br>
 
-Secweb is the pack of middlewares for setting security headers for fastapi and can also be used for any framework created on starlette it has 16 middlewares for setting headers of your website and also for your api`s
+Secweb is the pack of middlewares for setting security headers for fastapi and can also be used for any framework created on starlette it has 16 middlewares for setting headers of your website and also for your api(s)
+
+Now all the middlewares are pure ASGI implemented middlewares and from now on all the release will have sigstore signatures you can get them from the github release for both dev and production Secweb.
 
 #### The PermissionsPolicy middleware lies in development branch [here](https://github.com/tmotagam/Secweb/tree/Secweb-Beta#readme)
 
 The list of middleware is as follows:
 
 1. Content Security Policy (CSP)
 
@@ -147,15 +165,15 @@
 12. `'clearSiteData'` for calling ClearSiteData class to set the user-defined values
 <br>
 
 13. `'cacheControl'` for calling CacheControl class to set the user-defined values
 
 ```python
 # Example of the values
-SecWeb(app=app, Option={'csp': {'default-src': ["'self'"]}, 'xframe': {'X-Frame-Options': 'SAMEORIGIN'}, 'xss': {'X-XSS-Protection': '1; mode=block'}, 'hsts': {'max-age': 4, 'preload': True}, 'xcdp': {'X-Permitted-Cross-Domain-Policies': 'all'}, 'xdns': {'X-DNS-Prefetch-Control': 'on'}, 'referrer': {'Referrer-Policy': 'no-referrer'}, 'expectCt': {'max-age': 128, 'enforce': True, 'report-uri': "https://example.com/example"}, 'coep': {'Cross-Origin-Embedder-Policy': 'require-corp'}, 'coop': {'Cross-Origin-Opener-Policy': 'same-origin-allow-popups'}, 'corp': {'Cross-Origin-Resource-Policy': 'same-site'}, 'clearSiteData': {'cache': True, 'storage': True}, 'cacheControl': {'public': True, 's-maxage': 600}}, Routes=['/login', '/logout/{id}'])
+SecWeb(app=app, Option={'csp': {'default-src': ["'self'"]}, 'xframe': {'X-Frame-Options': 'SAMEORIGIN'}, 'xss': {'X-XSS-Protection': '1; mode=block'}, 'hsts': {'max-age': 4, 'preload': True}, 'xcdp': {'X-Permitted-Cross-Domain-Policies': 'all'}, 'xdns': {'X-DNS-Prefetch-Control': 'on'}, 'referrer': {'Referrer-Policy': 'no-referrer'}, 'expectCt': {'max-age': 128, 'enforce': True, 'report-uri': "https://example.com/example"}, 'coep': {'Cross-Origin-Embedder-Policy': 'require-corp'}, 'coop': {'Cross-Origin-Opener-Policy': 'same-origin-allow-popups'}, 'corp': {'Cross-Origin-Resource-Policy': 'same-site'}, 'clearSiteData': {'cache': True, 'storage': True}, 'cacheControl': {'public': True, 's-maxage': 600}}, Routes=['/login/{id}', '/logout/{id:uuid}/username/{username:string}'])
 ```
 ### Middleware Classes
 
 #### Content Security Policy (CSP)
 
 ContentSecurityPolicy class sets the csp header
 
@@ -367,15 +385,14 @@
 from starlette.applications import Starlette
 from Secweb.XDownloadOptions import XDownloadOptions
 
 app = Starlette()
 
 app.add_middleware(XDownloadOptions)
 ```
-For more detail on X-Download-Options header go to this [NWebsec Site](https://www.nwebsec.com/HttpHeaders/SecurityHeaders/XDownloadOptions)
 
 #### X-Frame
 
 XFrame class sets the X-Frame-Options header
 
 ```python
 from fastapi import FastAPI
@@ -565,8 +582,8 @@
 [Github](https://github.com/tmotagam/Secweb)
 
 ## License
 [MLP 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
 
 ## Secweb Icon
 
-[Secweb Icon](https://github.com/tmotagam/Secweb/blob/main/Secweb.jpg) © 2021 - 2022 by [Motagamwala Taha Arif Ali](https://github.com/tmotagam) is licensed under [Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1)
+[Secweb Icon](https://github.com/tmotagam/Secweb/blob/main/Secweb.jpg) © 2021 - 2023 by [Motagamwala Taha Arif Ali](https://github.com/tmotagam) is licensed under [Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1)
```

### Comparing `Secweb-1.6.0/src/Secweb/CacheControl/CacheControlMiddleware.py` & `Secweb-1.7.1/src/Secweb/CacheControl/CacheControlMiddleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,72 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-
-class CacheControl(BaseHTTPMiddleware):
+class CacheControl:
     ''' CacheControl class sets Cache-Control header it takes one Parameter
 
     Example:
         app.add_middleware(CacheControl, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'max-age': 86400, 'private': True}) -> None:
-        super().__init__(app)
-        self.Option = Option
-        self.policyString = ''
-
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
+    def __init__(self, app: ASGIApp, Option: dict[str, int | bool] = {'max-age': 86400, 'private': True }):
+        self.app = app
         self.policyString = ''
-        option = dict(self.Option)
-        response = await call_next(request)
-        if 'max-age' in option and option['max-age'] >= 0:
-            self.policyString += f'max-age={str(option["max-age"])}' if list(
-                option.keys()).__len__() == 1 else f'max-age={str(option["max-age"])}, '
-            option.pop('max-age')
-        if 's-maxage' in option and option['s-maxage'] >= 0:
-            self.policyString += f's-maxage={str(option["s-maxage"])}' if list(
-                option.keys()).__len__() == 1 else f's-maxage={str(option["s-maxage"])}, '
-            option.pop('s-maxage')
-        if 'no-cache' in option and option['no-cache'] is True:
-            self.policyString += 'no-cache' if list(
-                option.keys()).__len__() == 1 else 'no-cache, '
-            option.pop('no-cache')
-        if 'no-store' in option and option['no-store'] is True:
-            self.policyString += 'no-store' if list(
-                option.keys()).__len__() == 1 else 'no-store, '
-            option.pop('no-store')
-        if 'no-transform' in option and option['no-transform'] is True:
-            self.policyString += 'no-transform' if list(
-                option.keys()).__len__() == 1 else 'no-transform, '
-            option.pop('no-transform')
-        if 'must-revalidate' in option and option['must-revalidate'] is True:
-            self.policyString += 'must-revalidate' if list(
-                option.keys()).__len__() == 1 else 'must-revalidate, '
-            option.pop('must-revalidate')
-        if 'proxy-revalidate' in option and option['proxy-revalidate'] is True:
-            self.policyString += 'proxy-revalidate' if list(
-                option.keys()).__len__() == 1 else 'proxy-revalidate, '
-            option.pop('proxy-revalidate')
-        if 'must-understand' in option and option['must-understand'] is True:
-            self.policyString += 'must-understand' if list(
-                option.keys()).__len__() == 1 else 'must-understand, '
-            option.pop('must-understand')
-        if 'private' in option and option['private'] is True:
-            self.policyString += 'private' if list(
-                option.keys()).__len__() == 1 else 'private, '
-            option.pop('private')
-        if 'public' in option and option['public'] is True:
-            self.policyString += 'public' if list(
-                option.keys()).__len__() == 1 else 'public, '
-            option.pop('public')
-        if 'immutable' in option and option['immutable'] is True:
-            self.policyString += 'immutable' if list(
-                option.keys()).__len__() == 1 else 'immutable, '
-            option.pop('immutable')
-        if 'stale-while-revalidate' in option and option['stale-while-revalidate'] > 0:
-            self.policyString += f'stale-while-revalidate={str(option["stale-while-revalidate"])}' if list(
-                option.keys()).__len__() == 1 else f'stale-while-revalidate={str(option["stale-while-revalidate"])}, '
-            option.pop('stale-while-revalidate')
-        if list(option.keys()).__len__() != 0:
+        if 'max-age' in Option and Option['max-age'] >= 0:
+            self.policyString += f'max-age={str(Option["max-age"])}' if list(Option.keys()).__len__() == 1 else f'max-age={str(Option["max-age"])}, '
+            Option.pop('max-age')
+        if 's-maxage' in Option and Option['s-maxage'] >= 0:
+            self.policyString += f's-maxage={str(Option["s-maxage"])}' if list(Option.keys()).__len__() == 1 else f's-maxage={str(Option["s-maxage"])}, '
+            Option.pop('s-maxage')
+        if 'no-cache' in Option and Option['no-cache'] is True:
+            self.policyString += 'no-cache' if list(Option.keys()).__len__() == 1 else 'no-cache, '
+            Option.pop('no-cache')
+        if 'no-store' in Option and Option['no-store'] is True:
+            self.policyString += 'no-store' if list(Option.keys()).__len__() == 1 else 'no-store, '
+            Option.pop('no-store')
+        if 'no-transform' in Option and Option['no-transform'] is True:
+            self.policyString += 'no-transform' if list(Option.keys()).__len__() == 1 else 'no-transform, '
+            Option.pop('no-transform')
+        if 'must-revalidate' in Option and Option['must-revalidate'] is True:
+            self.policyString += 'must-revalidate' if list(Option.keys()).__len__() == 1 else 'must-revalidate, '
+            Option.pop('must-revalidate')
+        if 'proxy-revalidate' in Option and Option['proxy-revalidate'] is True:
+            self.policyString += 'proxy-revalidate' if list(Option.keys()).__len__() == 1 else 'proxy-revalidate, '
+            Option.pop('proxy-revalidate')
+        if 'must-understand' in Option and Option['must-understand'] is True:
+            self.policyString += 'must-understand' if list(Option.keys()).__len__() == 1 else 'must-understand, '
+            Option.pop('must-understand')
+        if 'private' in Option and Option['private'] is True:
+            self.policyString += 'private' if list(Option.keys()).__len__() == 1 else 'private, '
+            Option.pop('private')
+        if 'public' in Option and Option['public'] is True:
+            self.policyString += 'public' if list(Option.keys()).__len__() == 1 else 'public, '
+            Option.pop('public')
+        if 'immutable' in Option and Option['immutable'] is True:
+            self.policyString += 'immutable' if list(Option.keys()).__len__() == 1 else 'immutable, '
+            Option.pop('immutable')
+        if 'stale-while-revalidate' in Option and Option['stale-while-revalidate'] > 0:
+            self.policyString += f'stale-while-revalidate={str(Option["stale-while-revalidate"])}' if list(Option.keys()).__len__() == 1 else f'stale-while-revalidate={str(Option["stale-while-revalidate"])}, '
+            Option.pop('stale-while-revalidate')
+        if list(Option.keys()).__len__() != 0 :
             raise SyntaxError('Cache-Control has 12 options 1> "max-age" 2> "s-maxage" 3> "no-cache" 4> "no-store" 5> "no-transform" 6> "must-revalidate" 7> "proxy-revalidate" 8> "must-understand" 9> "private" 10> "public" 11> "immutable" 12> "stale-while-revalidate" ')
-        response.headers['Cache-Control'] = self.policyString
-        return response
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_Cache_Control(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('Cache-Control', self.policyString)
+
+            await send(message)
+
+        await self.app(scope, receive, set_Cache_Control)
```

### Comparing `Secweb-1.6.0/src/Secweb/ContentSecurityPolicy/ContentSecurityPolicyMiddleware.py` & `Secweb-1.7.1/src/Secweb/ContentSecurityPolicy/ContentSecurityPolicyMiddleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,116 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
-import secrets
+from secrets import token_urlsafe
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
 nonce = None
 
-
 def Nonce_Processor(DEFAULT_ENTROPY=90):
     ''' This is the Nonce Processor module that will create the nonce for inline style and script
     It will be needed to call on the route which needs nonce for the inline script and css
 
     Example :
         @app.get("/")
         async def root():
             nonce = Nonce_Processor(DEFAULT_ENTROPY=20)  # inject the nonce variable into the jinja or html
 
     Parameter :
-    DEFAULT_ENTROPY=20 This option sets the default entropy of the secrets module used for generating nonce'''
+    DEFAULT_ENTROPY=20 This option sets the default entropy used for generating nonce'''
     global nonce
-    secrets.DEFAULT_ENTROPY = DEFAULT_ENTROPY
-    nonce = secrets.token_urlsafe()
+    nonce = token_urlsafe(DEFAULT_ENTROPY)
     return nonce
 
-
-class ContentSecurityPolicy(BaseHTTPMiddleware):
+class ContentSecurityPolicy:
     ''' ContentSecurityPolicy class takes three prarameters script_nonce, style_nonce, Option for
     creating your csp header
 
     Example :
         app.add_middleware(ContentSecurityPolicy, Option={}, script_nonce=False, style_nonce=True)
 
     Parameters :
 
     Option={} This is a dictionary
 
     script_nonce=False This is the nonce flag for script
 
     style_nocne=True This is the nonce flag for style css'''
-
-    def __init__(self, app: ASGIApp, script_nonce: bool = False, style_nonce: bool = False, Option: dict = {'default-src': ["'self'"], 'base-uri': ["'self'"], 'block-all-mixed-content': [], 'font-src': ["'self'", 'https:', 'data:'], 'frame-ancestors': ["'self'"], 'img-src': ["'self'", 'data:'], "object-src": ["'none'"], "script-src": ["'self'"], "script-src-attr": ["'none'"], "style-src": ["'self'", "https:", "'unsafe-inline'"], "upgrade-insecure-requests": [], "require-trusted-types-for": ["'script'"]}) -> None:
-        super().__init__(app)
-        self.Option = Option
+    def __init__(self, app: ASGIApp, script_nonce: bool = False, style_nonce: bool = False, Option: dict[str, list[str]] = {'default-src': ["'self'"], 'base-uri': ["'self'"], 'block-all-mixed-content': [], 'font-src': ["'self'", 'https:', 'data:'], 'frame-ancestors': ["'self'"], 'img-src': ["'self'", 'data:'], "object-src": ["'none'"], "script-src": ["'self'"], "script-src-attr": ["'none'"], "style-src": ["'self'", "https:", "'unsafe-inline'"], "upgrade-insecure-requests": [], "require-trusted-types-for": ["'script'"]}):
+        self.app = app
+        self.PolicyString = ''
         self.script_nonce = script_nonce
         self.style_nonce = style_nonce
-        self.PolicyString = ''
-        self.Policy = ['child-src', 'connect-src', 'default-src', 'font-src', 'frame-src', 'img-src', 'manifest-src', 'media-src', 'object-src', 'prefetch-src', 'script-src', 'script-src-elem', 'script-src-attr', 'style-src', 'style-src-elem', 'style-src-attr',
-                       'worker-src', 'base-uri', 'plugin-types', 'sandbox', 'form-action', 'frame-ancestors', 'navigate-to', 'report-uri', 'report-to', 'block-all-mixed-content', 'require-sri-for', 'require-trusted-types-for', 'trusted-types', 'upgrade-insecure-requests']
-
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        response = await call_next(request)
-        self.__PolicyCheck__()
-        response.headers['Content-Security-Policy'] = self.PolicyString
-        return response
+        Policy = ['child-src', 'connect-src', 'default-src', 'font-src', 'frame-src', 'img-src', 'manifest-src', 'media-src', 'object-src', 'script-src', 'script-src-elem', 'script-src-attr', 'style-src', 'style-src-elem', 'style-src-attr', 'worker-src', 'base-uri', 'plugin-types', 'sandbox', 'form-action', 'frame-ancestors', 'navigate-to', 'report-uri', 'report-to', 'block-all-mixed-content', 'require-trusted-types-for', 'trusted-types', 'upgrade-insecure-requests']
+        self.__PolicyCheck__(Option, Policy)
 
-    def __PolicyCheck__(self):
-        self.PolicyString = ''
-        keys = list(self.Option.keys())
+    def __PolicyCheck__(self, Option: dict[str, list[str]], Policy: list[str]):
+        keys = list(Option.keys())
 
         if self.script_nonce is True:
             if keys.index('script-src') is None:
                 raise SyntaxError('script-src is compulsory for nonce')
 
-            if len(self.Option['script-src']) == 0:
-                raise SyntaxError(
-                    'script-src cannot be empty for nonce to be applied')
-
         if self.style_nonce is True:
             if keys.index('style-src') is None:
                 raise SyntaxError('style-src is compulsory for nonce')
 
-            if len(self.Option['style-src']) == 0:
-                raise SyntaxError(
-                    'style-src cannot be empty for nonce to be applied')
-
         for i in range(len(keys)):
-            if keys[i] in self.Policy:
+            if keys[i] in Policy:
                 self.PolicyString += keys[i]
-                values = self.Option[keys[i]]
-                if i == len(keys) - 1:
+                values = Option[keys[i]]
+                if (keys[i] == 'script-src' and self.script_nonce is True and len(values) == 0) or (keys[i] == 'style-src' and self.style_nonce is True and len(values) == 0):
+                    self.PolicyString += " "
+                elif i == len(keys) - 1:
                     if len(values) != 0:
                         self.PolicyString += " "
                     else:
                         self.PolicyString += ''
                 elif len(values) == 0:
                     self.PolicyString += '; '
                 else:
                     self.PolicyString += " "
 
                 if keys[i] == 'script-src' and self.script_nonce is True:
-                    self.PolicyString += "'nonce-" + nonce + "' "
+                    self.PolicyString += "'nonce-{script_nonce_value}'" if i == len(keys) - 1 and len(values) == 0 else "'nonce-{script_nonce_value}'; " if len(values) == 0 else "'nonce-{script_nonce_value}' "
 
                 if keys[i] == 'style-src' and self.style_nonce is True:
-                    self.PolicyString += "'nonce-" + nonce + "' "
+                    self.PolicyString += "'nonce-{style_nonce_value}'" if i == len(keys) - 1 and len(values) == 0 else "'nonce-{style_nonce_value}'; " if len(values) == 0 else "'nonce-{style_nonce_value}' "
 
                 for j in range(len(values)):
                     self.PolicyString += values[j]
                     if j == len(values) - 1:
                         if i == len(keys) - 1:
                             self.PolicyString += ''
                         else:
                             self.PolicyString += '; '
                     else:
                         self.PolicyString += ' '
             else:
                 raise SyntaxError(f'The Policy { keys[i] } does not exists')
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_Content_Security_Policy(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                if self.script_nonce is True and self.style_nonce is True:
+                    PS = self.PolicyString
+                    headers.append('Content-Security-Policy', PS.format(script_nonce_value=nonce, style_nonce_value=nonce))
+                elif self.style_nonce is True:
+                    PS = self.PolicyString
+                    headers.append('Content-Security-Policy', PS.format(style_nonce_value=nonce))
+                elif self.script_nonce is True:
+                    PS = self.PolicyString
+                    headers.append('Content-Security-Policy', PS.format(script_nonce_value=nonce))
+                else:
+                    headers.append('Content-Security-Policy', self.PolicyString)
+
+            await send(message)
+
+        await self.app(scope, receive, set_Content_Security_Policy)
```

### Comparing `Secweb-1.6.0/src/Secweb/CrossOriginEmbedderPolicy/CrossOriginEmbedderPolicyMiddleware.py` & `Secweb-1.7.1/src/Secweb/CrossOriginEmbedderPolicy/CrossOriginEmbedderPolicyMiddleware.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-
-class CrossOriginEmbedderPolicy(BaseHTTPMiddleware):
+class CrossOriginEmbedderPolicy:
     ''' CrossOriginEmbedderPolicy class sets Cross-Origin-Embedder-Policy header it takes one Parameter
 
     Example:
         app.add_middleware(CrossOriginEmbedderPolicy, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'Cross-Origin-Embedder-Policy': 'unsafe-none'}) -> None:
-        super().__init__(app)
+    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'Cross-Origin-Embedder-Policy': 'unsafe-none'}):
+        self.app = app
         self.Option = Option
-        self.Policies = ['require-corp', 'unsafe-none']
+        Policies = ['require-corp', 'unsafe-none', 'credentialless']
+        if self.Option['Cross-Origin-Embedder-Policy'] not in Policies:
+            raise SyntaxError('Cross-Origin-Embedder-Policy has 3 options 1> "unsafe-none" 2> "require-corp" 3> "credentialless"')
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_Cross_Origin_Embedder_Policy(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('Cross-Origin-Embedder-Policy', self.Option['Cross-Origin-Embedder-Policy'])
+
+            await send(message)
 
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        response = await call_next(request)
-        if self.Option['Cross-Origin-Embedder-Policy'] in self.Policies:
-            response.headers['Cross-Origin-Embedder-Policy'] = self.Option['Cross-Origin-Embedder-Policy']
-        else:
-            raise SyntaxError(
-                'Cross-Origin-Embedder-Policy has 2 options 1> "unsafe-none" 2> "require-corp"')
-        return response
+        await self.app(scope, receive, set_Cross_Origin_Embedder_Policy)
```

### Comparing `Secweb-1.6.0/src/Secweb/CrossOriginOpenerPolicy/CrossOriginOpenerPolicyMiddleware.py` & `Secweb-1.7.1/src/Secweb/CrossOriginOpenerPolicy/CrossOriginOpenerPolicyMiddleware.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-
-class CrossOriginOpenerPolicy(BaseHTTPMiddleware):
+class CrossOriginOpenerPolicy:
     ''' CrossOriginOpenerPolicy class sets Cross-Origin-Opener-Policy header it takes one Parameter
 
     Example:
         app.add_middleware(CrossOriginOpenerPolicy, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'Cross-Origin-Opener-Policy': 'unsafe-none'}) -> None:
-        super().__init__(app)
+    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'Cross-Origin-Opener-Policy': 'unsafe-none'}):
+        self.app = app
         self.Option = Option
-        self.Policies = ['unsafe-none',
-                         'same-origin-allow-popups', 'same-origin']
+        Policies = ['unsafe-none', 'same-origin-allow-popups', 'same-origin']
+        if self.Option['Cross-Origin-Opener-Policy'] not in Policies:
+            raise SyntaxError('Cross-Origin-Opener-Policy has 3 options 1> "unsafe-none" 2> "same-origin-allow-popups" 3> "same-origin"')
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_Cross_Origin_Opener_Policy(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('Cross-Origin-Opener-Policy', self.Option['Cross-Origin-Opener-Policy'])
+
+            await send(message)
 
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        response = await call_next(request)
-        if self.Option['Cross-Origin-Opener-Policy'] in self.Policies:
-            response.headers['Cross-Origin-Opener-Policy'] = self.Option['Cross-Origin-Opener-Policy']
-        else:
-            raise SyntaxError(
-                'Cross-Origin-Opener-Policy has 3 options 1> "unsafe-none" 2> "same-origin-allow-popups" 3> "same-origin"')
-        return response
+        await self.app(scope, receive, set_Cross_Origin_Opener_Policy)
```

### Comparing `Secweb-1.6.0/src/Secweb/CrossOriginResourcePolicy/CrossOriginResourcePolicyMiddleware.py` & `Secweb-1.7.1/src/Secweb/XDNSPrefetchControl/XDNSPrefetchControlMiddleware.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-
-class CrossOriginResourcePolicy(BaseHTTPMiddleware):
-    ''' CrossOriginResourcePolicy class sets Cross-Origin-Resource-Policy header it takes one Parameter
+class XDNSPrefetchControl:
+    ''' XDNSPrefetchControl class sets X-DNS-Prefetch-Control header it takes one Parameter
 
     Example:
-        app.add_middleware(CrossOriginResourcePolicy, Option={})
+        app.add_middleware(XDNSPrefetchControl, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'Cross-Origin-Resource-Policy': 'cross-origin'}) -> None:
-        super().__init__(app)
+    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'X-DNS-Prefetch-Control': 'off'}):
+        self.app = app
         self.Option = Option
-        self.Policies = ['same-site', 'same-origin', 'cross-origin']
+        if self.Option['X-DNS-Prefetch-Control'] != 'on' and self.Option['X-DNS-Prefetch-Control'] != 'off':
+            raise SyntaxError('X-DNS-Prefetch-Control has two values only 1> "on" 2> "off"')
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_x_DNS_Prefetch_Control(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('X-DNS-Prefetch-Control', self.Option['X-DNS-Prefetch-Control'])
+
+            await send(message)
 
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        response = await call_next(request)
-        if self.Option['Cross-Origin-Resource-Policy'] in self.Policies:
-            response.headers['Cross-Origin-Resource-Policy'] = self.Option['Cross-Origin-Resource-Policy']
-        else:
-            raise SyntaxError(
-                'Cross-Origin-Resource-Policy has 3 options 1> "same-site" 2> "same-origin" 3> "cross-origin"')
-        return response
+        await self.app(scope, receive, set_x_DNS_Prefetch_Control)
```

### Comparing `Secweb-1.6.0/src/Secweb/ExpectCt/ExpectCtMiddleware.py` & `Secweb-1.7.1/src/Secweb/ExpectCt/ExpectCtMiddleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from warnings import warn
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-import warnings
-
-
-class ExpectCt(BaseHTTPMiddleware):
+class ExpectCt:
     ''' ExpectCt class takes only one parameter Option for setting the Expect-CT header (deprecated)
 
     Example :
         app.add_middleware(ExpectCt, Option={})
 
     Parameter :
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'max-age': 123, 'enforce': False, 'report-uri': ''}) -> None:
-        super().__init__(app)
-        self.Option = Option
-        self.PolicyString = ''
-
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
+    def __init__(self, app: ASGIApp, Option: dict[str, str | bool | int] = {'max-age': 123, 'enforce': False, 'report-uri': ''}):
+        self.app = app
         self.PolicyString = ''
-        response = await call_next(request)
-        warnings.warn(
-            "Expect-CT Header is now deprecated by browsers and may be removed from the library in the upcoming versions", SyntaxWarning, 2)
-        if 'max-age' in self.Option:
-            if int(self.Option['max-age']) and self.Option['max-age'] > 0:
-                self.PolicyString += 'max-age=' + str(self.Option['max-age'])
+        warn("Expect-CT Header is now deprecated by browsers and may be removed from the library in the upcoming versions", SyntaxWarning, 2)
+        if 'max-age' in Option:
+            if int(Option['max-age']) and int(Option['max-age']) > 0:
+                self.PolicyString += 'max-age=' + str(Option['max-age'])
             else:
                 raise SyntaxError('max-age needs to be a positive integer')
 
-            if 'enforce' in self.Option and self.Option['enforce'] is True:
+            if 'enforce' in Option and Option['enforce'] is True:
                 self.PolicyString += ', enforce'
 
-            if 'report-uri' in self.Option and self.Option['report-uri'] != '':
-                self.PolicyString += ', report-uri=' + '"' + \
-                    str(self.Option['report-uri']) + '"'
+            if 'report-uri' in Option and Option['report-uri'] != '':
+                self.PolicyString += ', report-uri=' + '"' + str(Option['report-uri']) + '"'
 
-            response.headers['Expect-CT'] = self.PolicyString
         else:
-            raise SyntaxError(
-                'Expect-CT has 3 options 1> "max-age=<Age>" <- This is the compulsory option 2> "enforce" 3> "report-uri=<Your URI>"')
-        return response
+            raise SyntaxError('Expect-CT has 3 options 1> "max-age=<Age>" <- This is the compulsory option 2> "enforce" 3> "report-uri=<Your URI>"')
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_Expect_CT(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('Expect-CT', self.PolicyString)
+
+            await send(message)
+
+        await self.app(scope, receive, set_Expect_CT)
```

### Comparing `Secweb-1.6.0/src/Secweb/ReferrerPolicy/ReferrerPolicyMiddleware.py` & `Secweb-1.7.1/src/Secweb/ReferrerPolicy/ReferrerPolicyMiddleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-
-class ReferrerPolicy(BaseHTTPMiddleware):
+class ReferrerPolicy:
     ''' ReferrerPolicy class sets Referrer-Policy header it takes one Parameter
 
     Example:
         app.add_middleware(ReferrerPolicy, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'Referrer-Policy': 'strict-origin-when-cross-origin'}) -> None:
-        super().__init__(app)
-        self.Option = Option
-        self.Policies = ['no-referrer', 'no-referrer-when-downgrade', 'origin', 'origin-when-cross-origin',
-                         'same-origin', 'strict-origin', 'strict-origin-when-cross-origin', 'unsafe-url']
-
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        response = await call_next(request)
-        if self.Option['Referrer-Policy'] in self.Policies:
-            response.headers['Referrer-Policy'] = self.Option['Referrer-Policy']
-        elif len(self.Option['Referrer-Policy']) == 2:
-            if self.Option['Referrer-Policy'][0] in self.Policies and self.Option['Referrer-Policy'][1] in self.Policies:
-                response.headers['Referrer-Policy'] = ', '.join(
-                    self.Option['Referrer-Policy'])
+    def __init__(self, app: ASGIApp, Option: dict[str, str | list[str]] = {'Referrer-Policy': 'strict-origin-when-cross-origin'}):
+        self.app = app
+        Policies = ['no-referrer', 'no-referrer-when-downgrade', 'origin', 'origin-when-cross-origin', 'same-origin', 'strict-origin', 'strict-origin-when-cross-origin', 'unsafe-url']
+        self.policystring = ''
+        if Option['Referrer-Policy'] in Policies:
+            self.policystring = Option['Referrer-Policy']
+        elif len(Option['Referrer-Policy']) > 1:
+            for option in Option['Referrer-Policy']:
+                if option not in Policies:
+                    raise SyntaxError('Referrer-Policy has 8 options 1> "no-referrer" 2> "no-referrer-when-downgrade" 3> "origin" 4> "origin-when-cross-origin" 5> "same-origin" 6> "strict-origin" 7> "strict-origin-when-cross-origin" 8> "unsafe-url"')
+            self.policystring = ', '.join(Option['Referrer-Policy'])
         else:
             raise SyntaxError('Referrer-Policy has 8 options 1> "no-referrer" 2> "no-referrer-when-downgrade" 3> "origin" 4> "origin-when-cross-origin" 5> "same-origin" 6> "strict-origin" 7> "strict-origin-when-cross-origin" 8> "unsafe-url"')
-        return response
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_Referrer_Policy(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('Referrer-Policy', self.policystring)
+
+            await send(message)
+
+        await self.app(scope, receive, set_Referrer_Policy)
```

### Comparing `Secweb-1.6.0/src/Secweb/StrictTransportSecurity/StrictTransportSecurityMiddleware.py` & `Secweb-1.7.1/src/Secweb/CrossOriginResourcePolicy/CrossOriginResourcePolicyMiddleware.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,37 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
+class CrossOriginResourcePolicy:
+    ''' CrossOriginResourcePolicy class sets Cross-Origin-Resource-Policy header it takes one Parameter
 
-class HSTS(BaseHTTPMiddleware):
-    ''' HSTS class sets Strict-Transport-Security Header it takes one parameter
+    Example:
+        app.add_middleware(CrossOriginResourcePolicy, Option={})
 
-    Example :
-        app.add_middleware(HSTS, Option={})
-
-    Parameter :
+    Parameter:
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'max-age': 432000, 'includeSubDomains': True, 'preload': False}) -> None:
-        super().__init__(app)
+    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'Cross-Origin-Resource-Policy': 'cross-origin'}):
+        self.app = app
         self.Option = Option
-        self.PolicyString = ''
+        Policies = ['same-site', 'same-origin', 'cross-origin']
+        if self.Option['Cross-Origin-Resource-Policy'] not in Policies:
+            raise SyntaxError('Cross-Origin-Resource-Policy has 3 options 1> "same-site" 2> "same-origin" 3> "cross-origin"')
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_Cross_Origin_Resource_Policy(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('Cross-Origin-Resource-Policy', self.Option['Cross-Origin-Resource-Policy'])
+
+            await send(message)
 
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        self.PolicyString = ''
-        response = await call_next(request)
-        if 'max-age' in self.Option:
-            if int(self.Option['max-age']) and self.Option['max-age'] > 0:
-                self.PolicyString += 'max-age=' + str(self.Option['max-age'])
-            else:
-                raise SyntaxError('max-age needs to be a positive integer')
-
-            try:
-                if self.Option['includeSubDomains'] is not False:
-                    self.PolicyString += '; includeSubDomains'
-            except KeyError:
-                self.PolicyString += '; includeSubDomains'
-
-            if 'preload' in self.Option and self.Option['preload'] is True:
-                self.PolicyString += '; preload'
-
-            response.headers['Strict-Transport-Security'] = self.PolicyString
-
-        else:
-            raise SyntaxError(
-                'Strict-Transport-Security has 3 options 1> "max-age=<expire-time>" <- This is the compulsory option 2> "includeSubDomains" 3> "preload"')
-        return response
+        await self.app(scope, receive, set_Cross_Origin_Resource_Policy)
```

### Comparing `Secweb-1.6.0/src/Secweb/XDownloadOptions/XDownloadOptionsMiddleware.py` & `Secweb-1.7.1/src/Secweb/XDownloadOptions/XDownloadOptionsMiddleware.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-
-class XDownloadOptions(BaseHTTPMiddleware):
+class XDownloadOptions:
     ''' XDownloadOptions sets the X-Download-Options header it takes no parameter
 
     Example :
         app.add_middleware(XDownloadOptions)'''
+    def __init__(self, app: ASGIApp):
+        self.app = app
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_x_Download_Options(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('X-Download-Options', 'noopen')
+
+            await send(message)
 
-    def __init__(self, app: ASGIApp) -> None:
-        super().__init__(app)
-        pass
-
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        response = await call_next(request)
-        response.headers['X-Download-Options'] = 'noopen'
-        return response
+        await self.app(scope, receive, set_x_Download_Options)
```

### Comparing `Secweb-1.6.0/src/Secweb/XFrameOptions/XFrameOptionsMiddleware.py` & `Secweb-1.7.1/src/Secweb/xXSSProtection/xXSSProtectionMiddleware.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-
-class XFrame(BaseHTTPMiddleware):
-    ''' XFrame class sets X-Frame-Options header it takes one Parameter
+class xXSSProtection:
+    ''' xXSSProtection class sets X-XSS-Protection header it takes one Parameter
 
     Example:
-        app.add_middleware(XFrame, Option={})
+        app.add_middleware(xXSSProtection, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'X-Frame-Options': 'DENY'}) -> None:
-        super().__init__(app)
+    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'X-XSS-Protection': '0'}):
+        self.app = app
         self.Option = Option
+        if self.Option['X-XSS-Protection'] != '0' and self.Option['X-XSS-Protection'] != '1' and self.Option['X-XSS-Protection'] != '1; mode=block' and '1; report=' not in self.Option['X-XSS-Protection']:
+            raise SyntaxError('X-XSS-Protection has 4 options 1> "0" 2> "1" 3> "1; mode=block" 4> "1; report=<Your Reporting Uri>"')
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_x_XSS_Protection(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('X-XSS-Protection', self.Option['X-XSS-Protection'])
+
+            await send(message)
 
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        response = await call_next(request)
-        if self.Option['X-Frame-Options'] == 'SAMEORIGIN' or self.Option['X-Frame-Options'] == 'DENY':
-            response.headers['X-Frame-Options'] = self.Option['X-Frame-Options']
-        else:
-            raise SyntaxError(
-                'X-Frame-Options has two values only 1> "DENY" 2> "SAMEORIGIN"')
-        return response
+        await self.app(scope, receive, set_x_XSS_Protection)
```

### Comparing `Secweb-1.6.0/src/Secweb/XPermittedCrossDomainPolicies/XPermittedCrossDomainPoliciesMiddleware.py` & `Secweb-1.7.1/src/Secweb/XPermittedCrossDomainPolicies/XPermittedCrossDomainPoliciesMiddleware.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from starlette.requests import Request
-from starlette.responses import Response
-from starlette.types import ASGIApp
+from starlette.types import Scope, Receive, Send, ASGIApp, Message
+from starlette.datastructures import MutableHeaders
 
-
-class XPermittedCrossDomainPolicies(BaseHTTPMiddleware):
+class XPermittedCrossDomainPolicies:
     ''' XPermittedCrossDomainPolicies class sets X-Permitted-Cross-Domain-Policies header it takes one Parameter
 
     Example:
         app.add_middleware(XPermittedCrossDomainPolicies, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-
-    def __init__(self, app: ASGIApp, Option: dict = {'X-Permitted-Cross-Domain-Policies': 'none'}) -> None:
-        super().__init__(app)
+    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'X-Permitted-Cross-Domain-Policies': 'none'}):
+        self.app = app
         self.Option = Option
-        self.Policies = ['none', 'master-only', 'by-content-type', 'all']
+        Policies = ['none', 'master-only', 'by-content-type', 'all']
+        if self.Option['X-Permitted-Cross-Domain-Policies'] not in Policies:
+            raise SyntaxError('X-Permitted-Cross-Domain-Policies has four values 1> "none" 2> "master-only" 3> "by-content-type" 4> "all"')
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
+
+        async def set_x_Permitted_Cross_Domain_Policies(message: Message):
+            if message["type"] == "http.response.start":
+                headers = MutableHeaders(scope=message)
+                headers.append('X-Permitted-Cross-Domain-Policies', self.Option['X-Permitted-Cross-Domain-Policies'])
+
+            await send(message)
 
-    async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        response = await call_next(request)
-        if self.Option['X-Permitted-Cross-Domain-Policies'] in self.Policies:
-            response.headers['X-Permitted-Cross-Domain-Policies'] = self.Option['X-Permitted-Cross-Domain-Policies']
-        else:
-            raise SyntaxError(
-                'X-Permitted-Cross-Domain-Policies has four values 1> "none" 2> "master-only" 3> "by-content-type" 4> "all"')
-        return response
+        await self.app(scope, receive, set_x_Permitted_Cross_Domain_Policies)
```

### Comparing `Secweb-1.6.0/src/Secweb/index.py` & `Secweb-1.7.1/src/Secweb/index.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-  Copyright 2021-2022, Motagamwala Taha Arif Ali '''
+  Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
 from starlette.types import ASGIApp
 
 from .XFrameOptions.XFrameOptionsMiddleware import XFrame
 from .CrossOriginEmbedderPolicy.CrossOriginEmbedderPolicyMiddleware import CrossOriginEmbedderPolicy
 from .CrossOriginOpenerPolicy.CrossOriginOpenerPolicyMiddleware import CrossOriginOpenerPolicy
 from .CrossOriginResourcePolicy.CrossOriginResourcePolicyMiddleware import CrossOriginResourcePolicy
@@ -20,31 +20,31 @@
 from .OriginAgentCluster.OriginAgentClusterMiddleware import OriginAgentCluster
 from .ExpectCt.ExpectCtMiddleware import ExpectCt
 from .ContentSecurityPolicy.ContentSecurityPolicyMiddleware import ContentSecurityPolicy
 from .ClearSiteData.ClearSiteDataMiddleware import ClearSiteData
 from .CacheControl.CacheControlMiddleware import CacheControl
 
 
-class SecWeb():
-    ''' This Class is used for initializing all the middlewares CSP, ExceptCt, etc
+class SecWeb:
+    """This Class is used for initializing all the middlewares CSP, ExceptCt, etc
 
     Example :
         SecWeb(app=app, Option={'csp': {'default-src': ["'self'"]}}, Routes=[], script_nonce=False, style_nonce=False)
 
     Parameters :
 
      app=YourappName This is the compulsory parameter
 
      Option={} This is a dictionary and not compulsory option
 
      Routes=[] This is a list of routes for Clear-Site-Data header and a compulsory option if you want to use the header
 
-     script_nonce=False This is an optional flag it will set nonce for your inline Js script
+     script_nonce=False This is an optional flag it will set nonce for your JS script
 
-     style_nonce=False This is an optional flag it will set the nonce for your inline css
+     style_nonce=False This is an optional flag it will set the nonce for your CSS stylesheet
 
     Values :
         'csp' for ContentSecurityPolicy
 
         'coop' for CrossOriginOpenerPolicy
 
         'coep' for CrossOriginEmbedderPolicy
@@ -65,100 +65,98 @@
 
         'xframe' for XFrame
 
         'clearSiteData' for Clear-Site-Data
 
         'cacheControl' for Cache-Control
 
-    This Values are for Option parameter'''
+    This Values are for Option parameter"""
 
-    def __init__(self, app: ASGIApp, Option: dict = {}, Routes: list = [], script_nonce: bool = False, style_nonce: bool = False) -> None:
+    def __init__(
+        self,
+        app: ASGIApp,
+        Option: dict[str, dict[str, list[str] | str | bool | int]] = {},
+        Routes: list[str] = [],
+        script_nonce: bool = False,
+        style_nonce: bool = False,
+    ) -> None:
         if not Option:
             app.add_middleware(XFrame)
             app.add_middleware(xXSSProtection)
             app.add_middleware(HSTS)
             app.add_middleware(XPermittedCrossDomainPolicies)
             app.add_middleware(XDownloadOptions)
             app.add_middleware(XDNSPrefetchControl)
             app.add_middleware(XContentTypeOptions)
             app.add_middleware(ReferrerPolicy)
             app.add_middleware(OriginAgentCluster)
-            app.add_middleware(
-                ContentSecurityPolicy, script_nonce=script_nonce, style_nonce=style_nonce)
+            app.add_middleware(ContentSecurityPolicy,script_nonce=script_nonce,style_nonce=style_nonce)
             app.add_middleware(CacheControl)
             app.add_middleware(CrossOriginEmbedderPolicy)
             app.add_middleware(CrossOriginOpenerPolicy)
             if Routes.__len__() > 0:
                 app.add_middleware(ClearSiteData, Routes=Routes)
         else:
             app.add_middleware(XDownloadOptions)
             app.add_middleware(XContentTypeOptions)
             app.add_middleware(OriginAgentCluster)
 
-            if 'csp' in Option.keys():
-                app.add_middleware(
-                    ContentSecurityPolicy, Option=Option['csp'], script_nonce=script_nonce, style_nonce=style_nonce)
-            else:
-                app.add_middleware(
-                    ContentSecurityPolicy, script_nonce=script_nonce, style_nonce=style_nonce)
-
-            if 'coop' in Option.keys():
-                app.add_middleware(CrossOriginOpenerPolicy,
-                                   Option=Option['coop'])
+            if "csp" in Option.keys():
+                app.add_middleware(ContentSecurityPolicy,Option=Option["csp"],script_nonce=script_nonce,style_nonce=style_nonce,)
+            else:
+                app.add_middleware(ContentSecurityPolicy,script_nonce=script_nonce,style_nonce=style_nonce)
+
+            if "coop" in Option.keys():
+                app.add_middleware(CrossOriginOpenerPolicy, Option=Option["coop"])
             else:
                 app.add_middleware(CrossOriginOpenerPolicy)
 
-            if 'coep' in Option.keys():
-                app.add_middleware(CrossOriginEmbedderPolicy,
-                                   Option=Option['coep'])
+            if "coep" in Option.keys():
+                app.add_middleware(CrossOriginEmbedderPolicy, Option=Option["coep"])
             else:
                 app.add_middleware(CrossOriginEmbedderPolicy)
 
-            if 'corp' in Option.keys():
-                app.add_middleware(CrossOriginResourcePolicy,
-                                   Option=Option['corp'])
+            if "corp" in Option.keys():
+                app.add_middleware(CrossOriginResourcePolicy, Option=Option["corp"])
 
-            if 'expectCt' in Option.keys():
-                app.add_middleware(ExpectCt, Option=Option['expectCt'])
+            if "expectCt" in Option.keys():
+                app.add_middleware(ExpectCt, Option=Option["expectCt"])
 
-            if 'referrer' in Option.keys():
-                app.add_middleware(ReferrerPolicy, Option=Option['referrer'])
+            if "referrer" in Option.keys():
+                app.add_middleware(ReferrerPolicy, Option=Option["referrer"])
             else:
                 app.add_middleware(ReferrerPolicy)
 
-            if 'xdns' in Option.keys():
-                app.add_middleware(XDNSPrefetchControl, Option=Option['xdns'])
+            if "xdns" in Option.keys():
+                app.add_middleware(XDNSPrefetchControl, Option=Option["xdns"])
             else:
                 app.add_middleware(XDNSPrefetchControl)
 
-            if 'xcdp' in Option.keys():
-                app.add_middleware(
-                    XPermittedCrossDomainPolicies, Option=Option['xcdp'])
+            if "xcdp" in Option.keys():
+                app.add_middleware(XPermittedCrossDomainPolicies, Option=Option["xcdp"])
             else:
                 app.add_middleware(XPermittedCrossDomainPolicies)
 
-            if 'hsts' in Option.keys():
-                app.add_middleware(HSTS, Option=Option['hsts'])
+            if "hsts" in Option.keys():
+                app.add_middleware(HSTS, Option=Option["hsts"])
             else:
                 app.add_middleware(HSTS)
 
-            if 'xss' in Option.keys():
-                app.add_middleware(xXSSProtection, Option=Option['xss'])
+            if "xss" in Option.keys():
+                app.add_middleware(xXSSProtection, Option=Option["xss"])
             else:
                 app.add_middleware(xXSSProtection)
 
-            if 'xframe' in Option.keys():
-                app.add_middleware(XFrame, Option=Option['xframe'])
+            if "xframe" in Option.keys():
+                app.add_middleware(XFrame, Option=Option["xframe"])
             else:
                 app.add_middleware(XFrame)
 
-            if 'clearSiteData' in Option.keys() and Routes.__len__() > 0:
-                app.add_middleware(
-                    ClearSiteData, Option=Option['clearSiteData'], Routes=Routes)
-
-            if Routes.__len__() > 0:
+            if "clearSiteData" in Option.keys() and Routes.__len__() > 0:
+                app.add_middleware(ClearSiteData, Option=Option["clearSiteData"], Routes=Routes)
+            elif Routes.__len__() > 0:
                 app.add_middleware(ClearSiteData, Routes=Routes)
 
-            if 'cacheControl' in Option.keys():
-                app.add_middleware(CacheControl, Option=Option['cacheControl'])
+            if "cacheControl" in Option.keys():
+                app.add_middleware(CacheControl, Option=Option["cacheControl"])
             else:
                 app.add_middleware(CacheControl)
```

### Comparing `Secweb-1.6.0/src/Secweb.egg-info/PKG-INFO` & `Secweb-1.7.1/src/Secweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: Secweb
-Version: 1.6.0
-Summary: Secweb is a pack of security middlewares for fastApi and starlette servers it includes CSP, HSTS, and many more
-Home-page: https://github.com/tmotagam/Secweb
-Author: Motagamwala Taha Arif Ali
-Author-email: tahaar5321@gmail.com
+Version: 1.7.1
+Summary: Secweb is a pack of security middlewares for fastApi and starlette server it includes CSP, HSTS, and many more
+Author-email: Motagamwala Taha Arif Ali <tahaar5321@gmail.com>
+Project-URL: Homepage, https://github.com/tmotagam/Secweb
 Project-URL: Bug Tracker, https://github.com/tmotagam/Secweb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
@@ -18,15 +17,17 @@
 <p align = "center"><img alt="Secweb logo" src="https://raw.githubusercontent.com/tmotagam/Secweb/main/Secweb.jpg"></p>
 
 <p align="center"><em>Secweb helps in setting security headers for FastApi and Starlette</em></p>
 
 ---
 <br>
 
-Secweb is the pack of middlewares for setting security headers for fastapi and can also be used for any framework created on starlette it has 16 middlewares for setting headers of your website and also for your api`s
+Secweb is the pack of middlewares for setting security headers for fastapi and can also be used for any framework created on starlette it has 16 middlewares for setting headers of your website and also for your api(s)
+
+Now all the middlewares are pure ASGI implemented middlewares and from now on all the release will have sigstore signatures you can get them from the github release for both dev and production Secweb.
 
 #### The PermissionsPolicy middleware lies in development branch [here](https://github.com/tmotagam/Secweb/tree/Secweb-Beta#readme)
 
 The list of middleware is as follows:
 
 1. Content Security Policy (CSP)
 
@@ -164,15 +165,15 @@
 12. `'clearSiteData'` for calling ClearSiteData class to set the user-defined values
 <br>
 
 13. `'cacheControl'` for calling CacheControl class to set the user-defined values
 
 ```python
 # Example of the values
-SecWeb(app=app, Option={'csp': {'default-src': ["'self'"]}, 'xframe': {'X-Frame-Options': 'SAMEORIGIN'}, 'xss': {'X-XSS-Protection': '1; mode=block'}, 'hsts': {'max-age': 4, 'preload': True}, 'xcdp': {'X-Permitted-Cross-Domain-Policies': 'all'}, 'xdns': {'X-DNS-Prefetch-Control': 'on'}, 'referrer': {'Referrer-Policy': 'no-referrer'}, 'expectCt': {'max-age': 128, 'enforce': True, 'report-uri': "https://example.com/example"}, 'coep': {'Cross-Origin-Embedder-Policy': 'require-corp'}, 'coop': {'Cross-Origin-Opener-Policy': 'same-origin-allow-popups'}, 'corp': {'Cross-Origin-Resource-Policy': 'same-site'}, 'clearSiteData': {'cache': True, 'storage': True}, 'cacheControl': {'public': True, 's-maxage': 600}}, Routes=['/login', '/logout/{id}'])
+SecWeb(app=app, Option={'csp': {'default-src': ["'self'"]}, 'xframe': {'X-Frame-Options': 'SAMEORIGIN'}, 'xss': {'X-XSS-Protection': '1; mode=block'}, 'hsts': {'max-age': 4, 'preload': True}, 'xcdp': {'X-Permitted-Cross-Domain-Policies': 'all'}, 'xdns': {'X-DNS-Prefetch-Control': 'on'}, 'referrer': {'Referrer-Policy': 'no-referrer'}, 'expectCt': {'max-age': 128, 'enforce': True, 'report-uri': "https://example.com/example"}, 'coep': {'Cross-Origin-Embedder-Policy': 'require-corp'}, 'coop': {'Cross-Origin-Opener-Policy': 'same-origin-allow-popups'}, 'corp': {'Cross-Origin-Resource-Policy': 'same-site'}, 'clearSiteData': {'cache': True, 'storage': True}, 'cacheControl': {'public': True, 's-maxage': 600}}, Routes=['/login/{id}', '/logout/{id:uuid}/username/{username:string}'])
 ```
 ### Middleware Classes
 
 #### Content Security Policy (CSP)
 
 ContentSecurityPolicy class sets the csp header
 
@@ -384,15 +385,14 @@
 from starlette.applications import Starlette
 from Secweb.XDownloadOptions import XDownloadOptions
 
 app = Starlette()
 
 app.add_middleware(XDownloadOptions)
 ```
-For more detail on X-Download-Options header go to this [NWebsec Site](https://www.nwebsec.com/HttpHeaders/SecurityHeaders/XDownloadOptions)
 
 #### X-Frame
 
 XFrame class sets the X-Frame-Options header
 
 ```python
 from fastapi import FastAPI
@@ -582,8 +582,8 @@
 [Github](https://github.com/tmotagam/Secweb)
 
 ## License
 [MLP 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
 
 ## Secweb Icon
 
-[Secweb Icon](https://github.com/tmotagam/Secweb/blob/main/Secweb.jpg) © 2021 - 2022 by [Motagamwala Taha Arif Ali](https://github.com/tmotagam) is licensed under [Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1)
+[Secweb Icon](https://github.com/tmotagam/Secweb/blob/main/Secweb.jpg) © 2021 - 2023 by [Motagamwala Taha Arif Ali](https://github.com/tmotagam) is licensed under [Attribution-NonCommercial-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1)
```

### Comparing `Secweb-1.6.0/src/Secweb.egg-info/SOURCES.txt` & `Secweb-1.7.1/src/Secweb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 src/Secweb/__init__.py
 src/Secweb/index.py
 src/Secweb.egg-info/PKG-INFO
 src/Secweb.egg-info/SOURCES.txt
 src/Secweb.egg-info/dependency_links.txt
 src/Secweb.egg-info/top_level.txt
 src/Secweb/CacheControl/CacheControlMiddleware.py
```

