# Comparing `tmp/asklora_portal-1.1.8.tar.gz` & `tmp/asklora_portal-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asklora_portal-1.1.8.tar", max compression
+gzip compressed data, was "asklora_portal-1.1.9.tar", max compression
```

## Comparing `asklora_portal-1.1.8.tar` & `asklora_portal-1.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1074 2023-01-24 04:17:44.288375 asklora_portal-1.1.8/LICENSE
--rw-r--r--   0        0        0     3898 2023-02-15 07:59:20.702404 asklora_portal-1.1.8/README.md
--rw-r--r--   0        0        0     3898 2023-02-15 07:59:20.702690 asklora_portal-1.1.8/asklora/README.md
--rw-r--r--   0        0        0     1377 2023-02-22 02:35:15.693679 asklora_portal-1.1.8/asklora/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 04:17:44.289004 asklora_portal-1.1.8/asklora/brokerage/__init__.py
--rw-r--r--   0        0        0     4215 2023-02-27 02:45:17.130696 asklora_portal-1.1.8/asklora/brokerage/client.py
--rw-r--r--   0        0        0     1429 2023-01-24 04:17:44.289210 asklora_portal-1.1.8/asklora/brokerage/common.py
--rw-r--r--   0        0        0     4763 2023-03-15 07:36:24.399964 asklora_portal-1.1.8/asklora/brokerage/enums.py
--rw-r--r--   0        0        0      848 2023-01-24 04:17:44.289365 asklora_portal-1.1.8/asklora/brokerage/exceptions.py
--rw-r--r--   0        0        0     9220 2023-03-15 07:36:24.400372 asklora_portal-1.1.8/asklora/brokerage/ibkr.py
--rw-r--r--   0        0        0     1171 2023-03-15 07:36:24.400692 asklora_portal-1.1.8/asklora/brokerage/iex.py
--rw-r--r--   0        0        0     2477 2023-02-27 02:45:17.131599 asklora_portal-1.1.8/asklora/brokerage/logs.py
--rw-r--r--   0        0        0    19120 2023-03-15 07:36:24.401098 asklora_portal-1.1.8/asklora/brokerage/models.py
--rw-r--r--   0        0        0    18306 2023-02-22 02:35:15.695294 asklora_portal-1.1.8/asklora/brokerage/rest.py
--rw-r--r--   0        0        0     1902 2023-03-15 07:36:24.401416 asklora_portal-1.1.8/asklora/brokerage/vars.py
--rw-r--r--   0        0        0    10940 2023-02-27 02:45:17.132909 asklora_portal-1.1.8/asklora/dam.py
--rw-r--r--   0        0        0      233 2023-02-15 07:59:20.711192 asklora_portal-1.1.8/asklora/exceptions/__init__.py
--rw-r--r--   0        0        0      343 2023-02-15 07:59:20.711440 asklora_portal-1.1.8/asklora/exceptions/pgp.py
--rw-r--r--   0        0        0     2554 2023-02-27 02:45:17.133262 asklora_portal-1.1.8/asklora/logger.py
--rw-r--r--   0        0        0     7963 2023-02-22 06:53:51.483226 asklora_portal-1.1.8/asklora/pgp.py
--rw-r--r--   0        0        0     1663 2023-02-15 07:59:20.712819 asklora_portal-1.1.8/asklora/portal.py
--rw-r--r--   0        0        0      627 2023-02-15 07:59:20.713210 asklora_portal-1.1.8/asklora/singleton.py
--rw-r--r--   0        0        0      205 2023-02-15 07:59:20.713822 asklora_portal-1.1.8/asklora/utils/__init__.py
--rw-r--r--   0        0        0     1232 2023-02-15 07:59:20.714238 asklora_portal-1.1.8/asklora/utils/common.py
--rw-r--r--   0        0        0      974 2023-02-15 07:59:20.714696 asklora_portal-1.1.8/asklora/utils/file.py
--rw-r--r--   0        0        0      226 2023-02-15 07:59:20.714952 asklora_portal-1.1.8/asklora/utils/regexes.py
--rw-r--r--   0        0        0      999 2023-03-15 07:36:24.402109 asklora_portal-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 asklora_portal-1.1.8/setup.py
--rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 asklora_portal-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-01-24 04:17:44.288375 asklora_portal-1.1.9/LICENSE
+-rw-r--r--   0        0        0     3898 2023-02-15 07:59:20.702404 asklora_portal-1.1.9/README.md
+-rw-r--r--   0        0        0     3898 2023-02-15 07:59:20.702690 asklora_portal-1.1.9/asklora/README.md
+-rw-r--r--   0        0        0     1377 2023-02-22 02:35:15.693679 asklora_portal-1.1.9/asklora/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 04:17:44.289004 asklora_portal-1.1.9/asklora/brokerage/__init__.py
+-rw-r--r--   0        0        0     4215 2023-02-27 02:45:17.130696 asklora_portal-1.1.9/asklora/brokerage/client.py
+-rw-r--r--   0        0        0     1429 2023-01-24 04:17:44.289210 asklora_portal-1.1.9/asklora/brokerage/common.py
+-rw-r--r--   0        0        0     4763 2023-03-15 07:36:24.399964 asklora_portal-1.1.9/asklora/brokerage/enums.py
+-rw-r--r--   0        0        0      848 2023-01-24 04:17:44.289365 asklora_portal-1.1.9/asklora/brokerage/exceptions.py
+-rw-r--r--   0        0        0    11030 2023-04-03 01:33:35.476695 asklora_portal-1.1.9/asklora/brokerage/ibkr.py
+-rw-r--r--   0        0        0     1171 2023-03-15 07:36:24.400692 asklora_portal-1.1.9/asklora/brokerage/iex.py
+-rw-r--r--   0        0        0     2477 2023-02-27 02:45:17.131599 asklora_portal-1.1.9/asklora/brokerage/logs.py
+-rw-r--r--   0        0        0    26347 2023-04-03 01:33:35.477309 asklora_portal-1.1.9/asklora/brokerage/models.py
+-rw-r--r--   0        0        0    18306 2023-02-22 02:35:15.695294 asklora_portal-1.1.9/asklora/brokerage/rest.py
+-rw-r--r--   0        0        0     1902 2023-03-15 07:36:24.401416 asklora_portal-1.1.9/asklora/brokerage/vars.py
+-rw-r--r--   0        0        0     3791 2023-04-03 01:33:35.477757 asklora_portal-1.1.9/asklora/dam.py
+-rw-r--r--   0        0        0      233 2023-02-15 07:59:20.711192 asklora_portal-1.1.9/asklora/exceptions/__init__.py
+-rw-r--r--   0        0        0      343 2023-02-15 07:59:20.711440 asklora_portal-1.1.9/asklora/exceptions/pgp.py
+-rw-r--r--   0        0        0     2554 2023-02-27 02:45:17.133262 asklora_portal-1.1.9/asklora/logger.py
+-rw-r--r--   0        0        0     7963 2023-02-22 06:53:51.483226 asklora_portal-1.1.9/asklora/pgp.py
+-rw-r--r--   0        0        0     1663 2023-02-15 07:59:20.712819 asklora_portal-1.1.9/asklora/portal.py
+-rw-r--r--   0        0        0      627 2023-02-15 07:59:20.713210 asklora_portal-1.1.9/asklora/singleton.py
+-rw-r--r--   0        0        0      205 2023-02-15 07:59:20.713822 asklora_portal-1.1.9/asklora/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2023-02-15 07:59:20.714238 asklora_portal-1.1.9/asklora/utils/common.py
+-rw-r--r--   0        0        0      974 2023-02-15 07:59:20.714696 asklora_portal-1.1.9/asklora/utils/file.py
+-rw-r--r--   0        0        0      226 2023-02-15 07:59:20.714952 asklora_portal-1.1.9/asklora/utils/regexes.py
+-rw-r--r--   0        0        0      999 2023-04-03 01:33:35.478136 asklora_portal-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 asklora_portal-1.1.9/setup.py
+-rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 asklora_portal-1.1.9/PKG-INFO
```

### Comparing `asklora_portal-1.1.8/LICENSE` & `asklora_portal-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/README.md` & `asklora_portal-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/README.md` & `asklora_portal-1.1.9/asklora/README.md`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/__init__.py` & `asklora_portal-1.1.9/asklora/__init__.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/brokerage/client.py` & `asklora_portal-1.1.9/asklora/brokerage/client.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/brokerage/common.py` & `asklora_portal-1.1.9/asklora/brokerage/common.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/brokerage/enums.py` & `asklora_portal-1.1.9/asklora/brokerage/enums.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/brokerage/exceptions.py` & `asklora_portal-1.1.9/asklora/brokerage/exceptions.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/brokerage/iex.py` & `asklora_portal-1.1.9/asklora/brokerage/iex.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/brokerage/logs.py` & `asklora_portal-1.1.9/asklora/brokerage/logs.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/brokerage/models.py` & `asklora_portal-1.1.9/asklora/brokerage/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,17 +11,25 @@
 ECA_NSMAP = {"": "http://www.interactivebrokers.com/schemas/IBCust_import"}
 ECA_CA_NSMAP = {"": "http://www.cstools.interactivebrokers.com"}
 FB_NSMAP = {
     "": "http://www.interactivebrokers.com/fbfb_instruction_set",
     "xsi": "http://www.w3.org/2001/XMLSchema-instance",
 }
 
-# ===================== ECA Models =====================
 
+# ------------------------------- Broker response model ------------------------------ #
+class BrokerResponse(BaseModel):
+    url: str
+    raw_payload: str | dict | None = None
+    payload: dict
+    raw_response: dict | None = None
+    response: dict | None = None
 
+
+# ------------------------------------ ECA models ------------------------------------ #
 class CustomXmlEncoder(XmlEncoder):
     def __init__(self):
         super().__init__(str)
 
     def encode(self, obj: Any) -> str:
         if isinstance(obj, bool):
             return str(obj).lower()
@@ -109,15 +117,15 @@
 
 
 class EmployerAddress(BaseXmlModel, nsmap=ECA_NSMAP):
     country: str = attr()
     state: str | None = attr()
     city: constr(max_length=100) | None = attr()
     postal_code: constr(max_length=20) | None = attr()
-    street_1: constr(max_length=20) | None = attr()
+    street_1: constr(max_length=200) | None = attr()
 
 
 class EmploymentDetails(BaseXmlModel, nsmap=ECA_NSMAP):
     employer: constr(max_length=128) = element()
     occupation: str | None = element()
     employer_business: str | None = element()
     employer_address: EmployerAddress = element()
@@ -157,16 +165,16 @@
     mailing_address: MailingAddress | None = element(tag="MailingAddress")
     identification: Identification | None = element(tag="Identification")
     tax_residencies: list[TaxResidency] = wrapped(
         "TaxResidencies",
         element(tag="TaxResidency"),
     )
     w8ben: W8Ben | None = element(tag="W8Ben")
-    employment_type: enums.EmploymentTypeEnum = element(tag="EmploymentType")
-    employment_details: EmploymentDetails = element(tag="EmploymentDetails")
+    employment_type: enums.EmploymentTypeEnum | None = element(tag="EmploymentType")
+    employment_details: EmploymentDetails | None = element(tag="EmploymentDetails")
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class SourceOfWealth(BaseXmlModel, nsmap=ECA_NSMAP):
     percentage: int = attr()
@@ -392,14 +400,210 @@
         ]
 
         if IS_EMPLOYED and DATA_IS_NOT_COMPLETE:
             raise ValueError("Need to complete employment information")
 
         return values
 
+    def generate_application_xml(self):
+        from pathlib import Path
+        from asklora.utils import get_file_sha1, get_file_size
+
+        current_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+
+        mailing_address = None
+        employment_details = None
+
+        w8ben_file = (
+            Path(self.w8ben_file)
+            if isinstance(self.w8ben_file, str)
+            else self.w8ben_file
+        )
+        proof_of_identity_file = (
+            Path(self.proof_of_identity_file)
+            if isinstance(self.proof_of_identity_file, str)
+            else self.proof_of_identity_file
+        )
+        proof_of_address_file = (
+            Path(self.proof_of_address_file)
+            if isinstance(self.proof_of_address_file, str)
+            else self.proof_of_address_file
+        )
+
+        email = Email(email=self.email)
+        name = Name(
+            first=self.first_name,
+            last=self.last_name,
+            middle=self.middle_name,
+        )
+        identification = Identification(
+            citizenship=self.identification_citizenship,
+            issuing_country=self.identification_issuing_country,
+            national_card=self.identification_number,
+        )
+        residence = Residence(
+            country=self.country,
+            state=self.state,
+            city=self.city,
+            postal_code=self.postal_code,
+            street_1=self.street_name,
+        )
+
+        if not self.is_mailing_address:
+            mailing_address = MailingAddress(
+                country=self.mailing_country,
+                state=self.mailing_state,
+                city=self.mailing_city,
+                postal_code=self.mailing_postal_code,
+                street_1=self.mailing_street_name,
+            )
+
+        if self.employment_type in [
+            enums.EmploymentTypeEnum.EMPLOYED,
+            enums.EmploymentTypeEnum.SELFEMPLOYED,
+        ]:
+            employment_details = EmploymentDetails(
+                employer=self.employer,
+                occupation=self.occupation,
+                employer_business=self.employer_business,
+                employer_address=EmployerAddress(
+                    country=self.employer_address_country,
+                    state=self.employer_address_state,
+                    city=self.employer_address_city,
+                    postal_code=self.employer_address_postal_code,
+                    street_1=self.employer_address_street_name,
+                ),
+            )
+
+        tax_residency = TaxResidency(
+            country=self.tax_country,
+            tin_type=enums.TINTypeEnum.NON_US.value,
+            tin=self.tin,
+        )
+        financial_information = FinancialInformation(
+            sources_of_wealth=self.sources_of_wealth
+        )
+        w8ben = W8Ben(
+            cert=True,
+            part_2_9a_country="N/A",
+            name=name.get_full_name(),
+            proprietary_form_number="5001",
+            blank_form=True,
+            tax_form_file="Form5001.pdf",
+            foreign_tax_id=self.tin,
+        )
+
+        account_holder = AccountHolder(
+            details=AccountHolderDetails(
+                external_id=self.user_id,
+                same_mail_address=self.is_mailing_address,
+                name=name,
+                country_of_birth=self.country_of_birth,
+                dob=self.date_of_birth,
+                email=email,
+                residence=residence,
+                mailing_address=mailing_address,
+                identification=identification,
+                tax_residencies=[tax_residency],
+                w8ben=w8ben,
+                employment_type=self.employment_type,
+                employment_details=employment_details,
+            ),
+            financial_information=financial_information,
+        )
+
+        # main models
+        customer = Customer(
+            email=self.email,
+            external_id=self.user_id,
+            prefix="lora",
+            customer_type="INDIVIDUAL",
+            md_status_nonpro=False,
+            meets_aml_standard=True,
+            has_direct_trading_access=False,
+            account_holder=account_holder,
+        )
+
+        account = Account(
+            external_id=self.user_id,
+            base_currency="USD",
+            margin=enums.AccountMarginEnum.CASH.value,
+            multicurrency=False,
+            drip=False,
+            client_active_trading=False,
+            trading_permissions=[
+                TradingPermission(product="STOCKS", country="UNITED STATES"),
+                # TradingPermission(exchange_group="FOREX"),
+            ],
+        )
+        user = User(
+            external_individual_id=self.user_id,
+            external_user_id=self.user_id,
+            prefix="lora",
+        )
+
+        documents = [
+            Document(
+                form_no="5001",
+                exec_ts=current_timestamp,
+                exec_login_ts=current_timestamp,
+                signed_by=name.get_full_name(with_initial=True),
+                attached_file=AttachedFile(
+                    file_name=w8ben_file.name,
+                    file_length=get_file_size(w8ben_file),
+                    sha1_checksum=get_file_sha1(w8ben_file),
+                ),
+            ),
+            Document(
+                form_no="8001",
+                exec_ts=current_timestamp,
+                exec_login_ts=current_timestamp,
+                proof_of_identity_type="National ID Card",
+                signed_by=name.get_full_name(with_initial=True),
+                attached_file=AttachedFile(
+                    file_name=proof_of_identity_file.name,
+                    file_length=get_file_size(proof_of_identity_file),
+                    sha1_checksum=get_file_sha1(proof_of_identity_file),
+                ),
+            ),
+        ]
+
+        if proof_of_address_file:
+            proof_of_address_document = Document(
+                form_no="8002",
+                exec_ts=current_timestamp,
+                exec_login_ts=current_timestamp,
+                proof_of_address_type=self.proof_of_address_type.value,
+                signed_by=name.get_full_name(with_initial=True),
+                attached_file=AttachedFile(
+                    file_name=proof_of_address_file.name,
+                    file_length=get_file_size(proof_of_address_file),
+                    sha1_checksum=get_file_sha1(proof_of_address_file),
+                ),
+            )
+
+            documents.append(proof_of_address_document)
+
+        application = Application(
+            customer=customer,
+            accounts=[account],
+            users=[user],
+            documents=documents,
+        )
+
+        applications = Applications(applications=[application])
+
+        return applications.to_xml(
+            encoder=CustomXmlEncoder(),
+            pretty_print=True,
+            encoding="UTF-8",
+            skip_empty=True,
+            standalone=True,
+        ).decode()
+
 
 # --------------------------------- Corporate actions -------------------------------- #
 class CASearchRequest(BaseXmlModel, nsmap=ECA_CA_NSMAP):
     corp_action_type: enums.CorpActionType = attr(name="corpActionType")
     account_id: str = attr(name="accountId")
     account_ids: str | None = attr(name="accountIds")
     sub_accounts_choice: enums.SubAccuntsChoice = attr(name="subAccountsChoice")
```

