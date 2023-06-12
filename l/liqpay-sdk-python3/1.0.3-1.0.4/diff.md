# Comparing `tmp/liqpay-sdk-python3-1.0.3.tar.gz` & `tmp/liqpay-sdk-python3-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/liqpay-sdk-python3-1.0.3.tar", last modified: Mon Jun 22 08:14:45 2020, max compression
+gzip compressed data, was "liqpay-sdk-python3-1.0.4.tar", last modified: Mon Jun 12 15:49:15 2023, max compression
```

## Comparing `liqpay-sdk-python3-1.0.3.tar` & `liqpay-sdk-python3-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2020-06-22 08:14:45.000000 liqpay-sdk-python3-1.0.3/
--rw-r--r--   0 alex       (501) staff       (20)     6878 2020-06-22 08:14:45.000000 liqpay-sdk-python3-1.0.3/PKG-INFO
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2020-06-22 08:14:45.000000 liqpay-sdk-python3-1.0.3/liqpay_sdk_python3.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     6878 2020-06-22 08:14:44.000000 liqpay-sdk-python3-1.0.3/liqpay_sdk_python3.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      321 2020-06-22 08:14:44.000000 liqpay-sdk-python3-1.0.3/liqpay_sdk_python3.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        9 2020-06-22 08:14:44.000000 liqpay-sdk-python3-1.0.3/liqpay_sdk_python3.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        7 2020-06-22 08:14:44.000000 liqpay-sdk-python3-1.0.3/liqpay_sdk_python3.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2020-06-22 08:14:44.000000 liqpay-sdk-python3-1.0.3/liqpay_sdk_python3.egg-info/dependency_links.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2020-06-22 08:14:45.000000 liqpay-sdk-python3-1.0.3/liqpay/
--rw-r--r--   0 alex       (501) staff       (20)     5632 2020-06-22 07:55:51.000000 liqpay-sdk-python3-1.0.3/liqpay/liqpay3.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2020-06-22 08:14:45.000000 liqpay-sdk-python3-1.0.3/liqpay/tests/
--rw-r--r--   0 alex       (501) staff       (20)        0 2020-06-19 11:14:50.000000 liqpay-sdk-python3-1.0.3/liqpay/tests/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1617 2020-06-19 11:16:05.000000 liqpay-sdk-python3-1.0.3/liqpay/tests/test_pay_simple.py
--rw-r--r--   0 alex       (501) staff       (20)       24 2020-06-19 11:14:32.000000 liqpay-sdk-python3-1.0.3/liqpay/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5212 2020-06-22 08:11:06.000000 liqpay-sdk-python3-1.0.3/README.md
--rw-r--r--   0 alex       (501) staff       (20)      475 2020-06-22 08:13:04.000000 liqpay-sdk-python3-1.0.3/setup.py
--rw-r--r--   0 alex       (501) staff       (20)       38 2020-06-22 08:14:45.000000 liqpay-sdk-python3-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 15:49:15.424590 liqpay-sdk-python3-1.0.4/
+-rw-rw-rw-   0        0        0     5561 2023-06-12 15:49:15.424590 liqpay-sdk-python3-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5368 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 15:49:15.414590 liqpay-sdk-python3-1.0.4/liqpay/
+-rw-rw-rw-   0        0        0       24 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/liqpay/__init__.py
+-rw-rw-rw-   0        0        0     6790 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/liqpay/liqpay3.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:49:15.416589 liqpay-sdk-python3-1.0.4/liqpay/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-12 10:46:25.000000 liqpay-sdk-python3-1.0.4/liqpay/tests/__init__.py
+-rw-rw-rw-   0        0        0     1137 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/liqpay/tests/test_pay_simple.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:49:15.422590 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/
+-rw-rw-rw-   0        0        0     5561 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 15:49:15.000000 liqpay-sdk-python3-1.0.4/liqpay_sdk_python3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 15:49:15.425593 liqpay-sdk-python3-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      493 2023-06-12 15:48:54.000000 liqpay-sdk-python3-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `liqpay-sdk-python3-1.0.3/liqpay/liqpay3.py` & `liqpay-sdk-python3-1.0.4/liqpay/liqpay3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,160 +1,187 @@
-"""
-LiqPay Python SDK
-~~~~~~~~~~~~~~~~~
-supports python 3 version
-requires requests module
-"""
-
-__title__ = "LiqPay Python3 SDK"
-__version__ = "1.0.1"
-
-import base64
-from copy import deepcopy
-import hashlib
-import json
-from urllib.parse import urljoin
-
-import requests
-
-
-class ParamValidationError(Exception):
-    pass
-
-
-class LiqPay(object):
-    FORM_TEMPLATE = """\
-        <form method="post" action="{action}" accept-charset="utf-8">
-        \t{param_inputs}
-            <input type="image" src="//static.liqpay.ua/buttons/p1{language}.radius.png" name="btn_text" />
-        </form>"""
-    INPUT_TEMPLATE = "<input type='hidden' name='{name}' value='{value}'/>"
-
-    SUPPORTED_PARAMS = [
-        "public_key", "amount", "currency", "description", "order_id",
-        "result_url", "server_url", "type", "signature", "language", "sandbox"
-    ]
-
-    def __init__(self, public_key, private_key, host="https://www.liqpay.ua/api/"):
-        self._public_key = public_key
-        self._private_key = private_key
-        self._host = host
-
-    def _make_signature(self, *args):
-        joined_fields = "".join(x for x in args)
-        joined_fields = joined_fields.encode("utf-8")
-        return base64.b64encode(hashlib.sha1(joined_fields).digest()).decode("ascii")
-
-    def _prepare_params(self, params):
-        params = {} if params is None else deepcopy(params)
-        params.update(public_key=self._public_key)
-        return params
-
-    def _encode_params(self, params):
-        """
-        :param params: dict
-        :return: dict
-        """
-        params = self._prepare_params(params)
-        params_validator = (
-            ("amount", lambda x: x is not None and float(x) > 0),
-            ("description", lambda x: x is not None)
-        )
-        for key, validator in params_validator:
-            if validator(params.get(key)):
-                continue
-
-            raise ParamValidationError("Invalid param: '{}'".format(key))
-
-        # spike to set correct values for language, currency and sandbox params
-        language = params.get("language", "ru")
-        currency = params["currency"]
-        params.update(
-            language=language,
-            currency=currency if currency != "RUR" else "RUB",
-            sandbox=int(bool(params.get("sandbox")))
-        )
-
-        encoded_data = self.data_to_sign(params)
-        return encoded_data
-
-
-    def api(self, url, params=None):
-        params = self._prepare_params(params)
-
-        json_encoded_params = json.dumps(params)
-        private_key = self._private_key
-        signature = self._make_signature(private_key, json_encoded_params, private_key)
-
-        request_url = urljoin(self._host, url)
-        request_data = {"data": json_encoded_params, "signature": signature}
-        response = requests.post(request_url, data=request_data, verify=False)
-        return json.loads(response.content.decode("utf-8"))
-
-    def checkout_url(self, params):
-        """
-        This method contains almost same like cnb_form, except we are return just
-        url which will helpful for building Restful services.
-        :param params:
-        :return:
-        """
-        encoded_data = self._encode_params(params)
-        signature = self._make_signature(self._private_key, encoded_data, self._private_key)
-        form_action_url = urljoin(self._host, "3/checkout/")
-
-        return f'{form_action_url}?data={encoded_data}&signature={signature}'
-
-    def cnb_form(self, params):
-        encoded_data = self._encode_params(params)
-        params_templ = {"data": encoded_data}
-        language = params.get("language", "ru")
-
-        params_templ["signature"] = self._make_signature(self._private_key, params_templ["data"], self._private_key)
-        form_action_url = urljoin(self._host, "3/checkout/")
-        format_input = (lambda k, v: self.INPUT_TEMPLATE.format(name=k, value=v))
-        inputs = [format_input(k, v) for k, v in params_templ.items()]
-        return self.FORM_TEMPLATE.format(
-            action=form_action_url,
-            language=language,
-            param_inputs="\n\t".join(inputs)
-        )
-
-    def cnb_signature(self, params):
-        params = self._prepare_params(params)
-
-        data_to_sign = self.data_to_sign(params)
-        return self._make_signature(self._private_key, data_to_sign, self._private_key)
-
-    def cnb_data(self, params):
-        params = self._prepare_params(params)
-        return self.data_to_sign(params)
-
-    def str_to_sign(self, str):
-        return base64.b64encode(hashlib.sha1(str.encode("utf-8")).digest()).decode("ascii")
-
-    def data_to_sign(self, params):
-        return base64.b64encode(json.dumps(params).encode("utf-8")).decode("ascii")
-
-    def decode_data_from_str(self, data):
-        """Decoding data that were encoded by base64.b64encode(str)
-
-        Note:
-            Often case of using is decoding data from LiqPay Callback.
-            Dict contains all information about payment.
-            More info about callback params see in documentation
-            https://www.liqpay.ua/documentation/api/callback.
-
-        Args:
-            data: json string with api params and encoded by base64.b64encode(str).
-
-        Returns:
-            Dict
-
-        Example:
-            liqpay = LiqPay(settings.LIQPAY_PUBLIC_KEY, settings.LIQPAY_PRIVATE_KEY)
-            data = request.POST.get('data')
-            response = liqpay.decode_data_from_str(data)
-            print(response)
-            {'commission_credit': 0.0, 'order_id': 'order_id_1', 'liqpay_order_id': 'T8SRXWM71509085055293216', ...}
-
-        """
-        return json.loads(base64.b64decode(data).decode('utf-8'))
+"""
+LiqPay Python SDK
+~~~~~~~~~~~~~~~~~
+supports python 3 version
+requires requests module
+"""
+
+__title__ = "LiqPay Python3 SDK"
+__version__ = "1.0.4"
+
+import base64
+from copy import deepcopy
+import hashlib
+import json
+from urllib.parse import urljoin
+
+import requests
+
+
+TRANSLATIONS = {
+    "en": "PAY",
+    "ru": "Оплатить",
+    "uk": "Сплатити",
+}
+
+
+class ParamValidationError(Exception):
+    pass
+
+
+class LiqPay(object):
+    FORM_TEMPLATE = """<form method="POST" action="{action}" accept-charset="utf-8">
+        \t{param_inputs}
+            <button style="border: none !important;display:inline-block !important;text-align: center !important; padding: 7px 20px !important; color: #fff !important;font-size:16px !important; font-weight: 600 !important; font-family:OpenSans, sans-serif;cursor: pointer !important;border-radius: 2px !important;background: rgba(122,183,43,1) !important;"onmouseover="this.style.opacity=0.5;" onmouseout="this.style.opacity=1;"> <img src="https://static.liqpay.ua/buttons/logo-small.png" name="btn_text" style="margin-right: 7px !important; vertical-align: middle !important;"/> 
+            <span style="vertical-align:middle;!important">{text} {amount} {currency}</span>
+            </button>
+    </form>"""
+    INPUT_TEMPLATE = "<input type='hidden' name='{name}' value='{value}'/>"
+
+    SUPPORTED_PARAMS = [
+        "public_key",
+        "amount",
+        "currency",
+        "description",
+        "order_id",
+        "result_url",
+        "server_url",
+        "type",
+        "signature",
+        "language",
+        "sandbox",
+    ]
+
+    def __init__(self, public_key, private_key, host="https://www.liqpay.ua/api/"):
+        self._public_key = public_key
+        self._private_key = private_key
+        self._host = host
+
+    def _make_signature(self, *args):
+        joined_fields = "".join(x for x in args)
+        joined_fields = joined_fields.encode("utf-8")
+        return base64.b64encode(hashlib.sha1(joined_fields).digest()).decode("ascii")
+
+    def _prepare_params(self, params):
+        params = {} if params is None else deepcopy(params)
+        params.update(public_key=self._public_key)
+        return params
+
+    def _encode_params(self, params):
+        """
+        :param params: dict
+        :return: dict
+        """
+        params = self._prepare_params(params)
+        params_validator = (
+            ("amount", lambda x: x is not None and float(x) > 0),
+            ("description", lambda x: x is not None),
+        )
+        for key, validator in params_validator:
+            if validator(params.get(key)):
+                continue
+
+            raise ParamValidationError("Invalid param: '{}'".format(key))
+
+        # spike to set correct values for language, currency and sandbox params
+        language = params.get("language", "ru")
+        currency = params["currency"]
+        params.update(
+            language=language,
+            currency=currency if currency != "RUR" else "RUB",
+            sandbox=int(bool(params.get("sandbox"))),
+        )
+
+        encoded_data = self.data_to_sign(params)
+        return encoded_data
+
+    def api(self, url, params=None):
+        params = self._prepare_params(params)
+
+        json_encoded_params = json.dumps(params)
+        private_key = self._private_key
+        signature = self._make_signature(private_key, json_encoded_params, private_key)
+
+        request_url = urljoin(self._host, url)
+        request_data = {"data": json_encoded_params, "signature": signature}
+        response = requests.post(request_url, data=request_data, verify=False)
+        return json.loads(response.content.decode("utf-8"))
+
+    def checkout_url(self, params):
+        """
+        This method contains almost same like cnb_form, except we are return just
+        url which will helpful for building Restful services.
+        :param params:
+        :return:
+        """
+        encoded_data = self._encode_params(params)
+        signature = self._make_signature(
+            self._private_key, encoded_data, self._private_key
+        )
+        form_action_url = urljoin(self._host, "3/checkout/")
+
+        return f"{form_action_url}?data={encoded_data}&signature={signature}"
+
+    def cnb_form(self, params):
+        encoded_data = self._encode_params(params)
+        params_templ = {"data": encoded_data}
+        language = params.get("language", "uk")
+
+        params_templ["signature"] = self._make_signature(
+            self._private_key, params_templ["data"], self._private_key
+        )
+        form_action_url = urljoin(self._host, "3/checkout/")
+        inputs = [self.format_input(k, v) for k, v in params_templ.items()]
+        return self.FORM_TEMPLATE.format(
+            action=form_action_url,
+            language=language,
+            text=TRANSLATIONS.get(language, "uk"),
+            amount=params["amount"],
+            currency=params["currency"],
+            param_inputs="\n\t".join(inputs),
+        )
+
+    def cnb_signature(self, params):
+        params = self._prepare_params(params)
+
+        data_to_sign = self.data_to_sign(params)
+        return self._make_signature(self._private_key, data_to_sign, self._private_key)
+
+    def cnb_data(self, params):
+        params = self._prepare_params(params)
+        return self.data_to_sign(params)
+
+    def str_to_sign(self, str):
+        return base64.b64encode(hashlib.sha1(str.encode("utf-8")).digest()).decode(
+            "ascii"
+        )
+
+    def data_to_sign(self, params):
+        return base64.b64encode(json.dumps(params).encode("utf-8")).decode("ascii")
+
+    def decode_data_from_str(self, data):
+        """Decoding data that were encoded by base64.b64encode(str)
+
+        Note:
+            Often case of using is decoding data from LiqPay Callback.
+            Dict contains all information about payment.
+            More info about callback params see in documentation
+            https://www.liqpay.ua/documentation/api/callback.
+
+        Args:
+            data: json string with api params and encoded by base64.b64encode(str).
+
+        Returns:
+            Dict
+
+        Example:
+            liqpay = LiqPay(settings.LIQPAY_PUBLIC_KEY, settings.LIQPAY_PRIVATE_KEY)
+            data = request.POST.get('data')
+            response = liqpay.decode_data_from_str(data)
+            print(response)
+            {'commission_credit': 0.0, 'order_id': 'order_id_1', 'liqpay_order_id': 'T8SRXWM71509085055293216', ...}
+
+        """
+        return json.loads(base64.b64decode(data).decode("utf-8"))
+
+    def format_input(self, key, value):
+        return self.INPUT_TEMPLATE.format(name=key, value=value)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `liqpay-sdk-python3-1.0.3/README.md` & `liqpay-sdk-python3-1.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,180 +1,183 @@
-[![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
-
-|liqpaylogo| image::  https://www.liqpay.ua/1508940109424071/static/img/images/logo.svg
-
-=====
-|liqpaylogo| SDK-Python
-=====
-
-:Version: 1.0.2
-:Web: https://www.liqpay.ua/
-:Download: https://pypi.org/project/liqpay-sdk-python3/
-:Source: https://github.com/aorzh/liqpay-sdk-python3
-:Documentation: https://www.liqpay.ua/documentation/en/
-:Keywords: liqpay, privat24, privatbank, python, internet acquiring, P2P payments, two-step payments
-
-
-What python version is supported?
-============
-- Python 3.4, 3.5, 3.6
-
-Get Started
-============
-1. Sign up in https://www.liqpay.ua/en/authorization.
-2. Create a company.
-3. In company settings, on API tab, get **Public key** and **Private key**.
-4. Done.
-
-Installation
-============
-From pip
-```pip install liqpay-sdk-python3```
-
-Working with LiqPay Callback locally
-============
-If you need debugging API Callback on local environment use https://localtunnel.github.io/www/
-
-How it use?
-============
-
-Example 1: Basic
--------
-
-**Backend**
-Get payment button (html response)
-```
-liqpay = LiqPay(public_key, private_key)
-html = liqpay.cnb_form({
-    'action': 'pay',
-    'amount': '1',
-    'currency': 'USD',
-    'description': 'description text',
-    'order_id': 'order_id_1',
-    'version': '3',
-    'language': 'ru|uk|en'
-})
-```
-
-Get plain checkout url:
-
-```
-liqpay = LiqPay(public_key, private_key)
-html = liqpay.checkout_url({
-    'action': 'auth',
-    'amount': '1',
-    'currency': 'USD',
-    'description': 'description text',
-    'order_id': 'order_id_1',
-    'version': '3',
-    'language': 'ru|uk|en',
-    'recurringbytoken': '1'
-})
-# Response:
-
-str: https://www.liqpay.ua/api/3/checkout/?data=<decoded data>&signature=<decoded signature>
-
-```
-
-
-**Frontend**
-
-Variable ``html`` will contain next html form
-
-```
-    <form method="POST" action="https://www.liqpay.ua/api/3/checkout" accept-charset="utf-8">
-        <input type="hidden" name="data" value="eyAidmVyc2lvbiIgOiAzLCAicHVibGljX2tleSIgOiAieW91cl9wdWJsaWNfa2V5IiwgImFjdGlv
-        biIgOiAicGF5IiwgImFtb3VudCIgOiAxLCAiY3VycmVuY3kiIDogIlVTRCIsICJkZXNjcmlwdGlv
-        biIgOiAiZGVzY3JpcHRpb24gdGV4dCIsICJvcmRlcl9pZCIgOiAib3JkZXJfaWRfMSIgfQ=="/>
-        <input type="hidden" name="signature" value="QvJD5u9Fg55PCx/Hdz6lzWtYwcI="/>
-        <input type="image"
-        src="//static.liqpay.ua/buttons/p1ru.radius.png"/>
-    </form>
-```
-
-Example 2: Integrate Payment widget to Django
--------
-`Payment widget documentation` 
-https://www.liqpay.ua/documentation/en/api/aquiring/widget/
-
-*Backend*
-
-`views.py`
-
-```
-
-    from liqpay import LiqPay
-
-    from django.views.generic import TemplateView
-    from django.shortcuts import render
-    from django.http import HttpResponse
-
-    class PayView(TemplateView):
-    template_name = 'billing/pay.html'
-
-    def get(self, request, *args, **kwargs):
-        liqpay = LiqPay(settings.LIQPAY_PUBLIC_KEY, settings.LIQPAY_PRIVATE_KEY)
-        params = {
-            'action': 'pay',
-            'amount': '100',
-            'currency': 'USD',
-            'description': 'Payment for clothes',
-            'order_id': 'order_id_1',
-            'version': '3',
-            'sandbox': 0, # sandbox mode, set to 1 to enable it
-            'server_url': 'https://test.com/billing/pay-callback/', # url to callback view
-        }
-        signature = liqpay.cnb_signature(params)
-        data = liqpay.cnb_data(params)
-        return render(request, self.template_name, {'signature': signature, 'data': data})
-
-    @method_decorator(csrf_exempt, name='dispatch')
-    class PayCallbackView(View):
-        def post(self, request, *args, **kwargs):
-            liqpay = LiqPay(settings.LIQPAY_PUBLIC_KEY, settings.LIQPAY_PRIVATE_KEY)
-            data = request.POST.get('data')
-            signature = request.POST.get('signature')
-            sign = liqpay.str_to_sign(settings.LIQPAY_PRIVATE_KEY + data + settings.LIQPAY_PRIVATE_KEY)
-            if sign == signature:
-                print('callback is valid')
-            response = liqpay.decode_data_from_str(data)
-            print('callback data', response)
-            return HttpResponse()
-```
-`urls.py`
-
-```
-
-    from django.conf.urls import url
-
-    from billing.views import PayView, PayCallbackView
-
-
-    urlpatterns = [
-        url(r'^pay/$', PayView.as_view(), name='pay_view'),
-        url(r'^pay-callback/$', PayCallbackView.as_view(), name='pay_callback'),
-    ]
-```
-*Frontend*
-
-```
-
-    <div id="liqpay_checkout"></div>
-    <script>
-        window.LiqPayCheckoutCallback = function() {
-            LiqPayCheckout.init({
-                data: "{{ data }}",
-                signature: "{{ signature }}",
-                embedTo: "#liqpay_checkout",
-                mode: "embed" // embed || popup,
-            }).on("liqpay.callback", function(data){
-                console.log(data.status);
-                console.log(data);
-            }).on("liqpay.ready", function(data){
-                // ready
-            }).on("liqpay.close", function(data){
-                // close
-            });
-        };
-    </script>
-    <script src="//static.liqpay.ua/libjs/checkout.js" async></script>
-```
+Metadata-Version: 2.1
+Name: liqpay-sdk-python3
+Version: 1.0.4
+Summary: LiqPay Python3 SDK
+Home-page: https://github.com/aorzh/liqpay-sdk-python3
+Description-Content-Type: text/markdown
+
+[![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+
+[![SDK-Python3](https://www.liqpay.ua/logo_liqpay_main.svg)](https://www.liqpay.ua/documentation/api/home)
+
+* Version: 1.0.3
+* Web: https://www.liqpay.ua/
+* Download: https://pypi.org/project/liqpay-sdk-python3/
+* Source: https://github.com/aorzh/liqpay-sdk-python3
+* Documentation: https://www.liqpay.ua/documentation/en/
+* Keywords: liqpay, privat24, privatbank, python, internet acquiring, P2P payments, two-step payments
+
+
+What python version is supported?
+============
+- Python 3.4+
+
+Get Started
+============
+1. Sign up in https://www.liqpay.ua/en/authorization.
+2. Create a company.
+3. In company settings, on API tab, get **Public key** and **Private key**.
+4. Done.
+
+Installation
+============
+From pip
+```pip install liqpay-sdk-python3```
+
+Working with LiqPay Callback locally
+============
+If you need debugging API Callback on local environment use https://localtunnel.github.io/www/
+
+How it use?
+============
+
+Example 1: Basic
+-------
+
+**Backend**
+Get payment button (html response)
+```
+liqpay = LiqPay(public_key, private_key)
+html = liqpay.cnb_form({
+    'action': 'pay',
+    'amount': '1',
+    'currency': 'USD',
+    'description': 'description text',
+    'order_id': 'order_id_1',
+    'version': '3',
+    'language': 'ru|uk|en'
+})
+```
+
+Get plain checkout url:
+
+```
+liqpay = LiqPay(public_key, private_key)
+html = liqpay.checkout_url({
+    'action': 'auth',
+    'amount': '1',
+    'currency': 'USD',
+    'description': 'description text',
+    'order_id': 'order_id_1',
+    'version': '3',
+    'language': 'ru|uk|en',
+    'recurringbytoken': '1'
+})
+# Response:
+
+str: https://www.liqpay.ua/api/3/checkout/?data=<decoded data>&signature=<decoded signature>
+
+```
+
+
+**Frontend**
+
+Variable ``html`` will contain next html form
+
+```
+    <form method="POST" action="https://www.liqpay.ua/api/3/checkout" accept-charset="utf-8">
+        <input type="hidden" name="data" value="eyAidmVyc2lvbiIgOiAzLCAicHVibGljX2tleSIgOiAieW91cl9wdWJsaWNfa2V5IiwgImFjdGlv
+        biIgOiAicGF5IiwgImFtb3VudCIgOiAxLCAiY3VycmVuY3kiIDogIlVTRCIsICJkZXNjcmlwdGlv
+        biIgOiAiZGVzY3JpcHRpb24gdGV4dCIsICJvcmRlcl9pZCIgOiAib3JkZXJfaWRfMSIgfQ=="/>
+        <input type="hidden" name="signature" value="QvJD5u9Fg55PCx/Hdz6lzWtYwcI="/>
+        <input type="image"
+        src="//static.liqpay.ua/buttons/p1ru.radius.png"/>
+    </form>
+```
+
+Example 2: Integrate Payment widget to Django
+-------
+`Payment widget documentation` 
+https://www.liqpay.ua/documentation/en/api/aquiring/widget/
+
+*Backend*
+
+`views.py`
+
+```
+
+    from liqpay import LiqPay
+
+    from django.views.generic import TemplateView
+    from django.shortcuts import render
+    from django.http import HttpResponse
+
+    class PayView(TemplateView):
+    template_name = 'billing/pay.html'
+
+    def get(self, request, *args, **kwargs):
+        liqpay = LiqPay(settings.LIQPAY_PUBLIC_KEY, settings.LIQPAY_PRIVATE_KEY)
+        params = {
+            'action': 'pay',
+            'amount': '100',
+            'currency': 'USD',
+            'description': 'Payment for clothes',
+            'order_id': 'order_id_1',
+            'version': '3',
+            'sandbox': 0, # sandbox mode, set to 1 to enable it
+            'server_url': 'https://test.com/billing/pay-callback/', # url to callback view
+        }
+        signature = liqpay.cnb_signature(params)
+        data = liqpay.cnb_data(params)
+        return render(request, self.template_name, {'signature': signature, 'data': data})
+
+    @method_decorator(csrf_exempt, name='dispatch')
+    class PayCallbackView(View):
+        def post(self, request, *args, **kwargs):
+            liqpay = LiqPay(settings.LIQPAY_PUBLIC_KEY, settings.LIQPAY_PRIVATE_KEY)
+            data = request.POST.get('data')
+            signature = request.POST.get('signature')
+            sign = liqpay.str_to_sign(settings.LIQPAY_PRIVATE_KEY + data + settings.LIQPAY_PRIVATE_KEY)
+            if sign == signature:
+                print('callback is valid')
+            response = liqpay.decode_data_from_str(data)
+            print('callback data', response)
+            return HttpResponse()
+```
+`urls.py`
+
+```
+
+    from django.conf.urls import url
+
+    from billing.views import PayView, PayCallbackView
+
+
+    urlpatterns = [
+        url(r'^pay/$', PayView.as_view(), name='pay_view'),
+        url(r'^pay-callback/$', PayCallbackView.as_view(), name='pay_callback'),
+    ]
+```
+*Frontend*
+
+```
+
+    <div id="liqpay_checkout"></div>
+    <script>
+        window.LiqPayCheckoutCallback = function() {
+            LiqPayCheckout.init({
+                data: "{{ data }}",
+                signature: "{{ signature }}",
+                embedTo: "#liqpay_checkout",
+                mode: "embed" // embed || popup,
+            }).on("liqpay.callback", function(data){
+                console.log(data.status);
+                console.log(data);
+            }).on("liqpay.ready", function(data){
+                // ready
+            }).on("liqpay.close", function(data){
+                // close
+            });
+        };
+    </script>
+    <script src="//static.liqpay.ua/libjs/checkout.js" async></script>
+```
```

