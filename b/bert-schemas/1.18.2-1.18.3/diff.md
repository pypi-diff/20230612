# Comparing `tmp/bert_schemas-1.18.2.tar.gz` & `tmp/bert_schemas-1.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_schemas-1.18.2.tar", max compression
+gzip compressed data, was "bert_schemas-1.18.3.tar", max compression
```

## Comparing `bert_schemas-1.18.2.tar` & `bert_schemas-1.18.3.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0      481 2023-05-15 14:27:01.954881 bert_schemas-1.18.2/README.md
--rw-r--r--   0        0        0       80 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/__init__.py
--rw-r--r--   0        0        0      870 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/access.py
--rw-r--r--   0        0        0      357 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/group.py
--rw-r--r--   0        0        0    44878 2023-05-31 15:48:17.261694 bert_schemas-1.18.2/bert_schemas/job.py
--rw-r--r--   0        0        0      770 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/message.py
--rw-r--r--   0        0        0     1388 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/qpu.py
--rw-r--r--   0        0        0     1967 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/questionnaire.py
--rw-r--r--   0        0        0      175 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/report.py
--rw-r--r--   0        0        0       51 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/factories/__init__.py
--rw-r--r--   0        0        0      492 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/factories/helpers.py
--rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/factories/job/__init__.py
--rw-r--r--   0        0        0     2713 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/barrier.py
--rw-r--r--   0        0        0     2509 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/bec.py
--rw-r--r--   0        0        0     2611 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/bragg.py
--rw-r--r--   0        0        0     2715 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/paint_1d.py
--rw-r--r--   0        0        0     2866 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/transistor.py
--rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/fixtures/__init__.py
--rw-r--r--   0        0        0     9136 2023-04-26 21:05:16.851464 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/__init__.py
--rw-r--r--   0        0        0     6106 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/barrier.py
--rw-r--r--   0        0        0     5846 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/bec.py
--rw-r--r--   0        0        0     5980 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/bragg.py
--rw-r--r--   0        0        0     6148 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/paint_1d.py
--rw-r--r--   0        0        0     6283 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/transistor.py
--rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/schemas/__init__.py
--rw-r--r--   0        0        0     1568 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/__init__.py
--rw-r--r--   0        0        0     2275 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/barrier.py
--rw-r--r--   0        0        0     2180 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/bec.py
--rw-r--r--   0        0        0     2197 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/bragg.py
--rw-r--r--   0        0        0     2368 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/paint_1d.py
--rw-r--r--   0        0        0     2340 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/shared.py
--rw-r--r--   0        0        0     2465 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/transistor.py
--rw-r--r--   0        0        0     1960 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/user.py
--rw-r--r--   0        0        0     1329 2023-05-31 15:48:27.073624 bert_schemas-1.18.2/pyproject.toml
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 bert_schemas-1.18.2/setup.py
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 bert_schemas-1.18.2/PKG-INFO
+-rw-r--r--   0        0        0      481 2023-05-15 14:27:01.954881 bert_schemas-1.18.3/README.md
+-rw-r--r--   0        0        0       77 2023-06-07 18:12:41.945841 bert_schemas-1.18.3/bert_schemas/__init__.py
+-rw-r--r--   0        0        0    44886 2023-06-09 20:18:50.900638 bert_schemas-1.18.3/bert_schemas/job.py
+-rw-r--r--   0        0        0      770 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/message.py
+-rw-r--r--   0        0        0     1427 2023-06-09 20:19:02.268643 bert_schemas-1.18.3/bert_schemas/qpu.py
+-rw-r--r--   0        0        0      849 2023-06-07 18:12:41.945841 bert_schemas-1.18.3/bert_schemas/qpu_access.py
+-rw-r--r--   0        0        0     1967 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/questionnaire.py
+-rw-r--r--   0        0        0      175 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/report.py
+-rw-r--r--   0        0        0       51 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/testing/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/testing/factories/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/testing/factories/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/testing/factories/job/__init__.py
+-rw-r--r--   0        0        0     2713 2023-04-28 17:21:29.074962 bert_schemas-1.18.3/bert_schemas/testing/factories/job/barrier.py
+-rw-r--r--   0        0        0     2509 2023-04-28 17:21:29.074962 bert_schemas-1.18.3/bert_schemas/testing/factories/job/bec.py
+-rw-r--r--   0        0        0     2611 2023-04-28 17:21:29.074962 bert_schemas-1.18.3/bert_schemas/testing/factories/job/bragg.py
+-rw-r--r--   0        0        0     2715 2023-04-28 17:21:29.074962 bert_schemas-1.18.3/bert_schemas/testing/factories/job/paint_1d.py
+-rw-r--r--   0        0        0     2866 2023-04-28 17:21:29.074962 bert_schemas-1.18.3/bert_schemas/testing/factories/job/transistor.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/testing/fixtures/__init__.py
+-rw-r--r--   0        0        0     9136 2023-04-26 21:05:16.851464 bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/__init__.py
+-rw-r--r--   0        0        0     6106 2023-05-19 14:05:39.418474 bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/barrier.py
+-rw-r--r--   0        0        0     5846 2023-05-19 14:05:39.418474 bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/bec.py
+-rw-r--r--   0        0        0     5980 2023-05-19 14:05:39.418474 bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/bragg.py
+-rw-r--r--   0        0        0     6148 2023-05-19 14:05:39.418474 bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/paint_1d.py
+-rw-r--r--   0        0        0     6283 2023-05-19 14:05:39.418474 bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/transistor.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/testing/schemas/__init__.py
+-rw-r--r--   0        0        0     1568 2023-04-14 20:15:22.201190 bert_schemas-1.18.3/bert_schemas/testing/schemas/job/__init__.py
+-rw-r--r--   0        0        0     2275 2023-04-28 21:15:25.564351 bert_schemas-1.18.3/bert_schemas/testing/schemas/job/barrier.py
+-rw-r--r--   0        0        0     2180 2023-04-28 21:15:25.564351 bert_schemas-1.18.3/bert_schemas/testing/schemas/job/bec.py
+-rw-r--r--   0        0        0     2197 2023-04-28 21:15:25.564351 bert_schemas-1.18.3/bert_schemas/testing/schemas/job/bragg.py
+-rw-r--r--   0        0        0     2368 2023-04-28 21:15:25.564351 bert_schemas-1.18.3/bert_schemas/testing/schemas/job/paint_1d.py
+-rw-r--r--   0        0        0     2340 2023-04-28 21:15:25.564351 bert_schemas-1.18.3/bert_schemas/testing/schemas/job/shared.py
+-rw-r--r--   0        0        0     2465 2023-04-28 21:15:25.564351 bert_schemas-1.18.3/bert_schemas/testing/schemas/job/transistor.py
+-rw-r--r--   0        0        0     2644 2023-06-07 18:12:41.945841 bert_schemas-1.18.3/bert_schemas/user.py
+-rw-r--r--   0        0        0     1329 2023-06-09 20:19:14.816648 bert_schemas-1.18.3/pyproject.toml
+-rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 bert_schemas-1.18.3/setup.py
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 bert_schemas-1.18.3/PKG-INFO
```

### Comparing `bert_schemas-1.18.2/bert_schemas/access.py` & `bert_schemas-1.18.3/bert_schemas/qpu_access.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date, time
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from typing import Optional
 
