# Comparing `tmp/platinumtools-0.4.4.tar.gz` & `tmp/platinumtools-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platinumtools-0.4.4.tar", last modified: Tue Jun  6 20:02:49 2023, max compression
+gzip compressed data, was "platinumtools-0.4.5.tar", last modified: Mon Jun 12 16:58:13 2023, max compression
```

## Comparing `platinumtools-0.4.4.tar` & `platinumtools-0.4.5.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 20:02:49.939482 platinumtools-0.4.4/
--rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.4.4/LICENSE
--rw-rw-rw-   0        0        0      863 2023-06-06 20:02:49.937653 platinumtools-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 20:02:49.560798 platinumtools-0.4.4/platinumtools/
--rw-rw-rw-   0        0        0      423 2023-05-16 18:33:49.000000 platinumtools-0.4.4/platinumtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:02:49.781798 platinumtools-0.4.4/platinumtools/aws_classes/
--rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.4.4/platinumtools/aws_classes/CommonProcesor.py
--rw-rw-rw-   0        0        0     2408 2023-06-02 21:39:12.000000 platinumtools-0.4.4/platinumtools/aws_classes/JobListener.py
--rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 platinumtools-0.4.4/platinumtools/aws_classes/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.4.4/platinumtools/aws_classes/class_adapters.py
--rw-rw-rw-   0        0        0    28135 2023-06-02 21:37:56.000000 platinumtools-0.4.4/platinumtools/aws_classes/class_enhancement-legacy.py
--rw-rw-rw-   0        0        0    38714 2023-06-06 18:16:18.000000 platinumtools-0.4.4/platinumtools/aws_classes/class_enhancement.py
--rw-rw-rw-   0        0        0     2302 2023-06-02 21:37:56.000000 platinumtools-0.4.4/platinumtools/aws_classes/class_guardian.py
--rw-rw-rw-   0        0        0    23139 2023-06-06 19:36:00.000000 platinumtools-0.4.4/platinumtools/aws_classes/class_helpers.py
--rw-rw-rw-   0        0        0     1791 2023-06-02 21:37:56.000000 platinumtools-0.4.4/platinumtools/aws_classes/class_scheduling.py
--rw-rw-rw-   0        0        0     7173 2023-06-02 21:37:56.000000 platinumtools-0.4.4/platinumtools/aws_classes/config_mapper.py
--rw-rw-rw-   0        0        0    21007 2023-06-06 18:18:47.000000 platinumtools-0.4.4/platinumtools/aws_classes/config_mapper_df.py
--rw-rw-rw-   0        0        0    19382 2023-06-02 21:38:26.000000 platinumtools-0.4.4/platinumtools/aws_classes/config_mapper_df_legacy.py
--rw-rw-rw-   0        0        0    20754 2023-06-02 16:32:33.000000 platinumtools-0.4.4/platinumtools/dda_constants.py
--rw-rw-rw-   0        0        0    12349 2023-06-02 16:32:33.000000 platinumtools-0.4.4/platinumtools/dda_models-legacy.py
--rw-rw-rw-   0        0        0    16955 2023-06-06 17:40:33.000000 platinumtools-0.4.4/platinumtools/dda_models.py
--rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.4.4/platinumtools/etl_functions.py
--rw-rw-rw-   0        0        0      102 2023-06-02 21:40:09.000000 platinumtools-0.4.4/platinumtools/help.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:02:49.593091 platinumtools-0.4.4/platinumtools.egg-info/
--rw-rw-rw-   0        0        0      863 2023-06-06 20:02:48.000000 platinumtools-0.4.4/platinumtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-06-06 20:02:49.000000 platinumtools-0.4.4/platinumtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 20:02:48.000000 platinumtools-0.4.4/platinumtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-06 20:02:49.000000 platinumtools-0.4.4/platinumtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 20:02:49.940042 platinumtools-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      990 2023-06-06 20:02:01.000000 platinumtools-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:02:49.935343 platinumtools-0.4.4/test_scenarios/
--rw-rw-rw-   0        0        0     4580 2023-06-02 21:37:56.000000 platinumtools-0.4.4/test_scenarios/JobListener.py
--rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.4.4/test_scenarios/__init__.py
--rw-rw-rw-   0        0        0     9427 2023-06-02 21:37:56.000000 platinumtools-0.4.4/test_scenarios/test_adapters.py
--rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.4.4/test_scenarios/test_code.py
--rw-rw-rw-   0        0        0     4180 2023-06-02 16:32:33.000000 platinumtools-0.4.4/test_scenarios/test_common_processing.py
--rw-rw-rw-   0        0        0    11107 2023-06-06 19:38:09.000000 platinumtools-0.4.4/test_scenarios/test_enhancement.py
--rw-rw-rw-   0        0        0    20020 2023-06-02 21:37:56.000000 platinumtools-0.4.4/test_scenarios/test_event_normalization.py
--rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.4.4/test_scenarios/test_guardian.py
--rw-rw-rw-   0        0        0     4599 2023-06-02 21:37:56.000000 platinumtools-0.4.4/test_scenarios/test_helpers.py
--rw-rw-rw-   0        0        0     5415 2023-06-02 16:32:33.000000 platinumtools-0.4.4/test_scenarios/test_scheduling.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:58:13.394269 platinumtools-0.4.5/
+-rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0      863 2023-06-12 16:58:13.391275 platinumtools-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 16:58:13.281947 platinumtools-0.4.5/platinumtools/
+-rw-rw-rw-   0        0        0      423 2023-05-16 18:33:49.000000 platinumtools-0.4.5/platinumtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:58:13.360186 platinumtools-0.4.5/platinumtools/aws_classes/
+-rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.4.5/platinumtools/aws_classes/CommonProcesor.py
+-rw-rw-rw-   0        0        0     2408 2023-06-02 21:39:12.000000 platinumtools-0.4.5/platinumtools/aws_classes/JobListener.py
+-rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 platinumtools-0.4.5/platinumtools/aws_classes/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.4.5/platinumtools/aws_classes/class_adapters.py
+-rw-rw-rw-   0        0        0    28139 2023-06-12 14:49:23.000000 platinumtools-0.4.5/platinumtools/aws_classes/class_enhancement-legacy.py
+-rw-rw-rw-   0        0        0    39072 2023-06-12 16:35:22.000000 platinumtools-0.4.5/platinumtools/aws_classes/class_enhancement.py
+-rw-rw-rw-   0        0        0     2302 2023-06-02 21:37:56.000000 platinumtools-0.4.5/platinumtools/aws_classes/class_guardian.py
+-rw-rw-rw-   0        0        0    26137 2023-06-12 12:49:40.000000 platinumtools-0.4.5/platinumtools/aws_classes/class_helpers.py
+-rw-rw-rw-   0        0        0     1791 2023-06-02 21:37:56.000000 platinumtools-0.4.5/platinumtools/aws_classes/class_scheduling.py
+-rw-rw-rw-   0        0        0     7173 2023-06-02 21:37:56.000000 platinumtools-0.4.5/platinumtools/aws_classes/config_mapper.py
+-rw-rw-rw-   0        0        0    21196 2023-06-07 13:31:54.000000 platinumtools-0.4.5/platinumtools/aws_classes/config_mapper_df.py
+-rw-rw-rw-   0        0        0    19382 2023-06-02 21:38:26.000000 platinumtools-0.4.5/platinumtools/aws_classes/config_mapper_df_legacy.py
+-rw-rw-rw-   0        0        0    20754 2023-06-02 16:32:33.000000 platinumtools-0.4.5/platinumtools/dda_constants.py
+-rw-rw-rw-   0        0        0    12357 2023-06-12 14:49:23.000000 platinumtools-0.4.5/platinumtools/dda_models-legacy.py
+-rw-rw-rw-   0        0        0    18188 2023-06-12 14:49:23.000000 platinumtools-0.4.5/platinumtools/dda_models.py
+-rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.4.5/platinumtools/etl_functions.py
+-rw-rw-rw-   0        0        0      102 2023-06-02 21:40:09.000000 platinumtools-0.4.5/platinumtools/help.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:58:13.324621 platinumtools-0.4.5/platinumtools.egg-info/
+-rw-rw-rw-   0        0        0      863 2023-06-12 16:58:12.000000 platinumtools-0.4.5/platinumtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-06-12 16:58:13.000000 platinumtools-0.4.5/platinumtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:58:12.000000 platinumtools-0.4.5/platinumtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-12 16:58:12.000000 platinumtools-0.4.5/platinumtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 16:58:13.396268 platinumtools-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-06-12 16:52:25.000000 platinumtools-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:58:13.386270 platinumtools-0.4.5/test_scenarios/
+-rw-rw-rw-   0        0        0     4580 2023-06-09 14:01:55.000000 platinumtools-0.4.5/test_scenarios/JobListener.py
+-rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.4.5/test_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     2056 2023-06-09 19:46:55.000000 platinumtools-0.4.5/test_scenarios/event-data-into-timeslots.py
+-rw-rw-rw-   0        0        0     9427 2023-06-02 21:37:56.000000 platinumtools-0.4.5/test_scenarios/test_adapters.py
+-rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.4.5/test_scenarios/test_code.py
+-rw-rw-rw-   0        0        0     2709 2023-06-08 17:46:11.000000 platinumtools-0.4.5/test_scenarios/test_common_processing.py
+-rw-rw-rw-   0        0        0    12508 2023-06-12 16:22:38.000000 platinumtools-0.4.5/test_scenarios/test_enhancement.py
+-rw-rw-rw-   0        0        0    20020 2023-06-02 21:37:56.000000 platinumtools-0.4.5/test_scenarios/test_event_normalization.py
+-rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.4.5/test_scenarios/test_guardian.py
+-rw-rw-rw-   0        0        0     4603 2023-06-07 15:55:40.000000 platinumtools-0.4.5/test_scenarios/test_helpers.py
+-rw-rw-rw-   0        0        0     5423 2023-06-07 15:55:40.000000 platinumtools-0.4.5/test_scenarios/test_scheduling.py
+-rw-rw-rw-   0        0        0     3570 2023-06-09 20:07:53.000000 platinumtools-0.4.5/test_scenarios/test_splitting_algorthm.py
```

### Comparing `platinumtools-0.4.4/LICENSE` & `platinumtools-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/PKG-INFO` & `platinumtools-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.4.4
+Version: 0.4.5
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/CommonProcesor.py` & `platinumtools-0.4.5/platinumtools/aws_classes/CommonProcesor.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/JobListener.py` & `platinumtools-0.4.5/platinumtools/aws_classes/JobListener.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/class_adapters.py` & `platinumtools-0.4.5/platinumtools/aws_classes/class_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/class_enhancement-legacy.py` & `platinumtools-0.4.5/platinumtools/aws_classes/class_enhancement-legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class MockAdapter(SourceAdapter):
     """Mock Adaptation to be used until the other interfaces work.
     """
 
     # I will be mocking a standard interface with evertything one could have?
     def __init__(self) -> None:
         super().__init__()
