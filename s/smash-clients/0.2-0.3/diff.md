# Comparing `tmp/smash-clients-0.2.tar.gz` & `tmp/smash-clients-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smash-clients-0.2.tar", last modified: Tue Feb 21 05:44:14 2023, max compression
+gzip compressed data, was "smash-clients-0.3.tar", last modified: Mon Jun 12 07:57:46 2023, max compression
```

## Comparing `smash-clients-0.2.tar` & `smash-clients-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Drew       (501) staff       (20)        0 2023-02-21 05:44:14.100742 smash-clients-0.2/
--rw-r--r--   0 Drew       (501) staff       (20)      954 2023-02-21 05:44:14.100037 smash-clients-0.2/PKG-INFO
--rw-r--r--   0 Drew       (501) staff       (20)      716 2023-01-07 05:23:31.000000 smash-clients-0.2/README.md
--rw-r--r--   0 Drew       (501) staff       (20)       38 2023-02-21 05:44:14.100921 smash-clients-0.2/setup.cfg
--rw-r--r--   0 Drew       (501) staff       (20)      826 2023-01-16 09:10:55.000000 smash-clients-0.2/setup.py
-drwxr-xr-x   0 Drew       (501) staff       (20)        0 2023-02-21 05:44:14.095153 smash-clients-0.2/smash/
--rw-r--r--   0 Drew       (501) staff       (20)        0 2022-12-06 06:54:57.000000 smash-clients-0.2/smash/__init__.py
--rw-r--r--   0 Drew       (501) staff       (20)      139 2023-01-16 08:19:42.000000 smash-clients-0.2/smash/__main__.py
--rw-r--r--   0 Drew       (501) staff       (20)     2296 2023-02-18 21:11:56.000000 smash-clients-0.2/smash/cli.py
--rw-r--r--   0 Drew       (501) staff       (20)     5389 2023-02-18 18:59:36.000000 smash-clients-0.2/smash/config.py
--rwxr-xr-x   0 Drew       (501) staff       (20)     5249 2023-02-21 05:37:54.000000 smash-clients-0.2/smash/smash.py
--rw-r--r--   0 Drew       (501) staff       (20)       68 2023-02-21 05:43:17.000000 smash-clients-0.2/smash/version.py
--rw-r--r--   0 Drew       (501) staff       (20)     2482 2023-02-21 02:03:35.000000 smash-clients-0.2/smash/xbar.py
-drwxr-xr-x   0 Drew       (501) staff       (20)        0 2023-02-21 05:44:14.099342 smash-clients-0.2/smash_clients.egg-info/
--rw-r--r--   0 Drew       (501) staff       (20)      954 2023-02-21 05:44:14.000000 smash-clients-0.2/smash_clients.egg-info/PKG-INFO
--rw-r--r--   0 Drew       (501) staff       (20)      353 2023-02-21 05:44:14.000000 smash-clients-0.2/smash_clients.egg-info/SOURCES.txt
--rw-r--r--   0 Drew       (501) staff       (20)        1 2023-02-21 05:44:14.000000 smash-clients-0.2/smash_clients.egg-info/dependency_links.txt
--rw-r--r--   0 Drew       (501) staff       (20)       70 2023-02-21 05:44:14.000000 smash-clients-0.2/smash_clients.egg-info/entry_points.txt
--rw-r--r--   0 Drew       (501) staff       (20)       25 2023-02-21 05:44:14.000000 smash-clients-0.2/smash_clients.egg-info/requires.txt
--rw-r--r--   0 Drew       (501) staff       (20)        6 2023-02-21 05:44:14.000000 smash-clients-0.2/smash_clients.egg-info/top_level.txt
+drwxr-xr-x   0 Drew       (501) staff       (20)        0 2023-06-12 07:57:46.623346 smash-clients-0.3/
+-rw-r--r--   0 Drew       (501) staff       (20)      928 2023-06-12 07:57:46.622886 smash-clients-0.3/PKG-INFO
+-rw-r--r--   0 Drew       (501) staff       (20)      690 2023-06-09 16:35:52.000000 smash-clients-0.3/README.md
+-rw-r--r--   0 Drew       (501) staff       (20)       38 2023-06-12 07:57:46.623477 smash-clients-0.3/setup.cfg
+-rw-r--r--   0 Drew       (501) staff       (20)      826 2023-06-12 07:53:49.000000 smash-clients-0.3/setup.py
+drwxr-xr-x   0 Drew       (501) staff       (20)        0 2023-06-12 07:57:46.618916 smash-clients-0.3/smash/
+-rw-r--r--   0 Drew       (501) staff       (20)        0 2023-06-12 07:56:16.000000 smash-clients-0.3/smash/__init__.py
+-rw-r--r--   0 Drew       (501) staff       (20)      139 2023-01-16 08:19:42.000000 smash-clients-0.3/smash/__main__.py
+-rw-r--r--   0 Drew       (501) staff       (20)     2392 2023-06-12 07:05:15.000000 smash-clients-0.3/smash/cli.py
+-rw-r--r--   0 Drew       (501) staff       (20)     5389 2023-06-09 16:40:59.000000 smash-clients-0.3/smash/config.py
+-rwxr-xr-x   0 Drew       (501) staff       (20)     6203 2023-06-12 07:39:48.000000 smash-clients-0.3/smash/smash.py
+-rw-r--r--   0 Drew       (501) staff       (20)       68 2023-06-12 07:56:19.000000 smash-clients-0.3/smash/version.py
+-rw-r--r--   0 Drew       (501) staff       (20)     4454 2023-06-12 07:19:44.000000 smash-clients-0.3/smash/xbar.py
+drwxr-xr-x   0 Drew       (501) staff       (20)        0 2023-06-12 07:57:46.622255 smash-clients-0.3/smash_clients.egg-info/
+-rw-r--r--   0 Drew       (501) staff       (20)      928 2023-06-12 07:57:46.000000 smash-clients-0.3/smash_clients.egg-info/PKG-INFO
+-rw-r--r--   0 Drew       (501) staff       (20)      353 2023-06-12 07:57:46.000000 smash-clients-0.3/smash_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 Drew       (501) staff       (20)        1 2023-06-12 07:57:46.000000 smash-clients-0.3/smash_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 Drew       (501) staff       (20)       70 2023-06-12 07:57:46.000000 smash-clients-0.3/smash_clients.egg-info/entry_points.txt
+-rw-r--r--   0 Drew       (501) staff       (20)       25 2023-06-12 07:57:46.000000 smash-clients-0.3/smash_clients.egg-info/requires.txt
+-rw-r--r--   0 Drew       (501) staff       (20)        6 2023-06-12 07:57:46.000000 smash-clients-0.3/smash_clients.egg-info/top_level.txt
```

### Comparing `smash-clients-0.2/README.md` & `smash-clients-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,33 @@
+Metadata-Version: 2.1
+Name: smash-clients
+Version: 0.3
+Summary: Smash clients
+Home-page: https://p0nk.net/smash
+Author: dlek
+Author-email: dlek@p0nk.net
+License: MIT license
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # SMASH client
 
 Local Python clients for Smash.  And maybe a library you can use with them or
 something, idk.
 
 ## SMASH xbar
 
 The SMASH xbar client works with [xbar](https://xbarapp.com/) to provide
-near-realtime information on node and service status in your Mac menu bar.
-(xbar is a fantastic app--I use it for several things).
+current information on node and service status in your Mac menu bar.
 
 ## SMASH CLI client
 
 The CLI client provides a command-line interface to the Smash API.
 
+```
 smash register node	# wait isn't this done by the agent?  Did I mean
 			# something else?  Otherwise what's the use case for
 			# providing this functionality here?
 smash get node[:status]
-smash delete node[:status] [ node[:status] ... ]
+smash delete node[:status] [ node[:status] ... ]   ### NOT IMPLEMENTED sorry
 smash ack[nowledge] node:status [-x expires when] message
+```
```

### Comparing `smash-clients-0.2/setup.py` & `smash-clients-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `smash-clients-0.2/smash/cli.py` & `smash-clients-0.3/smash/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# pylint:
+# pylint: disable=too-many-branches
+#   This is fine.
 #
 """
 Smash command-line interface client.
 """
+import json
 from smash import config
 from smash import smash
 
 
 def json_result(result):
     """ Print result as JSON. """
-    print("<< JSON result >>")
     print(result)
 
 
 def json_error(errmsg):
     """ Print error as JSON. """
     print(f'"error":"{errmsg}"')
 
 
 def print_result(result):
     """ Print result as text. """
-    # DO something different
-    print("<< plaintext result >>")
-    print(result)
+    print(json.dumps(result, indent=2))
 
 
 def print_error(errmsg):
     """ Print error as text. """
     print(f"Error: {errmsg}")
 
 
@@ -41,54 +40,56 @@
         conf.merge()
     except Exception as e:
         print(f"Could not load Smash configuration: {e}")
         return
 
     api = smash.ApiHandler(conf)
 
-    print(f"Args: {vars(args)}")
-
     # for collecting output and result
     output = None
 
     # DO put this next section in a try..except thingy (maybe)
     # the idea being to capture any exceptions and output them appropriately
 
     # handle command
     if args.cmd == 'get':
 
         output = []
-        for ns in args.nodestatus:
-            if ns[1]:
-                output.append(api.get_node_status(ns[0], ns[1]))
-            else:
-                output.append(api.get_node(ns[0]))
+        if args.nodestatus:
+            for ns in args.nodestatus:
+                if ns[1]:
+                    output.append(api.get_node_status(ns[0], ns[1]))
+                else:
+                    output.append(api.get_node(ns[0]))
+        else:
+            output.append(api.get_all_status())
 
-#    elif args.cmd in ['del, 'delete']:
+# Delete operation not yet supported--requires authentication
+#    elif args.cmd in ['del', 'delete']:
 #
-#        node = args.nodestatus[0]
-#        status = args.nodestatus[1]
-#        if node and status:
-#            output = api.delete_node_status(node, status)
-#        elif node:
-#            output = api.delete_node(node)
+#        output = []
+#        for ns in args.nodestatus:
+#            if ns[1]:
+#                output.append(api.delete_node_status(ns[0], ns[1]))
+#            else:
+#                output.append(api.delete_node(ns[0]))
 
     elif args.cmd in ['ack', 'acknowledge']:
         output = api.acknowledge(args.nodestatus[0], args.nodestatus[1],
             args.message, args.state, args.expire_after)
 
     else:
         print_error(f"Not recognized: command {args.cmd}")
 
     # handle output
     if not output:
         if args.json:
-            json_error(f"This sucks: {args.cmd} unsuccessful")
+            json_error(f"{args.cmd} unsuccessful")
         else:
-            print_error(f"This sucks: {args.cmd} unsuccessful")
+            print_error(f"{args.cmd} unsuccessful")
     else:
         if args.json:
             json_result(output)
         else:
             print_result(output)
```

### Comparing `smash-clients-0.2/smash/config.py` & `smash-clients-0.3/smash/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     conf.config_argparser(conf.argparser)
     parsers = conf.argparser.add_subparsers(
         help='CLI command help', dest='cmd', required=True
     )
 
     # get command
     get_parser = parsers.add_parser('get', help='Get node status')
-    get_parser.add_argument('nodestatus', type=str, nargs='+',
+    get_parser.add_argument('nodestatus', type=str, nargs='*',
         help='nodes and/or node-status pairs to retrieve',
         metavar='node[:status]',
         action=NodeMaybeStatusSplitAction)
 
     # delete command
     delete_parser = parsers.add_parser('delete', aliases=['del'],
         help='Delete node or status')
```

### Comparing `smash-clients-0.2/smash/smash.py` & `smash-clients-0.3/smash/smash.py`

 * *Files 15% similar despite different names*

```diff
@@ -65,14 +65,18 @@
         overall = overall or 'okay'
     if summary_parts:
         summary = " ".join(summary_parts) + f" of {totals['all']}"
     else:
         summary = f"All {totals['all']} ok"
     return(overall, summary)
 
+# TODO: Make this unit-testable, so given the JSON, interpret the objects
+#   With whatever mechanism uses `yield()`, create function that takes the
+#   URL and creates the node objects
+# TODO: simplify with new /status/ API call
 def load_nodes(api_url, timeout):
     """ Loads nodes from Smash server and their statuses.
     """
     nodes = requests.get(api_url + '/nodes/', timeout=timeout).json()
     for node in nodes:
 
         node['totals'] = {
@@ -167,14 +171,23 @@
         # request status
         status = requests.get(
             f"{self._api_url}/nodes/{node}/status/{status}", timeout=self._timeout
         ).json()
 
         return status
 
+    def get_all_status(self):
+        """
+        Retrieve all current status.
+        """
+
+        return requests.get(
+            f"{self._api_url}/", timeout=self._timeout
+        ).json()
+
     def acknowledge(self, node, status, message=None, state=None, expiry=None):
         """
         Acknowledge a particular status on a node.
         """
 
         result = requests.put(
             f"{self._api_url}/nodes/{node}/status/{status}/acknowledgement",
@@ -183,7 +196,31 @@
                 'message': message,
                 'state': state,
                 'expiry': expiry
             }
         ).json()
 
         return result
+
+    def delete_node(self, node):
+        """
+        Delete a node.
+        """
+
+        result = requests.delete(
+            f"{self._api_url}/nodes/{node}",
+            timeout=self._timeout
+        ).json()
+
+        return result
+
+    def delete_node_status(self, node, status):
+        """
+        Delete the given status for the given node.
+        """
+
+        result = requests.delete(
+            f"{self._api_url}/nodes/{node}/status/{status}",
+            timeout=self._timeout
+        ).json()
+
+        return result
```