-from . import job as job_schema
+from . import qpu
 
 
 class DayOfWeek(StrEnum):
     MONDAY = "MONDAY"
     TUESDAY = "TUESDAY"
     WEDNESDAY = "WEDNESDAY"
     THURSDAY = "THURSDAY"
@@ -34,11 +34,11 @@
     start_date: date
     end_date: Optional[date]
     start_time: time
     end_time: time
 
 
 class Access(BaseModel):
-    qpu_name: job_schema.QPUName
+    qpu_name: qpu.QPUName
     access_name: Optional[str]
     access_type: AccessType
     access_slots: list[AccessSlot] = []
```

### Comparing `bert_schemas-1.18.2/bert_schemas/job.py` & `bert_schemas-1.18.3/bert_schemas/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     conint,
     conlist,
     root_validator,
     validator,
 )
 from scipy.interpolate import interp1d
 from typing_extensions import TypedDict
-from .qpu import QPU, QPUName
+from .qpu import QPUBase, QPUName
 
 
 class JobOrigin(StrEnum):
     WEB = auto()
     OQTANT = auto()
 
 
@@ -1171,15 +1171,15 @@
     class Config:
         orm_mode = True
 
 
 class JobResponse(JobBase):
     external_id: UUID
     status: JobStatus
-    qpu: Optional[QPU]
+    qpu: Optional[QPUBase]
     time_submit: datetime
     inputs: List[ResponseInput]
     failed_inputs: List[int] = []
 
 
 class JobInputsResponse(JobBase):
     external_id: UUID
