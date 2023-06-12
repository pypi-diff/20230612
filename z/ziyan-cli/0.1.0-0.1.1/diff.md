# Comparing `tmp/ziyan_cli-0.1.0.tar.gz` & `tmp/ziyan_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziyan_cli-0.1.0.tar", max compression
+gzip compressed data, was "ziyan_cli-0.1.1.tar", max compression
```

## Comparing `ziyan_cli-0.1.0.tar` & `ziyan_cli-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      298 2023-06-12 01:38:41.457310 ziyan_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1376 2023-06-12 01:39:07.783563 ziyan_cli-0.1.0/ziyan_cli/__init__.py
--rw-r--r--   0        0        0      495 2023-06-12 01:39:13.168962 ziyan_cli-0.1.0/setup.py
--rw-r--r--   0        0        0      242 2023-06-12 01:39:13.169240 ziyan_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      298 2023-06-12 02:26:18.024347 ziyan_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1228 2023-06-12 02:22:52.722636 ziyan_cli-0.1.1/ziyan_cli/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-12 02:26:27.484438 ziyan_cli-0.1.1/setup.py
+-rw-r--r--   0        0        0      242 2023-06-12 02:26:27.484703 ziyan_cli-0.1.1/PKG-INFO
```

### Comparing `ziyan_cli-0.1.0/ziyan_cli/__init__.py` & `ziyan_cli-0.1.1/ziyan_cli/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 __version__ = '0.1.0'
+
+
 def update_variables(vars_dict):
-    def update_var(var_name, value):
-        # Function to update the value of a variable
-        vars_dict[var_name] = value
-
-    def confirm():
-        # Function to ask for confirmation
-        confirm_input = input("Are you sure you want to update the variable? (yes/no): ").lower()
-        while confirm_input not in ["yes", "no"]:
-            print("Invalid input, please enter 'yes' or 'no'.")
-            confirm_input = input("Are you sure you want to update the variable? (yes/no): ").lower()
-        
-        if confirm_input == 'yes':
-            return True
-        else:
-            return False
-
-    while True:
-        print("Current values:")
-        for k, v in vars_dict.items():
-            print(f"{k}: {v}")
-        
-        var_name = input("Which variable do you want to update? Or type 'exit' to quit: ")
-        
-        if var_name.lower() == 'exit':
-            break
-        
-        if var_name in vars_dict:
-            new_value = input(f"Enter a new value for {var_name}: ")
-            
-            if confirm():
-                update_var(var_name, new_value)
-                print(f"{var_name} updated successfully.\n")
-            else:
-                print(f"Update for {var_name} cancelled.\n")
-        else:
-            print(f"Variable {var_name} not found. Please try again.\n")
+
+  def update_var(var_name, value):
+    # Function to update the value of a variable
+    vars_dict[var_name] = value
+
+  def confirm():
+    # Function to ask for confirmation
+    confirm_input = input(
+      "Are you sure you want to update the variable? (yes/no): ").lower()
+    while confirm_input not in ["yes", "no"]:
+      print("Invalid input, please enter 'yes' or 'no'.")
+      confirm_input = input(
+        "Are you sure you want to update the variable? (yes/no): ").lower()
+
+    if confirm_input == 'yes':
+      return True
+    else:
+      return False
+
+  while True:
+    print("Current values:")
+    for k, v in vars_dict.items():
+      print(f"{k}: {v}")
+
+    var_name = input(
+      "Which variable do you want to update? Or type 'exit' to quit: ")
+
+    if var_name.lower() == 'exit':
+      return vars_dict
+
+    if var_name in vars_dict:
+      new_value = input(f"Enter a new value for {var_name}: ")
+
+      if confirm():
+        update_var(var_name, new_value)
+        print(f"{var_name} updated successfully.\n")
+      else:
+        print(f"Update for {var_name} cancelled.\n")
+    else:
+      print(f"Variable {var_name} not found. Please try again.\n")
```