### Comparing `asklora_portal-1.1.8/asklora/brokerage/rest.py` & `asklora_portal-1.1.9/asklora/brokerage/rest.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/brokerage/vars.py` & `asklora_portal-1.1.9/asklora/brokerage/vars.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/logger.py` & `asklora_portal-1.1.9/asklora/logger.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/pgp.py` & `asklora_portal-1.1.9/asklora/pgp.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/portal.py` & `asklora_portal-1.1.9/asklora/portal.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/singleton.py` & `asklora_portal-1.1.9/asklora/singleton.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/utils/common.py` & `asklora_portal-1.1.9/asklora/utils/common.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/asklora/utils/file.py` & `asklora_portal-1.1.9/asklora/utils/file.py`

 * *Files identical despite different names*

### Comparing `asklora_portal-1.1.8/pyproject.toml` & `asklora_portal-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asklora-portal"
-version = "1.1.8"
+version = "1.1.9"
 description = "portal to use various api data service"
 authors = ["redloratech <rede.akbar@loratechai.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "asklora"}]
 
 [tool.poetry.dependencies]
```

### Comparing `asklora_portal-1.1.8/setup.py` & `asklora_portal-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'python-gnupg>=0.5.0,<0.6.0',
  'requests>=2.28.1,<3.0.0',
  'sseclient-py>=1.7.2,<2.0.0',
  'structlog>=22.3.0,<23.0.0']
 
 setup_kwargs = {
     'name': 'asklora-portal',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': 'portal to use various api data service',
     'long_description': '# Asklora Portal\n\nShared utilities and helper classes used in Asklora projects\n\n## Contents\n\n1. Clients for external services (MarketData, Broker, PriceData, DAMECAClient, DAMFBClient) and their supporting classes (DAM, pydantic models for xml serialising and de-serialising)\n2. Helper classes (SingletonMeta, ExtendedEnum, PGPHelper)\n3. Helper functions (deep_get, get_file_size, get_file_sha1)\n\n## Information on specific sections\n\n### Broker, PriceData and MarketData client\n\n#### required .env config when importing these\n\n- `BROKER_API_URL=brokerurl`\n- `MARKET_API_URL=market url`\n- `BROKER_KEY=key`\n- `BROKER_SECRET=secret`\n\n#### usage\n\n```python\nfrom asklora import Broker\n\nbroker = Broker()\nbroker.create_account(...)\n```\n\nor you can use our Portal class to get the specific model\n\n```python\nimport asklora\n\nportal = asklora.Portal()\n\nrest = portal.get_broker_client() # get a REST client for trade, user, position , order\nmarketrest = portal.get_market_client() # get a REST client for market data\neventclient = portal.get_event_client() # get an event client for trade, user, position, order\n```\n\n### PriceData (for IEX)\n\n#### required .env config\n\n- `IEX_API_URL`\n- `IEX_TOKEN`\n\n#### usage\n\n```python\nfrom asklora import PriceData\n\nprice_data = PriceData()\nprice_data.get_lastestPrice("MSFT")\n```\n\n### DAMECAClient and DAMFBClient\n\n#### required .env config\n\n- `DAM_URL`\n- `DAM_CSID`\n\n#### usage\n\nFor these clients, you can find the Pydantic models needed by some of the class methods in the `models` and `enums` module.\n\nfor example, in the `DAMECAClient`, in the `generate_application_payload` method, the first argument accepts `DAMApplicationPayload` model that will automatically processed to xml the API endpoint needs.\n\n### examples\n\n- DAMECAClient\n\n  ```python\n  from asklora import DAMECAClient, PGPHelper\n  from asklora.models import DAMApplicationPayload\n\n  client = DAMECAClient()\n\n  # Build payload\n  payload = DAMApplicationPayload(\n      user_id=56,\n      first_name="Jane",\n      last_name="Smith",\n      ...\n  )\n\n  # Needed for encryption\n  pgp_helper = PGPHelper(\n      private_key_path=...,\n      public_key_path=...,\n      remote_public_key_path=...,\n  )\n\n  # Send the request\n  client.create_account(payload, pgp_helper=pgp_helper)\n  ```\n\n- DAMFBClient\n\n  ```python\n  from asklora import DAMFBClient, PGPHelper\n  from asklora.models import InstructionSet, InternalCashTransfer, CancelTransaction\n\n  client = DAMFBClient()\n\n  instruction_set = InstructionSet(\n      instructions=[\n          InternalCashTransfer(\n             id=4,\n             source="U199516",\n             destination="U34516",\n             amount=1000,\n             currency="USD",\n          ),\n          CancelTransaction(\n             id=5,\n             ib_instr_id="3",\n             reason="Wrong destination",\n          ),\n      ]\n  )\n  pgp_helper = PGPHelper(\n      private_key_path=...,\n      public_key_path=...,\n      remote_public_key_path=...,\n  )\n\n  client.create_instruction(instruction_set, pgp_helper=pgp_helper)\n\n  # if needed, you can also send xml directly\n  payload = """<?xml version="1.0" encoding="UTF-8"?>\n  <instruction_set\n    xmlns="http://www.interactivebrokers.com/fbfb_instruction_set"\n    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"\n    xsi:schemaLocation="http://www.interactivebrokers.com/fbfb_instruction_set fbfb_instruction_set.xsd "\n    creation_date="2019-01-11" id="2450" version="1">\n    <close_account id="2450">\n        <client_ib_acct_id>U1234567</client_ib_acct_id>\n        <close_reason> No longer needed </close_reason>\n    </close_account>\n  </instruction_set>"""\n\n  client.create_instruction(payload, pgp_helper=pgp_helper)\n  ```\n\n- Both\n\n  You can also initialise one or both of the classes above like this:\n\n  ```python\n  from asklora import IBClient\n\n  eca_client = IBClient.get_ECA_client()\n  fb_client = IBClient.get_FB_client()\n  ```\n',
     'author': 'redloratech',
     'author_email': 'rede.akbar@loratechai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `asklora_portal-1.1.8/PKG-INFO` & `asklora_portal-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asklora-portal
-Version: 1.1.8
+Version: 1.1.9
 Summary: portal to use various api data service
 License: MIT
 Author: redloratech
 Author-email: rede.akbar@loratechai.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