```

### Comparing `bert_schemas-1.18.2/bert_schemas/message.py` & `bert_schemas-1.18.3/bert_schemas/message.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/qpu.py` & `bert_schemas-1.18.3/bert_schemas/qpu.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import datetime
-from typing import Dict, List, Optional
+from datetime import time
+from typing import List, Optional
 from fastapi_utils.enums import StrEnum
-from pydantic import BaseModel, root_validator, validator
+from pydantic import BaseModel, validator
 
 
 class QPUName(StrEnum):
     SMALLBERT = "SMALLBERT"
     BIGBERT = "BIGBERT"
     UNDEFINED = "UNDEFINED"
 
@@ -17,33 +17,39 @@
     ONLINE = "ONLINE"
     OFFLINE = "OFFLINE"
 
     def __str__(self):
         return str(self.value)
 
 
-class QPUAccess(BaseModel):
-    day: str
-    start_time: datetime.time
-    end_time: datetime.time
+class QPUJobType(BaseModel):
+    name: str
 
     class Config:
         orm_mode = True
 
 
-class QPUJobType(BaseModel):
-    name: str
+class QPUAccess(BaseModel):
+    day: str
+    start_time: time
+    end_time: time
 
     class Config:
         orm_mode = True
 
 
-class QPU(BaseModel):
+class QPUBase(BaseModel):
     name: QPUName
     status: QPUStatus
+
+    class Config:
+        orm_mode = True
+
+
+class QPU(QPUBase):
     qpu_access: List[QPUAccess]
     job_types: List[QPUJobType]
 
     @validator("job_types", pre=False)
     def job_type_names(cls, value):
         return [i.name for i in value]
```

### Comparing `bert_schemas-1.18.2/bert_schemas/questionnaire.py` & `bert_schemas-1.18.3/bert_schemas/questionnaire.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/factories/job/barrier.py` & `bert_schemas-1.18.3/bert_schemas/testing/factories/job/barrier.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/factories/job/bec.py` & `bert_schemas-1.18.3/bert_schemas/testing/factories/job/bec.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/factories/job/bragg.py` & `bert_schemas-1.18.3/bert_schemas/testing/factories/job/bragg.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/factories/job/paint_1d.py` & `bert_schemas-1.18.3/bert_schemas/testing/factories/job/paint_1d.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/factories/job/transistor.py` & `bert_schemas-1.18.3/bert_schemas/testing/factories/job/transistor.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/__init__.py` & `bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/barrier.py` & `bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/barrier.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/bec.py` & `bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/bec.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/bragg.py` & `bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/bragg.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/paint_1d.py` & `bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/paint_1d.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/transistor.py` & `bert_schemas-1.18.3/bert_schemas/testing/fixtures/job/transistor.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/__init__.py` & `bert_schemas-1.18.3/bert_schemas/testing/schemas/job/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/barrier.py` & `bert_schemas-1.18.3/bert_schemas/testing/schemas/job/barrier.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/bec.py` & `bert_schemas-1.18.3/bert_schemas/testing/schemas/job/bec.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/bragg.py` & `bert_schemas-1.18.3/bert_schemas/testing/schemas/job/bragg.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/paint_1d.py` & `bert_schemas-1.18.3/bert_schemas/testing/schemas/job/paint_1d.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/shared.py` & `bert_schemas-1.18.3/bert_schemas/testing/schemas/job/shared.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/transistor.py` & `bert_schemas-1.18.3/bert_schemas/testing/schemas/job/transistor.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.2/bert_schemas/user.py` & `bert_schemas-1.18.3/bert_schemas/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 # type: ignore
 from datetime import datetime
 from typing import List, Optional, Type
 
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel, EmailStr, constr
 
-from .group import GroupName, RoleName
 from .questionnaire import RegistrationQandA
 
 external_user_id: Type[str] = constr(regex=r"^auth0|[a-z0-9]{24}$")
 
 
