# Comparing `tmp/ms_salesforce_api-0.0.44.tar.gz` & `tmp/ms_salesforce_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-0.0.44.tar", max compression
+gzip compressed data, was "ms_salesforce_api-1.0.0.tar", max compression
```

## Comparing `ms_salesforce_api-0.0.44.tar` & `ms_salesforce_api-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2023-06-09 11:28:08.006216 ms_salesforce_api-0.0.44/LICENSE
--rw-r--r--   0        0        0     5635 2023-06-09 11:28:08.006216 ms_salesforce_api-0.0.44/README.md
--rw-r--r--   0        0        0        0 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2712 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2395 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3347 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15436 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     3055 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    19325 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    20653 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0     6021 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    17775 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13715 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0     1056 2023-06-09 11:28:08.010216 ms_salesforce_api-0.0.44/pyproject.toml
--rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 ms_salesforce_api-0.0.44/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5631 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2712 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2395 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3347 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15406 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     7675 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    19543 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    20551 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0     8894 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    17755 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13717 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0     1055 2023-06-12 12:27:36.533168 ms_salesforce_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 ms_salesforce_api-1.0.0/PKG-INFO
```

### Comparing `ms_salesforce_api-0.0.44/LICENSE` & `ms_salesforce_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/README.md` & `ms_salesforce_api-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 The opportunities variable will contain an array of opportunity objects with the transformed data. For example:
 
 ```python
 {
     "success": true,
     "opportunities": [
         {
-            "client_fiscal_name": "ESMProjectAcc",
-            "client_account_name": "ESMProjectAccount",
+            "account_business_name": "ESMProjectAcc",
+            "account_name": "ESMProjectAccount",
             "currency": "EUR",
             "amount": 0,
             "invoicing_country_code": "ES",
             "operation_coordinator_email": "jhon.doe@ext.makingscience.com",
             "operation_coordinator_sub_email": "jhon.doe@ext.makingscience.com",
             "created_at": "2020-07-14T12:55:56.000+0000",
             "last_updated_at": "2023-05-16T13:18:04.000+0000",
```

#### html2text {}

```diff
@@ -17,16 +17,16 @@
 project = Project( client_id="your_client_id", username="your_username",
 domain="your_domain", private_key="your_private_key", audience="https://
 login.salesforce.com", # Default value session_duration_hours=1, # Default
 value api_version='57.0', # Default value ) ``` Now, you can call the
 get_opportunities method with a query to get the opportunities data: ```python
 opportunities = project.get_opportunities() ``` The opportunities variable will
 contain an array of opportunity objects with the transformed data. For example:
-```python { "success": true, "opportunities": [ { "client_fiscal_name":
-"ESMProjectAcc", "client_account_name": "ESMProjectAccount", "currency": "EUR",
+```python { "success": true, "opportunities": [ { "account_business_name":
+"ESMProjectAcc", "account_name": "ESMProjectAccount", "currency": "EUR",
 "amount": 0, "invoicing_country_code": "ES", "operation_coordinator_email":
 "jhon.doe@ext.makingscience.com", "operation_coordinator_sub_email":
 "jhon.doe@ext.makingscience.com", "created_at": "2020-07-14T12:55:56.000+0000",
 "last_updated_at": "2023-05-16T13:18:04.000+0000", "opportunity_name":
 "ESMOPP", "stage": "Qualification", "billing_country": "ES", "lead_source":
 "Other", "project_code": "ESMSEX00430", "project_id": "a003X000015kaPxQAI",
 "project_name": "ESMProject", "project_start_date": "2023-05-13",
```

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,18 +163,18 @@
         )
         opportunities = project.get_opportunities(format="dto")
         self.assertEqual(len(opportunities), 1)
 
         opportunity = opportunities[0]
         self.assertIsInstance(opportunity, OpportunityDTO)
         self.assertEqual(
-            opportunity.client_fiscal_name,
+            opportunity.account_business_name,
             "ESMProjectAcc",
         )
-        self.assertEqual(opportunity.client_account_name, "ESMProjectAccount")
+        self.assertEqual(opportunity.account_name, "ESMProjectAccount")
         self.assertEqual(opportunity.currency, "EUR")
         self.assertEqual(opportunity.amount, 0)
         self.assertEqual(opportunity.invoicing_country_code, "ES")
         self.assertEqual(
             opportunity.operation_coordinator_email,
             "jhon.doe@ext.makingscience.com",
         )
@@ -264,20 +264,18 @@
         )
         opportunities = project.get_opportunities()
         self.assertEqual(len(opportunities), 1)
 
         opportunity = opportunities[0]
         self.assertIsInstance(opportunity, dict)
         self.assertEqual(
-            opportunity["client_fiscal_name"],
+            opportunity["account_business_name"],
             "ESMProjectAcc",
         )
-        self.assertEqual(
-            opportunity["client_account_name"], "ESMProjectAccount"
-        )
+        self.assertEqual(opportunity["account_name"], "ESMProjectAccount")
         self.assertEqual(opportunity["currency"], "EUR")
         self.assertEqual(opportunity["amount"], 0)
         self.assertEqual(opportunity["invoicing_country_code"], "ES")
         self.assertEqual(
             opportunity["operation_coordinator_email"],
             "jhon.doe@ext.makingscience.com",
         )
```

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,17 @@
     ProjectLineItemDTO,
 )
 
 
 class OpportunityDTO(object):
     def __init__(
         self,
-        client_fiscal_name,
-        client_account_name,
+        account_business_name,
+        account_name,
+        account_id,
         currency,
         amount,
         invoicing_country_code,
         operation_coordinator_email,
         operation_coordinator_sub_email,
         created_at,
         last_updated_at,
@@ -29,15 +30,15 @@
         cost_center,
         project_tier,
         jira_task_url,
         opportunity_percentage,
         account_assigment_group,
         account_tax_category,
         account_tax_classification,
-        account_txt_sapid,
+        account_sap_id,
         account_business_function,
         account_tax_id_type,
         account_currency_code,
         account_created_date,
         account_tier,
         account_pec_email,
         account_phone,
@@ -53,16 +54,17 @@
         account_payment_terms,
         account_billing_state_code,
         account_mail_invoicing,
         account_invoicing_email,
         billing_lines=[],
         project_line_items=[],
     ):
-        self.client_fiscal_name = client_fiscal_name
-        self.client_account_name = client_account_name
+        self.account_business_name = account_business_name
+        self.account_name = account_name
+        self.account_id = account_id
         self.currency = currency
         self.amount = amount
         self.invoicing_country_code = invoicing_country_code
         self.operation_coordinator_email = operation_coordinator_email
         self.operation_coordinator_sub_email = operation_coordinator_sub_email
         self.created_at = created_at
         self.last_updated_at = last_updated_at
@@ -82,15 +84,15 @@
         self.jira_task_url = jira_task_url
         self.opportunity_percentage = opportunity_percentage
         self.billing_lines = billing_lines
         self.project_line_items = project_line_items
         self.account_assigment_group = account_assigment_group
         self.account_tax_category = account_tax_category
         self.account_tax_classification = account_tax_classification
-        self.account_txt_sapid = account_txt_sapid
+        self.account_sap_id = account_sap_id
         self.account_business_function = account_business_function
         self.account_tax_id_type = account_tax_id_type
         self.account_currency_code = account_currency_code
         self.account_created_date = account_created_date
         self.account_tier = account_tier
         self.account_pec_email = account_pec_email
         self.account_phone = account_phone
@@ -114,26 +116,32 @@
             try:
                 return (
                     text.replace("\n", "").replace("\r", "").replace("'", "")
                 )
             except AttributeError:
                 return text
 
-        def _get_client_fiscal_name():
+        def _get_account_business_name():
             try:
                 return record["Project_Account__r"]["Business_Name__c"]
             except (TypeError, KeyError):
                 return ""
 
-        def _get_client_account_name():
+        def _get_account_name():
             try:
                 return record["Project_Account__r"]["Name"]
             except (TypeError, KeyError):
                 return ""
 
+        def _get_account_id():
+            try:
+                return record["Project_Account__r"]["Id"]
+            except (TypeError, KeyError):
+                return ""
+
         def _get_account_billing_country():
             try:
                 return record["Project_Account__r"]["BillingCountryCode"]
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_assigment_group():
@@ -156,15 +164,15 @@
             try:
                 return record["Project_Account__r"][
                     "MS_Customer_Tax_Classification__c"
                 ]
             except (TypeError, KeyError):
                 return ""
 
-        def _get_account_txt_sapid():
+        def _get_account_sap_id():
             try:
                 return record["Project_Account__r"]["TXT_SAPId__c"]
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_business_function():
             try:
@@ -387,16 +395,17 @@
                 )
             ]
             if record.get("Project_Line_Items__r")
             else []
         )
 
         return OpportunityDTO(
-            client_fiscal_name=_get_client_fiscal_name(),
-            client_account_name=_get_client_account_name(),
+            account_business_name=_get_account_business_name(),
+            account_name=_get_account_name(),
+            account_id=_get_account_id(),
             currency=record["CurrencyIsoCode"],
             amount=record.get("Total_Project_Amount__c", 0),
             invoicing_country_code=record["Invoicing_Country_Code__c"],
             operation_coordinator_email=_get_operation_coordinator_email(),
             operation_coordinator_sub_email=_get_operation_coordinator_sub_email(),  # noqa: E501
             created_at=record["CreatedDate"],
             last_updated_at=record["LastModifiedDate"],
@@ -415,15 +424,15 @@
             project_tier=_get_project_tier(),
             jira_task_url=_get_jira_task_url(),
             opportunity_percentage=_get_opportunity_percentage(),
             project_line_items=project_line_items,
             account_assigment_group=_get_account_assigment_group(),
             account_tax_category=_get_account_tax_category(),
             account_tax_classification=_get_account_tax_classification(),
-            account_txt_sapid=_get_account_txt_sapid(),
+            account_sap_id=_get_account_sap_id(),
             account_business_function=_get_account_business_function(),
             account_tax_id_type=_get_account_tax_id_type(),
             account_currency_code=_get_account_currency_code(),
             account_created_date=_get_account_created_date(),
             account_tier=_get_account_tier(),
             account_pec_email=_get_account_pec_email(),
             account_phone=_get_account_phone(),
@@ -443,26 +452,23 @@
         )
 
     def add_billing_lines(self, billing_lines):
         self.billing_lines.extend(billing_lines)
 
     def to_dict(self):
         return {
-            "client_fiscal_name": self.client_fiscal_name,
-            "client_account_name": self.client_account_name,
             "currency": self.currency,
             "amount": self.amount,
             "invoicing_country_code": self.invoicing_country_code,
             "operation_coordinator_email": self.operation_coordinator_email,
             "operation_coordinator_sub_email": self.operation_coordinator_sub_email,  # noqa: E501
             "created_at": self.created_at,
             "last_updated_at": self.last_updated_at,
             "opportunity_name": self.opportunity_name,
             "stage": self.stage,
-            "account_billing_country": self.account_billing_country,
             "lead_source": self.lead_source,
             "project_code": self.project_code,
             "project_id": self.project_id,
             "project_name": self.project_name,
             "project_start_date": self.project_start_date,
             "controller_email": self.controller_email,
             "controller_sub_email": self.controller_sub_email,
@@ -471,18 +477,21 @@
             "project_tier": self.project_tier,
             "jira_task_url": self.jira_task_url,
             "opportunity_percentage": self.opportunity_percentage,
             "billing_lines": [bl.to_dict() for bl in self.billing_lines],
             "project_line_items": [
                 pli.to_dict() for pli in self.project_line_items
             ],
+            "account_billing_country": self.account_billing_country,
+            "account_business_name": self.account_business_name,
+            "account_name": self.account_name,
             "account_assigment_group": self.account_assigment_group,
             "account_tax_category": self.account_tax_category,
             "account_tax_classification": self.account_tax_classification,
-            "account_txt_sapid": self.account_txt_sapid,
+            "account_sap_id": self.account_sap_id,
             "account_business_function": self.account_business_function,
             "account_tax_id_type": self.account_tax_id_type,
             "account_currency_code": self.account_currency_code,
             "account_created_date": self.account_created_date,
             "account_tier": self.account_tier,
             "account_pec_email": self.account_pec_email,
             "account_phone": self.account_phone,
```

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,38 +69,38 @@
                 "total_price": "STRING",
                 "unit_price": "STRING",
             },
             "accounts": {
                 "id": "STRING",
                 "project_id": "STRING",
                 "name": "STRING",
-                "account_assigment_group": "STRING",
+                "assigment_group": "STRING",
                 "tax_category": "STRING",
                 "tax_classification": "STRING",
                 "sap_id": "STRING",
                 "business_function": "STRING",
                 "tax_id_type": "STRING",
                 "currency_code": "STRING",
                 "created_date": "STRING",
                 "tier": "STRING",
                 "pec_email": "STRING",
                 "phone": "STRING",
                 "fax": "STRING",
                 "website": "STRING",
                 "cif": "STRING",
-                "billing_country_code": "STRING",
+                "billing_country": "STRING",
                 "business_name": "STRING",
                 "billing_address": "STRING",
                 "billing_city": "STRING",
                 "billing_postal_code": "STRING",
                 "billing_street": "STRING",
                 "company_invoicing": "STRING",
                 "office": "STRING",
                 "payment_terms": "STRING",
-                "billing_state_sode": "STRING",
+                "billing_state_code": "STRING",
                 "mail_invoicing": "STRING",
                 "invoicing_email": "STRING",
             },
         }
 
         for table_name, table_schema in self.schemas.items():
             self.client.create_table_if_not_exists(table_name, table_schema)
@@ -320,37 +320,35 @@
                 ) VALUES {', '.join(project_line_items_values)};
             """
             self.client.execute_query(insert_project_line_items_query, None)
 
     def _export_accounts(self, opportunities):
         account_values = []
         for opp in opportunities:
-            client_account_name = (
-                f'"{opp["client_account_name"]}"'
-                if opp["client_account_name"]
-                else "NULL"
+            account_name = (
+                f'"{opp["account_name"]}"' if opp["account_name"] else "NULL"
             )
-            account_assigment_group = (
+            assigment_group = (
                 f'"{opp["account_assigment_group"]}"'
                 if opp["account_assigment_group"]
                 else "NULL"
             )
             account_tax_category = (
                 f'"{opp["account_tax_category"]}"'
                 if opp["account_tax_category"]
                 else "NULL"
             )
             account_tax_classification = (
                 f'"{opp["account_tax_classification"]}"'
                 if opp["account_tax_classification"]
                 else "NULL"
             )
-            account_txt_sapid = (
-                f'"{opp["account_txt_sapid"]}"'
-                if opp["account_txt_sapid"]
+            account_sap_id = (
+                f'"{opp["account_sap_id"]}"'
+                if opp["account_sap_id"]
                 else "NULL"
             )
             account_business_function = (
                 f'"{opp["account_business_function"]}"'
                 if opp["account_business_function"]
                 else "NULL"
             )
@@ -392,17 +390,17 @@
                 f'"{opp["account_cif"]}"' if opp["account_cif"] else "NULL"
             )
             account_billing_country = (
                 f'"{opp["account_billing_country"]}"'
                 if opp["account_billing_country"]
                 else "NULL"
             )
-            client_fiscal_name = (
-                f'"{opp["client_fiscal_name"]}"'
-                if opp["client_fiscal_name"]
+            account_business_name = (
+                f'"{opp["account_business_name"]}"'
+                if opp["account_business_name"]
                 else "NULL"
             )
             account_billing_address = (
                 f'"{opp["account_billing_address"]}"'
                 if opp["account_billing_address"]
                 else "NULL"
             )
@@ -452,31 +450,31 @@
                 else "NULL"
             )
 
             account_values.append(
                 f"""
                 (
                     "{opp['project_id']}",
-                    {client_account_name},
-                    {account_assigment_group},
+                    {account_name},
+                    {assigment_group},
                     {account_tax_category},
                     {account_tax_classification},
-                    {account_txt_sapid},
+                    {account_sap_id},
                     {account_business_function},
                     {account_tax_id_type},
                     {account_currency_code},
                     {account_created_date},
                     {account_tier},
                     {account_pec_email},
                     {account_phone},
                     {account_fax},
                     {account_website},
                     {account_cif},
                     {account_billing_country},
-                    {client_fiscal_name},
+                    {account_business_name},
                     {account_billing_address},
                     {account_billing_city},
                     {account_billing_postal_code},
                     {account_billing_street},
                     {account_company_invoicing},
                     {account_office},
                     {account_payment_terms},
@@ -487,38 +485,38 @@
                 """
             )
         if account_values:
             insert_opportunities_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.accounts` (
                     project_id,
                     name,
-                    account_assigment_group,
+                    assigment_group,
                     tax_category,
                     tax_classification,
                     sap_id,
                     business_function,
                     tax_id_type,
                     currency_code,
                     created_date,
                     tier,
                     pec_email,
                     phone,
                     fax,
                     website,
                     cif,
-                    billing_country_code,
+                    billing_country,
                     business_name,
                     billing_address,
                     billing_city,
                     billing_postal_code,
                     billing_street,
                     company_invoicing,
                     office,
                     payment_terms,
-                    billing_state_sode,
+                    billing_state_code,
                     mail_invoicing,
                     invoicing_email
                 ) VALUES {', '.join(account_values)};
             """
             self.client.execute_query(insert_opportunities_query, None)
 
     def export_data(self, opportunities):
```

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 import logging
 
 import psycopg2
 from psycopg2 import sql
 
+from ms_salesforce_api.salesforce.project.constants import (
+    DEFAULT_DELETE_ACCOUNTS_TABLE,
+    DEFAULT_DELETE_BILLINGLINES_TABLE,
+    DEFAULT_DELETE_OPPORTUNITIES_TABLE,
+    DEFAULT_DELETE_PROJECTLINES_TABLE,
+    DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP,
+)
+
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 
 class CloudSQL:
     BATCH_SIZE = 200
@@ -19,14 +27,16 @@
         self.connection = psycopg2.connect(
             host=host,
             user=user,
             password=password,
             dbname=dbname,
         )
 
+        self.check_and_create_tables()
+
     def check_and_create_database(self, host, user, password, database):
         conn = psycopg2.connect(
             host=host,
             user=user,
             password=password,
             dbname="postgres",
         )
@@ -47,21 +57,57 @@
             logging.info(f"Database '{database}' created.")
 
         conn.commit()
 
         cursor.close()
         conn.close()
 
+    def check_and_create_tables(self):
+        cursor = self.connection.cursor()
+
+        for (
+            table_name,
+            create_table_query,
+        ) in DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP.items():
+            # Check if table exists
+            check_table_query = f"SELECT EXISTS (SELECT 1 FROM information_schema.tables WHERE table_name = '{table_name.lower()}')"  # noqa: E501
+
+            cursor.execute(check_table_query)
+
+            result = cursor.fetchone()
+
+            if not result[0]:
+                cursor.execute(create_table_query)
+                logging.info(f"Table '{table_name}' created.")
+
+        self.connection.commit()
+
+        cursor.close()
+
+    def delete_all_rows(self):
+        cursor = self.connection.cursor()
+        logging.info("Deleting all tables...")
+
+        cursor.execute(DEFAULT_DELETE_BILLINGLINES_TABLE)
+        cursor.execute(DEFAULT_DELETE_PROJECTLINES_TABLE)
+        cursor.execute(DEFAULT_DELETE_ACCOUNTS_TABLE)
+        cursor.execute(DEFAULT_DELETE_OPPORTUNITIES_TABLE)
+
+        self.connection.commit()
+
+        cursor.close()
+
     def export_data(self, opportunities):
         with self.connection.cursor() as cursor:
             opportunity_batches = self._create_batches(
                 opportunities, self.BATCH_SIZE
             )
             for opportunity_batch in opportunity_batches:
                 self._insert_opportunities_batch(cursor, opportunity_batch)
+                self._insert_accounts_batch(cursor, opportunity_batch)
 
                 billing_lines = []
                 project_lines = []
 
                 for opportunity in opportunity_batch:
                     billing_lines.extend(
                         self._create_billing_lines(
@@ -102,14 +148,15 @@
 
     def _insert_opportunities_batch(self, cursor, opportunities):
         opportunity_fixed = [
             {
                 key: (value if value != "" else None)
                 for key, value in opportunity.items()
                 if key not in ["billing_lines", "project_line_items"]
+                and "account_" not in key
             }
             for opportunity in opportunities
         ]
 
         insert_query = sql.SQL(
             """
             INSERT INTO Opportunities ({})
@@ -132,14 +179,58 @@
                     insert_query.as_string(cursor.connection),
                     opportunity_fixed,
                 ).decode("utf-8")
                 logging.info(insert_query_string)
             logging.error(
                 f"[ERROR - _insert_opportunities_batch (cloudsql)] - {e}"
             )
