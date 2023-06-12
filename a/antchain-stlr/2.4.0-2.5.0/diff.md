# Comparing `tmp/antchain_stlr-2.4.0.tar.gz` & `tmp/antchain_stlr-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_stlr-2.4.0.tar", last modified: Mon Jun  5 11:46:59 2023, max compression
+gzip compressed data, was "dist/antchain_stlr-2.5.0.tar", last modified: Mon Jun 12 03:57:38 2023, max compression
```

## Comparing `antchain_stlr-2.4.0.tar` & `antchain_stlr-2.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_sdk_stlr/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/antchain_sdk_stlr/__init__.py
--rw-r--r--   0 root         (0) root         (0)   106791 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/antchain_sdk_stlr/client.py
--rw-r--r--   0 root         (0) root         (0)   247416 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/antchain_sdk_stlr/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_sdk_stlr/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_sdk_stlr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111327 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_sdk_stlr/client.py
+-rw-r--r--   0 root         (0) root         (0)   261187 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_sdk_stlr/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/setup.py
```

### Comparing `antchain_stlr-2.4.0/LICENSE` & `antchain_stlr-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.4.0/PKG-INFO` & `antchain_stlr-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_stlr
-Version: 2.4.0
+Version: 2.5.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.4.0/README-CN.md` & `antchain_stlr-2.5.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.4.0/README.md` & `antchain_stlr-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.4.0/antchain_sdk_stlr/client.py` & `antchain_stlr-2.5.0/antchain_sdk_stlr/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.4.0',
+                    'sdk_version': '2.5.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.4.0',
+                    'sdk_version': '2.5.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -2433,14 +2433,126 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             stlr_models.QueryEcarOffsetaccountResponse(),
             await self.do_request_async('1.0', 'antchain.carbon.ecar.offsetaccount.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def detail_ecar_offsetdatum(
+        self,
+        request: stlr_models.DetailEcarOffsetdatumRequest,
+    ) -> stlr_models.DetailEcarOffsetdatumResponse:
+        """
+        Description: 查询碳补偿数据详情
+        Summary: 碳补偿数据详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.detail_ecar_offsetdatum_ex(request, headers, runtime)
+
+    async def detail_ecar_offsetdatum_async(
+        self,
+        request: stlr_models.DetailEcarOffsetdatumRequest,
+    ) -> stlr_models.DetailEcarOffsetdatumResponse:
+        """
+        Description: 查询碳补偿数据详情
+        Summary: 碳补偿数据详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.detail_ecar_offsetdatum_ex_async(request, headers, runtime)
+
+    def detail_ecar_offsetdatum_ex(
+        self,
+        request: stlr_models.DetailEcarOffsetdatumRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.DetailEcarOffsetdatumResponse:
+        """
+        Description: 查询碳补偿数据详情
+        Summary: 碳补偿数据详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.DetailEcarOffsetdatumResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.offsetdatum.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def detail_ecar_offsetdatum_ex_async(
+        self,
+        request: stlr_models.DetailEcarOffsetdatumRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.DetailEcarOffsetdatumResponse:
+        """
+        Description: 查询碳补偿数据详情
+        Summary: 碳补偿数据详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.DetailEcarOffsetdatumResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.offsetdatum.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def detail_ecar_offsettranslate(
+        self,
+        request: stlr_models.DetailEcarOffsettranslateRequest,
+    ) -> stlr_models.DetailEcarOffsettranslateResponse:
+        """
+        Description: 查询碳普惠减碳量转移记录详情
+        Summary: 碳普惠减碳量转移记录详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.detail_ecar_offsettranslate_ex(request, headers, runtime)
+
+    async def detail_ecar_offsettranslate_async(
+        self,
+        request: stlr_models.DetailEcarOffsettranslateRequest,
+    ) -> stlr_models.DetailEcarOffsettranslateResponse:
+        """
+        Description: 查询碳普惠减碳量转移记录详情
+        Summary: 碳普惠减碳量转移记录详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.detail_ecar_offsettranslate_ex_async(request, headers, runtime)
+
+    def detail_ecar_offsettranslate_ex(
+        self,
+        request: stlr_models.DetailEcarOffsettranslateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.DetailEcarOffsettranslateResponse:
+        """
+        Description: 查询碳普惠减碳量转移记录详情
+        Summary: 碳普惠减碳量转移记录详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.DetailEcarOffsettranslateResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.offsettranslate.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def detail_ecar_offsettranslate_ex_async(
+        self,
+        request: stlr_models.DetailEcarOffsettranslateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.DetailEcarOffsettranslateResponse:
+        """
+        Description: 查询碳普惠减碳量转移记录详情
+        Summary: 碳普惠减碳量转移记录详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.DetailEcarOffsettranslateResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.offsettranslate.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_third_cert(
         self,
         request: stlr_models.QueryThirdCertRequest,
     ) -> stlr_models.QueryThirdCertResponse:
         """
         Description: 三方平台调用此接口，查询用户的证书信息
         Summary: 证书查询
```

### Comparing `antchain_stlr-2.4.0/antchain_sdk_stlr/models.py` & `antchain_stlr-2.5.0/antchain_sdk_stlr/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -661,14 +661,71 @@
         if m.get('counteraction_amount') is not None:
             self.counteraction_amount = m.get('counteraction_amount')
         if m.get('data_unit') is not None:
             self.data_unit = m.get('data_unit')
         return self
 
 
+class CarbonOffsetActiveDataDetail(TeaModel):
+    def __init__(
+        self,
+        active_data_no: str = None,
+        active_data_name: str = None,
+        active_data_unit: str = None,
+        description: str = None,
+        active_data_value: str = None,
+    ):
+        # 活动数据编号
+        self.active_data_no = active_data_no
+        # 活动数据名称
+        self.active_data_name = active_data_name
+        # 活动数据单位
+        self.active_data_unit = active_data_unit
+        # 活动数据描述文案
+        self.description = description
+        # 活动数据值
+        self.active_data_value = active_data_value
+
+    def validate(self):
+        self.validate_required(self.active_data_no, 'active_data_no')
+        self.validate_required(self.active_data_value, 'active_data_value')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_data_no is not None:
+            result['active_data_no'] = self.active_data_no
+        if self.active_data_name is not None:
+            result['active_data_name'] = self.active_data_name
+        if self.active_data_unit is not None:
+            result['active_data_unit'] = self.active_data_unit
+        if self.description is not None:
+            result['description'] = self.description
+        if self.active_data_value is not None:
+            result['active_data_value'] = self.active_data_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('active_data_no') is not None:
+            self.active_data_no = m.get('active_data_no')
+        if m.get('active_data_name') is not None:
+            self.active_data_name = m.get('active_data_name')
+        if m.get('active_data_unit') is not None:
+            self.active_data_unit = m.get('active_data_unit')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('active_data_value') is not None:
+            self.active_data_value = m.get('active_data_value')
+        return self
+
+
 class EnterpriseMemberSummary(TeaModel):
     def __init__(
         self,
         account_did: str = None,
         name: str = None,
         mobile: str = None,
         register_time: str = None,
@@ -6312,14 +6369,315 @@
         if m.get('account_did') is not None:
             self.account_did = m.get('account_did')
         if m.get('offset_balance') is not None:
             self.offset_balance = m.get('offset_balance')
         return self
 
 
+class DetailEcarOffsetdatumRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        acquisition_item_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务发生时的调用方的业务单号
+        self.acquisition_item_no = acquisition_item_no
+
+    def validate(self):
+        self.validate_required(self.acquisition_item_no, 'acquisition_item_no')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.acquisition_item_no is not None:
+            result['acquisition_item_no'] = self.acquisition_item_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('acquisition_item_no') is not None:
+            self.acquisition_item_no = m.get('acquisition_item_no')
+        return self
+
+
+class DetailEcarOffsetdatumResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        project_no: str = None,
+        project_name: str = None,
+        account_did: str = None,
+        acquisition_item_no: str = None,
+        occurrent_time: str = None,
+        scenario_code: str = None,
+        scenario_name: str = None,
+        platform_no: str = None,
+        offset_volume: str = None,
+        carbon_energy: int = None,
+        active_data_list: List[CarbonOffsetActiveDataDetail] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 碳补偿项目编码
+        self.project_no = project_no
+        # 碳普惠项目名称
+        self.project_name = project_name
+        # 会员账户DID
+        self.account_did = account_did
+        # 采集数据单号
+        # 
+        self.acquisition_item_no = acquisition_item_no
+        # 发生时间
+        self.occurrent_time = occurrent_time
+        # 发生场景编码
+        self.scenario_code = scenario_code
+        # 发生场景名称
+        self.scenario_name = scenario_name
+        # 碳普惠平台编码，如果非平台采集数据，则显示为自采编码：Self
+        self.platform_no = platform_no
+        # 减碳量
+        self.offset_volume = offset_volume
+        # 碳能量值
+        self.carbon_energy = carbon_energy
+        # 活动数据详情列表
+        self.active_data_list = active_data_list
+
+    def validate(self):
+        if self.active_data_list:
+            for k in self.active_data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        if self.project_name is not None:
+            result['project_name'] = self.project_name
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.acquisition_item_no is not None:
+            result['acquisition_item_no'] = self.acquisition_item_no
+        if self.occurrent_time is not None:
+            result['occurrent_time'] = self.occurrent_time
+        if self.scenario_code is not None:
+            result['scenario_code'] = self.scenario_code
+        if self.scenario_name is not None:
+            result['scenario_name'] = self.scenario_name
+        if self.platform_no is not None:
+            result['platform_no'] = self.platform_no
+        if self.offset_volume is not None:
+            result['offset_volume'] = self.offset_volume
+        if self.carbon_energy is not None:
+            result['carbon_energy'] = self.carbon_energy
+        result['active_data_list'] = []
+        if self.active_data_list is not None:
+            for k in self.active_data_list:
+                result['active_data_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        if m.get('project_name') is not None:
+            self.project_name = m.get('project_name')
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('acquisition_item_no') is not None:
+            self.acquisition_item_no = m.get('acquisition_item_no')
+        if m.get('occurrent_time') is not None:
+            self.occurrent_time = m.get('occurrent_time')
+        if m.get('scenario_code') is not None:
+            self.scenario_code = m.get('scenario_code')
+        if m.get('scenario_name') is not None:
+            self.scenario_name = m.get('scenario_name')
+        if m.get('platform_no') is not None:
+            self.platform_no = m.get('platform_no')
+        if m.get('offset_volume') is not None:
+            self.offset_volume = m.get('offset_volume')
+        if m.get('carbon_energy') is not None:
+            self.carbon_energy = m.get('carbon_energy')
+        self.active_data_list = []
+        if m.get('active_data_list') is not None:
+            for k in m.get('active_data_list'):
+                temp_model = CarbonOffsetActiveDataDetail()
+                self.active_data_list.append(temp_model.from_map(k))
+        return self
+
+
+class DetailEcarOffsettranslateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        translation_item_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 减碳数据转移记录业务方的业务单号
+        self.translation_item_no = translation_item_no
+
+    def validate(self):
+        self.validate_required(self.translation_item_no, 'translation_item_no')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.translation_item_no is not None:
+            result['translation_item_no'] = self.translation_item_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('translation_item_no') is not None:
+            self.translation_item_no = m.get('translation_item_no')
+        return self
+
+
+class DetailEcarOffsettranslateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        translation_item_no: str = None,
+        occurrence_time: str = None,
+        amount: str = None,
+        project_no: str = None,
+        project_name: str = None,
+        drawing_account_did: str = None,
+        receipt_account_did: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 业务方的业务单号
+        self.translation_item_no = translation_item_no
+        # 发生时间
+        self.occurrence_time = occurrence_time
+        # 业务发生量：转移量
+        self.amount = amount
+        # 碳补偿项目编码
+        self.project_no = project_no
+        # 碳普惠项目名称
+        self.project_name = project_name
+        # 转出碳账户DID
+        self.drawing_account_did = drawing_account_did
+        # 转入碳账户DID
+        self.receipt_account_did = receipt_account_did
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.translation_item_no is not None:
+            result['translation_item_no'] = self.translation_item_no
+        if self.occurrence_time is not None:
+            result['occurrence_time'] = self.occurrence_time
+        if self.amount is not None:
+            result['amount'] = self.amount
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        if self.project_name is not None:
+            result['project_name'] = self.project_name
+        if self.drawing_account_did is not None:
+            result['drawing_account_did'] = self.drawing_account_did
+        if self.receipt_account_did is not None:
+            result['receipt_account_did'] = self.receipt_account_did
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('translation_item_no') is not None:
+            self.translation_item_no = m.get('translation_item_no')
+        if m.get('occurrence_time') is not None:
+            self.occurrence_time = m.get('occurrence_time')
+        if m.get('amount') is not None:
+            self.amount = m.get('amount')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        if m.get('project_name') is not None:
+            self.project_name = m.get('project_name')
+        if m.get('drawing_account_did') is not None:
+            self.drawing_account_did = m.get('drawing_account_did')
+        if m.get('receipt_account_did') is not None:
+            self.receipt_account_did = m.get('receipt_account_did')
+        return self
+
+
 class QueryThirdCertRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         product_id: str = None,
         certification_type: str = None,
```

### Comparing `antchain_stlr-2.4.0/antchain_stlr.egg-info/PKG-INFO` & `antchain_stlr-2.5.0/antchain_stlr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-stlr
-Version: 2.4.0
+Version: 2.5.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.4.0/setup.py` & `antchain_stlr-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_stlr.
 
-Created on 05/06/2023
+Created on 12/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_stlr"
 NAME = "antchain_stlr" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain STLR SDK Library for Python"
```