+class TierName(StrEnum):
+    GROUND = "GROUND"
+    EXPLORER = "EXPLORER"
+    INNOVATOR = "INNOVATOR"
+    ADMIN = "ADMIN"
+
+    def __str__(self):
+        return str(self.value)
+
+
+class RoleName(StrEnum):
+    SUPERUSER = "SUPERUSER"
+    ORG_ADMIN = "ORG_ADMIN"
+
+    def __str__(self):
+        return str(self.value)
+
+
+class JobLimitType(StrEnum):
+    JOB_RATE = "JOB_RATE"
+    JOB_QUOTA = "JOB_QUOTA"
+
+
 class ExternalUserId(BaseModel):
     id: external_user_id
 
 
-class GroupBase(BaseModel):
-    name: GroupName
+class TierBase(BaseModel):
+    name: TierName
     description: Optional[str]
 
     class Config:
         orm_mode = True
 
 
-class Group(GroupBase):
+class Tier(TierBase):
     pass
 
 
-class GroupCreate(GroupBase):
+class TierCreate(TierBase):
     pass
 
 
 class RoleBase(BaseModel):
     name: RoleName
     description: Optional[str]
 
@@ -39,37 +61,56 @@
         orm_mode = True
 
 
 class Role(RoleBase):
     pass
 
 
+class TierSubscription(BaseModel):
+    start_date: datetime
+    end_date: datetime = None
+
+    class Config:
+        orm_mode = True
+
+
+class Organization(BaseModel):
+    name: str
+
+    class Config:
+        orm_mode = True
+
+
 class UserBase(BaseModel):
     name: constr(min_length=1, max_length=100)
     email: EmailStr
     affiliation: str
 
     class Config:
         orm_mode = True
         extra = "forbid"
 
 
 class UserResponse(UserBase):
     signup_date: datetime
     external_user_id: external_user_id
-    group: Optional[Group]
+    tier: Optional[Tier]
+    subscription: Optional[TierSubscription]
     roles: Optional[List[Role]]
+    organizations: Optional[List[Organization]]
 
 
 class User(UserBase):
     id: int
     external_user_id: external_user_id
     signup_date: datetime
-    group: Optional[Group]
+    tier: Optional[Tier]
+    subscription: Optional[List[TierSubscription]]
     roles: Optional[List[Role]]
+    organizations: Optional[List[Organization]]
 
 
 class UserCreate(UserBase):
     external_user_id: external_user_id
 
 
 class UserSignUp(UserBase):
@@ -93,16 +134,11 @@
 
 
 class JobLimit(BaseModel):
     quotas: List[Quota]
     rates: List[Rate]
 
 
-class JobLimitType(StrEnum):
-    JOB_RATE = "JOB_RATE"
-    JOB_QUOTA = "JOB_QUOTA"
-
-
 class ContactUs(BaseModel):
     subject: str
     email: EmailStr
     content: constr(min_length=1, max_length=500)
```

### Comparing `bert_schemas-1.18.2/pyproject.toml` & `bert_schemas-1.18.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bert-schemas"
-version = "1.18.2"
+version = "1.18.3"
 description = "Bert service schemas"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
 exclude = ["**/.pytest_cache/**/*", "**/__pycache__", ".gitignore"]
```

### Comparing `bert_schemas-1.18.2/setup.py` & `bert_schemas-1.18.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'matplotlib>=3.6.2,<3.7.0',
  'pydantic-factories>=1.17.0,<2.0.0',
  'pytest>=7.2.0,<8.0.0',
  'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'bert-schemas',
-    'version': '1.18.2',
+    'version': '1.18.3',
     'description': 'Bert service schemas',
     'long_description': '# Bert Schemas\n\n[![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)\n\n## 🚀 Quick Install\n\n```python\npip install bert-schemas\n```\n\n## 🧭 Introduction\n\nThese Pydantic schemas are used by projects such as Oqtant for defining and validating REST payloads.\n',
     'author': 'Larry Buza',
     'author_email': 'lawrence.buza@coldquanta.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bert_schemas-1.18.2/PKG-INFO` & `bert_schemas-1.18.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-schemas
-Version: 1.18.2
+Version: 1.18.3
 Summary: Bert service schemas
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