-        self.mock_adapt_result ={'guid':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','version':'1.0','connector_guid':'365_MANAGEMENT','type':'','organization_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','actor':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','operation':2,'item_count':5,'details':[{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-24T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-24T18:23:36','Id':'c878338a-15ff-4986-8bd3-5d6eac071b4a','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':43,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','ApplicationMode':'Standard','ItemName':'HelloThere','LabelAction':'None','LabelAppliedDateTime':'2022-10-25T18:23:32','LabelId':'defa4170-0d19-0005-0004-bc88714345d2','LabelName':'AllEmployees(unrestricted)','Receivers':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'Sender':'nelson@o365.devcooks.com'},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:36','Id':'c17eedb7-6977-4169-b625-bb26e0ede079','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':13,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','IncidentId':'11bb1d67-ae3d-d176-4000-08dab6b85275','PolicyDetails':[{'PolicyId':'00000000-0000-0000-0000-000000000000','Rules':[{'Actions':[],'ConditionsMatched':{'ConditionMatchedInNewScheme':True,'OtherConditions':[{'Name':'SensitivityLabels','Value':'defa4170-0d19-0005-0004-bc88714345d2'}]},'RuleId':'defa4170-0d19-0005-0004-bc88714345d2','RuleMode':'Enable','RuleName':'defa4170-0d19-0005-0004-bc88714345d2','Severity':'Low'}]}],'SensitiveInfoDetectionIsIncluded':False,'ExchangeMetaData':{'BCC':[],'CC':[],'FileSize':17579,'From':'nelson@o365.devcooks.com','MessageID':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','RecipientCount':2,'Sent':'2022-10-25T18:23:33','Subject':'HelloThere','To':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'UniqueID':'fe03264d-a22d-4c70-57b1-08dab6b60675'}},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:33','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:33','Id':'e01bd1fb-a635-4f09-57b1-08dab6b60675','Operation':'Send','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':2,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','ClientIP':'68.160.247.154','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Item':{'Id':'Unknown','InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','ParentFolder':{'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEPAAAB','Path':'\\Drafts'},'SizeInBytes':3991,'Subject':'HelloThere'}},'application':'Exchange','operation':'Send','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:04','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:04','Id':'daf566de-6581-486c-b9f7-f8df1d07457f','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Folders':[{'FolderItems':[{'InternetMessageId':'<ceafc3fa-fd0a-46ba-9754-e033ee56ce75@az.westcentralus.production.microsoft.com>'},{'InternetMessageId':'<ae042a57-4cd4-466a-adf0-417549c30a96@az.westeurope.production.microsoft.com>'},{'InternetMessageId':'<abccdb15-1bd4-476f-88f8-0bde5349cb61@az.westus2.production.microsoft.com>'},{'InternetMessageId':'<5c06433f-d7f6-48c7-8752-72f5cf93011c@az.westus.production.microsoft.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEMAAAB','Path':'\\Inbox'},{'FolderItems':[{'InternetMessageId':'<CY5PR05MB91439309823940F866A9629EDD2E9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB9143FB7EF878879EED5FC05CDD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91439292F10817DCB3DE6FC6DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91436B02DD20921A28720BA4DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':8},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:41','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:41','Id':'0d77eaad-2ddd-4e39-8ce1-469113caf263','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientAppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientIPAddress':'2603:10b6:930:3d::7','ClientInfoString':'Client=REST;Client=RESTSystem;;','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','Folders':[{'FolderItems':[{'InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':1},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}}],'hash_1':'','hash_2':''}
+        self.mock_adapt_result ={'guid':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','version':'1.0','connector_guid':'365_MANAGEMENT','activity':'','organization_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','actor':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','operation':2,'item_count':5,'details':[{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-24T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-24T18:23:36','Id':'c878338a-15ff-4986-8bd3-5d6eac071b4a','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':43,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','ApplicationMode':'Standard','ItemName':'HelloThere','LabelAction':'None','LabelAppliedDateTime':'2022-10-25T18:23:32','LabelId':'defa4170-0d19-0005-0004-bc88714345d2','LabelName':'AllEmployees(unrestricted)','Receivers':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'Sender':'nelson@o365.devcooks.com'},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:36','Id':'c17eedb7-6977-4169-b625-bb26e0ede079','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':13,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','IncidentId':'11bb1d67-ae3d-d176-4000-08dab6b85275','PolicyDetails':[{'PolicyId':'00000000-0000-0000-0000-000000000000','Rules':[{'Actions':[],'ConditionsMatched':{'ConditionMatchedInNewScheme':True,'OtherConditions':[{'Name':'SensitivityLabels','Value':'defa4170-0d19-0005-0004-bc88714345d2'}]},'RuleId':'defa4170-0d19-0005-0004-bc88714345d2','RuleMode':'Enable','RuleName':'defa4170-0d19-0005-0004-bc88714345d2','Severity':'Low'}]}],'SensitiveInfoDetectionIsIncluded':False,'ExchangeMetaData':{'BCC':[],'CC':[],'FileSize':17579,'From':'nelson@o365.devcooks.com','MessageID':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','RecipientCount':2,'Sent':'2022-10-25T18:23:33','Subject':'HelloThere','To':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'UniqueID':'fe03264d-a22d-4c70-57b1-08dab6b60675'}},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:33','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:33','Id':'e01bd1fb-a635-4f09-57b1-08dab6b60675','Operation':'Send','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':2,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','ClientIP':'68.160.247.154','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Item':{'Id':'Unknown','InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','ParentFolder':{'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEPAAAB','Path':'\\Drafts'},'SizeInBytes':3991,'Subject':'HelloThere'}},'application':'Exchange','operation':'Send','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:04','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:04','Id':'daf566de-6581-486c-b9f7-f8df1d07457f','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Folders':[{'FolderItems':[{'InternetMessageId':'<ceafc3fa-fd0a-46ba-9754-e033ee56ce75@az.westcentralus.production.microsoft.com>'},{'InternetMessageId':'<ae042a57-4cd4-466a-adf0-417549c30a96@az.westeurope.production.microsoft.com>'},{'InternetMessageId':'<abccdb15-1bd4-476f-88f8-0bde5349cb61@az.westus2.production.microsoft.com>'},{'InternetMessageId':'<5c06433f-d7f6-48c7-8752-72f5cf93011c@az.westus.production.microsoft.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEMAAAB','Path':'\\Inbox'},{'FolderItems':[{'InternetMessageId':'<CY5PR05MB91439309823940F866A9629EDD2E9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB9143FB7EF878879EED5FC05CDD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91439292F10817DCB3DE6FC6DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91436B02DD20921A28720BA4DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':8},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:41','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:41','Id':'0d77eaad-2ddd-4e39-8ce1-469113caf263','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientAppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientIPAddress':'2603:10b6:930:3d::7','ClientInfoString':'Client=REST;Client=RESTSystem;;','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','Folders':[{'FolderItems':[{'InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':1},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}}],'hash_1':'','hash_2':''}
 
     def adapt(self, staging_events: dict)->dict:
         return self.mock_adapt_result
 
 class Microsoft365ManagementAdapter(SourceAdapter):
 
     def __init__(self, organizationQuerier: OrganizationalQuerier):
```

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/class_enhancement.py` & `platinumtools-0.4.5/platinumtools/aws_classes/class_enhancement.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class MockAdapter(SourceAdapter):
     """Mock Adaptation to be used until the other interfaces work.
     """
 
     # I will be mocking a standard interface with evertything one could have?
     def __init__(self) -> None:
         super().__init__()
-        self.mock_adapt_result ={'guid':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','version':'1.0','connector_guid':'365_MANAGEMENT','type':'','organization_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','actor':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','operation':2,'item_count':5,'details':[{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-24T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-24T18:23:36','Id':'c878338a-15ff-4986-8bd3-5d6eac071b4a','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':43,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','ApplicationMode':'Standard','ItemName':'HelloThere','LabelAction':'None','LabelAppliedDateTime':'2022-10-25T18:23:32','LabelId':'defa4170-0d19-0005-0004-bc88714345d2','LabelName':'AllEmployees(unrestricted)','Receivers':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'Sender':'nelson@o365.devcooks.com'},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:36','Id':'c17eedb7-6977-4169-b625-bb26e0ede079','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':13,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','IncidentId':'11bb1d67-ae3d-d176-4000-08dab6b85275','PolicyDetails':[{'PolicyId':'00000000-0000-0000-0000-000000000000','Rules':[{'Actions':[],'ConditionsMatched':{'ConditionMatchedInNewScheme':True,'OtherConditions':[{'Name':'SensitivityLabels','Value':'defa4170-0d19-0005-0004-bc88714345d2'}]},'RuleId':'defa4170-0d19-0005-0004-bc88714345d2','RuleMode':'Enable','RuleName':'defa4170-0d19-0005-0004-bc88714345d2','Severity':'Low'}]}],'SensitiveInfoDetectionIsIncluded':False,'ExchangeMetaData':{'BCC':[],'CC':[],'FileSize':17579,'From':'nelson@o365.devcooks.com','MessageID':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','RecipientCount':2,'Sent':'2022-10-25T18:23:33','Subject':'HelloThere','To':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'UniqueID':'fe03264d-a22d-4c70-57b1-08dab6b60675'}},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:33','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:33','Id':'e01bd1fb-a635-4f09-57b1-08dab6b60675','Operation':'Send','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':2,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','ClientIP':'68.160.247.154','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Item':{'Id':'Unknown','InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','ParentFolder':{'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEPAAAB','Path':'\\Drafts'},'SizeInBytes':3991,'Subject':'HelloThere'}},'application':'Exchange','operation':'Send','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:04','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:04','Id':'daf566de-6581-486c-b9f7-f8df1d07457f','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Folders':[{'FolderItems':[{'InternetMessageId':'<ceafc3fa-fd0a-46ba-9754-e033ee56ce75@az.westcentralus.production.microsoft.com>'},{'InternetMessageId':'<ae042a57-4cd4-466a-adf0-417549c30a96@az.westeurope.production.microsoft.com>'},{'InternetMessageId':'<abccdb15-1bd4-476f-88f8-0bde5349cb61@az.westus2.production.microsoft.com>'},{'InternetMessageId':'<5c06433f-d7f6-48c7-8752-72f5cf93011c@az.westus.production.microsoft.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEMAAAB','Path':'\\Inbox'},{'FolderItems':[{'InternetMessageId':'<CY5PR05MB91439309823940F866A9629EDD2E9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB9143FB7EF878879EED5FC05CDD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91439292F10817DCB3DE6FC6DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91436B02DD20921A28720BA4DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':8},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:41','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:41','Id':'0d77eaad-2ddd-4e39-8ce1-469113caf263','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientAppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientIPAddress':'2603:10b6:930:3d::7','ClientInfoString':'Client=REST;Client=RESTSystem;;','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','Folders':[{'FolderItems':[{'InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':1},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}}],'hash_1':'','hash_2':''}
+        self.mock_adapt_result ={'guid':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','version':'1.0','connector_guid':'365_MANAGEMENT','activity':'','organization_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','actor':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','operation':2,'item_count':5,'details':[{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-24T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-24T18:23:36','Id':'c878338a-15ff-4986-8bd3-5d6eac071b4a','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':43,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','ApplicationMode':'Standard','ItemName':'HelloThere','LabelAction':'None','LabelAppliedDateTime':'2022-10-25T18:23:32','LabelId':'defa4170-0d19-0005-0004-bc88714345d2','LabelName':'AllEmployees(unrestricted)','Receivers':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'Sender':'nelson@o365.devcooks.com'},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:36','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:36','Id':'c17eedb7-6977-4169-b625-bb26e0ede079','Operation':'MipLabel','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':13,'UserKey':'c397ec65-e71e-493f-94f2-2e53cdd9b02e','UserType':4,'Version':1,'Workload':'Exchange','ObjectId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','UserId':'nelson@o365.devcooks.com','IncidentId':'11bb1d67-ae3d-d176-4000-08dab6b85275','PolicyDetails':[{'PolicyId':'00000000-0000-0000-0000-000000000000','Rules':[{'Actions':[],'ConditionsMatched':{'ConditionMatchedInNewScheme':True,'OtherConditions':[{'Name':'SensitivityLabels','Value':'defa4170-0d19-0005-0004-bc88714345d2'}]},'RuleId':'defa4170-0d19-0005-0004-bc88714345d2','RuleMode':'Enable','RuleName':'defa4170-0d19-0005-0004-bc88714345d2','Severity':'Low'}]}],'SensitiveInfoDetectionIsIncluded':False,'ExchangeMetaData':{'BCC':[],'CC':[],'FileSize':17579,'From':'nelson@o365.devcooks.com','MessageID':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','RecipientCount':2,'Sent':'2022-10-25T18:23:33','Subject':'HelloThere','To':['nwang@platinumfilings.com','wangnelson2@gmail.com'],'UniqueID':'fe03264d-a22d-4c70-57b1-08dab6b60675'}},'application':'Exchange','operation':'MipLabel','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:33','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:33','Id':'e01bd1fb-a635-4f09-57b1-08dab6b60675','Operation':'Send','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':2,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','ClientIP':'68.160.247.154','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Item':{'Id':'Unknown','InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>','ParentFolder':{'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEPAAAB','Path':'\\Drafts'},'SizeInBytes':3991,'Subject':'HelloThere'}},'application':'Exchange','operation':'Send','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:04','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:04','Id':'daf566de-6581-486c-b9f7-f8df1d07457f','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'00000002-0000-0ff1-ce00-000000000000','ClientIPAddress':'68.160.247.154','ClientInfoString':'Client=OWA;Action=ViaProxy','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','SessionId':'e01c84f0-8db1-439e-87bc-5ee52fdf90d4','Folders':[{'FolderItems':[{'InternetMessageId':'<ceafc3fa-fd0a-46ba-9754-e033ee56ce75@az.westcentralus.production.microsoft.com>'},{'InternetMessageId':'<ae042a57-4cd4-466a-adf0-417549c30a96@az.westeurope.production.microsoft.com>'},{'InternetMessageId':'<abccdb15-1bd4-476f-88f8-0bde5349cb61@az.westus2.production.microsoft.com>'},{'InternetMessageId':'<5c06433f-d7f6-48c7-8752-72f5cf93011c@az.westus.production.microsoft.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEMAAAB','Path':'\\Inbox'},{'FolderItems':[{'InternetMessageId':'<CY5PR05MB91439309823940F866A9629EDD2E9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB9143FB7EF878879EED5FC05CDD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91439292F10817DCB3DE6FC6DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'},{'InternetMessageId':'<CY5PR05MB91436B02DD20921A28720BA4DD2D9@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':8},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}},{'event_guid':'74d25673-b01c-4211-a7c4-9930610fb7eb','user_guid':'ab3c-asd1-100G','timestamp_utc':'2022-10-25T18:23:41','loadbatch_id':'a08f815f-12fa-47fb-9f6d-5c3d7fe53eff','raw_details':{'CreationTime':'2022-10-25T18:23:41','Id':'0d77eaad-2ddd-4e39-8ce1-469113caf263','Operation':'MailItemsAccessed','OrganizationId':'74d25673-b01c-4211-a7c4-9930610fb7eb','RecordType':50,'ResultStatus':'Succeeded','UserKey':'10032002359E261F','UserType':0,'Version':1,'Workload':'Exchange','UserId':'nelson@o365.devcooks.com','AppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientAppId':'13937bba-652e-4c46-b222-3003f4d1ff97','ClientIPAddress':'2603:10b6:930:3d::7','ClientInfoString':'Client=REST;Client=RESTSystem;;','ExternalAccess':False,'InternalLogonType':0,'LogonType':0,'LogonUserSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxGuid':'bd6abed2-5d3b-4206-aada-31ca71605e63','MailboxOwnerSid':'S-1-5-21-3007612343-326144747-4028531239-4420872','MailboxOwnerUPN':'nelson@o365.devcooks.com','OperationProperties':[{'Name':'MailAccessType','Value':'Bind'},{'Name':'IsThrottled','Value':'False'}],'OrganizationName':'devcooks.onmicrosoft.com','OriginatingServer':'CY5PR05MB9143(15.20.4200.000)\r\n','Folders':[{'FolderItems':[{'InternetMessageId':'<CY5PR05MB9143EE143E6008D69C9391F5DD319@CY5PR05MB9143.namprd05.prod.outlook.com>'}],'Id':'LgAAAAALcWhVmnTeRJS8qp8HxA25AQC/yWJ3KK0XQJ7UyikjUZtEAAAAAAEJAAAB','Path':'\\SentItems'}],'OperationCount':1},'application':'Exchange','operation':'MailItemsAccessed','version_source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0},'source_uri':{'id':'','uri':'','file_type':'','file_extension':'','size':0}}],'hash_1':'','hash_2':''}
 
     def adapt(self, staging_events: dict)->dict:
         return self.mock_adapt_result
 
 
 
 class SalesforceAdapter(SourceAdapter):
@@ -107,15 +107,15 @@
                 to_address=None,
                 email_bcc=None,
                 email_cc=None,
                 email_imid=None,
                 phone_result=None,
                 record_url=Utils.NoneSafe(event, "Record_Link__c"),
                 recording_url=None,
-                record_id=None
+                record_id=Utils.NoneSafe(event, "RecordId__c")
             )
             new_details.append(fileEvent)
         management_api.details = new_details
         return management_api.to_dict()
 
 
 class ChromeAdapter(SourceAdapter):
@@ -423,15 +423,15 @@
                 eventData = Utils.eventDataIntoTimeSlots(event)
                 timeslots_list.extend(eventData)
             
             # Always create an event based event.
             new_event = Event.from_dict(event)
             events_list.append(new_event.to_dict())
 
-
+        print("1 | events_list", len(events_list), "timeslots_list", len(timeslots_list))
         return {
             "events": events_list,
             "timeslots": timeslots_list
         }
 
 
     def businessEnhancements(self, events: StagingModel) -> dict["events": List[Event], "timeslots": List[Timeslot]]:
@@ -449,31 +449,33 @@
         # organization_params: List[dict] = self.organizationDBProvider.getOrganizationParameters(normalized_events[0]['user_guid'])
         organization_params: List[dict] = self.organizationDBProvider.getOrganizationParametersByOrganizationID(normalized_events[0]["organization_id"])
         joint_events = ConfigMapper.join_organization_fields(
             normalized_events=normalized_events,
             user_information_table=organization_params
         )
         date_mapped_events = ConfigMapper.date_related_population(join_events=joint_events)
+        
 
         # Convert into pandas first.
         # date_mapped_events_df = pd.DataFrame(date_mapped_events)
         processed_events = ConfigMapper.categorization_jobs(date_mapped_events=date_mapped_events)
         # processed_events = classified_events_df
         
         # Have the separatation between events and timeslots
+        # print("2 | events_list", len(processed_events["evemts"]), "timeslots_list", len(processed_events["timeslots"]))
         return self.separateEvent(processed_events)
 
 
 
     def adapt(self, staging_events: dict) -> dict:
         return self.default_source_adapter.adapt(staging_events = staging_events)
 
     
-    def publish(self, enhanced_events: List[dict]):
-        self.publishingDBProvider.publish(enhanced_events)
+    def publish(self, enhanced_events: List[dict], table_name=""):
+        self.publishingDBProvider.publish(enhanced_events, table_name=table_name)
 
     def fetchBusinessRules():
         """Using the self.organizationDBProvider it receives and updates the Dataset
         """
         pass
 
 class CommonProcessor():
@@ -687,21 +689,21 @@
         """Understanding the transformation that is provided by the item. We want to make the transformation later on.
         The idea is toreceive the getTransformationStrategy on the project.
         """
 
         # For now I can dummy return Chrom Basic enhancer
         # If connector guid starts with chrome then use Chrome adapter
         adapter_map = {
-            "chrome-extension-ddap-1": SalesforceAdapter,
-            2: ChromeAdapter,
+            "salesforce-connector": SalesforceAdapter,
+            "chrome-extension-ddap-1": ChromeAdapter,
             3: WindowsAdapter
         }
         
         adapter = ChromeAdapter(organizationQuerier=self.organization_provider) # Default adapter
-        
+        print("staging_event => ", staging_event)
         adapter_id = staging_event[CONNECTOR_GUID]
         if (adapter_id in adapter_map):
             adapter = adapter_map[adapter_id](organizationQuerier=self.organization_provider)
             
 
         basic_enhancment = BasicEnhancement(
             organizationDBProvider=self.organization_provider,
```

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/class_guardian.py` & `platinumtools-0.4.5/platinumtools/aws_classes/class_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/class_helpers.py` & `platinumtools-0.4.5/platinumtools/aws_classes/class_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from typing import List
 from platinumtools.dda_constants import *
 from platinumtools.dda_models import *
 import json, random, string
 
 from pytz import timezone
 import math, datetime, pytz
-from dateutil import parser
+from dateutil import parser, tz
+import json
+from typing import List
+
 # awsconfig_mapper import ConfigMapper
 
 
 
 class DatabaseProvider(ABC):
     def __init__(self, credentials, settings):
         self.credentials = credentials
@@ -18,31 +21,31 @@
         
 
     @abstractmethod
     def publish(self, events: List[dict]):
         print("publishing to database:", events)
 
     @abstractmethod
-    def getOne(self, key_value, key_column: str = "guid"):
+    def getOne(self, key_value, key_column: str = "guid", table_name: str = "events"):
         print("Getting source with: ", key_value, "in", key_column, "column")
 
 class MockDatabaseProvider(DatabaseProvider):
     """Prints publishing and getters, using for debugging, also returns static examples
-    Records the json for quicke edition and visualization in a local file.
+    Records the json for quick edition and visualization in a local file.
     """
     def __init__(self, credentials, settings):
         super().__init__(credentials, settings)
         self.db = []
 
-    def publish(self, events: List[dict]):
+    def publish(self, events: List[dict], table_name="mock_db.json"):
         self.db.extend(events)
 
         # Save as .. code-block:: json
         
-        with open("mock_db.json", "w") as f:
+        with open(table_name, "w") as f:
             f.write(json.dumps(self.db, indent=4))
 
         return super().publish(events=events)
 
     def getOne(self, key_value, key_column: str = "guid"):
         super().getOne(key_column)
         try:
@@ -106,33 +109,38 @@
         Returns:
             _type_: _description_
         """
         if key in fetchFrom:
             return fetchFrom[key]
         return elseGets
     
-    def publish(self, events: List[dict]):
+    def publish(self, events: List[dict], table_name="mock_db.json"):
         """Publishes
         Expected parameters to have unders settings:
         - TABLENAME
         - COLUMN_NAMES
     
         Args:
             events (List[dict]): List of events to publish.
         """
 
         # Fetches the proper credentials based on the environemnt
 
 
         # Update Settings"
-        column_names = self.settings.get("COLUMN_NAMES", ["user_guid", "timestamp_utc", "application", "operation"])
-        tablename= self.settings.get("TABLENAME", "events")
+        tablename_events= self.settings.get("TABLENAME_EVENTS", "events")
+        column_names_events = self.settings.get("COLUMN_NAMES_EVENTS", [])
+
+        tablename_timeslot = self.settings.get("TABLENAME_TIMESLOT", "timeslot")
+        column_names_timeslot = self.settings.get("COLUMN_NAMES_TIMESLOT", [])
+        
+
 
         # Pushes the changes into SQL
-        insert_sql = f"INSERT INTO {tablename} ({', '.join(column_names)}) VALUES ({', '.join(['%s'] * len(column_names))})"
+        insert_sql = f"INSERT INTO {tablename_events} ({', '.join(column_names_events)}) VALUES ({', '.join(['%s'] * len(column_names_events))})"
         # # print("Created insert_SQL:", insert_sql)
         # Execute the INSERT statement for each dictionary in the list
         # print("attepting to get rows from events:", events)
 
         import json
         from typing import List
 
@@ -146,15 +154,15 @@
                 for(i, item) in enumerate(queryArgument):
                     queryArgument[i] = cleanQueryArgument(item)
             
             return queryArgument
 
         for row in events:
             values = []
-            for col in column_names:
+            for col in column_names_events:
                 value = row.get(col, None)
                 values.append(cleanQueryArgument(value))
             try:
                 self.cursor.execute(insert_sql, values)
             except Exception as e:
                 print("Exception at publish:", e, "values:", values)
         self.connection.commit()
@@ -179,16 +187,99 @@
         if row:
             row_dict = dict(zip([desc[0] for desc in self.cursor.description], row))
             # print(row_dict)
         else:
             print("No rows found")
         return row_dict
 
+class PostgreSQLProviderTimeSlotPlusEventsPublishing(PostgreSQLProvider):
+    """This improvement overwrites simple PostgreSQLProvider to be
+     both Timeslot and also events to be published on publish time.
+    """
+
+    def __init__(self, credentials, settings):
+        """Initiates with the database credentials, and settings as the specfici tables it is looking for
+        Requires:
+            pandas
+            psycopg2
+
+        Args:
+            credentials (dict): Credentails for database {USERNAME, PASSWORD, HOST, DB}
+            settings (dict): {TABLE}
+        """
+        super().__init__(credentials, settings)
+        
+
+
+        
+    def publish(self, events: dict["events": List[dict], "timeslot": List[dict]], table_name=""):
+        """Publishes
+        Expected parameters to have unders settings:
+        - TABLENAME
+        - COLUMN_NAMES
+    
+        Args:
+            events (List[dict]): List of events to publish.
+        """
+
+        # Fetches the proper credentials based on the environemnt
+
+
+        # Update Settings"
+        tablename_events= self.settings.get("TABLENAME_EVENTS", "events")
+        column_names_events = self.settings.get("COLUMN_NAMES_EVENTS", [])
+
+        tablename_timeslot = self.settings.get("TABLENAME_TIMESLOTS", "timeslot")
+        column_names_timeslot = self.settings.get("COLUMN_NAMES_TIMESLOTS", [])
 
+        self.publish_to(events["events"], column_names_events, tablename_events)
+        self.publish_to(events["timeslots"], column_names_timeslot, tablename_timeslot)
+
+
+    def publish_to(self, events: List[dict], column_names: List[str], tablename: str):
+        """Publishes into the postgresdatabase the timeslot and events
+        @param events: List of events to publish.
+        @param column_names: List of column names to publish        
     
+        Args:
+            events (List[dict]): List of events to publish.
+        """
+
+
+        # Pushes the changes into SQL
+        insert_sql = f"INSERT INTO {tablename} ({', '.join(column_names)}) VALUES ({', '.join(['%s'] * len(column_names))})"
+        
+        def cleanQueryArgument(queryArgument):
+            # If the queryArg is a list or dict, format it into a way that is query insertable
+            if isinstance(queryArgument, (dict)):
+                # If the is List and the first element is a dict, then it is a list of objects
+                return json.dumps(queryArgument)
+            if isinstance(queryArgument, List) and len(queryArgument) >0 and isinstance(queryArgument[0], dict):
+                # return an array of strings of the json
+                for(i, item) in enumerate(queryArgument):
+                    queryArgument[i] = cleanQueryArgument(item)
+            
+            return queryArgument
+
+        for row in events:
+            values = []
+            for col in column_names:
+                value = row.get(col, None)
+                values.append(cleanQueryArgument(value))
+            try:
+                self.cursor.execute(insert_sql, values)
+            except Exception as e:
+                
+                print("publishing to "+ tablename +"; received the following events:", events)
+                # print("attributes timeslot:", Timeslot.get_attribute_keys())
+                print("Insert sql created:", insert_sql)
+                print("Exception at publish:", e, "values:", values)
+        self.connection.commit()
+
+       
 class Utils:
     """Some random utitlities
     Requirements:
     - json
     """
     
     def date_related_population(join_events: List[dict]) -> List[dict]:
@@ -293,59 +384,56 @@
             except Exception as e:
                 # print("Exception at NoneSafe:", e
                 #       , "dictItem:", type(dictItem) ,dictItem, 
                 #       "key:",  type(key),key)
                 pass
         return default
     
+    
+
     def eventDataIntoTimeSlots(eventData: dict, limit_minutes_per_slot=10) -> List[Timeslot]:
-        """_summary_
+        """
+        Split the events into time slots based on the next 10th multiple of minutes.
 
         Args:
-            eventData (dict): _description_
-            limit_minutes_per_slot (int, optional): The max time in minutes to split the events into. Defaults to 10.
+            eventData (dict): Event data dictionary.
+            limit_minutes_per_slot (int, optional): The maximum time in minutes to split the events into. Defaults to 10.
 
         Returns:
-            List[Timeslot]: A list of Timeslot Events if they are proper.
+            List[Timeslot]: A list of Timeslot events.
         """
-        # if( duration is larger than 10 minutes): Then loop until it gets to end_time and populate the list of Timeslots to return
         timeslots_res = []
         timeslots_event_data = []
-        duration =  eventData["duration"]
-        # If duration is not None and larger than 0
-        if(duration is not None and duration > 0):
-            
-            # start_time = datetime.datetime.strptime(eventData["timestamp"][:-1], "%Y-%m-%dT%H:%M:%S.%fZ")
-            # end_time = datetime.datetime.strptime(eventData["end_time"][:-1], "%Y-%m-%dT%H:%M:%S.%fZ")
-            start_time = parser.parse(eventData["timestamp"]).astimezone(timezone("UTC"))
-            end_time = parser.parse(eventData["end_time"]).astimezone(timezone("UTC"))
-            
-            while(start_time < end_time):
-                print()
-                # Create a new imeslot
-                # Next start time as the limit minutes per slot (minutes) * 60s + start_time
-                next_start_time = start_time + datetime.timedelta(minutes=limit_minutes_per_slot)
-                print("comparing: next_start_time", next_start_time, "| end_time", end_time, "| start_time", start_time)
-                current_endtime = min(next_start_time, end_time)
+        duration = eventData["duration"]
+
+        if duration is not None and duration > 0:
+            start_time = parser.parse(eventData["timestamp"]).astimezone(tz.UTC)
+            end_time = parser.parse(eventData["end_time"]).astimezone(tz.UTC)
+
+            while start_time < end_time:
+                next_multiple_of_limit = datetime.datetime(
+                    start_time.year, start_time.month, start_time.day,
+                    start_time.hour, start_time.minute + limit_minutes_per_slot - (start_time.minute % limit_minutes_per_slot),
+                    tzinfo=tz.UTC
+                )
+
+                current_endtime = min(next_multiple_of_limit, end_time)
 
-                # Copy the entire eventData and change the start_time and end_time and duration
                 eventDataCopy = eventData.copy()
                 eventDataCopy["timestamp"] = start_time.isoformat()
                 eventDataCopy["end_time"] = current_endtime.isoformat()
-                # print("attempting to process:", eventDataCopy)
                 timeslots_event_data.append(eventDataCopy)
+
                 start_time = current_endtime
-                print("start_time", start_time, "| end_time",end_time, "| current_endtime",current_endtime)
 
-        if(len(timeslots_event_data) > 0):
-            # run date related type of processing
+        if len(timeslots_event_data) > 0:
             date_formatted_events_data = Utils.date_related_population(timeslots_event_data)
 
-            # Now into Timeslot type of dict, add them into the list: timeslots_res
             for timeslot_event_data in date_formatted_events_data:
+                timeslot_event_data["event_guid"] = eventData["guid"]
                 timeslot = Timeslot.from_dict(timeslot_event_data).to_dict()
                 timeslots_res.append(timeslot)
 
         return timeslots_res
 
 
 class OrganizationalQuerier(ABC):
@@ -447,34 +535,34 @@
             dict: organization parameters
         """
         return {}
 
 # Sample profile of an employee, that is just used by default.
 
 sample_profile_user_1 = {
-            "organization_id": 123456,
+            "organization_id": 1,
             "user_guid": "ab3c-asd1-100G",
             "user_id": 1,
-            "user_team_id": [1, 2, 3],
-            "profile_id": [4, 5, 6],
+            "user_team_id": [1, 2],
+            "profile_id": [1],
             "user_timezone": "US/Eastern",
             "user_time_slot_split": 6,
             "user_work_hours_start": [9, 10, 11, 9, 9, 0, 0],
             "user_work_days": [0, 1, 2, 3, 4],
             "user_work_hours_end": [17, 18, 19, 17, 17, 0, 0],
             "user_escape_dates": ["2022-04-15", "2022-06-10"],
             "profile_mapping_instruction": {"instruction1": "value1", "instruction2": "value2"}
     }
 
 sample_profile_user_2 =  {
-                "organization_id": 123456,
+                "organization_id": 1,
                 "user_id": 2,
-                "user_team_id": [7, 8],
+                "user_team_id": [1],
                 "user_guid": "ab3c-asd1-561a",
-                "profile_id": [1, 2, 3],
+                "profile_id": [1, 2],
                 "user_timezone": "Asia/Tokyo",
                 "user_time_slot_split": 6,
                 "user_work_hours_start": [9, 10, 11, 9, 9, 0, 0],
                 "user_work_days": [0, 1, 2, 3, 4],
                 "user_work_hours_end": [17, 18, 19, 17, 17, 0, 0],
                 "user_escape_dates": ["2022-03-01", "2022-09-01"],
                 "profile_mapping_instruction": {"instruction5": "value5", "instruction6": "value6"}
```

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/class_scheduling.py` & `platinumtools-0.4.5/platinumtools/aws_classes/class_scheduling.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/config_mapper.py` & `platinumtools-0.4.5/platinumtools/aws_classes/config_mapper.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/config_mapper_df.py` & `platinumtools-0.4.5/platinumtools/aws_classes/config_mapper_df.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,68 +144,75 @@
             user_info = user_info_dict.get(user_id) # Fetches otherwise gets none. (wont run the following.)
             if user_info:
                 joined_event = {**event, **user_info}
                 joined_events.append(joined_event)
         
         return joined_events
         
+    def event_population(event: dict):
+        timestamp: datetime.datetime = parser.parse(event['timestamp']).replace(tzinfo=pytz.utc)
+        timezone_str: str = event['user_timezone']
+        local_timestamp: datetime.datetime = timestamp.astimezone(timezone(timezone_str))
+        event['timestamp_local'] = local_timestamp.isoformat()
+        event["local_timezone"] = timezone_str
+
+        # Extract timeslot
+        timeslot = (local_timestamp.hour * 60 + local_timestamp.minute) // 10
+        event['timeslot'] = timeslot
+        event['timeslot_local'] = (timeslot + 6) % 24
+
+        # Extract UTC date and time components
+        event['hour'] = timestamp.hour
+        event['minute'] = timestamp.minute
+        event['day'] = timestamp.day
+        event['month'] = timestamp.month
+        event['year'] = timestamp.year
+        event['week'] = timestamp.isocalendar()[1]
+        event['weekday'] = timestamp.weekday()
+
+        # Extract local date and time components
+        event['hour_local'] = local_timestamp.hour
+        event['minute_local'] = local_timestamp.minute
+        event['day_local'] = local_timestamp.day
+        event['month_local'] = local_timestamp.month
+        event['year_local'] = local_timestamp.year
+        event['week_local'] = local_timestamp.isocalendar()[1]
+        event['weekday_local'] = local_timestamp.weekday()
+
+        # Check if end_time is None
+        if event['end_time'] is not None:
+            # Convert end_time to datetime object
+            endtime = parser.parse(event['end_time'])
+
+            # Convert timestamp and end_time to the specified timezone
+            local_endtime = endtime.astimezone(timezone(timezone_str))
+
+            # Populate the timestamp_local, end_time_local, and duration fields as isoformat strings
+            event['end_time_local'] = local_endtime.isoformat()
+            event['duration'] = (endtime - timestamp).total_seconds() / 3600
+        else:
+            # If end_time is None, set the remaining fields to None as well
+            event['end_time'] = None
+            event['end_time_local'] = None
+            event['duration'] = 0
 
-    
     def date_related_population(join_events: List[dict]) -> List[dict]:
         """
         For each of the events, populate the date-related items.
+        Probably for some toher events will just that be the case.
         """
         for event in join_events:
+            # print("Attempting date_related", event)
             # Convert timestamp to datetime object
-            timestamp: datetime.datetime = parser.parse(event['timestamp']).replace(tzinfo=pytz.utc)
-            timezone_str: str = event['user_timezone']
-            local_timestamp: datetime.datetime = timestamp.astimezone(timezone(timezone_str))
-            event['timestamp_local'] = local_timestamp.isoformat()
-            event["local_timezone"] = timezone_str
-
-            # Extract timeslot
-            timeslot = (local_timestamp.hour * 60 + local_timestamp.minute) // 10
-            event['timeslot'] = timeslot
-            event['timeslot_local'] = (timeslot + 6) % 24
-
-            # Extract UTC date and time components
-            event['hour'] = timestamp.hour
-            event['minute'] = timestamp.minute
-            event['day'] = timestamp.day
-            event['month'] = timestamp.month
-            event['year'] = timestamp.year
-            event['week'] = timestamp.isocalendar()[1]
-            event['weekday'] = timestamp.weekday()
-
-            # Extract local date and time components
-            event['hour_local'] = local_timestamp.hour
-            event['minute_local'] = local_timestamp.minute
-            event['day_local'] = local_timestamp.day
-            event['month_local'] = local_timestamp.month
-            event['year_local'] = local_timestamp.year
-            event['week_local'] = local_timestamp.isocalendar()[1]
-            event['weekday_local'] = local_timestamp.weekday()
-
-            # Check if end_time is None
-            if event['end_time'] is not None:
-                # Convert end_time to datetime object
-                endtime = parser.parse(event['end_time'])
-
-                # Convert timestamp and end_time to the specified timezone
-                local_endtime = endtime.astimezone(timezone(timezone_str))
-
-                # Populate the timestamp_local, end_time_local, and duration fields as isoformat strings
-                event['end_time_local'] = local_endtime.isoformat()
-                event['duration'] = (endtime - timestamp).total_seconds() / 3600
-            else:
-                # If end_time is None, set the remaining fields to None as well
-                event['end_time'] = None
-                event['end_time_local'] = None
-                event['duration'] = 0
-
+            try:
+                ConfigMapper.event_population(event)
+                continue
+            except Exception as e:
+                print(e)
+                print(event)
         return join_events
 
     def mapping_application(date_mapped_events_df: pd.core.frame.DataFrame, bucket_instructions: dict)->pd.core.frame.DataFrame:
         """maps application column, receives general business instruction.
 
         Args:
             date_mapped_events_df (pd.core.frame.DataFrame): _description_
```

### Comparing `platinumtools-0.4.4/platinumtools/aws_classes/config_mapper_df_legacy.py` & `platinumtools-0.4.5/platinumtools/aws_classes/config_mapper_df_legacy.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/platinumtools/dda_constants.py` & `platinumtools-0.4.5/platinumtools/dda_constants.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/platinumtools/dda_models-legacy.py` & `platinumtools-0.4.5/platinumtools/dda_models-legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,16 +324,16 @@
         """
         if 'guid' in data:
             self.guid = data['guid']
         if 'version' in data:
             self.version = data['version']
         if 'connector_guid' in data:
             self.connector_guid = data['connector_guid']
-        if 'type' in data:
-            self.type = data['type']
+        if 'activity' in data:
+            self.type = data['activity']
         if 'organization_guid' in data:
             self.organization_guid = data['organization_guid']
         if 'actor' in data:
             self.actor = data['actor']
         if 'item_count' in data:
             self.item_count = data['item_count']
         if 'details' in data:
```

### Comparing `platinumtools-0.4.4/platinumtools/dda_models.py` & `platinumtools-0.4.5/platinumtools/dda_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,40 @@
             "id": self.id,
             "uri": self.uri,
             "file_type": self.file_type,
             "file_extension": self.file_extension,
             "size": self.size
         }
 
-class EventData:
+class StructureModel:
+    """Structure model for the data being used in the DDA.
+    Allows:
+    - To create a model from a dictionary.
+    - To convert a model to a dictionary.
+    - To get the attributes of the model as a list.
+
+    """
+    
+    @classmethod
+    def from_dict(cls, timeslot_dict):
+        valid_keys = set(cls.__init__.__code__.co_varnames[1:])
+        filtered_dict = {k: v for k, v in timeslot_dict.items() if k in valid_keys}
+        return cls(**filtered_dict)
+    
+    def to_dict(self):
+        return {k: v for k, v in self.__dict__.items() if v is not None}
+
+class EventData(StructureModel):
     """
     Time based events Also includes keystrocks and mousclicks just because they might be there, and need them.
     Not the Event Dataset that is on the database (having it's own table), but is on the staging area.
+
+    Automated:
+    - guid is generated automatically at creation (cannot be assigned).
+
     """
     def __init__(self,
                  user_id: str,
                  organization_guid: str,
                  application: str,
                  app: str,
                  app_type: str,
@@ -70,14 +92,15 @@
                  recording_url: str,
                  record_id: int,
                 #  These are the only ones that are not in the original model
                  mouse_clicks: int = 0,
                  keystrokes: int = 0,
                  ):
         
+        self.guid = str(uuid.uuid4())
         self.user_id = user_id
         self.organization_guid = organization_guid
         self.application = application
         self.app = app
         self.app_type = app_type
         self.operation = operation
         self.operation_type = operation_type
@@ -114,45 +137,43 @@
         self.record_url = record_url
         self.recording_url = recording_url
         self.record_id = record_id
         self.mouse_clicks = mouse_clicks
         self.keystrokes = keystrokes
 
 
-class Event:
+class Event(StructureModel):
     """
     This is the time based event. Which will be used on modeling the database.
     """
-    def __init__(self, user_id: str, organization_guid: str, application: str, app: str,
-                 app_type: str, operation: str, operation_type: str, event_guid: str,
-                 staging_guid: str, platform_id: str, organization_id: str, local_timezone: str,
+    def __init__(self, guid: str, user_id: str, application: str, app: str,
+                 app_type: str, operation: str, operation_type: str, event_guid: str, platform_id: str, organization_id: str, local_timezone: str,
                  timestamp: datetime, end_time: datetime, timestamp_local: datetime,
                  end_time_local: datetime, duration: float, description: str, title: str,
                  url: str, site: str, url_domain: str, files: List[dict], file_count: int,
                  action_type: str, geolocation: dict, ipv4: str, local_ipv4: str,
                  size: int, sha2: str, email_subject: str, from_address: str, to_address: str,
                  email_cc: str, email_bcc: str, email_imid: str, phone_result: str,
                  record_url: str, recording_url: str, record_id: int):
+        # Generate random guid
+        self.guid = guid
         self.user_id = user_id
-        self.organization_guid = organization_guid
         self.application = application
         self.app = app
         self.app_type = app_type
         self.operation = operation
         self.operation_type = operation_type
         self.event_guid = event_guid
-        self.staging_guid = staging_guid
         self.platform_id = platform_id
         self.organization_id = organization_id
         self.local_timezone = local_timezone
         self.timestamp = timestamp
         self.end_time = end_time
         self.timestamp_local = timestamp_local
         self.end_time_local = end_time_local
-        self.duration = duration
         self.description = description
         self.title = title
         self.url = url
         self.site = site
         self.url_domain = url_domain
         self.files = files
         self.file_count = file_count
@@ -169,33 +190,46 @@
         self.email_bcc = email_bcc
         self.email_imid = email_imid
         self.phone_result = phone_result
         self.record_url = record_url
         self.recording_url = recording_url
         self.record_id = record_id
 
-    @classmethod
-    def from_dict(cls, timeslot_dict):
-        valid_keys = set(cls.__init__.__code__.co_varnames[1:])
-        filtered_dict = {k: v for k, v in timeslot_dict.items() if k in valid_keys}
-        return cls(**filtered_dict)
-    
-    def to_dict(self):
-        return {k: v for k, v in self.__dict__.items() if v is not None}
+
+    @staticmethod
+    def get_attribute_keys():
+        """Returns all the attributes of the class.
+
+        Returns:
+            List[str]: List of attributes.
+        """
+        return [
+            "guid", "user_id",  "application", "app", "app_type",
+            "operation", "operation_type", "event_guid", "platform_id",
+            "organization_id", "local_timezone", "timestamp", "end_time", "timestamp_local",
+            "end_time_local", "duration", "description", "title", "url", "site",
+            "url_domain", "files", "file_count", "action_type", "geolocation", "ipv4",
+            "local_ipv4", "size", "sha2", "email_subject", "from_address", "to_address",
+            "email_cc", "email_bcc", "email_imid", "phone_result", "record_url",
+            "recording_url", "record_id"
+        ]
+
 
 
-class Timeslot:
+class Timeslot(StructureModel):
     """Timeslot
     This is the timeslot based event in which an hour is divided into 6 slots of 10 minutes.
     """
-    def __init__(self, timeslot: int, timeslot_local: int, hour: int, minute: int,
+    def __init__(self, event_guid: str, timeslot: int, timeslot_local: int, hour: int, minute: int,
                  day: int, month: int, year: int, week: int, weekday: int,
                  hour_local: int, minute_local: int, day_local: int, month_local: int,
                  year_local: int, week_local: int, weekday_local: int, mouse_clicks: int,
+                 staging_guid: str,
                  keystrokes: int):
+        self.event_guid = event_guid
         self.timeslot = timeslot
         self.timeslot_local = timeslot_local
         self.hour = hour
         self.minute = minute
         self.day = day
         self.month = month
         self.year = year
@@ -205,49 +239,49 @@
         self.minute_local = minute_local
         self.day_local = day_local
         self.month_local = month_local
         self.year_local = year_local
         self.week_local = week_local
         self.weekday_local = weekday_local
         self.mouse_clicks = mouse_clicks
+        self.staging_guid = staging_guid
         self.keystrokes = keystrokes
 
-    @classmethod
-    def from_dict(cls, timeslot_dict):
-        valid_keys = set(cls.__init__.__code__.co_varnames[1:])
-        filtered_dict = {k: v for k, v in timeslot_dict.items() if k in valid_keys}
-        return cls(**filtered_dict)
+    @staticmethod
+    def get_attribute_keys():
+        """Returns all the attributes of the class.
 
+        Args:
+            obj (Timeslot): An instance of the Timeslot class.
+
+        Returns:
+            List[str]: List of attributes.
+        """
+        return [
+            "event_guid", "timeslot", "timeslot_local", "hour", "minute", "day", "month",
+            "year", "week", "weekday", "hour_local", "minute_local", "day_local",
+            "month_local", "year_local", "week_local", "weekday_local", "mouse_clicks",
+            "staging_guid",
+            "keystrokes"
+        ]
 
-    def to_dict(self):
-        return {k: v for k, v in self.__dict__.items() if v is not None}
-    
     
 # TODO => Delete the following classes (legacy)
 
-class GenericEvent:
+class GenericEvent(StructureModel):
     """Generic event inside the staging area
     """
     def __init__(self, event_guid: str, user_guid: str, timestamp_utc: datetime, loadbatch_id: int, raw_details: str, application: str):
         self.event_guid = event_guid
         self.user_guid = user_guid
         self.timestamp_utc = timestamp_utc
         self.loadbatch_id = loadbatch_id
         self.raw_details = raw_details
         self.application = application
 
-    def to_dict(self):
-        return {
-            "event_guid": self.event_guid,
-            "user_guid": self.user_guid,
-            "timestamp_utc": self.timestamp_utc,
-            "loadbatch_id": self.loadbatch_id,
-            "raw_details": self.raw_details,
-            "application": self.application
-        }
 
 class FileEvent(GenericEvent):
     def __init__(self, event_guid: str, user_guid: str,  timestamp_utc: datetime, loadbatch_id: int, raw_details: str, operation: str, version_source_uri: Attachment, source_uri: Attachment, application: str):
         super().__init__(event_guid, user_guid,  timestamp_utc, loadbatch_id, raw_details, application=application)
         self.operation = operation
         self.version_source_uri = version_source_uri
         self.source_uri = source_uri
@@ -403,16 +437,16 @@
         """
         if 'guid' in data:
             self.guid = data['guid']
         if 'version' in data:
             self.version = data['version']
         if 'connector_guid' in data:
             self.connector_guid = data['connector_guid']
-        if 'type' in data:
-            self.type = data['type']
+        if 'activity' in data:
+            self.type = data['activity']
         if 'organization_guid' in data:
             self.organization_guid = data['organization_guid']
         if 'actor' in data:
             self.actor = data['actor']
         if 'item_count' in data:
             self.item_count = data['item_count']
         if 'details' in data:
```

### Comparing `platinumtools-0.4.4/platinumtools.egg-info/PKG-INFO` & `platinumtools-0.4.5/platinumtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.4.4
+Version: 0.4.5
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.4.4/platinumtools.egg-info/SOURCES.txt` & `platinumtools-0.4.5/platinumtools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 platinumtools/aws_classes/class_helpers.py
 platinumtools/aws_classes/class_scheduling.py
 platinumtools/aws_classes/config_mapper.py
 platinumtools/aws_classes/config_mapper_df.py
 platinumtools/aws_classes/config_mapper_df_legacy.py
 test_scenarios/JobListener.py
 test_scenarios/__init__.py
+test_scenarios/event-data-into-timeslots.py
 test_scenarios/test_adapters.py
 test_scenarios/test_code.py
 test_scenarios/test_common_processing.py
 test_scenarios/test_enhancement.py
 test_scenarios/test_event_normalization.py
 test_scenarios/test_guardian.py
 test_scenarios/test_helpers.py
-test_scenarios/test_scheduling.py
+test_scenarios/test_scheduling.py
+test_scenarios/test_splitting_algorthm.py
```

### Comparing `platinumtools-0.4.4/setup.py` & `platinumtools-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.4.4'
+VERSION = '0.4.5'
 DESCRIPTION = 'DDAPP Modules'
 LONG_DESCRIPTION = 'Common Constants, classes and methods for ETL and other python projects'
 
 # Setting up
 #nenewang08
 setup(
     name="platinumtools",
```

### Comparing `platinumtools-0.4.4/test_scenarios/JobListener.py` & `platinumtools-0.4.5/test_scenarios/JobListener.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,11 +114,12 @@
                 # Delete then the message from the queue.     
                 # Delete the message from the queue
                 sqs.delete_message(
                     QueueUrl=queue_url,
                     ReceiptHandle=message['ReceiptHandle']
                 )
         else:
-            # print('No messages in the queue.')
+            print('No messages in the queue.')
+
 
 # Call the function to start processing messages
 process_messages()
```

### Comparing `platinumtools-0.4.4/test_scenarios/test_adapters.py` & `platinumtools-0.4.5/test_scenarios/test_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/test_scenarios/test_common_processing.py` & `platinumtools-0.4.5/test_scenarios/test_common_processing.py`

 * *Files 27% similar despite different names*

```diff
@@ -46,67 +46,24 @@
         'USERNAME': "postgres",
         'PASSWORD': "dDueller123araM=!",
         "HOST": "test-ddanalytics-rds-v2.cpcwi20k2qgg.us-east-1.rds.amazonaws.com",
         "DB": "v1_2"
     }
 
     settings = {
-        "TABLENAME": "event",
         "GET_TABLENAME": "staging_events",
-         "COLUMN_NAMES": [
-                        "user_guid",
-                        "timestamp_utc",
-                        "application",
-                        "operation",
-                        "event_guid",
-                        "organization_guid",
-                        "staging_guid",
-                        "source_type",
-                        "connector_guid",
-                        "version",
-                        "organization_id",
-                        "user_id",
-                        "user_team_id",
-                        "profile_id",
-                        "user_timezone",
-                        "timestamp_client_local",
-                        "month_number",
-                        "month_name",
-                        "weekday_number",
-                        "weekday_name",
-                        "day",
-                        "hour",
-                        "minute",
-                        "time_slot",
-                        "week_number",
-                        "date",
-                        "operation_type",
-                        "application_type",
-                        "interface_type",
-                        "work_hour_type",
-                        "raw_details",
-                        "start_time",
-                        "end_time",
-                        "duration",
-                        "description",
-                        "title",
-                        "url",
-                        "attachments",
-                        "action_origin",
-                        "span_guid",
-                        "root_reference",
-                        "root_start",
-                        "root_end",
-                        "root_duration"
-                        ]
-
+        "TABLENAME_EVENTS": "event",
+        "COLUMN_NAMES_EVENTS": Event.get_attribute_keys(),
+        "TABLENAME_TIMESLOTS": "timeslot",
+        "COLUMN_NAMES_TIMESLOTS": Timeslot.get_attribute_keys()
     }
-    publishingDBProvider = PostgreSQLProvider(credentials=credentials, settings=settings)
+    publishingDBProvider = PostgreSQLProviderTimeSlotPlusEventsPublishing(credentials=credentials, settings=settings)
+    mockingDBProvide = MockDatabaseProvider(credentials=credentials, settings=settings)
 
-    processor = BetterCommonProcessor(
-        job_parameters={"guid": "55c38902-37ed-9207-be6f-443ab4e68172",
-                       },
+    processor = ConnecToGUIDHarcodedDictBasedCommonProcessor(
+        job_parameters={"guid": "387a26ff-ceed-5015-a6c9-afa"},
         organization_provider=organizationDBProvider,
         publishingDBProvider=publishingDBProvider
+        # publishingDBProvider=mockingDBProvide
     ) 
     
     processor.runJobs() # Should also post at the Mock Database
```

### Comparing `platinumtools-0.4.4/test_scenarios/test_enhancement.py` & `platinumtools-0.4.5/test_scenarios/test_enhancement.py`

 * *Files 10% similar despite different names*

```diff
@@ -140,49 +140,77 @@
     "LastModifiedById": "0055x00000C68rTAAR"
   }
 ],
   "hash_1": "d8298e88a929de23ab1bcb06f7a05d0e694f871fb15ef31800d8027d0f76a2ff",
   "hash_2": "3baea71e7edcb8b8aa4417fb640c0fa0d7f9791c8a2b17ca3f499d10f7a43dcd"
 }
 
+
+# UPDATE : Reflect changes in details here.
 sample_chrome_raw_input = {
     'guid': '387a26ff-ceed-5015-a6c9-a2cad90329c0',
     'previous_guid': 'b5a496cb-8bfb-39fd-67f2-4d14feef1fa1',
     'version': "1.0.0",
     'date': "2023-05-12 17:50:00.026",
     'connector_guid': "chrome-extension-ddap-1",
     "organization_guid": "organization-1",
     "details":[
-  {
-    "url": "chrome://extensions/",
-    "guid": "bcf17e37-a4b9-17b4-bed2-69aaf120f68c",
-    "type": "tab-focus",
-    "title": "Extensions",
-    "domain": "extensions",
-    "params": {},
-    "duration": 2,
-    "spanId": "3a2a3726-4985-7034-21de-175622df3ed7",
-    "endTime": "2023-05-11T16:03:13.783Z",
+      {
+      "domain": "www.google.com",
+      "endTime": "2023-06-12T14:24:11.821Z",
+      "guid": "ac30bcd1-3e16-5ade-6bd6-8bb51735d053",
+      "incognito": False,
+      "interactions": {},
+      "isEventComplete": False,
+      "params": {},
+      "spanGUID": "460a111f-8bbf-870c-0428-cd927ba2b7c4",
+      "spanSequence": 0,
+      "spanStartTime": "2023-06-12T14:23:40.480Z",
+      "timestamp": "2023-06-12T14:23:40.480Z",
+      "title": "queriable site? - Google Search",
+      "type": "tab-focus",
+      "duration": 31.34,
+      "url": "https://www.google.com/search?q=queriable+site%3F&rlz=1C1GCEA_enUS1016US1016&oq=queriable+site%3F&aqs=chrome..69i57j33i10i160.2846j1j7&sourceid=chrome&ie=UTF-8"
+    },
+    {
+      "domain": "www.google.com",
+      "timestamp": "2023-06-12T14:24:11.821Z",
+      "endTime": "2023-06-12T14:24:11.821Z",
+      "duration": 10,
+      "guid": "ac30bcd1-3e16-5ade-6bd6-8bb51735d054",
+      "incognito": False,
+      "interactions": {},
+      "isEventComplete": True,
+      "params": {},
+      "spanGUID": "460a111f-8bbf-870c-0428-cd927ba2b7c4",
+      "spanSequence": 1,
+      "spanStartTime": "2023-06-12T14:23:40.480Z",
+      "title": "queriable site? - Google Search (Part 2)",
+      "type": "tab-focus",
+      "url": "https://www.google.com/search?q=queriable+site%3F&rlz=1C1GCEA_enUS1016US1016&oq=queriable+site%3F&aqs=chrome..69i57j33i10i160.2846j1j7&sourceid=chrome&ie=UTF-8"
+    },
+    # An extra large event.
+    {
+    "domain": "pnp.github.io",
+    "timestamp": "2023-06-12T14:23:36.135Z",
+    "endTime": "2023-06-12T14:43:40.477Z",
+    "duration": 1204.34,
+    "guid": "fee6724b-2abe-f829-d6a3-46eb5bd6c477",
     "incognito": False,
-    "startTime": "2023-05-11T16:03:12.408Z",
-    "timestamp": "2023-05-11T16:03:13.408Z"
-  },
-  {
-    "url": "chrome://extensions/",
-    "guid": "bcf17e37-a4b9-17b4-bed2-asd",
-    "type": "tab-focus",
-    "title": "Extensions",
-    "domain": "extensions",
+    "interactions": {
+        "scroll": 1
+    },
+    "isEventComplete": True,
     "params": {},
-    "duration": 1200,
-    "spanId": "3a2a3726-4985-7034-21de-asd",
-    "endTime": "2023-05-11T16:35:33.783Z",
-    "incognito": False,
-    "startTime": "2023-05-11T16:03:12.408Z",
-    "timestamp": "2023-05-11T16:03:13.408Z"
+    "spanGUID": "58e82818-800d-249e-dbac-42617821dbdb",
+    "spanSequence": 0,
+    "spanStartTime": "2023-06-12T14:23:36.135Z",
+    "title": "queryable - PnP/PnPjs",
+    "type": "tab-focus",
+    "url": "https://pnp.github.io/pnpjs/queryable/queryable/"
   },
   {
     "id": 16,
     "url": "https://mazzzystar.github.io/images/2023-05-10/superCLUE.jpg",
     "guid": "0adeb6d2-c889-4592-0b46-e43e887e4d71",
     "mime": "image/jpeg",
     "type": "download",
@@ -269,15 +297,16 @@
       publishingDBProvider=publishingDBProvider,
       source_adapter=ChromeAdapter(organizationQuerier=organizationDBProvider)
   )
 
   enhanced_events: dict["events": List[Event], "timeslots": List[Timeslot]] = basic_enhancment.transform(staging_events_events=sample_chrome_raw_input)
   print(enhanced_events)
   # basic_enhancment.publish(enhanced_events=enhanced_events["events"])
-  basic_enhancment.publish(enhanced_events=enhanced_events["timeslots"])
+  basic_enhancment.publish(enhanced_events=enhanced_events["timeslots"], table_name="timeslots.json" )
+  basic_enhancment.publish(enhanced_events=enhanced_events["events"], table_name="events.json" )
 
 # def test_windows_enhancement_integration():
 #   """Tests if Windows Adapter is used correctly
 #   """
 #   organizationDBProvider = MockOrganizationQuerier
 #   credentials = {}
 #   settings = {}
```

#### html2text {}

```diff
@@ -52,34 +52,48 @@
 "0055x00000C68rTAAR", "sfid__c": "00Q7c00000Et2nGEAR", "Actor__c":
 "nwang@platinumfilings.com", "Object__c": "LEAD", "Activity__c": "UPDATE",
 "CreatedById": "0055x00000C68rTAAR", "Source_IP__c": "68.160.247.154",
 "ActionDate__c": "2023-04-27T20:18:23.000Z", "Description__c": "Peter Pan ()",
 "Record_Link__c": "LEAD", "SessionType__c": "Aura", "IsInteractive__c": True,
 "LastModifiedById": "0055x00000C68rTAAR" } ], "hash_1":
 "d8298e88a929de23ab1bcb06f7a05d0e694f871fb15ef31800d8027d0f76a2ff", "hash_2":
-"3baea71e7edcb8b8aa4417fb640c0fa0d7f9791c8a2b17ca3f499d10f7a43dcd" }
-sample_chrome_raw_input = { 'guid': '387a26ff-ceed-5015-a6c9-a2cad90329c0',
-'previous_guid': 'b5a496cb-8bfb-39fd-67f2-4d14feef1fa1', 'version': "1.0.0",
-'date': "2023-05-12 17:50:00.026", 'connector_guid': "chrome-extension-ddap-1",
-"organization_guid": "organization-1", "details":[ { "url": "chrome://
-extensions/", "guid": "bcf17e37-a4b9-17b4-bed2-69aaf120f68c", "type": "tab-
-focus", "title": "Extensions", "domain": "extensions", "params": {},
-"duration": 2, "spanId": "3a2a3726-4985-7034-21de-175622df3ed7", "endTime":
-"2023-05-11T16:03:13.783Z", "incognito": False, "startTime": "2023-05-11T16:03:
-12.408Z", "timestamp": "2023-05-11T16:03:13.408Z" }, { "url": "chrome://
-extensions/", "guid": "bcf17e37-a4b9-17b4-bed2-asd", "type": "tab-focus",
-"title": "Extensions", "domain": "extensions", "params": {}, "duration": 1200,
-"spanId": "3a2a3726-4985-7034-21de-asd", "endTime": "2023-05-11T16:35:33.783Z",
-"incognito": False, "startTime": "2023-05-11T16:03:12.408Z", "timestamp":
-"2023-05-11T16:03:13.408Z" }, { "id": 16, "url": "https://mazzzystar.github.io/
-images/2023-05-10/superCLUE.jpg", "guid": "0adeb6d2-c889-4592-0b46-
-e43e887e4d71", "mime": "image/jpeg", "type": "download", "state": "complete",
-"title": "The Leverage of LLMs for Individuals | TL;DR", "danger": "safe",
-"domain": "mazzzystar.github.io", "exists": True, "paused": False, "endTime":
-"2023-05-11T16:03:31.427Z", "fileSize": 72801, "filename": "C:
+"3baea71e7edcb8b8aa4417fb640c0fa0d7f9791c8a2b17ca3f499d10f7a43dcd" } # UPDATE :
+Reflect changes in details here. sample_chrome_raw_input = { 'guid': '387a26ff-
+ceed-5015-a6c9-a2cad90329c0', 'previous_guid': 'b5a496cb-8bfb-39fd-67f2-
+4d14feef1fa1', 'version': "1.0.0", 'date': "2023-05-12 17:50:00.026",
+'connector_guid': "chrome-extension-ddap-1", "organization_guid":
+"organization-1", "details":[ { "domain": "www.google.com", "endTime": "2023-
+06-12T14:24:11.821Z", "guid": "ac30bcd1-3e16-5ade-6bd6-8bb51735d053",
+"incognito": False, "interactions": {}, "isEventComplete": False, "params": {},
+"spanGUID": "460a111f-8bbf-870c-0428-cd927ba2b7c4", "spanSequence": 0,
+"spanStartTime": "2023-06-12T14:23:40.480Z", "timestamp": "2023-06-12T14:23:
+40.480Z", "title": "queriable site? - Google Search", "type": "tab-focus",
+"duration": 31.34, "url": "https://www.google.com/
+search?q=queriable+site%3F&rlz=1C1GCEA_enUS1016US1016&oq=queriable+site%3F&aqs=chrome..69i57j33i10i160.2846j1j7&sourceid=chrome&ie=UTF-
+8" }, { "domain": "www.google.com", "timestamp": "2023-06-12T14:24:11.821Z",
+"endTime": "2023-06-12T14:24:11.821Z", "duration": 10, "guid": "ac30bcd1-3e16-
+5ade-6bd6-8bb51735d054", "incognito": False, "interactions": {},
+"isEventComplete": True, "params": {}, "spanGUID": "460a111f-8bbf-870c-0428-
+cd927ba2b7c4", "spanSequence": 1, "spanStartTime": "2023-06-12T14:23:40.480Z",
+"title": "queriable site? - Google Search (Part 2)", "type": "tab-focus",
+"url": "https://www.google.com/
+search?q=queriable+site%3F&rlz=1C1GCEA_enUS1016US1016&oq=queriable+site%3F&aqs=chrome..69i57j33i10i160.2846j1j7&sourceid=chrome&ie=UTF-
+8" }, # An extra large event. { "domain": "pnp.github.io", "timestamp": "2023-
+06-12T14:23:36.135Z", "endTime": "2023-06-12T14:43:40.477Z", "duration":
+1204.34, "guid": "fee6724b-2abe-f829-d6a3-46eb5bd6c477", "incognito": False,
+"interactions": { "scroll": 1 }, "isEventComplete": True, "params": {},
+"spanGUID": "58e82818-800d-249e-dbac-42617821dbdb", "spanSequence": 0,
+"spanStartTime": "2023-06-12T14:23:36.135Z", "title": "queryable - PnP/PnPjs",
+"type": "tab-focus", "url": "https://pnp.github.io/pnpjs/queryable/queryable/
+" }, { "id": 16, "url": "https://mazzzystar.github.io/images/2023-05-10/
+superCLUE.jpg", "guid": "0adeb6d2-c889-4592-0b46-e43e887e4d71", "mime": "image/
+jpeg", "type": "download", "state": "complete", "title": "The Leverage of LLMs
+for Individuals | TL;DR", "danger": "safe", "domain": "mazzzystar.github.io",
+"exists": True, "paused": False, "endTime": "2023-05-11T16:03:31.427Z",
+"fileSize": 72801, "filename": "C:
 \\Users\\NelsonWang\\Downloads\\guide\\superCLUE (2).jpg", "finalUrl": "https:/
 /mazzzystar.github.io/images/2023-05-10/superCLUE.jpg", "referrer": "https://
 mazzzystar.github.io/2023/05/10/LLM-for-individual/", "canResume": False,
 "incognito": False, "startTime": "2023-05-11T16:03:28.431Z", "timestamp":
 "2023-05-11T16:03:31.434Z", "totalBytes": 72801, "bytesReceived": 72801 },
 { "url": "https://imgbb.com/", "guid": "cfe2aea7-dfdf-b8a7-1d55-c870e14fc203",
 "type": "upload", "files": [ { "name": "iamge-.jpg", "size": 17292, "type":
@@ -110,15 +124,17 @@
 (credentials=credentials, settings=settings) basic_enhancment =
 BasicEnhancement( organizationDBProvider=organizationDBProvider,
 publishingDBProvider=publishingDBProvider, source_adapter=ChromeAdapter
 (organizationQuerier=organizationDBProvider) ) enhanced_events: dict["events":
 List[Event], "timeslots": List[Timeslot]] = basic_enhancment.transform
 (staging_events_events=sample_chrome_raw_input) print(enhanced_events) #
 basic_enhancment.publish(enhanced_events=enhanced_events["events"])
-basic_enhancment.publish(enhanced_events=enhanced_events["timeslots"]) # def
+basic_enhancment.publish(enhanced_events=enhanced_events["timeslots"],
+table_name="timeslots.json" ) basic_enhancment.publish
+(enhanced_events=enhanced_events["events"], table_name="events.json" ) # def
 test_windows_enhancement_integration(): # """Tests if Windows Adapter is used
 correctly # """ # organizationDBProvider = MockOrganizationQuerier #
 credentials = {} # settings = {} # publishingDBProvider = MockDatabaseProvider
 (credentials=credentials, settings=settings) # # Open the JSON file # with open
 ('sample_windows.json') as file: # # Load the JSON data into a variable #
 sample_windows_data = json.load(file) # basic_enhancment = BasicEnhancement( #
 organizationDBProvider=organizationDBProvider, #
```

### Comparing `platinumtools-0.4.4/test_scenarios/test_event_normalization.py` & `platinumtools-0.4.5/test_scenarios/test_event_normalization.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/test_scenarios/test_guardian.py` & `platinumtools-0.4.5/test_scenarios/test_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4.4/test_scenarios/test_helpers.py` & `platinumtools-0.4.5/test_scenarios/test_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -213,76 +213,76 @@
 00000d40: 636b 5f63 6f75 6e74 223a 2031 3030 302c  ck_count": 1000,
 00000d50: 0d0a 2020 2020 2020 2020 2020 2020 226b  ..            "k
 00000d60: 6579 7374 726f 6b65 5f63 6f75 6e74 223a  eystroke_count":
 00000d70: 2032 3330 3030 2c0d 0a20 2020 2020 2020   23000,..       
 00000d80: 2020 2020 2022 6170 706c 6963 6174 696f       "applicatio
 00000d90: 6e22 3a20 2245 7863 656c 222c 0d0a 2020  n": "Excel",..  
 00000da0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00000db0: 5f69 6422 3a20 2275 7267 682d 6173 6439  _id": "urgh-asd9
-00000dc0: 2d6e 756d 662d 7175 6164 222c 0d0a 2020  -numf-quad",..  
-00000dd0: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
-00000de0: 6964 223a 2022 2369 646e 656c 736f 6e22  id": "#idnelson"
-00000df0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000e00: 736f 7572 6365 5f73 7973 7465 6d22 3a20  source_system": 
-00000e10: 225a 6f6f 6d22 2c0d 0a20 2020 2020 2020  "Zoom",..       
-00000e20: 2020 2020 2022 7469 6d65 7374 616d 705f       "timestamp_
-00000e30: 7574 6322 3a20 2232 3031 382d 3039 2d31  utc": "2018-09-1
-00000e40: 3854 3039 3a32 353a 3033 2e30 3030 5a22  8T09:25:03.000Z"
-00000e50: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000e60: 6c6f 6164 6261 7463 5f69 6422 3a20 3233  loadbatc_id": 23
-00000e70: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000e80: 7261 775f 6465 7461 696c 7322 3a20 227b  raw_details": "{
-00000e90: 736f 7572 6365 e280 a62e 2e7d 220d 0a20  source.....}".. 
-00000ea0: 2020 2020 2020 2020 2020 207d 2c20 2020             },   
-00000eb0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00000ec0: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
-00000ed0: 2020 2020 2020 2020 2273 7461 7274 5f74          "start_t
-00000ee0: 696d 6522 3a20 2232 3031 382d 3039 2d31  ime": "2018-09-1
-00000ef0: 3854 3039 3a32 343a 3033 2e30 3030 5a22  8T09:24:03.000Z"
-00000f00: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000f10: 656e 645f 7469 6d65 223a 2022 3230 3138  end_time": "2018
-00000f20: 2d30 392d 3138 5430 393a 3235 3a30 302e  -09-18T09:25:00.
-00000f30: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
-00000f40: 2020 2020 226c 6f67 5f64 7572 6174 696f      "log_duratio
-00000f50: 6e22 3a20 3630 3030 302c 0d0a 2020 2020  n": 60000,..    
-00000f60: 2020 2020 2020 2020 2263 6963 6b5f 636f          "cick_co
-00000f70: 756e 7422 3a20 3130 3030 2c0d 0a20 2020  unt": 1000,..   
-00000f80: 2020 2020 2020 2020 2022 6b65 7973 7472           "keystr
-00000f90: 6f6b 655f 636f 756e 7422 3a20 3233 3030  oke_count": 2300
-00000fa0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00000fb0: 2261 7070 6c69 6361 7469 6f6e 223a 2022  "application": "
-00000fc0: 4578 6365 6c22 2c0d 0a20 2020 2020 2020  Excel",..       
-00000fd0: 2020 2020 2022 6576 656e 745f 6964 223a       "event_id":
-00000fe0: 2022 7572 6768 2d61 7364 392d 6e75 6d66   "urgh-asd9-numf
-00000ff0: 2d71 7561 6422 2c0d 0a20 2020 2020 2020  -quad",..       
-00001000: 2020 2020 2022 7573 6572 5f69 6422 3a20       "user_id": 
-00001010: 2223 6964 6e65 6c73 6f6e 222c 0d0a 2020  "#idnelson",..  
-00001020: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
-00001030: 655f 7379 7374 656d 223a 2022 5a6f 6f6d  e_system": "Zoom
-00001040: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001050: 2274 696d 6573 7461 6d70 5f75 7463 223a  "timestamp_utc":
-00001060: 2022 3230 3138 2d30 392d 3138 5430 393a   "2018-09-18T09:
-00001070: 3235 3a30 332e 3030 305a 222c 0d0a 2020  25:03.000Z",..  
-00001080: 2020 2020 2020 2020 2020 226c 6f61 6462            "loadb
-00001090: 6174 635f 6964 223a 2032 332c 0d0a 2020  atc_id": 23,..  
-000010a0: 2020 2020 2020 2020 2020 2272 6177 5f64            "raw_d
-000010b0: 6574 6169 6c73 223a 2022 7b73 6f75 7263  etails": "{sourc
-000010c0: 65e2 80a6 2e2e 7d22 0d0a 2020 2020 2020  e.....}"..      
-000010d0: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-000010e0: 205d 2c0d 0a20 2020 2020 2020 2022 6861   ],..        "ha
-000010f0: 7368 5f31 223a 2022 6438 3239 3865 3838  sh_1": "d8298e88
-00001100: 6139 3239 6465 3233 6162 3162 6362 3036  a929de23ab1bcb06
-00001110: 6637 6130 3564 3065 3639 3466 3837 3166  f7a05d0e694f871f
-00001120: 6231 3565 6633 3138 3030 6438 3032 3764  b15ef31800d8027d
-00001130: 3066 3736 6132 6666 222c 0d0a 2020 2020  0f76a2ff",..    
-00001140: 2020 2020 2268 6173 685f 3222 3a20 2233      "hash_2": "3
-00001150: 6261 6561 3731 6537 6564 6362 3862 3861  baea71e7edcb8b8a
-00001160: 6134 3431 3766 6236 3430 6330 6661 3064  a4417fb640c0fa0d
-00001170: 3766 3937 3931 6338 6132 6231 3763 6133  7f9791c8a2b17ca3
-00001180: 6634 3939 6431 3066 3761 3433 6463 6422  f499d10f7a43dcd"
-00001190: 2c0d 0a20 2020 2020 2020 2022 6372 6561  ,..        "crea
-000011a0: 7465 645f 7469 6d65 223a 2022 3230 3233  ted_time": "2023
-000011b0: 2d30 322d 3231 5431 323a 3334 3a35 365a  -02-21T12:34:56Z
-000011c0: 220d 0a20 2020 2020 2020 207d 0d0a 2020  "..        }..  
-000011d0: 2020 5d0d 0a0d 0a20 2020 2070 6750 726f    ]....    pgPro
-000011e0: 7669 6465 722e 7075 626c 6973 6828 6461  vider.publish(da
-000011f0: 7461 290d 0a0d 0a                        ta)....
+00000db0: 5f67 7569 6422 3a20 2275 7267 682d 6173  _guid": "urgh-as
+00000dc0: 6439 2d6e 756d 662d 7175 6164 222c 0d0a  d9-numf-quad",..
+00000dd0: 2020 2020 2020 2020 2020 2020 2275 7365              "use
+00000de0: 725f 6964 223a 2022 2369 646e 656c 736f  r_id": "#idnelso
+00000df0: 6e22 2c0d 0a20 2020 2020 2020 2020 2020  n",..           
+00000e00: 2022 736f 7572 6365 5f73 7973 7465 6d22   "source_system"
+00000e10: 3a20 225a 6f6f 6d22 2c0d 0a20 2020 2020  : "Zoom",..     
+00000e20: 2020 2020 2020 2022 7469 6d65 7374 616d         "timestam
+00000e30: 705f 7574 6322 3a20 2232 3031 382d 3039  p_utc": "2018-09
+00000e40: 2d31 3854 3039 3a32 353a 3033 2e30 3030  -18T09:25:03.000
+00000e50: 5a22 2c0d 0a20 2020 2020 2020 2020 2020  Z",..           
+00000e60: 2022 6c6f 6164 6261 7463 5f69 6422 3a20   "loadbatc_id": 
+00000e70: 3233 2c0d 0a20 2020 2020 2020 2020 2020  23,..           
+00000e80: 2022 7261 775f 6465 7461 696c 7322 3a20   "raw_details": 
+00000e90: 227b 736f 7572 6365 e280 a62e 2e7d 220d  "{source.....}".
+00000ea0: 0a20 2020 2020 2020 2020 2020 207d 2c20  .            }, 
+00000eb0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00000ec0: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
+00000ed0: 2020 2020 2020 2020 2020 2273 7461 7274            "start
+00000ee0: 5f74 696d 6522 3a20 2232 3031 382d 3039  _time": "2018-09
+00000ef0: 2d31 3854 3039 3a32 343a 3033 2e30 3030  -18T09:24:03.000
+00000f00: 5a22 2c0d 0a20 2020 2020 2020 2020 2020  Z",..           
+00000f10: 2022 656e 645f 7469 6d65 223a 2022 3230   "end_time": "20
+00000f20: 3138 2d30 392d 3138 5430 393a 3235 3a30  18-09-18T09:25:0
+00000f30: 302e 3030 305a 222c 0d0a 2020 2020 2020  0.000Z",..      
+00000f40: 2020 2020 2020 226c 6f67 5f64 7572 6174        "log_durat
+00000f50: 696f 6e22 3a20 3630 3030 302c 0d0a 2020  ion": 60000,..  
+00000f60: 2020 2020 2020 2020 2020 2263 6963 6b5f            "cick_
+00000f70: 636f 756e 7422 3a20 3130 3030 2c0d 0a20  count": 1000,.. 
+00000f80: 2020 2020 2020 2020 2020 2022 6b65 7973             "keys
+00000f90: 7472 6f6b 655f 636f 756e 7422 3a20 3233  troke_count": 23
+00000fa0: 3030 302c 0d0a 2020 2020 2020 2020 2020  000,..          
+00000fb0: 2020 2261 7070 6c69 6361 7469 6f6e 223a    "application":
+00000fc0: 2022 4578 6365 6c22 2c0d 0a20 2020 2020   "Excel",..     
+00000fd0: 2020 2020 2020 2022 6576 656e 745f 6775         "event_gu
+00000fe0: 6964 223a 2022 7572 6768 2d61 7364 392d  id": "urgh-asd9-
+00000ff0: 6e75 6d66 2d71 7561 6422 2c0d 0a20 2020  numf-quad",..   
+00001000: 2020 2020 2020 2020 2022 7573 6572 5f69           "user_i
+00001010: 6422 3a20 2223 6964 6e65 6c73 6f6e 222c  d": "#idnelson",
+00001020: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
+00001030: 6f75 7263 655f 7379 7374 656d 223a 2022  ource_system": "
+00001040: 5a6f 6f6d 222c 0d0a 2020 2020 2020 2020  Zoom",..        
+00001050: 2020 2020 2274 696d 6573 7461 6d70 5f75      "timestamp_u
+00001060: 7463 223a 2022 3230 3138 2d30 392d 3138  tc": "2018-09-18
+00001070: 5430 393a 3235 3a30 332e 3030 305a 222c  T09:25:03.000Z",
+00001080: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
+00001090: 6f61 6462 6174 635f 6964 223a 2032 332c  oadbatc_id": 23,
+000010a0: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
+000010b0: 6177 5f64 6574 6169 6c73 223a 2022 7b73  aw_details": "{s
+000010c0: 6f75 7263 65e2 80a6 2e2e 7d22 0d0a 2020  ource.....}"..  
+000010d0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+000010e0: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
+000010f0: 2022 6861 7368 5f31 223a 2022 6438 3239   "hash_1": "d829
+00001100: 3865 3838 6139 3239 6465 3233 6162 3162  8e88a929de23ab1b
+00001110: 6362 3036 6637 6130 3564 3065 3639 3466  cb06f7a05d0e694f
+00001120: 3837 3166 6231 3565 6633 3138 3030 6438  871fb15ef31800d8
+00001130: 3032 3764 3066 3736 6132 6666 222c 0d0a  027d0f76a2ff",..
+00001140: 2020 2020 2020 2020 2268 6173 685f 3222          "hash_2"
+00001150: 3a20 2233 6261 6561 3731 6537 6564 6362  : "3baea71e7edcb
+00001160: 3862 3861 6134 3431 3766 6236 3430 6330  8b8aa4417fb640c0
+00001170: 6661 3064 3766 3937 3931 6338 6132 6231  fa0d7f9791c8a2b1
+00001180: 3763 6133 6634 3939 6431 3066 3761 3433  7ca3f499d10f7a43
+00001190: 6463 6422 2c0d 0a20 2020 2020 2020 2022  dcd",..        "
+000011a0: 6372 6561 7465 645f 7469 6d65 223a 2022  created_time": "
+000011b0: 3230 3233 2d30 322d 3231 5431 323a 3334  2023-02-21T12:34
+000011c0: 3a35 365a 220d 0a20 2020 2020 2020 207d  :56Z"..        }
+000011d0: 0d0a 2020 2020 5d0d 0a0d 0a20 2020 2070  ..    ]....    p
+000011e0: 6750 726f 7669 6465 722e 7075 626c 6973  gProvider.publis
+000011f0: 6828 6461 7461 290d 0a0d 0a              h(data)....
```

### Comparing `platinumtools-0.4.4/test_scenarios/test_scheduling.py` & `platinumtools-0.4.5/test_scenarios/test_scheduling.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,286 +54,286 @@
 00000350: 2020 2022 6369 636b 5f63 6f75 6e74 223a     "cick_count":
 00000360: 2031 3030 302c 0d0a 2020 2020 2020 2020   1000,..        
 00000370: 2020 2020 226b 6579 7374 726f 6b65 5f63      "keystroke_c
 00000380: 6f75 6e74 223a 2032 3330 3030 2c0d 0a20  ount": 23000,.. 
 00000390: 2020 2020 2020 2020 2020 2022 6170 706c             "appl
 000003a0: 6963 6174 696f 6e22 3a20 2245 7863 656c  ication": "Excel
 000003b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000003c0: 2265 7665 6e74 5f69 6422 3a20 2275 7267  "event_id": "urg
-000003d0: 682d 6173 6439 2d6e 756d 662d 7175 6164  h-asd9-numf-quad
-000003e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000003f0: 2275 7365 725f 6964 223a 2022 2369 646e  "user_id": "#idn
-00000400: 656c 736f 6e22 2c0d 0a20 2020 2020 2020  elson",..       
-00000410: 2020 2020 2022 736f 7572 6365 5f73 7973       "source_sys
-00000420: 7465 6d22 3a20 225a 6f6f 6d22 2c0d 0a20  tem": "Zoom",.. 
-00000430: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
-00000440: 7374 616d 705f 7574 6322 3a20 2232 3031  stamp_utc": "201
-00000450: 382d 3039 2d31 3854 3039 3a32 353a 3033  8-09-18T09:25:03
-00000460: 2e30 3030 5a22 2c0d 0a20 2020 2020 2020  .000Z",..       
-00000470: 2020 2020 2022 6c6f 6164 6261 7463 5f69       "loadbatc_i
-00000480: 6422 3a20 3233 2c0d 0a20 2020 2020 2020  d": 23,..       
-00000490: 2020 2020 2022 7261 775f 6465 7461 696c       "raw_detail
-000004a0: 7322 3a20 227b 736f 7572 6365 e280 a62e  s": "{source....
-000004b0: 2e7d 220d 0a20 2020 2020 2020 2020 2020  .}"..           
-000004c0: 207d 2c20 2020 2020 2020 2020 2020 2020   },             
-000004d0: 200d 0a20 2020 2020 2020 2020 2020 207b   ..            {
-000004e0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
-000004f0: 7461 7274 5f74 696d 6522 3a20 2232 3031  tart_time": "201
-00000500: 382d 3039 2d31 3854 3039 3a32 343a 3033  8-09-18T09:24:03
-00000510: 2e30 3030 5a22 2c0d 0a20 2020 2020 2020  .000Z",..       
-00000520: 2020 2020 2022 656e 645f 7469 6d65 223a       "end_time":
-00000530: 2022 3230 3138 2d30 392d 3138 5430 393a   "2018-09-18T09:
-00000540: 3235 3a30 302e 3030 305a 222c 0d0a 2020  25:00.000Z",..  
-00000550: 2020 2020 2020 2020 2020 226c 6f67 5f64            "log_d
-00000560: 7572 6174 696f 6e22 3a20 3630 3030 302c  uration": 60000,
-00000570: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
-00000580: 6963 6b5f 636f 756e 7422 3a20 3130 3030  ick_count": 1000
-00000590: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000005a0: 6b65 7973 7472 6f6b 655f 636f 756e 7422  keystroke_count"
-000005b0: 3a20 3233 3030 302c 0d0a 2020 2020 2020  : 23000,..      
-000005c0: 2020 2020 2020 2261 7070 6c69 6361 7469        "applicati
-000005d0: 6f6e 223a 2022 4578 6365 6c22 2c0d 0a20  on": "Excel",.. 
-000005e0: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-000005f0: 745f 6964 223a 2022 7572 6768 2d61 7364  t_id": "urgh-asd
-00000600: 392d 6e75 6d66 2d71 7561 6422 2c0d 0a20  9-numf-quad",.. 
-00000610: 2020 2020 2020 2020 2020 2022 7573 6572             "user
-00000620: 5f69 6422 3a20 2223 6964 6e65 6c73 6f6e  _id": "#idnelson
-00000630: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000640: 2273 6f75 7263 655f 7379 7374 656d 223a  "source_system":
-00000650: 2022 5a6f 6f6d 222c 0d0a 2020 2020 2020   "Zoom",..      
-00000660: 2020 2020 2020 2274 696d 6573 7461 6d70        "timestamp
-00000670: 5f75 7463 223a 2022 3230 3138 2d30 392d  _utc": "2018-09-
-00000680: 3138 5430 393a 3235 3a30 332e 3030 305a  18T09:25:03.000Z
-00000690: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000006a0: 226c 6f61 6462 6174 635f 6964 223a 2032  "loadbatc_id": 2
-000006b0: 332c 0d0a 2020 2020 2020 2020 2020 2020  3,..            
-000006c0: 2272 6177 5f64 6574 6169 6c73 223a 2022  "raw_details": "
-000006d0: 7b73 6f75 7263 65e2 80a6 2e2e 7d22 0d0a  {source.....}"..
-000006e0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-000006f0: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
-00000700: 2020 2022 6861 7368 5f31 223a 2022 6438     "hash_1": "d8
-00000710: 3239 3865 3838 6139 3239 6465 3233 6162  298e88a929de23ab
-00000720: 3162 6362 3036 6637 6130 3564 3065 3639  1bcb06f7a05d0e69
-00000730: 3466 3837 3166 6231 3565 6633 3138 3030  4f871fb15ef31800
-00000740: 6438 3032 3764 3066 3736 6132 6666 222c  d8027d0f76a2ff",
-00000750: 0d0a 2020 2020 2020 2020 2268 6173 685f  ..        "hash_
-00000760: 3222 3a20 2233 6261 6561 3731 6537 6564  2": "3baea71e7ed
-00000770: 6362 3862 3861 6134 3431 3766 6236 3430  cb8b8aa4417fb640
-00000780: 6330 6661 3064 3766 3937 3931 6338 6132  c0fa0d7f9791c8a2
-00000790: 6231 3763 6133 6634 3939 6431 3066 3761  b17ca3f499d10f7a
-000007a0: 3433 6463 6422 2c0d 0a20 2020 2020 2020  43dcd",..       
-000007b0: 2022 6372 6561 7465 645f 7469 6d65 223a   "created_time":
-000007c0: 2022 3230 3233 2d30 322d 3231 5431 323a   "2023-02-21T12:
-000007d0: 3334 3a35 365a 220d 0a20 2020 2020 2020  34:56Z"..       
-000007e0: 207d 0d0a 2020 2020 5d0d 0a20 2020 2073   }..    ]..    s
-000007f0: 696e 676c 655f 7363 6865 6475 6c65 7220  ingle_scheduler 
-00000800: 3d20 5369 6e67 6c65 5351 534a 6f62 5363  = SingleSQSJobSc
-00000810: 6865 6475 6c65 7228 0d0a 2020 2020 2020  heduler(..      
-00000820: 2020 7261 7750 7562 6c69 7368 696e 5374    rawPublishinSt
-00000830: 7261 7465 6769 6573 3d5b 6d6f 636b 4442  rategies=[mockDB
-00000840: 5072 6f76 6964 6572 5d2c 0d0a 2020 2020  Provider],..    
-00000850: 2020 2020 7371 735f 656e 706f 696e 743d      sqs_enpoint=
-00000860: 2268 7474 7073 3a2f 2f73 7173 2e75 732d  "https://sqs.us-
-00000870: 6561 7374 2d31 2e61 6d61 7a6f 6e61 7773  east-1.amazonaws
-00000880: 2e63 6f6d 2f37 3936 3532 3232 3738 3832  .com/79652227882
-00000890: 372f 4d6f 636b 5175 6575 652e 6669 666f  7/MockQueue.fifo
-000008a0: 220d 0a20 2020 2020 2020 2029 0d0a 2020  "..        )..  
-000008b0: 2020 0d0a 2020 2020 0d0a 2020 2020 7369    ..    ..    si
-000008c0: 6e67 6c65 5f73 6368 6564 756c 6572 2e70  ngle_scheduler.p
-000008d0: 7562 6c69 7368 5261 7728 6576 656e 7473  ublishRaw(events
-000008e0: 3d64 6174 615f 7265 6365 6976 6564 2920  =data_received) 
-000008f0: 2353 686f 756c 6420 7072 696e 7420 7468  #Should print th
-00000900: 6520 6576 656e 7420 7468 6174 2069 7320  e event that is 
-00000910: 6265 696e 6720 7075 626c 7369 6865 640d  being publsihed.
-00000920: 0a20 2020 2073 696e 676c 655f 7363 6865  .    single_sche
-00000930: 6475 6c65 722e 7363 6865 6475 6c65 4a6f  duler.scheduleJo
-00000940: 6228 6576 656e 7473 3d64 6174 615f 7265  b(events=data_re
-00000950: 6365 6976 6564 2920 2353 686f 756c 6420  ceived) #Should 
-00000960: 6163 7475 616c 6c79 2073 6368 6564 756c  actually schedul
-00000970: 6520 7468 6520 6a6f 622e 0d0a 2020 2020  e the job...    
-00000980: 0d0a 2020 2020 6173 7365 7274 286c 656e  ..    assert(len
-00000990: 286d 6f63 6b44 4250 726f 7669 6465 722e  (mockDBProvider.
-000009a0: 6462 293e 3d31 290d 0a0d 0a0d 0a64 6566  db)>=1)......def
-000009b0: 2074 6573 745f 696e 7465 6772 6174 696f   test_integratio
-000009c0: 6e5f 7371 735f 7363 6865 6475 6c65 725f  n_sqs_scheduler_
-000009d0: 706f 7374 6772 6573 7150 726f 7669 6465  postgresqProvide
-000009e0: 7228 293a 0d0a 2020 2020 2222 2259 6f75  r():..    """You
-000009f0: 2073 7469 6c6c 2068 6176 6520 746f 206d   still have to m
-00000a00: 616e 7561 6c6c 7920 6368 6563 6b20 7468  anually check th
-00000a10: 6520 706f 7374 6772 6573 2064 6174 6162  e postgres datab
-00000a20: 6173 6520 746f 2073 6565 2069 6620 6974  ase to see if it
-00000a30: 2077 6173 2061 6374 7561 6c6c 7920 6d6f   was actually mo
-00000a40: 6469 6669 6564 2e0d 0a20 2020 2022 2222  dified...    """
-00000a50: 0d0a 2020 2020 6372 6564 656e 7469 616c  ..    credential
-00000a60: 7320 3d20 7b0d 0a20 2020 2020 2020 2027  s = {..        '
-00000a70: 5553 4552 4e41 4d45 273a 2022 706f 7374  USERNAME': "post
-00000a80: 6772 6573 222c 0d0a 2020 2020 2020 2020  gres",..        
-00000a90: 2750 4153 5357 4f52 4427 3a20 2264 4475  'PASSWORD': "dDu
-00000aa0: 656c 6c65 7231 3233 6172 614d 3d21 222c  eller123araM=!",
-00000ab0: 0d0a 2020 2020 2020 2020 2248 4f53 5422  ..        "HOST"
-00000ac0: 3a20 2274 6573 742d 6464 616e 616c 7974  : "test-ddanalyt
-00000ad0: 6963 732d 7264 732d 7632 2e63 7063 7769  ics-rds-v2.cpcwi
-00000ae0: 3230 6b32 7167 672e 7573 2d65 6173 742d  20k2qgg.us-east-
-00000af0: 312e 7264 732e 616d 617a 6f6e 6177 732e  1.rds.amazonaws.
-00000b00: 636f 6d22 2c0d 0a20 2020 2020 2020 2022  com",..        "
-00000b10: 4442 223a 2022 7631 5f32 220d 0a20 2020  DB": "v1_2"..   
-00000b20: 207d 0d0a 0d0a 2020 2020 7365 7474 696e   }....    settin
-00000b30: 6773 203d 207b 0d0a 2020 2020 2020 2020  gs = {..        
-00000b40: 2254 4142 4c45 4e41 4d45 223a 2022 7374  "TABLENAME": "st
-00000b50: 6167 696e 675f 6576 656e 7473 222c 0d0a  aging_events",..
-00000b60: 2020 2020 2020 2020 2243 4f4c 554d 4e5f          "COLUMN_
-00000b70: 4e41 4d45 5322 3a20 5b22 6775 6964 222c  NAMES": ["guid",
-00000b80: 2022 7665 7273 696f 6e22 2c20 2273 6f75   "version", "sou
-00000b90: 7263 655f 6775 6964 222c 2022 7479 7065  rce_guid", "type
-00000ba0: 222c 2022 6f72 6761 6e69 7a61 7469 6f6e  ", "organization
-00000bb0: 5f67 7569 6422 2c20 2275 7365 725f 6775  _guid", "user_gu
-00000bc0: 6964 222c 2022 6f70 6572 6174 696f 6e22  id", "operation"
-00000bd0: 2c20 2269 7465 6d5f 636f 756e 7422 2c20  , "item_count", 
-00000be0: 2264 6574 6169 6c73 222c 2022 6861 7368  "details", "hash
-00000bf0: 5f31 222c 2022 6861 7368 5f32 222c 2022  _1", "hash_2", "
-00000c00: 6372 6561 7465 645f 7469 6d65 225d 2c0d  created_time"],.
-00000c10: 0a20 2020 207d 0d0a 2020 2020 6462 5072  .    }..    dbPr
-00000c20: 6f76 6964 6572 203d 2050 6f73 7467 7265  ovider = Postgre
-00000c30: 5351 4c50 726f 7669 6465 7228 6372 6564  SQLProvider(cred
-00000c40: 656e 7469 616c 733d 6372 6564 656e 7469  entials=credenti
-00000c50: 616c 732c 2073 6574 7469 6e67 733d 7365  als, settings=se
-00000c60: 7474 696e 6773 290d 0a20 2020 2072 616e  ttings)..    ran
-00000c70: 646f 6d5f 6964 656e 7469 6669 6572 203d  dom_identifier =
-00000c80: 2055 7469 6c73 2e63 7265 6174 6552 616e   Utils.createRan
-00000c90: 646f 6d53 7472 2829 0d0a 2020 2020 6461  domStr()..    da
-00000ca0: 7461 5f72 6563 6569 7665 6420 3d20 5b0d  ta_received = [.
-00000cb0: 0a0d 0a20 2020 2020 2020 207b 0d0a 2020  ...        {..  
-00000cc0: 2020 2020 2020 2267 7569 6422 3a20 2231        "guid": "1
-00000cd0: 3233 6534 3536 372d 6538 3962 2d31 3264  23e4567-e89b-12d
-00000ce0: 332d 6134 3536 2d22 2b72 616e 646f 6d5f  3-a456-"+random_
-00000cf0: 6964 656e 7469 6669 6572 2c0d 0a20 2020  identifier,..   
-00000d00: 2020 2020 2022 7665 7273 696f 6e22 3a20       "version": 
-00000d10: 2231 2e30 222c 0d0a 2020 2020 2020 2020  "1.0",..        
-00000d20: 2273 6f75 7263 655f 6775 6964 223a 2022  "source_guid": "
-00000d30: 3230 3233 2d30 322d 3231 5431 323a 3334  2023-02-21T12:34
-00000d40: 3a35 365a 222c 0d0a 2020 2020 2020 2020  :56Z",..        
-00000d50: 2274 7970 6522 3a20 224d 4f43 4b5f 5459  "type": "MOCK_TY
-00000d60: 5045 222c 0d0a 2020 2020 2020 2020 226f  PE",..        "o
-00000d70: 7267 616e 697a 6174 696f 6e5f 6775 6964  rganization_guid
-00000d80: 223a 2022 6f72 6731 3233 222c 0d0a 2020  ": "org123",..  
-00000d90: 2020 2020 2020 2275 7365 725f 6775 6964        "user_guid
-00000da0: 223a 2022 3132 3365 3435 3637 2d65 3839  ": "123e4567-e89
-00000db0: 622d 3132 6433 2d61 3435 362d 3432 3636  b-12d3-a456-4266
-00000dc0: 3535 3434 3030 3030 222c 0d0a 2020 2020  55440000",..    
-00000dd0: 2020 2020 226f 7065 7261 7469 6f6e 223a      "operation":
-00000de0: 2022 4d4f 434b 5f4f 5045 5241 5449 4f4e   "MOCK_OPERATION
-00000df0: 222c 0d0a 2020 2020 2020 2020 2269 7465  ",..        "ite
-00000e00: 6d5f 636f 756e 7422 3a20 2233 222c 0d0a  m_count": "3",..
-00000e10: 2020 2020 2020 2020 2264 6574 6169 6c73          "details
-00000e20: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-00000e30: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00000e40: 2022 7374 6172 745f 7469 6d65 223a 2022   "start_time": "
-00000e50: 3230 3138 2d30 392d 3138 5430 393a 3234  2018-09-18T09:24
-00000e60: 3a30 332e 3030 305a 222c 0d0a 2020 2020  :03.000Z",..    
-00000e70: 2020 2020 2020 2020 2265 6e64 5f74 696d          "end_tim
-00000e80: 6522 3a20 2232 3031 382d 3039 2d31 3854  e": "2018-09-18T
-00000e90: 3039 3a32 353a 3030 2e30 3030 5a22 2c0d  09:25:00.000Z",.
-00000ea0: 0a20 2020 2020 2020 2020 2020 2022 6c6f  .            "lo
-00000eb0: 675f 6475 7261 7469 6f6e 223a 2036 3030  g_duration": 600
-00000ec0: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
-00000ed0: 2022 6369 636b 5f63 6f75 6e74 223a 2031   "cick_count": 1
-00000ee0: 3030 302c 0d0a 2020 2020 2020 2020 2020  000,..          
-00000ef0: 2020 226b 6579 7374 726f 6b65 5f63 6f75    "keystroke_cou
-00000f00: 6e74 223a 2032 3330 3030 2c0d 0a20 2020  nt": 23000,..   
-00000f10: 2020 2020 2020 2020 2022 6170 706c 6963           "applic
-00000f20: 6174 696f 6e22 3a20 2245 7863 656c 222c  ation": "Excel",
-00000f30: 0d0a 2020 2020 2020 2020 2020 2020 2265  ..            "e
-00000f40: 7665 6e74 5f69 6422 3a20 2275 7267 682d  vent_id": "urgh-
-00000f50: 6173 6439 2d6e 756d 662d 7175 6164 222c  asd9-numf-quad",
-00000f60: 0d0a 2020 2020 2020 2020 2020 2020 2275  ..            "u
-00000f70: 7365 725f 6964 223a 2022 2369 646e 656c  ser_id": "#idnel
-00000f80: 736f 6e22 2c0d 0a20 2020 2020 2020 2020  son",..         
-00000f90: 2020 2022 736f 7572 6365 5f73 7973 7465     "source_syste
-00000fa0: 6d22 3a20 225a 6f6f 6d22 2c0d 0a20 2020  m": "Zoom",..   
-00000fb0: 2020 2020 2020 2020 2022 7469 6d65 7374           "timest
-00000fc0: 616d 705f 7574 6322 3a20 2232 3031 382d  amp_utc": "2018-
-00000fd0: 3039 2d31 3854 3039 3a32 353a 3033 2e30  09-18T09:25:03.0
-00000fe0: 3030 5a22 2c0d 0a20 2020 2020 2020 2020  00Z",..         
-00000ff0: 2020 2022 6c6f 6164 6261 7463 5f69 6422     "loadbatc_id"
-00001000: 3a20 3233 2c0d 0a20 2020 2020 2020 2020  : 23,..         
-00001010: 2020 2022 7261 775f 6465 7461 696c 7322     "raw_details"
-00001020: 3a20 227b 736f 7572 6365 e280 a62e 2e7d  : "{source.....}
-00001030: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
-00001040: 2c20 2020 2020 2020 2020 2020 2020 200d  ,              .
-00001050: 0a20 2020 2020 2020 2020 2020 207b 0d0a  .            {..
-00001060: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00001070: 7274 5f74 696d 6522 3a20 2232 3031 382d  rt_time": "2018-
-00001080: 3039 2d31 3854 3039 3a32 343a 3033 2e30  09-18T09:24:03.0
-00001090: 3030 5a22 2c0d 0a20 2020 2020 2020 2020  00Z",..         
-000010a0: 2020 2022 656e 645f 7469 6d65 223a 2022     "end_time": "
-000010b0: 3230 3138 2d30 392d 3138 5430 393a 3235  2018-09-18T09:25
-000010c0: 3a30 302e 3030 305a 222c 0d0a 2020 2020  :00.000Z",..    
-000010d0: 2020 2020 2020 2020 226c 6f67 5f64 7572          "log_dur
-000010e0: 6174 696f 6e22 3a20 3630 3030 302c 0d0a  ation": 60000,..
-000010f0: 2020 2020 2020 2020 2020 2020 2263 6963              "cic
-00001100: 6b5f 636f 756e 7422 3a20 3130 3030 2c0d  k_count": 1000,.
-00001110: 0a20 2020 2020 2020 2020 2020 2022 6b65  .            "ke
-00001120: 7973 7472 6f6b 655f 636f 756e 7422 3a20  ystroke_count": 
-00001130: 3233 3030 302c 0d0a 2020 2020 2020 2020  23000,..        
-00001140: 2020 2020 2261 7070 6c69 6361 7469 6f6e      "application
-00001150: 223a 2022 4578 6365 6c22 2c0d 0a20 2020  ": "Excel",..   
-00001160: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
-00001170: 6964 223a 2022 7572 6768 2d61 7364 392d  id": "urgh-asd9-
-00001180: 6e75 6d66 2d71 7561 6422 2c0d 0a20 2020  numf-quad",..   
-00001190: 2020 2020 2020 2020 2022 7573 6572 5f69           "user_i
-000011a0: 6422 3a20 2223 6964 6e65 6c73 6f6e 222c  d": "#idnelson",
-000011b0: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
-000011c0: 6f75 7263 655f 7379 7374 656d 223a 2022  ource_system": "
-000011d0: 5a6f 6f6d 222c 0d0a 2020 2020 2020 2020  Zoom",..        
-000011e0: 2020 2020 2274 696d 6573 7461 6d70 5f75      "timestamp_u
-000011f0: 7463 223a 2022 3230 3138 2d30 392d 3138  tc": "2018-09-18
-00001200: 5430 393a 3235 3a30 332e 3030 305a 222c  T09:25:03.000Z",
-00001210: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
-00001220: 6f61 6462 6174 635f 6964 223a 2032 332c  oadbatc_id": 23,
-00001230: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-00001240: 6177 5f64 6574 6169 6c73 223a 2022 7b73  aw_details": "{s
-00001250: 6f75 7263 65e2 80a6 2e2e 7d22 0d0a 2020  ource.....}"..  
-00001260: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00001270: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-00001280: 2022 6861 7368 5f31 223a 2022 6438 3239   "hash_1": "d829
-00001290: 3865 3838 6139 3239 6465 3233 6162 3162  8e88a929de23ab1b
-000012a0: 6362 3036 6637 6130 3564 3065 3639 3466  cb06f7a05d0e694f
-000012b0: 3837 3166 6231 3565 6633 3138 3030 6438  871fb15ef31800d8
-000012c0: 3032 3764 3066 3736 6132 6666 222c 0d0a  027d0f76a2ff",..
-000012d0: 2020 2020 2020 2020 2268 6173 685f 3222          "hash_2"
-000012e0: 3a20 2233 6261 6561 3731 6537 6564 6362  : "3baea71e7edcb
-000012f0: 3862 3861 6134 3431 3766 6236 3430 6330  8b8aa4417fb640c0
-00001300: 6661 3064 3766 3937 3931 6338 6132 6231  fa0d7f9791c8a2b1
-00001310: 3763 6133 6634 3939 6431 3066 3761 3433  7ca3f499d10f7a43
-00001320: 6463 6422 2c0d 0a20 2020 2020 2020 2022  dcd",..        "
-00001330: 6372 6561 7465 645f 7469 6d65 223a 2022  created_time": "
-00001340: 3230 3233 2d30 322d 3231 5431 323a 3334  2023-02-21T12:34
-00001350: 3a35 365a 220d 0a20 2020 2020 2020 207d  :56Z"..        }
-00001360: 0d0a 2020 2020 5d0d 0a20 2020 2073 696e  ..    ]..    sin
-00001370: 676c 655f 7363 6865 6475 6c65 7220 3d20  gle_scheduler = 
-00001380: 5369 6e67 6c65 5351 534a 6f62 5363 6865  SingleSQSJobSche
-00001390: 6475 6c65 7228 0d0a 2020 2020 2020 2020  duler(..        
-000013a0: 7261 7750 7562 6c69 7368 696e 5374 7261  rawPublishinStra
-000013b0: 7465 6769 6573 3d5b 6462 5072 6f76 6964  tegies=[dbProvid
-000013c0: 6572 5d2c 0d0a 2020 2020 2020 2020 7371  er],..        sq
-000013d0: 735f 656e 706f 696e 743d 2268 7474 7073  s_enpoint="https
-000013e0: 3a2f 2f73 7173 2e75 732d 6561 7374 2d31  ://sqs.us-east-1
-000013f0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f37  .amazonaws.com/7
-00001400: 3936 3532 3232 3738 3832 372f 4d6f 636b  96522278827/Mock
-00001410: 5175 6575 652e 6669 666f 220d 0a20 2020  Queue.fifo"..   
-00001420: 2020 2020 2029 0d0a 2020 2020 0d0a 2020       )..    ..  
-00001430: 2020 0d0a 2020 2020 7369 6e67 6c65 5f73    ..    single_s
-00001440: 6368 6564 756c 6572 2e70 7562 6c69 7368  cheduler.publish
-00001450: 5261 7728 6576 656e 7473 3d64 6174 615f  Raw(events=data_
-00001460: 7265 6365 6976 6564 2920 2353 686f 756c  received) #Shoul
-00001470: 6420 7072 696e 7420 7468 6520 6576 656e  d print the even
-00001480: 7420 7468 6174 2069 7320 6265 696e 6720  t that is being 
-00001490: 7075 626c 7369 6865 640d 0a20 2020 2073  publsihed..    s
-000014a0: 696e 676c 655f 7363 6865 6475 6c65 722e  ingle_scheduler.
-000014b0: 7363 6865 6475 6c65 4a6f 6228 6576 656e  scheduleJob(even
-000014c0: 7473 3d64 6174 615f 7265 6365 6976 6564  ts=data_received
-000014d0: 2920 2353 686f 756c 6420 6163 7475 616c  ) #Should actual
-000014e0: 6c79 2073 6368 6564 756c 6520 7468 6520  ly schedule the 
-000014f0: 6a6f 622e 0d0a 2020 2020 0d0a 2020 2020  job...    ..    
-00001500: 2320 6173 7365 7274 286c 656e 286d 6f63  # assert(len(moc
-00001510: 6b44 4250 726f 7669 6465 722e 6462 293e  kDBProvider.db)>
-00001520: 3d31 290d 0a0d 0a                        =1)....
+000003c0: 2265 7665 6e74 5f67 7569 6422 3a20 2275  "event_guid": "u
+000003d0: 7267 682d 6173 6439 2d6e 756d 662d 7175  rgh-asd9-numf-qu
+000003e0: 6164 222c 0d0a 2020 2020 2020 2020 2020  ad",..          
+000003f0: 2020 2275 7365 725f 6964 223a 2022 2369    "user_id": "#i
+00000400: 646e 656c 736f 6e22 2c0d 0a20 2020 2020  dnelson",..     
+00000410: 2020 2020 2020 2022 736f 7572 6365 5f73         "source_s
+00000420: 7973 7465 6d22 3a20 225a 6f6f 6d22 2c0d  ystem": "Zoom",.
+00000430: 0a20 2020 2020 2020 2020 2020 2022 7469  .            "ti
+00000440: 6d65 7374 616d 705f 7574 6322 3a20 2232  mestamp_utc": "2
+00000450: 3031 382d 3039 2d31 3854 3039 3a32 353a  018-09-18T09:25:
+00000460: 3033 2e30 3030 5a22 2c0d 0a20 2020 2020  03.000Z",..     
+00000470: 2020 2020 2020 2022 6c6f 6164 6261 7463         "loadbatc
+00000480: 5f69 6422 3a20 3233 2c0d 0a20 2020 2020  _id": 23,..     
+00000490: 2020 2020 2020 2022 7261 775f 6465 7461         "raw_deta
+000004a0: 696c 7322 3a20 227b 736f 7572 6365 e280  ils": "{source..
+000004b0: a62e 2e7d 220d 0a20 2020 2020 2020 2020  ...}"..         
+000004c0: 2020 207d 2c20 2020 2020 2020 2020 2020     },           
+000004d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000004e0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000004f0: 2273 7461 7274 5f74 696d 6522 3a20 2232  "start_time": "2
+00000500: 3031 382d 3039 2d31 3854 3039 3a32 343a  018-09-18T09:24:
+00000510: 3033 2e30 3030 5a22 2c0d 0a20 2020 2020  03.000Z",..     
+00000520: 2020 2020 2020 2022 656e 645f 7469 6d65         "end_time
+00000530: 223a 2022 3230 3138 2d30 392d 3138 5430  ": "2018-09-18T0
+00000540: 393a 3235 3a30 302e 3030 305a 222c 0d0a  9:25:00.000Z",..
+00000550: 2020 2020 2020 2020 2020 2020 226c 6f67              "log
+00000560: 5f64 7572 6174 696f 6e22 3a20 3630 3030  _duration": 6000
+00000570: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00000580: 2263 6963 6b5f 636f 756e 7422 3a20 3130  "cick_count": 10
+00000590: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
+000005a0: 2022 6b65 7973 7472 6f6b 655f 636f 756e   "keystroke_coun
+000005b0: 7422 3a20 3233 3030 302c 0d0a 2020 2020  t": 23000,..    
+000005c0: 2020 2020 2020 2020 2261 7070 6c69 6361          "applica
+000005d0: 7469 6f6e 223a 2022 4578 6365 6c22 2c0d  tion": "Excel",.
+000005e0: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+000005f0: 656e 745f 6775 6964 223a 2022 7572 6768  ent_guid": "urgh
+00000600: 2d61 7364 392d 6e75 6d66 2d71 7561 6422  -asd9-numf-quad"
+00000610: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000620: 7573 6572 5f69 6422 3a20 2223 6964 6e65  user_id": "#idne
+00000630: 6c73 6f6e 222c 0d0a 2020 2020 2020 2020  lson",..        
+00000640: 2020 2020 2273 6f75 7263 655f 7379 7374      "source_syst
+00000650: 656d 223a 2022 5a6f 6f6d 222c 0d0a 2020  em": "Zoom",..  
+00000660: 2020 2020 2020 2020 2020 2274 696d 6573            "times
+00000670: 7461 6d70 5f75 7463 223a 2022 3230 3138  tamp_utc": "2018
+00000680: 2d30 392d 3138 5430 393a 3235 3a30 332e  -09-18T09:25:03.
+00000690: 3030 305a 222c 0d0a 2020 2020 2020 2020  000Z",..        
+000006a0: 2020 2020 226c 6f61 6462 6174 635f 6964      "loadbatc_id
+000006b0: 223a 2032 332c 0d0a 2020 2020 2020 2020  ": 23,..        
+000006c0: 2020 2020 2272 6177 5f64 6574 6169 6c73      "raw_details
+000006d0: 223a 2022 7b73 6f75 7263 65e2 80a6 2e2e  ": "{source.....
+000006e0: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
+000006f0: 7d0d 0a20 2020 2020 2020 205d 2c0d 0a20  }..        ],.. 
+00000700: 2020 2020 2020 2022 6861 7368 5f31 223a         "hash_1":
+00000710: 2022 6438 3239 3865 3838 6139 3239 6465   "d8298e88a929de
+00000720: 3233 6162 3162 6362 3036 6637 6130 3564  23ab1bcb06f7a05d
+00000730: 3065 3639 3466 3837 3166 6231 3565 6633  0e694f871fb15ef3
+00000740: 3138 3030 6438 3032 3764 3066 3736 6132  1800d8027d0f76a2
+00000750: 6666 222c 0d0a 2020 2020 2020 2020 2268  ff",..        "h
+00000760: 6173 685f 3222 3a20 2233 6261 6561 3731  ash_2": "3baea71
+00000770: 6537 6564 6362 3862 3861 6134 3431 3766  e7edcb8b8aa4417f
+00000780: 6236 3430 6330 6661 3064 3766 3937 3931  b640c0fa0d7f9791
+00000790: 6338 6132 6231 3763 6133 6634 3939 6431  c8a2b17ca3f499d1
+000007a0: 3066 3761 3433 6463 6422 2c0d 0a20 2020  0f7a43dcd",..   
+000007b0: 2020 2020 2022 6372 6561 7465 645f 7469       "created_ti
+000007c0: 6d65 223a 2022 3230 3233 2d30 322d 3231  me": "2023-02-21
+000007d0: 5431 323a 3334 3a35 365a 220d 0a20 2020  T12:34:56Z"..   
+000007e0: 2020 2020 207d 0d0a 2020 2020 5d0d 0a20       }..    ].. 
+000007f0: 2020 2073 696e 676c 655f 7363 6865 6475     single_schedu
+00000800: 6c65 7220 3d20 5369 6e67 6c65 5351 534a  ler = SingleSQSJ
+00000810: 6f62 5363 6865 6475 6c65 7228 0d0a 2020  obScheduler(..  
+00000820: 2020 2020 2020 7261 7750 7562 6c69 7368        rawPublish
+00000830: 696e 5374 7261 7465 6769 6573 3d5b 6d6f  inStrategies=[mo
+00000840: 636b 4442 5072 6f76 6964 6572 5d2c 0d0a  ckDBProvider],..
+00000850: 2020 2020 2020 2020 7371 735f 656e 706f          sqs_enpo
+00000860: 696e 743d 2268 7474 7073 3a2f 2f73 7173  int="https://sqs
+00000870: 2e75 732d 6561 7374 2d31 2e61 6d61 7a6f  .us-east-1.amazo
+00000880: 6e61 7773 2e63 6f6d 2f37 3936 3532 3232  naws.com/7965222
+00000890: 3738 3832 372f 4d6f 636b 5175 6575 652e  78827/MockQueue.
+000008a0: 6669 666f 220d 0a20 2020 2020 2020 2029  fifo"..        )
+000008b0: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
+000008c0: 2020 7369 6e67 6c65 5f73 6368 6564 756c    single_schedul
+000008d0: 6572 2e70 7562 6c69 7368 5261 7728 6576  er.publishRaw(ev
+000008e0: 656e 7473 3d64 6174 615f 7265 6365 6976  ents=data_receiv
+000008f0: 6564 2920 2353 686f 756c 6420 7072 696e  ed) #Should prin
+00000900: 7420 7468 6520 6576 656e 7420 7468 6174  t the event that
+00000910: 2069 7320 6265 696e 6720 7075 626c 7369   is being publsi
+00000920: 6865 640d 0a20 2020 2073 696e 676c 655f  hed..    single_
+00000930: 7363 6865 6475 6c65 722e 7363 6865 6475  scheduler.schedu
+00000940: 6c65 4a6f 6228 6576 656e 7473 3d64 6174  leJob(events=dat
+00000950: 615f 7265 6365 6976 6564 2920 2353 686f  a_received) #Sho
+00000960: 756c 6420 6163 7475 616c 6c79 2073 6368  uld actually sch
+00000970: 6564 756c 6520 7468 6520 6a6f 622e 0d0a  edule the job...
+00000980: 2020 2020 0d0a 2020 2020 6173 7365 7274      ..    assert
+00000990: 286c 656e 286d 6f63 6b44 4250 726f 7669  (len(mockDBProvi
+000009a0: 6465 722e 6462 293e 3d31 290d 0a0d 0a0d  der.db)>=1).....
+000009b0: 0a64 6566 2074 6573 745f 696e 7465 6772  .def test_integr
+000009c0: 6174 696f 6e5f 7371 735f 7363 6865 6475  ation_sqs_schedu
+000009d0: 6c65 725f 706f 7374 6772 6573 7150 726f  ler_postgresqPro
+000009e0: 7669 6465 7228 293a 0d0a 2020 2020 2222  vider():..    ""
+000009f0: 2259 6f75 2073 7469 6c6c 2068 6176 6520  "You still have 
+00000a00: 746f 206d 616e 7561 6c6c 7920 6368 6563  to manually chec
+00000a10: 6b20 7468 6520 706f 7374 6772 6573 2064  k the postgres d
+00000a20: 6174 6162 6173 6520 746f 2073 6565 2069  atabase to see i
+00000a30: 6620 6974 2077 6173 2061 6374 7561 6c6c  f it was actuall
+00000a40: 7920 6d6f 6469 6669 6564 2e0d 0a20 2020  y modified...   
+00000a50: 2022 2222 0d0a 2020 2020 6372 6564 656e   """..    creden
+00000a60: 7469 616c 7320 3d20 7b0d 0a20 2020 2020  tials = {..     
+00000a70: 2020 2027 5553 4552 4e41 4d45 273a 2022     'USERNAME': "
+00000a80: 706f 7374 6772 6573 222c 0d0a 2020 2020  postgres",..    
+00000a90: 2020 2020 2750 4153 5357 4f52 4427 3a20      'PASSWORD': 
+00000aa0: 2264 4475 656c 6c65 7231 3233 6172 614d  "dDueller123araM
+00000ab0: 3d21 222c 0d0a 2020 2020 2020 2020 2248  =!",..        "H
+00000ac0: 4f53 5422 3a20 2274 6573 742d 6464 616e  OST": "test-ddan
+00000ad0: 616c 7974 6963 732d 7264 732d 7632 2e63  alytics-rds-v2.c
+00000ae0: 7063 7769 3230 6b32 7167 672e 7573 2d65  pcwi20k2qgg.us-e
+00000af0: 6173 742d 312e 7264 732e 616d 617a 6f6e  ast-1.rds.amazon
+00000b00: 6177 732e 636f 6d22 2c0d 0a20 2020 2020  aws.com",..     
+00000b10: 2020 2022 4442 223a 2022 7631 5f32 220d     "DB": "v1_2".
+00000b20: 0a20 2020 207d 0d0a 0d0a 2020 2020 7365  .    }....    se
+00000b30: 7474 696e 6773 203d 207b 0d0a 2020 2020  ttings = {..    
+00000b40: 2020 2020 2254 4142 4c45 4e41 4d45 223a      "TABLENAME":
+00000b50: 2022 7374 6167 696e 675f 6576 656e 7473   "staging_events
+00000b60: 222c 0d0a 2020 2020 2020 2020 2243 4f4c  ",..        "COL
+00000b70: 554d 4e5f 4e41 4d45 5322 3a20 5b22 6775  UMN_NAMES": ["gu
+00000b80: 6964 222c 2022 7665 7273 696f 6e22 2c20  id", "version", 
+00000b90: 2273 6f75 7263 655f 6775 6964 222c 2022  "source_guid", "
+00000ba0: 7479 7065 222c 2022 6f72 6761 6e69 7a61  type", "organiza
+00000bb0: 7469 6f6e 5f67 7569 6422 2c20 2275 7365  tion_guid", "use
+00000bc0: 725f 6775 6964 222c 2022 6f70 6572 6174  r_guid", "operat
+00000bd0: 696f 6e22 2c20 2269 7465 6d5f 636f 756e  ion", "item_coun
+00000be0: 7422 2c20 2264 6574 6169 6c73 222c 2022  t", "details", "
+00000bf0: 6861 7368 5f31 222c 2022 6861 7368 5f32  hash_1", "hash_2
+00000c00: 222c 2022 6372 6561 7465 645f 7469 6d65  ", "created_time
+00000c10: 225d 2c0d 0a20 2020 207d 0d0a 2020 2020  "],..    }..    
+00000c20: 6462 5072 6f76 6964 6572 203d 2050 6f73  dbProvider = Pos
+00000c30: 7467 7265 5351 4c50 726f 7669 6465 7228  tgreSQLProvider(
+00000c40: 6372 6564 656e 7469 616c 733d 6372 6564  credentials=cred
+00000c50: 656e 7469 616c 732c 2073 6574 7469 6e67  entials, setting
+00000c60: 733d 7365 7474 696e 6773 290d 0a20 2020  s=settings)..   
+00000c70: 2072 616e 646f 6d5f 6964 656e 7469 6669   random_identifi
+00000c80: 6572 203d 2055 7469 6c73 2e63 7265 6174  er = Utils.creat
+00000c90: 6552 616e 646f 6d53 7472 2829 0d0a 2020  eRandomStr()..  
+00000ca0: 2020 6461 7461 5f72 6563 6569 7665 6420    data_received 
+00000cb0: 3d20 5b0d 0a0d 0a20 2020 2020 2020 207b  = [....        {
+00000cc0: 0d0a 2020 2020 2020 2020 2267 7569 6422  ..        "guid"
+00000cd0: 3a20 2231 3233 6534 3536 372d 6538 3962  : "123e4567-e89b
+00000ce0: 2d31 3264 332d 6134 3536 2d22 2b72 616e  -12d3-a456-"+ran
+00000cf0: 646f 6d5f 6964 656e 7469 6669 6572 2c0d  dom_identifier,.
+00000d00: 0a20 2020 2020 2020 2022 7665 7273 696f  .        "versio
+00000d10: 6e22 3a20 2231 2e30 222c 0d0a 2020 2020  n": "1.0",..    
+00000d20: 2020 2020 2273 6f75 7263 655f 6775 6964      "source_guid
+00000d30: 223a 2022 3230 3233 2d30 322d 3231 5431  ": "2023-02-21T1
+00000d40: 323a 3334 3a35 365a 222c 0d0a 2020 2020  2:34:56Z",..    
+00000d50: 2020 2020 2274 7970 6522 3a20 224d 4f43      "type": "MOC
+00000d60: 4b5f 5459 5045 222c 0d0a 2020 2020 2020  K_TYPE",..      
+00000d70: 2020 226f 7267 616e 697a 6174 696f 6e5f    "organization_
+00000d80: 6775 6964 223a 2022 6f72 6731 3233 222c  guid": "org123",
+00000d90: 0d0a 2020 2020 2020 2020 2275 7365 725f  ..        "user_
+00000da0: 6775 6964 223a 2022 3132 3365 3435 3637  guid": "123e4567
+00000db0: 2d65 3839 622d 3132 6433 2d61 3435 362d  -e89b-12d3-a456-
+00000dc0: 3432 3636 3535 3434 3030 3030 222c 0d0a  426655440000",..
+00000dd0: 2020 2020 2020 2020 226f 7065 7261 7469          "operati
+00000de0: 6f6e 223a 2022 4d4f 434b 5f4f 5045 5241  on": "MOCK_OPERA
+00000df0: 5449 4f4e 222c 0d0a 2020 2020 2020 2020  TION",..        
+00000e00: 2269 7465 6d5f 636f 756e 7422 3a20 2233  "item_count": "3
+00000e10: 222c 0d0a 2020 2020 2020 2020 2264 6574  ",..        "det
+00000e20: 6169 6c73 223a 205b 0d0a 2020 2020 2020  ails": [..      
+00000e30: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00000e40: 2020 2020 2022 7374 6172 745f 7469 6d65       "start_time
+00000e50: 223a 2022 3230 3138 2d30 392d 3138 5430  ": "2018-09-18T0
+00000e60: 393a 3234 3a30 332e 3030 305a 222c 0d0a  9:24:03.000Z",..
+00000e70: 2020 2020 2020 2020 2020 2020 2265 6e64              "end
+00000e80: 5f74 696d 6522 3a20 2232 3031 382d 3039  _time": "2018-09
+00000e90: 2d31 3854 3039 3a32 353a 3030 2e30 3030  -18T09:25:00.000
+00000ea0: 5a22 2c0d 0a20 2020 2020 2020 2020 2020  Z",..           
+00000eb0: 2022 6c6f 675f 6475 7261 7469 6f6e 223a   "log_duration":
+00000ec0: 2036 3030 3030 2c0d 0a20 2020 2020 2020   60000,..       
+00000ed0: 2020 2020 2022 6369 636b 5f63 6f75 6e74       "cick_count
+00000ee0: 223a 2031 3030 302c 0d0a 2020 2020 2020  ": 1000,..      
+00000ef0: 2020 2020 2020 226b 6579 7374 726f 6b65        "keystroke
+00000f00: 5f63 6f75 6e74 223a 2032 3330 3030 2c0d  _count": 23000,.
+00000f10: 0a20 2020 2020 2020 2020 2020 2022 6170  .            "ap
+00000f20: 706c 6963 6174 696f 6e22 3a20 2245 7863  plication": "Exc
+00000f30: 656c 222c 0d0a 2020 2020 2020 2020 2020  el",..          
+00000f40: 2020 2265 7665 6e74 5f67 7569 6422 3a20    "event_guid": 
+00000f50: 2275 7267 682d 6173 6439 2d6e 756d 662d  "urgh-asd9-numf-
+00000f60: 7175 6164 222c 0d0a 2020 2020 2020 2020  quad",..        
+00000f70: 2020 2020 2275 7365 725f 6964 223a 2022      "user_id": "
+00000f80: 2369 646e 656c 736f 6e22 2c0d 0a20 2020  #idnelson",..   
+00000f90: 2020 2020 2020 2020 2022 736f 7572 6365           "source
+00000fa0: 5f73 7973 7465 6d22 3a20 225a 6f6f 6d22  _system": "Zoom"
+00000fb0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000fc0: 7469 6d65 7374 616d 705f 7574 6322 3a20  timestamp_utc": 
+00000fd0: 2232 3031 382d 3039 2d31 3854 3039 3a32  "2018-09-18T09:2
+00000fe0: 353a 3033 2e30 3030 5a22 2c0d 0a20 2020  5:03.000Z",..   
+00000ff0: 2020 2020 2020 2020 2022 6c6f 6164 6261           "loadba
+00001000: 7463 5f69 6422 3a20 3233 2c0d 0a20 2020  tc_id": 23,..   
+00001010: 2020 2020 2020 2020 2022 7261 775f 6465           "raw_de
+00001020: 7461 696c 7322 3a20 227b 736f 7572 6365  tails": "{source
+00001030: e280 a62e 2e7d 220d 0a20 2020 2020 2020  .....}"..       
+00001040: 2020 2020 207d 2c20 2020 2020 2020 2020       },         
+00001050: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00001060: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00001070: 2020 2273 7461 7274 5f74 696d 6522 3a20    "start_time": 
+00001080: 2232 3031 382d 3039 2d31 3854 3039 3a32  "2018-09-18T09:2
+00001090: 343a 3033 2e30 3030 5a22 2c0d 0a20 2020  4:03.000Z",..   
+000010a0: 2020 2020 2020 2020 2022 656e 645f 7469           "end_ti
+000010b0: 6d65 223a 2022 3230 3138 2d30 392d 3138  me": "2018-09-18
+000010c0: 5430 393a 3235 3a30 302e 3030 305a 222c  T09:25:00.000Z",
+000010d0: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
+000010e0: 6f67 5f64 7572 6174 696f 6e22 3a20 3630  og_duration": 60
+000010f0: 3030 302c 0d0a 2020 2020 2020 2020 2020  000,..          
+00001100: 2020 2263 6963 6b5f 636f 756e 7422 3a20    "cick_count": 
+00001110: 3130 3030 2c0d 0a20 2020 2020 2020 2020  1000,..         
+00001120: 2020 2022 6b65 7973 7472 6f6b 655f 636f     "keystroke_co
+00001130: 756e 7422 3a20 3233 3030 302c 0d0a 2020  unt": 23000,..  
+00001140: 2020 2020 2020 2020 2020 2261 7070 6c69            "appli
+00001150: 6361 7469 6f6e 223a 2022 4578 6365 6c22  cation": "Excel"
+00001160: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00001170: 6576 656e 745f 6775 6964 223a 2022 7572  event_guid": "ur
+00001180: 6768 2d61 7364 392d 6e75 6d66 2d71 7561  gh-asd9-numf-qua
+00001190: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
+000011a0: 2022 7573 6572 5f69 6422 3a20 2223 6964   "user_id": "#id
+000011b0: 6e65 6c73 6f6e 222c 0d0a 2020 2020 2020  nelson",..      
+000011c0: 2020 2020 2020 2273 6f75 7263 655f 7379        "source_sy
+000011d0: 7374 656d 223a 2022 5a6f 6f6d 222c 0d0a  stem": "Zoom",..
+000011e0: 2020 2020 2020 2020 2020 2020 2274 696d              "tim
+000011f0: 6573 7461 6d70 5f75 7463 223a 2022 3230  estamp_utc": "20
+00001200: 3138 2d30 392d 3138 5430 393a 3235 3a30  18-09-18T09:25:0
+00001210: 332e 3030 305a 222c 0d0a 2020 2020 2020  3.000Z",..      
+00001220: 2020 2020 2020 226c 6f61 6462 6174 635f        "loadbatc_
+00001230: 6964 223a 2032 332c 0d0a 2020 2020 2020  id": 23,..      
+00001240: 2020 2020 2020 2272 6177 5f64 6574 6169        "raw_detai
+00001250: 6c73 223a 2022 7b73 6f75 7263 65e2 80a6  ls": "{source...
+00001260: 2e2e 7d22 0d0a 2020 2020 2020 2020 2020  ..}"..          
+00001270: 2020 7d0d 0a20 2020 2020 2020 205d 2c0d    }..        ],.
+00001280: 0a20 2020 2020 2020 2022 6861 7368 5f31  .        "hash_1
+00001290: 223a 2022 6438 3239 3865 3838 6139 3239  ": "d8298e88a929
+000012a0: 6465 3233 6162 3162 6362 3036 6637 6130  de23ab1bcb06f7a0
+000012b0: 3564 3065 3639 3466 3837 3166 6231 3565  5d0e694f871fb15e
+000012c0: 6633 3138 3030 6438 3032 3764 3066 3736  f31800d8027d0f76
+000012d0: 6132 6666 222c 0d0a 2020 2020 2020 2020  a2ff",..        
+000012e0: 2268 6173 685f 3222 3a20 2233 6261 6561  "hash_2": "3baea
+000012f0: 3731 6537 6564 6362 3862 3861 6134 3431  71e7edcb8b8aa441
+00001300: 3766 6236 3430 6330 6661 3064 3766 3937  7fb640c0fa0d7f97
+00001310: 3931 6338 6132 6231 3763 6133 6634 3939  91c8a2b17ca3f499
+00001320: 6431 3066 3761 3433 6463 6422 2c0d 0a20  d10f7a43dcd",.. 
+00001330: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
+00001340: 7469 6d65 223a 2022 3230 3233 2d30 322d  time": "2023-02-
+00001350: 3231 5431 323a 3334 3a35 365a 220d 0a20  21T12:34:56Z".. 
+00001360: 2020 2020 2020 207d 0d0a 2020 2020 5d0d         }..    ].
+00001370: 0a20 2020 2073 696e 676c 655f 7363 6865  .    single_sche
+00001380: 6475 6c65 7220 3d20 5369 6e67 6c65 5351  duler = SingleSQ
+00001390: 534a 6f62 5363 6865 6475 6c65 7228 0d0a  SJobScheduler(..
+000013a0: 2020 2020 2020 2020 7261 7750 7562 6c69          rawPubli
+000013b0: 7368 696e 5374 7261 7465 6769 6573 3d5b  shinStrategies=[
+000013c0: 6462 5072 6f76 6964 6572 5d2c 0d0a 2020  dbProvider],..  
+000013d0: 2020 2020 2020 7371 735f 656e 706f 696e        sqs_enpoin
+000013e0: 743d 2268 7474 7073 3a2f 2f73 7173 2e75  t="https://sqs.u
+000013f0: 732d 6561 7374 2d31 2e61 6d61 7a6f 6e61  s-east-1.amazona
+00001400: 7773 2e63 6f6d 2f37 3936 3532 3232 3738  ws.com/796522278
+00001410: 3832 372f 4d6f 636b 5175 6575 652e 6669  827/MockQueue.fi
+00001420: 666f 220d 0a20 2020 2020 2020 2029 0d0a  fo"..        )..
+00001430: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+00001440: 7369 6e67 6c65 5f73 6368 6564 756c 6572  single_scheduler
+00001450: 2e70 7562 6c69 7368 5261 7728 6576 656e  .publishRaw(even
+00001460: 7473 3d64 6174 615f 7265 6365 6976 6564  ts=data_received
+00001470: 2920 2353 686f 756c 6420 7072 696e 7420  ) #Should print 
+00001480: 7468 6520 6576 656e 7420 7468 6174 2069  the event that i
+00001490: 7320 6265 696e 6720 7075 626c 7369 6865  s being publsihe
+000014a0: 640d 0a20 2020 2073 696e 676c 655f 7363  d..    single_sc
+000014b0: 6865 6475 6c65 722e 7363 6865 6475 6c65  heduler.schedule
+000014c0: 4a6f 6228 6576 656e 7473 3d64 6174 615f  Job(events=data_
+000014d0: 7265 6365 6976 6564 2920 2353 686f 756c  received) #Shoul
+000014e0: 6420 6163 7475 616c 6c79 2073 6368 6564  d actually sched
+000014f0: 756c 6520 7468 6520 6a6f 622e 0d0a 2020  ule the job...  
+00001500: 2020 0d0a 2020 2020 2320 6173 7365 7274    ..    # assert
+00001510: 286c 656e 286d 6f63 6b44 4250 726f 7669  (len(mockDBProvi
+00001520: 6465 722e 6462 293e 3d31 290d 0a0d 0a    der.db)>=1)....
```