+            raise (e)
+
+    def _insert_accounts_batch(self, cursor, opportunities):
+        opportunity_fixed = [
+            {
+                key.replace("account_", ""): (value if value != "" else None)
+                for key, value in opportunity.items()
+                if "account_" in key
+            }
+            for opportunity in opportunities
+        ]
+
+        insert_query = sql.SQL(
+            """
+            INSERT INTO Accounts ({})
+            VALUES ({})
+            """
+        ).format(
+            sql.SQL(", ").join(
+                map(sql.Identifier, opportunity_fixed[0].keys())
+            ),
+            sql.SQL(", ").join(
+                map(sql.Placeholder, opportunity_fixed[0].keys())
+            ),
+        )
+
+        try:
+            cursor.executemany(insert_query, opportunity_fixed)
+        except Exception as e:
+            from pprint import pprint
+
+            pprint(opportunity_fixed)
+
+            if self.debug_mode:
+                insert_query_string = cursor.mogrify(
+                    insert_query.as_string(cursor.connection),
+                    opportunity_fixed,
+                ).decode("utf-8")
+                logging.info(insert_query_string)
+            logging.error(
+                f"[ERROR - _insert_opportunities_batch (cloudsql)] - {e}"
+            )
+
+            raise (e)
 
     def _insert_billing_lines_batch(self, cursor, billing_lines):
         insert_query = sql.SQL(
             """
             INSERT INTO BillingLines ({})
             VALUES ({})
         """
@@ -155,14 +246,15 @@
                 insert_query_string = cursor.mogrify(
                     cursor.query, billing_lines
                 ).decode("utf-8")
                 logging.info(insert_query_string)
             logging.error(
                 f"[ERROR - _insert_billing_lines_batch (cloudsql)] - {e}"
             )
+            raise (e)
 
     def _insert_project_lines_batch(self, cursor, project_lines):
         insert_query = sql.SQL(
             """
             INSERT INTO ProjectLine ({})
             VALUES ({})
         """
```

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 class BigQueryExporterTestCase(unittest.TestCase):
     def setUp(self):
         self.project_id = "your-project-id"
         self.dataset_id = "your-dataset-id"
 
         self.opportunities = [
             {
-                "client_fiscal_name": "ESMProjectAcc",
-                "client_account_name": "ESMProjectAccount",
+                "account_business_name": "ESMProjectAcc",
+                "account_name": "ESMProjectAccount",
                 "currency": "EUR",
                 "amount": 0,
                 "invoicing_country_code": "ES",
                 "operation_coordinator_email": "test@test.com",
                 "operation_coordinator_sub_email": "test@test.com",
                 "created_at": "2020-07-14T12:55:56.000+0000",
                 "last_updated_at": "2023-05-16T13:18:04.000+0000",
@@ -70,15 +70,15 @@
                         "unit_price": 90.0,
                     }
                 ],
                 "account_billing_country": "ES",
                 "account_assigment_group": None,
                 "account_tax_category": None,
                 "account_tax_classification": "0",
-                "account_txt_sapid": "10004171",
+                "account_sap_id": "10004171",
                 "account_business_function": "BP03",
                 "account_tax_id_type": "CA2",
                 "account_currency_code": "",
                 "account_created_date": "2023-02-15T09:27:46.000+0000",
                 "account_tier": "T1",
                 "account_pec_email": None,
                 "account_phone": None,
@@ -392,38 +392,38 @@
                 "a003X000015kaPxQAI"
             );
         """
         expected_accounts_query = """
             INSERT INTO `your-project-id.your-dataset-id.accounts` (
                 project_id,
                 name,
-                account_assigment_group,
+                assigment_group,
                 tax_category,
                 tax_classification,
                 sap_id,
                 business_function,
                 tax_id_type,
                 currency_code,
                 created_date,
                 tier,
                 pec_email,
                 phone,
                 fax,
                 website,
                 cif,
-                billing_country_code,
+                billing_country,
                 business_name,
                 billing_address,
                 billing_city,
                 billing_postal_code,
                 billing_street,
                 company_invoicing,
                 office,
                 payment_terms,
-                billing_state_sode,
+                billing_state_code,
                 mail_invoicing,
                 invoicing_email
             ) VALUES
                 (
                     "a003X000015kaPxQAI",
                     "ESMProjectAccount",
                     NULL,
```

### Comparing `ms_salesforce_api-0.0.44/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     @patch("psycopg2.connect")
     def test_export_data(self, mock_connect):
         mock_connection = mock_connect.return_value
         mock_cursor = mock_connection.cursor.return_value
 
         opportunities = [
             {
-                "client_fiscal_name": "ESMProjectAcc",
-                "client_account_name": "ESMProjectAccount",
+                "account_business_name": "ESMProjectAcc",
+                "account_name": "ESMProjectAccount",
                 "currency": "EUR",
                 "amount": 0,
                 "invoicing_country_code": "ES",
                 "operation_coordinator_email": "test@test.com",
                 "operation_coordinator_sub_email": "test@test.com",
                 "created_at": "2020-07-14T12:55:56.000+0000",
                 "last_updated_at": "2023-05-16T13:18:04.000+0000",
@@ -117,16 +117,16 @@
                 ],
             }
         ]
 
         opportunity_fixed = [
             {
                 "opportunity_name": "ESMOPP",
-                "client_fiscal_name": "ESMProjectAcc",
-                "client_account_name": "ESMProjectAccount",
+                "account_business_name": "ESMProjectAcc",
+                "account_name": "ESMProjectAccount",
                 "currency": "EUR",
                 "amount": 0,
                 "invoicing_country_code": "ES",
                 "operation_coordinator_email": "test@test.com",
                 "operation_coordinator_sub_email": "test@test.com",
                 "created_at": "2020-07-14T12:55:56.000+0000",
                 "last_updated_at": "2023-05-16T13:18:04.000+0000",
@@ -196,16 +196,16 @@
 
         with patch("psycopg2.connect", mock_connect):
             cloudsql = CloudSQL("host", "user", "password", "dbname")
             cloudsql.export_data(opportunities)
 
         mock_cursor.executemany.assert_called()
         self.assertEqual(
-            mock_cursor.executemany.call_count, 3
-        )  # 3 tables: Opportunities, BillingLines, ProjectLine
+            mock_cursor.executemany.call_count, 4
+        )  # 4 tables: Opportunities, BillingLines, ProjectLine, Accounts
 
         queries = [
             sql.SQL(str(call[0][0]))
             for call in mock_cursor.executemany.call_args_list
         ]
         query_strings = [
             query.as_string(mock_cursor.executemany.call_args[0][1])
```

### Comparing `ms_salesforce_api-0.0.44/pyproject.toml` & `ms_salesforce_api-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "0.0.44"
+version = "1.0.0"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-0.0.44/PKG-INFO` & `ms_salesforce_api-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 0.0.44
+Version: 1.0.0
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -92,16 +92,16 @@
 The opportunities variable will contain an array of opportunity objects with the transformed data. For example:
 
 ```python
 {
     "success": true,
     "opportunities": [
         {
-            "client_fiscal_name": "ESMProjectAcc",
-            "client_account_name": "ESMProjectAccount",
+            "account_business_name": "ESMProjectAcc",
+            "account_name": "ESMProjectAccount",
             "currency": "EUR",
             "amount": 0,
             "invoicing_country_code": "ES",
             "operation_coordinator_email": "jhon.doe@ext.makingscience.com",
             "operation_coordinator_sub_email": "jhon.doe@ext.makingscience.com",
             "created_at": "2020-07-14T12:55:56.000+0000",
             "last_updated_at": "2023-05-16T13:18:04.000+0000",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ms-salesforce-api Version: 0.0.44 Summary: Python
+Metadata-Version: 2.1 Name: ms-salesforce-api Version: 1.0.0 Summary: Python
 library used to extract data from Salesforce API and migrate it to Bigquery and
 Postgres. Author: Making Science Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: gc-google-services-api (>=1.2.7,<2.0.0) Requires-Dist: isort
 (>=5.12.0,<6.0.0) Requires-Dist: pre-commit (>=3.1.1,<4.0.0) Requires-Dist:
@@ -27,16 +27,16 @@
 project = Project( client_id="your_client_id", username="your_username",
 domain="your_domain", private_key="your_private_key", audience="https://
 login.salesforce.com", # Default value session_duration_hours=1, # Default
 value api_version='57.0', # Default value ) ``` Now, you can call the
 get_opportunities method with a query to get the opportunities data: ```python
 opportunities = project.get_opportunities() ``` The opportunities variable will
 contain an array of opportunity objects with the transformed data. For example:
-```python { "success": true, "opportunities": [ { "client_fiscal_name":
-"ESMProjectAcc", "client_account_name": "ESMProjectAccount", "currency": "EUR",
+```python { "success": true, "opportunities": [ { "account_business_name":
+"ESMProjectAcc", "account_name": "ESMProjectAccount", "currency": "EUR",
 "amount": 0, "invoicing_country_code": "ES", "operation_coordinator_email":
 "jhon.doe@ext.makingscience.com", "operation_coordinator_sub_email":
 "jhon.doe@ext.makingscience.com", "created_at": "2020-07-14T12:55:56.000+0000",
 "last_updated_at": "2023-05-16T13:18:04.000+0000", "opportunity_name":
 "ESMOPP", "stage": "Qualification", "billing_country": "ES", "lead_source":
 "Other", "project_code": "ESMSEX00430", "project_id": "a003X000015kaPxQAI",
 "project_name": "ESMProject", "project_start_date": "2023-05-13",
```

