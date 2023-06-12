# Comparing `tmp/splitit_web_python_sdk-2.2.0.tar.gz` & `tmp/splitit_web_python_sdk-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitit_web_python_sdk-2.2.0.tar", max compression
+gzip compressed data, was "splitit_web_python_sdk-2.3.0.tar", max compression
```

## Comparing `splitit_web_python_sdk-2.2.0.tar` & `splitit_web_python_sdk-2.3.0.tar`

### file list

```diff
@@ -1,228 +1,228 @@
--rw-r--r--   0        0        0     1081 2023-06-08 11:55:07.661154 splitit_web_python_sdk-2.2.0/LICENSE
--rw-r--r--   0        0        0     8335 2023-06-08 11:55:07.728491 splitit_web_python_sdk-2.2.0/README.md
--rw-r--r--   0        0        0      737 2023-06-08 11:55:07.608986 splitit_web_python_sdk-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      725 2023-06-08 11:55:07.609258 splitit_web_python_sdk-2.2.0/splitit_client/__init__.py
--rw-r--r--   0        0        0    73578 2023-06-08 11:55:07.609403 splitit_web_python_sdk-2.2.0/splitit_client/api_client.py
--rw-r--r--   0        0        0      663 2023-06-08 11:55:07.609506 splitit_web_python_sdk-2.2.0/splitit_client/api_response.py
--rw-r--r--   0        0        0      214 2023-06-08 11:55:07.609599 splitit_web_python_sdk-2.2.0/splitit_client/apis/__init__.py
--rw-r--r--   0        0        0     3411 2023-06-08 11:55:07.609690 splitit_web_python_sdk-2.2.0/splitit_client/apis/path_to_api.py
--rw-r--r--   0        0        0      241 2023-06-08 11:55:07.609784 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      127 2023-06-08 11:55:07.609867 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans.py
--rw-r--r--   0        0        0      161 2023-06-08 11:55:07.609966 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_check_eligibility.py
--rw-r--r--   0        0        0      144 2023-06-08 11:55:07.610068 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_initiate.py
--rw-r--r--   0        0        0      169 2023-06-08 11:55:07.610169 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number.py
--rw-r--r--   0        0        0      185 2023-06-08 11:55:07.610276 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_cancel.py
--rw-r--r--   0        0        0      185 2023-06-08 11:55:07.610372 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_refund.py
--rw-r--r--   0        0        0      192 2023-06-08 11:55:07.610472 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_updateorder.py
--rw-r--r--   0        0        0      208 2023-06-08 11:55:07.610580 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_verifyauthorization.py
--rw-r--r--   0        0        0      137 2023-06-08 11:55:07.610666 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_search.py
--rw-r--r--   0        0        0      147 2023-06-08 11:55:07.610751 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_updateorder.py
--rw-r--r--   0        0        0      371 2023-06-08 11:55:07.610827 splitit_web_python_sdk-2.2.0/splitit_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      328 2023-06-08 11:55:07.610917 splitit_web_python_sdk-2.2.0/splitit_client/apis/tags/__init__.py
--rw-r--r--   0        0        0     1333 2023-06-08 11:55:07.610998 splitit_web_python_sdk-2.2.0/splitit_client/apis/tags/installment_plan_api.py
--rw-r--r--   0        0        0      989 2023-06-08 11:55:07.611082 splitit_web_python_sdk-2.2.0/splitit_client/client.py
--rw-r--r--   0        0        0      989 2023-06-08 11:55:07.611166 splitit_web_python_sdk-2.2.0/splitit_client/client.pyi
--rw-r--r--   0        0        0      669 2023-06-08 11:55:07.611270 splitit_web_python_sdk-2.2.0/splitit_client/client_custom.py
--rw-r--r--   0        0        0    18575 2023-06-08 11:55:07.611375 splitit_web_python_sdk-2.2.0/splitit_client/configuration.py
--rw-r--r--   0        0        0     7311 2023-06-08 11:55:07.611475 splitit_web_python_sdk-2.2.0/splitit_client/exceptions.py
--rw-r--r--   0        0        0     2274 2023-06-08 11:55:07.611606 splitit_web_python_sdk-2.2.0/splitit_client/exceptions_base.py
--rw-r--r--   0        0        0      348 2023-06-08 11:55:07.611770 splitit_web_python_sdk-2.2.0/splitit_client/model/__init__.py
--rw-r--r--   0        0        0     4871 2023-06-08 11:55:07.611881 splitit_web_python_sdk-2.2.0/splitit_client/model/address_data.py
--rw-r--r--   0        0        0     4871 2023-06-08 11:55:07.612011 splitit_web_python_sdk-2.2.0/splitit_client/model/address_data.pyi
--rw-r--r--   0        0        0     4894 2023-06-08 11:55:07.612152 splitit_web_python_sdk-2.2.0/splitit_client/model/address_data_model.py
--rw-r--r--   0        0        0     4894 2023-06-08 11:55:07.612282 splitit_web_python_sdk-2.2.0/splitit_client/model/address_data_model.pyi
--rw-r--r--   0        0        0     7418 2023-06-08 11:55:07.612459 splitit_web_python_sdk-2.2.0/splitit_client/model/authorization_model.py
--rw-r--r--   0        0        0     7418 2023-06-08 11:55:07.612659 splitit_web_python_sdk-2.2.0/splitit_client/model/authorization_model.pyi
--rw-r--r--   0        0        0     1752 2023-06-08 11:55:07.612803 splitit_web_python_sdk-2.2.0/splitit_client/model/card_brand.py
--rw-r--r--   0        0        0     1392 2023-06-08 11:55:07.613150 splitit_web_python_sdk-2.2.0/splitit_client/model/card_brand.pyi
--rw-r--r--   0        0        0     5874 2023-06-08 11:55:07.614295 splitit_web_python_sdk-2.2.0/splitit_client/model/card_data.py
--rw-r--r--   0        0        0     5874 2023-06-08 11:55:07.614545 splitit_web_python_sdk-2.2.0/splitit_client/model/card_data.pyi
--rw-r--r--   0        0        0     1571 2023-06-08 11:55:07.614764 splitit_web_python_sdk-2.2.0/splitit_client/model/card_type.py
--rw-r--r--   0        0        0     1251 2023-06-08 11:55:07.615025 splitit_web_python_sdk-2.2.0/splitit_client/model/card_type.pyi
--rw-r--r--   0        0        0     3738 2023-06-08 11:55:07.615263 splitit_web_python_sdk-2.2.0/splitit_client/model/check_installments_eligibility_request.py
--rw-r--r--   0        0        0     3738 2023-06-08 11:55:07.615455 splitit_web_python_sdk-2.2.0/splitit_client/model/check_installments_eligibility_request.pyi
--rw-r--r--   0        0        0     3357 2023-06-08 11:55:07.615654 splitit_web_python_sdk-2.2.0/splitit_client/model/error.py
--rw-r--r--   0        0        0     3357 2023-06-08 11:55:07.615875 splitit_web_python_sdk-2.2.0/splitit_client/model/error.pyi
--rw-r--r--   0        0        0     5464 2023-06-08 11:55:07.616090 splitit_web_python_sdk-2.2.0/splitit_client/model/error_extended.py
--rw-r--r--   0        0        0     5464 2023-06-08 11:55:07.616340 splitit_web_python_sdk-2.2.0/splitit_client/model/error_extended.pyi
--rw-r--r--   0        0        0     2403 2023-06-08 11:55:07.616513 splitit_web_python_sdk-2.2.0/splitit_client/model/events_endpoints_model.py
--rw-r--r--   0        0        0     2403 2023-06-08 11:55:07.616728 splitit_web_python_sdk-2.2.0/splitit_client/model/events_endpoints_model.pyi
--rw-r--r--   0        0        0     2898 2023-06-08 11:55:07.616934 splitit_web_python_sdk-2.2.0/splitit_client/model/failed_response.py
--rw-r--r--   0        0        0     2898 2023-06-08 11:55:07.617117 splitit_web_python_sdk-2.2.0/splitit_client/model/failed_response.pyi
--rw-r--r--   0        0        0     1188 2023-06-08 11:55:07.617353 splitit_web_python_sdk-2.2.0/splitit_client/model/gw_authorization_status.py
--rw-r--r--   0        0        0      991 2023-06-08 11:55:07.617536 splitit_web_python_sdk-2.2.0/splitit_client/model/gw_authorization_status.pyi
--rw-r--r--   0        0        0     4856 2023-06-08 11:55:07.617737 splitit_web_python_sdk-2.2.0/splitit_client/model/identifier_contract.py
--rw-r--r--   0        0        0     4856 2023-06-08 11:55:07.617931 splitit_web_python_sdk-2.2.0/splitit_client/model/identifier_contract.pyi
--rw-r--r--   0        0        0     9111 2023-06-08 11:55:07.618119 splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_plan_response.py
--rw-r--r--   0        0        0     9111 2023-06-08 11:55:07.618407 splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_plan_response.pyi
--rw-r--r--   0        0        0     3361 2023-06-08 11:55:07.618623 splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_redirection_endpoints_model.py
--rw-r--r--   0        0        0     3361 2023-06-08 11:55:07.618837 splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_redirection_endpoints_model.pyi
--rw-r--r--   0        0        0     4303 2023-06-08 11:55:07.619012 splitit_web_python_sdk-2.2.0/splitit_client/model/installment.py
--rw-r--r--   0        0        0     4303 2023-06-08 11:55:07.619174 splitit_web_python_sdk-2.2.0/splitit_client/model/installment.pyi
--rw-r--r--   0        0        0     2499 2023-06-08 11:55:07.619339 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_cancel_response.py
--rw-r--r--   0        0        0     2499 2023-06-08 11:55:07.619519 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_cancel_response.pyi
--rw-r--r--   0        0        0     8108 2023-06-08 11:55:07.619690 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_request.py
--rw-r--r--   0        0        0     8108 2023-06-08 11:55:07.619867 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_request.pyi
--rw-r--r--   0        0        0    13350 2023-06-08 11:55:07.620058 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_response.py
--rw-r--r--   0        0        0    13350 2023-06-08 11:55:07.620321 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_response.pyi
--rw-r--r--   0        0        0    14794 2023-06-08 11:55:07.620550 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_get_response.py
--rw-r--r--   0        0        0    14794 2023-06-08 11:55:07.620813 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_get_response.pyi
--rw-r--r--   0        0        0     7288 2023-06-08 11:55:07.621012 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_initiate_request.py
--rw-r--r--   0        0        0     7288 2023-06-08 11:55:07.621180 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_initiate_request.pyi
--rw-r--r--   0        0        0     3076 2023-06-08 11:55:07.621340 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_request.py
--rw-r--r--   0        0        0     3076 2023-06-08 11:55:07.621495 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_request.pyi
--rw-r--r--   0        0        0     5607 2023-06-08 11:55:07.621648 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_response.py
--rw-r--r--   0        0        0     5607 2023-06-08 11:55:07.621798 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_response.pyi
--rw-r--r--   0        0        0     3421 2023-06-08 11:55:07.621975 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_search_response.py
--rw-r--r--   0        0        0     3421 2023-06-08 11:55:07.622151 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_search_response.pyi
--rw-r--r--   0        0        0     4250 2023-06-08 11:55:07.622311 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request.py
--rw-r--r--   0        0        0     4250 2023-06-08 11:55:07.622459 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request.pyi
--rw-r--r--   0        0        0     4385 2023-06-08 11:55:07.622625 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request_by_identifier.py
--rw-r--r--   0        0        0     4385 2023-06-08 11:55:07.622741 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi
--rw-r--r--   0        0        0     4417 2023-06-08 11:55:07.622851 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_response.py
--rw-r--r--   0        0        0     4417 2023-06-08 11:55:07.623017 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_response.pyi
--rw-r--r--   0        0        0     1082 2023-06-08 11:55:07.623194 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_status.py
--rw-r--r--   0        0        0      911 2023-06-08 11:55:07.623364 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_status.pyi
--rw-r--r--   0        0        0     3487 2023-06-08 11:55:07.623535 splitit_web_python_sdk-2.2.0/splitit_client/model/installments_eligibility_response.py
--rw-r--r--   0        0        0     3487 2023-06-08 11:55:07.623694 splitit_web_python_sdk-2.2.0/splitit_client/model/installments_eligibility_response.pyi
--rw-r--r--   0        0        0     4052 2023-06-08 11:55:07.623836 splitit_web_python_sdk-2.2.0/splitit_client/model/links_data.py
--rw-r--r--   0        0        0     4052 2023-06-08 11:55:07.623973 splitit_web_python_sdk-2.2.0/splitit_client/model/links_data.pyi
--rw-r--r--   0        0        0     3679 2023-06-08 11:55:07.624168 splitit_web_python_sdk-2.2.0/splitit_client/model/links_model.py
--rw-r--r--   0        0        0     3679 2023-06-08 11:55:07.624392 splitit_web_python_sdk-2.2.0/splitit_client/model/links_model.pyi
--rw-r--r--   0        0        0     3476 2023-06-08 11:55:07.624544 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_model.py
--rw-r--r--   0        0        0     3476 2023-06-08 11:55:07.624699 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_model.pyi
--rw-r--r--   0        0        0      962 2023-06-08 11:55:07.624839 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_type.py
--rw-r--r--   0        0        0      826 2023-06-08 11:55:07.624967 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_type.pyi
--rw-r--r--   0        0        0     5439 2023-06-08 11:55:07.625086 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_plan_option_model.py
--rw-r--r--   0        0        0     5439 2023-06-08 11:55:07.625185 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_plan_option_model.pyi
--rw-r--r--   0        0        0    10239 2023-06-08 11:55:07.625299 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data.py
--rw-r--r--   0        0        0    10239 2023-06-08 11:55:07.625458 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data.pyi
--rw-r--r--   0        0        0     8734 2023-06-08 11:55:07.625663 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data_model.py
--rw-r--r--   0        0        0     8734 2023-06-08 11:55:07.625993 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data_model.pyi
--rw-r--r--   0        0        0     4276 2023-06-08 11:55:07.626176 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_error_response.py
--rw-r--r--   0        0        0     4276 2023-06-08 11:55:07.626323 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_error_response.pyi
--rw-r--r--   0        0        0     1345 2023-06-08 11:55:07.626538 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_status.py
--rw-r--r--   0        0        0     1089 2023-06-08 11:55:07.626665 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_status.pyi
--rw-r--r--   0        0        0     1091 2023-06-08 11:55:07.626772 splitit_web_python_sdk-2.2.0/splitit_client/model/purchase_method.py
--rw-r--r--   0        0        0      914 2023-06-08 11:55:07.626932 splitit_web_python_sdk-2.2.0/splitit_client/model/purchase_method.pyi
--rw-r--r--   0        0        0     4123 2023-06-08 11:55:07.627130 splitit_web_python_sdk-2.2.0/splitit_client/model/redirection_endpoints_model.py
--rw-r--r--   0        0        0     4123 2023-06-08 11:55:07.627292 splitit_web_python_sdk-2.2.0/splitit_client/model/redirection_endpoints_model.pyi
--rw-r--r--   0        0        0     5623 2023-06-08 11:55:07.627437 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_model.py
--rw-r--r--   0        0        0     5623 2023-06-08 11:55:07.627588 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_model.pyi
--rw-r--r--   0        0        0     1069 2023-06-08 11:55:07.627728 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_status.py
--rw-r--r--   0        0        0      902 2023-06-08 11:55:07.627871 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_status.pyi
--rw-r--r--   0        0        0     1485 2023-06-08 11:55:07.628015 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_strategy.py
--rw-r--r--   0        0        0     1136 2023-06-08 11:55:07.628156 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_strategy.pyi
--rw-r--r--   0        0        0     4246 2023-06-08 11:55:07.628294 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_summary.py
--rw-r--r--   0        0        0     4246 2023-06-08 11:55:07.628421 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_summary.pyi
--rw-r--r--   0        0        0    14808 2023-06-08 11:55:07.628600 splitit_web_python_sdk-2.2.0/splitit_client/model/search_installment_plan_response_item.py
--rw-r--r--   0        0        0    14808 2023-06-08 11:55:07.628825 splitit_web_python_sdk-2.2.0/splitit_client/model/search_installment_plan_response_item.pyi
--rw-r--r--   0        0        0     1075 2023-06-08 11:55:07.629036 splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status.py
--rw-r--r--   0        0        0      906 2023-06-08 11:55:07.629183 splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status.pyi
--rw-r--r--   0        0        0      958 2023-06-08 11:55:07.629328 splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status2.py
--rw-r--r--   0        0        0      823 2023-06-08 11:55:07.629467 splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status2.pyi
--rw-r--r--   0        0        0     3874 2023-06-08 11:55:07.629607 splitit_web_python_sdk-2.2.0/splitit_client/model/shopper_data.py
--rw-r--r--   0        0        0     3874 2023-06-08 11:55:07.629749 splitit_web_python_sdk-2.2.0/splitit_client/model/shopper_data.pyi
--rw-r--r--   0        0        0     1168 2023-06-08 11:55:07.629883 splitit_web_python_sdk-2.2.0/splitit_client/model/test_modes.py
--rw-r--r--   0        0        0      975 2023-06-08 11:55:07.630028 splitit_web_python_sdk-2.2.0/splitit_client/model/test_modes.pyi
--rw-r--r--   0        0        0     4386 2023-06-08 11:55:07.630166 splitit_web_python_sdk-2.2.0/splitit_client/model/three_ds_redirect_data_v3.py
--rw-r--r--   0        0        0     4386 2023-06-08 11:55:07.630313 splitit_web_python_sdk-2.2.0/splitit_client/model/three_ds_redirect_data_v3.pyi
--rw-r--r--   0        0        0     4223 2023-06-08 11:55:07.630452 splitit_web_python_sdk-2.2.0/splitit_client/model/update_order_request.py
--rw-r--r--   0        0        0     4223 2023-06-08 11:55:07.630611 splitit_web_python_sdk-2.2.0/splitit_client/model/update_order_request.pyi
--rw-r--r--   0        0        0     3409 2023-06-08 11:55:07.630805 splitit_web_python_sdk-2.2.0/splitit_client/model/ux_settings_model.py
--rw-r--r--   0        0        0     3409 2023-06-08 11:55:07.630994 splitit_web_python_sdk-2.2.0/splitit_client/model/ux_settings_model.pyi
--rw-r--r--   0        0        0     3864 2023-06-08 11:55:07.631158 splitit_web_python_sdk-2.2.0/splitit_client/model/verify_authorization_response.py
--rw-r--r--   0        0        0     3864 2023-06-08 11:55:07.631312 splitit_web_python_sdk-2.2.0/splitit_client/model/verify_authorization_response.pyi
--rw-r--r--   0        0        0     4366 2023-06-08 11:55:07.631475 splitit_web_python_sdk-2.2.0/splitit_client/models/__init__.py
--rw-r--r--   0        0        0     1223 2023-06-08 11:55:07.631644 splitit_web_python_sdk-2.2.0/splitit_client/paths/__init__.py
--rw-r--r--   0        0        0      327 2023-06-08 11:55:07.631809 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans/__init__.py
--rw-r--r--   0        0        0    26616 2023-06-08 11:55:07.632095 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans/post.py
--rw-r--r--   0        0        0    26167 2023-06-08 11:55:07.632436 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans/post.pyi
--rw-r--r--   0        0        0      362 2023-06-08 11:55:07.632672 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
--rw-r--r--   0        0        0    20196 2023-06-08 11:55:07.632883 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py
--rw-r--r--   0        0        0    19970 2023-06-08 11:55:07.633184 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi
--rw-r--r--   0        0        0      345 2023-06-08 11:55:07.633396 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_initiate/__init__.py
--rw-r--r--   0        0        0    25887 2023-06-08 11:55:07.633659 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_initiate/post.py
--rw-r--r--   0        0        0    25438 2023-06-08 11:55:07.634029 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_initiate/post.pyi
--rw-r--r--   0        0        0      375 2023-06-08 11:55:07.634244 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/__init__.py
--rw-r--r--   0        0        0    17857 2023-06-08 11:55:07.634480 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py
--rw-r--r--   0        0        0    17631 2023-06-08 11:55:07.634734 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi
--rw-r--r--   0        0        0      389 2023-06-08 11:55:07.634943 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/__init__.py
--rw-r--r--   0        0        0    17934 2023-06-08 11:55:07.635161 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py
--rw-r--r--   0        0        0    17708 2023-06-08 11:55:07.635429 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi
--rw-r--r--   0        0        0      389 2023-06-08 11:55:07.635636 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/__init__.py
--rw-r--r--   0        0        0    21776 2023-06-08 11:55:07.635849 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py
--rw-r--r--   0        0        0    21550 2023-06-08 11:55:07.636089 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi
--rw-r--r--   0        0        0      399 2023-06-08 11:55:07.636318 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/__init__.py
--rw-r--r--   0        0        0    22868 2023-06-08 11:55:07.636562 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py
--rw-r--r--   0        0        0    22642 2023-06-08 11:55:07.636861 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi
--rw-r--r--   0        0        0      415 2023-06-08 11:55:07.637099 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
--rw-r--r--   0        0        0    18102 2023-06-08 11:55:07.637281 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py
--rw-r--r--   0        0        0    17876 2023-06-08 11:55:07.637510 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi
--rw-r--r--   0        0        0      341 2023-06-08 11:55:07.637720 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/__init__.py
--rw-r--r--   0        0        0    21271 2023-06-08 11:55:07.637986 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/get.py
--rw-r--r--   0        0        0    21045 2023-06-08 11:55:07.638236 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/get.pyi
--rw-r--r--   0        0        0      351 2023-06-08 11:55:07.638454 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_updateorder/__init__.py
--rw-r--r--   0        0        0    21319 2023-06-08 11:55:07.638665 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_updateorder/put.py
--rw-r--r--   0        0        0    21093 2023-06-08 11:55:07.638936 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi
--rw-r--r--   0        0        0      639 2023-06-08 11:55:07.639159 splitit_web_python_sdk-2.2.0/splitit_client/request_after_hook.py
--rw-r--r--   0        0        0      640 2023-06-08 11:55:07.639383 splitit_web_python_sdk-2.2.0/splitit_client/request_before_hook.py
--rw-r--r--   0        0        0    10957 2023-06-08 11:55:07.639589 splitit_web_python_sdk-2.2.0/splitit_client/rest.py
--rw-r--r--   0        0        0    95571 2023-06-08 11:55:07.640105 splitit_web_python_sdk-2.2.0/splitit_client/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 11:55:07.640275 splitit_web_python_sdk-2.2.0/splitit_client/type/__init__.py
--rw-r--r--   0        0        0      561 2023-06-08 11:55:07.640426 splitit_web_python_sdk-2.2.0/splitit_client/type/address_data.py
--rw-r--r--   0        0        0      587 2023-06-08 11:55:07.640581 splitit_web_python_sdk-2.2.0/splitit_client/type/address_data_model.py
--rw-r--r--   0        0        0      887 2023-06-08 11:55:07.640741 splitit_web_python_sdk-2.2.0/splitit_client/type/authorization_model.py
--rw-r--r--   0        0        0      398 2023-06-08 11:55:07.640895 splitit_web_python_sdk-2.2.0/splitit_client/type/card_brand.py
--rw-r--r--   0        0        0      705 2023-06-08 11:55:07.641039 splitit_web_python_sdk-2.2.0/splitit_client/type/card_data.py
--rw-r--r--   0        0        0      388 2023-06-08 11:55:07.641189 splitit_web_python_sdk-2.2.0/splitit_client/type/card_type.py
--rw-r--r--   0        0        0      816 2023-06-08 11:55:07.641384 splitit_web_python_sdk-2.2.0/splitit_client/type/check_installments_eligibility_request.py
--rw-r--r--   0        0        0      481 2023-06-08 11:55:07.641566 splitit_web_python_sdk-2.2.0/splitit_client/type/error.py
--rw-r--r--   0        0        0      452 2023-06-08 11:55:07.641720 splitit_web_python_sdk-2.2.0/splitit_client/type/error_extended.py
--rw-r--r--   0        0        0      524 2023-06-08 11:55:07.641893 splitit_web_python_sdk-2.2.0/splitit_client/type/events_endpoints_model.py
--rw-r--r--   0        0        0      573 2023-06-08 11:55:07.642074 splitit_web_python_sdk-2.2.0/splitit_client/type/failed_response.py
--rw-r--r--   0        0        0      359 2023-06-08 11:55:07.642249 splitit_web_python_sdk-2.2.0/splitit_client/type/gw_authorization_status.py
--rw-r--r--   0        0        0      588 2023-06-08 11:55:07.642422 splitit_web_python_sdk-2.2.0/splitit_client/type/identifier_contract.py
--rw-r--r--   0        0        0     1018 2023-06-08 11:55:07.642680 splitit_web_python_sdk-2.2.0/splitit_client/type/initiate_plan_response.py
--rw-r--r--   0        0        0      617 2023-06-08 11:55:07.642907 splitit_web_python_sdk-2.2.0/splitit_client/type/initiate_redirection_endpoints_model.py
--rw-r--r--   0        0        0      640 2023-06-08 11:55:07.643135 splitit_web_python_sdk-2.2.0/splitit_client/type/installment.py
--rw-r--r--   0        0        0      575 2023-06-08 11:55:07.643349 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_cancel_response.py
--rw-r--r--   0        0        0     1257 2023-06-08 11:55:07.643532 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_create_request.py
--rw-r--r--   0        0        0     1510 2023-06-08 11:55:07.643757 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_create_response.py
--rw-r--r--   0        0        0     1591 2023-06-08 11:55:07.643992 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_get_response.py
--rw-r--r--   0        0        0     1242 2023-06-08 11:55:07.644256 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_initiate_request.py
--rw-r--r--   0        0        0      665 2023-06-08 11:55:07.644461 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_refund_request.py
--rw-r--r--   0        0        0      805 2023-06-08 11:55:07.644662 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_refund_response.py
--rw-r--r--   0        0        0      709 2023-06-08 11:55:07.644855 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_search_response.py
--rw-r--r--   0        0        0      709 2023-06-08 11:55:07.645105 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_request.py
--rw-r--r--   0        0        0      622 2023-06-08 11:55:07.645504 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_request_by_identifier.py
--rw-r--r--   0        0        0      768 2023-06-08 11:55:07.645696 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_response.py
--rw-r--r--   0        0        0      348 2023-06-08 11:55:07.645868 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_status.py
--rw-r--r--   0        0        0      695 2023-06-08 11:55:07.646045 splitit_web_python_sdk-2.2.0/splitit_client/type/installments_eligibility_response.py
--rw-r--r--   0        0        0      532 2023-06-08 11:55:07.646232 splitit_web_python_sdk-2.2.0/splitit_client/type/links_data.py
--rw-r--r--   0        0        0      530 2023-06-08 11:55:07.646385 splitit_web_python_sdk-2.2.0/splitit_client/type/links_model.py
--rw-r--r--   0        0        0      664 2023-06-08 11:55:07.646508 splitit_web_python_sdk-2.2.0/splitit_client/type/payment_method_model.py
--rw-r--r--   0        0        0      336 2023-06-08 11:55:07.646617 splitit_web_python_sdk-2.2.0/splitit_client/type/payment_method_type.py
--rw-r--r--   0        0        0      763 2023-06-08 11:55:07.646794 splitit_web_python_sdk-2.2.0/splitit_client/type/payment_plan_option_model.py
--rw-r--r--   0        0        0      838 2023-06-08 11:55:07.646933 splitit_web_python_sdk-2.2.0/splitit_client/type/plan_data.py
--rw-r--r--   0        0        0      824 2023-06-08 11:55:07.647027 splitit_web_python_sdk-2.2.0/splitit_client/type/plan_data_model.py
--rw-r--r--   0        0        0      484 2023-06-08 11:55:07.647119 splitit_web_python_sdk-2.2.0/splitit_client/type/plan_error_response.py
--rw-r--r--   0        0        0      371 2023-06-08 11:55:07.647218 splitit_web_python_sdk-2.2.0/splitit_client/type/plan_status.py
--rw-r--r--   0        0        0      347 2023-06-08 11:55:07.647297 splitit_web_python_sdk-2.2.0/splitit_client/type/purchase_method.py
--rw-r--r--   0        0        0      615 2023-06-08 11:55:07.647378 splitit_web_python_sdk-2.2.0/splitit_client/type/redirection_endpoints_model.py
--rw-r--r--   0        0        0      719 2023-06-08 11:55:07.647461 splitit_web_python_sdk-2.2.0/splitit_client/type/refund_model.py
--rw-r--r--   0        0        0      341 2023-06-08 11:55:07.647548 splitit_web_python_sdk-2.2.0/splitit_client/type/refund_status.py
--rw-r--r--   0        0        0      423 2023-06-08 11:55:07.647634 splitit_web_python_sdk-2.2.0/splitit_client/type/refund_strategy.py
--rw-r--r--   0        0        0      642 2023-06-08 11:55:07.647718 splitit_web_python_sdk-2.2.0/splitit_client/type/refund_summary.py
--rw-r--r--   0        0        0     1626 2023-06-08 11:55:07.647802 splitit_web_python_sdk-2.2.0/splitit_client/type/search_installment_plan_response_item.py
--rw-r--r--   0        0        0      344 2023-06-08 11:55:07.647884 splitit_web_python_sdk-2.2.0/splitit_client/type/shipping_status.py
--rw-r--r--   0        0        0      334 2023-06-08 11:55:07.647983 splitit_web_python_sdk-2.2.0/splitit_client/type/shipping_status2.py
--rw-r--r--   0        0        0      528 2023-06-08 11:55:07.648069 splitit_web_python_sdk-2.2.0/splitit_client/type/shopper_data.py
--rw-r--r--   0        0        0      345 2023-06-08 11:55:07.648154 splitit_web_python_sdk-2.2.0/splitit_client/type/test_modes.py
--rw-r--r--   0        0        0      567 2023-06-08 11:55:07.648240 splitit_web_python_sdk-2.2.0/splitit_client/type/three_ds_redirect_data_v3.py
--rw-r--r--   0        0        0      656 2023-06-08 11:55:07.648338 splitit_web_python_sdk-2.2.0/splitit_client/type/update_order_request.py
--rw-r--r--   0        0        0      524 2023-06-08 11:55:07.648430 splitit_web_python_sdk-2.2.0/splitit_client/type/ux_settings_model.py
--rw-r--r--   0        0        0      708 2023-06-08 11:55:07.648516 splitit_web_python_sdk-2.2.0/splitit_client/type/verify_authorization_response.py
--rw-r--r--   0        0        0      491 2023-06-08 11:55:07.648605 splitit_web_python_sdk-2.2.0/splitit_client/type_util.py
--rw-r--r--   0        0        0     3170 2023-06-08 11:55:07.648691 splitit_web_python_sdk-2.2.0/splitit_client/validation_metadata.py
--rw-r--r--   0        0        0     9244 1970-01-01 00:00:00.000000 splitit_web_python_sdk-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-12 15:48:13.543645 splitit_web_python_sdk-2.3.0/LICENSE
+-rw-r--r--   0        0        0     8335 2023-06-12 15:48:37.968114 splitit_web_python_sdk-2.3.0/README.md
+-rw-r--r--   0        0        0      737 2023-06-12 15:48:37.969471 splitit_web_python_sdk-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      725 2023-06-12 15:48:37.969984 splitit_web_python_sdk-2.3.0/splitit_client/__init__.py
+-rw-r--r--   0        0        0    73578 2023-06-12 15:48:37.970475 splitit_web_python_sdk-2.3.0/splitit_client/api_client.py
+-rw-r--r--   0        0        0      663 2023-06-12 15:48:13.491627 splitit_web_python_sdk-2.3.0/splitit_client/api_response.py
+-rw-r--r--   0        0        0      214 2023-06-12 15:48:13.491748 splitit_web_python_sdk-2.3.0/splitit_client/apis/__init__.py
+-rw-r--r--   0        0        0     3411 2023-06-12 15:48:13.491863 splitit_web_python_sdk-2.3.0/splitit_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      241 2023-06-12 15:48:13.492003 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      127 2023-06-12 15:48:13.492108 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans.py
+-rw-r--r--   0        0        0      161 2023-06-12 15:48:13.492205 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_check_eligibility.py
+-rw-r--r--   0        0        0      144 2023-06-12 15:48:13.492325 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_initiate.py
+-rw-r--r--   0        0        0      169 2023-06-12 15:48:13.492448 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number.py
+-rw-r--r--   0        0        0      185 2023-06-12 15:48:13.492556 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_cancel.py
+-rw-r--r--   0        0        0      185 2023-06-12 15:48:13.492663 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_refund.py
+-rw-r--r--   0        0        0      192 2023-06-12 15:48:13.492793 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_updateorder.py
+-rw-r--r--   0        0        0      208 2023-06-12 15:48:13.492906 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_verifyauthorization.py
+-rw-r--r--   0        0        0      137 2023-06-12 15:48:13.493033 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_search.py
+-rw-r--r--   0        0        0      147 2023-06-12 15:48:13.493143 splitit_web_python_sdk-2.3.0/splitit_client/apis/paths/api_installmentplans_updateorder.py
+-rw-r--r--   0        0        0      371 2023-06-12 15:48:13.493251 splitit_web_python_sdk-2.3.0/splitit_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      328 2023-06-12 15:48:13.493366 splitit_web_python_sdk-2.3.0/splitit_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1333 2023-06-12 15:48:13.493493 splitit_web_python_sdk-2.3.0/splitit_client/apis/tags/installment_plan_api.py
+-rw-r--r--   0        0        0      989 2023-06-12 15:48:13.493602 splitit_web_python_sdk-2.3.0/splitit_client/client.py
+-rw-r--r--   0        0        0      989 2023-06-12 15:48:13.493720 splitit_web_python_sdk-2.3.0/splitit_client/client.pyi
+-rw-r--r--   0        0        0      669 2023-06-12 15:48:13.493843 splitit_web_python_sdk-2.3.0/splitit_client/client_custom.py
+-rw-r--r--   0        0        0    18575 2023-06-12 15:48:37.971007 splitit_web_python_sdk-2.3.0/splitit_client/configuration.py
+-rw-r--r--   0        0        0     7615 2023-06-12 15:48:37.971340 splitit_web_python_sdk-2.3.0/splitit_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-06-12 15:48:13.494429 splitit_web_python_sdk-2.3.0/splitit_client/exceptions_base.py
+-rw-r--r--   0        0        0      348 2023-06-12 15:48:13.494614 splitit_web_python_sdk-2.3.0/splitit_client/model/__init__.py
+-rw-r--r--   0        0        0     4871 2023-06-12 15:48:13.494721 splitit_web_python_sdk-2.3.0/splitit_client/model/address_data.py
+-rw-r--r--   0        0        0     4871 2023-06-12 15:48:13.494909 splitit_web_python_sdk-2.3.0/splitit_client/model/address_data.pyi
+-rw-r--r--   0        0        0     4894 2023-06-12 15:48:13.495043 splitit_web_python_sdk-2.3.0/splitit_client/model/address_data_model.py
+-rw-r--r--   0        0        0     4894 2023-06-12 15:48:13.495178 splitit_web_python_sdk-2.3.0/splitit_client/model/address_data_model.pyi
+-rw-r--r--   0        0        0     7418 2023-06-12 15:48:13.495302 splitit_web_python_sdk-2.3.0/splitit_client/model/authorization_model.py
+-rw-r--r--   0        0        0     7418 2023-06-12 15:48:13.495441 splitit_web_python_sdk-2.3.0/splitit_client/model/authorization_model.pyi
+-rw-r--r--   0        0        0     1752 2023-06-12 15:48:13.495589 splitit_web_python_sdk-2.3.0/splitit_client/model/card_brand.py
+-rw-r--r--   0        0        0     1392 2023-06-12 15:48:13.495738 splitit_web_python_sdk-2.3.0/splitit_client/model/card_brand.pyi
+-rw-r--r--   0        0        0     5874 2023-06-12 15:48:13.495874 splitit_web_python_sdk-2.3.0/splitit_client/model/card_data.py
+-rw-r--r--   0        0        0     5874 2023-06-12 15:48:13.495992 splitit_web_python_sdk-2.3.0/splitit_client/model/card_data.pyi
+-rw-r--r--   0        0        0     1571 2023-06-12 15:48:13.496111 splitit_web_python_sdk-2.3.0/splitit_client/model/card_type.py
+-rw-r--r--   0        0        0     1251 2023-06-12 15:48:13.496263 splitit_web_python_sdk-2.3.0/splitit_client/model/card_type.pyi
+-rw-r--r--   0        0        0     3738 2023-06-12 15:48:13.496415 splitit_web_python_sdk-2.3.0/splitit_client/model/check_installments_eligibility_request.py
+-rw-r--r--   0        0        0     3738 2023-06-12 15:48:13.496542 splitit_web_python_sdk-2.3.0/splitit_client/model/check_installments_eligibility_request.pyi
+-rw-r--r--   0        0        0     3357 2023-06-12 15:48:13.496664 splitit_web_python_sdk-2.3.0/splitit_client/model/error.py
+-rw-r--r--   0        0        0     3357 2023-06-12 15:48:13.496781 splitit_web_python_sdk-2.3.0/splitit_client/model/error.pyi
+-rw-r--r--   0        0        0     5464 2023-06-12 15:48:13.496892 splitit_web_python_sdk-2.3.0/splitit_client/model/error_extended.py
+-rw-r--r--   0        0        0     5464 2023-06-12 15:48:13.497003 splitit_web_python_sdk-2.3.0/splitit_client/model/error_extended.pyi
+-rw-r--r--   0        0        0     2403 2023-06-12 15:48:13.497089 splitit_web_python_sdk-2.3.0/splitit_client/model/events_endpoints_model.py
+-rw-r--r--   0        0        0     2403 2023-06-12 15:48:13.497173 splitit_web_python_sdk-2.3.0/splitit_client/model/events_endpoints_model.pyi
+-rw-r--r--   0        0        0     2898 2023-06-12 15:48:13.497317 splitit_web_python_sdk-2.3.0/splitit_client/model/failed_response.py
+-rw-r--r--   0        0        0     2898 2023-06-12 15:48:13.497446 splitit_web_python_sdk-2.3.0/splitit_client/model/failed_response.pyi
+-rw-r--r--   0        0        0     1188 2023-06-12 15:48:13.497561 splitit_web_python_sdk-2.3.0/splitit_client/model/gw_authorization_status.py
+-rw-r--r--   0        0        0      991 2023-06-12 15:48:13.497655 splitit_web_python_sdk-2.3.0/splitit_client/model/gw_authorization_status.pyi
+-rw-r--r--   0        0        0     4856 2023-06-12 15:48:13.497756 splitit_web_python_sdk-2.3.0/splitit_client/model/identifier_contract.py
+-rw-r--r--   0        0        0     4856 2023-06-12 15:48:13.497853 splitit_web_python_sdk-2.3.0/splitit_client/model/identifier_contract.pyi
+-rw-r--r--   0        0        0     9111 2023-06-12 15:48:13.497957 splitit_web_python_sdk-2.3.0/splitit_client/model/initiate_plan_response.py
+-rw-r--r--   0        0        0     9111 2023-06-12 15:48:13.498073 splitit_web_python_sdk-2.3.0/splitit_client/model/initiate_plan_response.pyi
+-rw-r--r--   0        0        0     3361 2023-06-12 15:48:13.498179 splitit_web_python_sdk-2.3.0/splitit_client/model/initiate_redirection_endpoints_model.py
+-rw-r--r--   0        0        0     3361 2023-06-12 15:48:13.498276 splitit_web_python_sdk-2.3.0/splitit_client/model/initiate_redirection_endpoints_model.pyi
+-rw-r--r--   0        0        0     4303 2023-06-12 15:48:13.498375 splitit_web_python_sdk-2.3.0/splitit_client/model/installment.py
+-rw-r--r--   0        0        0     4303 2023-06-12 15:48:13.498471 splitit_web_python_sdk-2.3.0/splitit_client/model/installment.pyi
+-rw-r--r--   0        0        0     2499 2023-06-12 15:48:13.498578 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_cancel_response.py
+-rw-r--r--   0        0        0     2499 2023-06-12 15:48:13.498684 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_cancel_response.pyi
+-rw-r--r--   0        0        0     8108 2023-06-12 15:48:13.498782 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_create_request.py
+-rw-r--r--   0        0        0     8108 2023-06-12 15:48:13.498885 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_create_request.pyi
+-rw-r--r--   0        0        0    13350 2023-06-12 15:48:13.498993 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_create_response.py
+-rw-r--r--   0        0        0    13350 2023-06-12 15:48:13.499116 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_create_response.pyi
+-rw-r--r--   0        0        0    14794 2023-06-12 15:48:13.499230 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_get_response.py
+-rw-r--r--   0        0        0    14794 2023-06-12 15:48:13.499428 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_get_response.pyi
+-rw-r--r--   0        0        0     7288 2023-06-12 15:48:13.499586 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_initiate_request.py
+-rw-r--r--   0        0        0     7288 2023-06-12 15:48:13.499728 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_initiate_request.pyi
+-rw-r--r--   0        0        0     3076 2023-06-12 15:48:13.499868 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_refund_request.py
+-rw-r--r--   0        0        0     3076 2023-06-12 15:48:13.500004 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_refund_request.pyi
+-rw-r--r--   0        0        0     5607 2023-06-12 15:48:13.500132 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_refund_response.py
+-rw-r--r--   0        0        0     5607 2023-06-12 15:48:13.500272 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_refund_response.pyi
+-rw-r--r--   0        0        0     3421 2023-06-12 15:48:13.500525 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_search_response.py
+-rw-r--r--   0        0        0     3421 2023-06-12 15:48:13.500820 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_search_response.pyi
+-rw-r--r--   0        0        0     4250 2023-06-12 15:48:13.501117 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_request.py
+-rw-r--r--   0        0        0     4250 2023-06-12 15:48:13.501348 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_request.pyi
+-rw-r--r--   0        0        0     4385 2023-06-12 15:48:13.501571 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_request_by_identifier.py
+-rw-r--r--   0        0        0     4385 2023-06-12 15:48:13.501744 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi
+-rw-r--r--   0        0        0     4417 2023-06-12 15:48:13.501985 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_response.py
+-rw-r--r--   0        0        0     4417 2023-06-12 15:48:13.502191 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_response.pyi
+-rw-r--r--   0        0        0     1082 2023-06-12 15:48:13.502381 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_status.py
+-rw-r--r--   0        0        0      911 2023-06-12 15:48:13.502553 splitit_web_python_sdk-2.3.0/splitit_client/model/installment_status.pyi
+-rw-r--r--   0        0        0     4161 2023-06-12 15:48:37.971604 splitit_web_python_sdk-2.3.0/splitit_client/model/installments_eligibility_response.py
+-rw-r--r--   0        0        0     4161 2023-06-12 15:48:37.971800 splitit_web_python_sdk-2.3.0/splitit_client/model/installments_eligibility_response.pyi
+-rw-r--r--   0        0        0     4052 2023-06-12 15:48:13.503075 splitit_web_python_sdk-2.3.0/splitit_client/model/links_data.py
+-rw-r--r--   0        0        0     4052 2023-06-12 15:48:13.503217 splitit_web_python_sdk-2.3.0/splitit_client/model/links_data.pyi
+-rw-r--r--   0        0        0     3679 2023-06-12 15:48:13.503377 splitit_web_python_sdk-2.3.0/splitit_client/model/links_model.py
+-rw-r--r--   0        0        0     3679 2023-06-12 15:48:13.503536 splitit_web_python_sdk-2.3.0/splitit_client/model/links_model.pyi
+-rw-r--r--   0        0        0     3476 2023-06-12 15:48:13.503725 splitit_web_python_sdk-2.3.0/splitit_client/model/payment_method_model.py
+-rw-r--r--   0        0        0     3476 2023-06-12 15:48:13.503931 splitit_web_python_sdk-2.3.0/splitit_client/model/payment_method_model.pyi
+-rw-r--r--   0        0        0      962 2023-06-12 15:48:13.504094 splitit_web_python_sdk-2.3.0/splitit_client/model/payment_method_type.py
+-rw-r--r--   0        0        0      826 2023-06-12 15:48:13.504217 splitit_web_python_sdk-2.3.0/splitit_client/model/payment_method_type.pyi
+-rw-r--r--   0        0        0     6852 2023-06-12 15:48:37.972014 splitit_web_python_sdk-2.3.0/splitit_client/model/payment_plan_option_model.py
+-rw-r--r--   0        0        0     6852 2023-06-12 15:48:37.972211 splitit_web_python_sdk-2.3.0/splitit_client/model/payment_plan_option_model.pyi
+-rw-r--r--   0        0        0    10239 2023-06-12 15:48:13.504715 splitit_web_python_sdk-2.3.0/splitit_client/model/plan_data.py
+-rw-r--r--   0        0        0    10239 2023-06-12 15:48:13.504898 splitit_web_python_sdk-2.3.0/splitit_client/model/plan_data.pyi
+-rw-r--r--   0        0        0     8734 2023-06-12 15:48:13.505099 splitit_web_python_sdk-2.3.0/splitit_client/model/plan_data_model.py
+-rw-r--r--   0        0        0     8734 2023-06-12 15:48:13.505304 splitit_web_python_sdk-2.3.0/splitit_client/model/plan_data_model.pyi
+-rw-r--r--   0        0        0     4276 2023-06-12 15:48:13.505444 splitit_web_python_sdk-2.3.0/splitit_client/model/plan_error_response.py
+-rw-r--r--   0        0        0     4276 2023-06-12 15:48:13.505550 splitit_web_python_sdk-2.3.0/splitit_client/model/plan_error_response.pyi
+-rw-r--r--   0        0        0     1345 2023-06-12 15:48:13.505695 splitit_web_python_sdk-2.3.0/splitit_client/model/plan_status.py
+-rw-r--r--   0        0        0     1089 2023-06-12 15:48:13.505797 splitit_web_python_sdk-2.3.0/splitit_client/model/plan_status.pyi
+-rw-r--r--   0        0        0     1091 2023-06-12 15:48:13.505877 splitit_web_python_sdk-2.3.0/splitit_client/model/purchase_method.py
+-rw-r--r--   0        0        0      914 2023-06-12 15:48:13.505962 splitit_web_python_sdk-2.3.0/splitit_client/model/purchase_method.pyi
+-rw-r--r--   0        0        0     4123 2023-06-12 15:48:13.506086 splitit_web_python_sdk-2.3.0/splitit_client/model/redirection_endpoints_model.py
+-rw-r--r--   0        0        0     4123 2023-06-12 15:48:13.506224 splitit_web_python_sdk-2.3.0/splitit_client/model/redirection_endpoints_model.pyi
+-rw-r--r--   0        0        0     5623 2023-06-12 15:48:13.506354 splitit_web_python_sdk-2.3.0/splitit_client/model/refund_model.py
+-rw-r--r--   0        0        0     5623 2023-06-12 15:48:13.506496 splitit_web_python_sdk-2.3.0/splitit_client/model/refund_model.pyi
+-rw-r--r--   0        0        0     1069 2023-06-12 15:48:13.506633 splitit_web_python_sdk-2.3.0/splitit_client/model/refund_status.py
+-rw-r--r--   0        0        0      902 2023-06-12 15:48:13.506782 splitit_web_python_sdk-2.3.0/splitit_client/model/refund_status.pyi
+-rw-r--r--   0        0        0     1485 2023-06-12 15:48:13.506959 splitit_web_python_sdk-2.3.0/splitit_client/model/refund_strategy.py
+-rw-r--r--   0        0        0     1136 2023-06-12 15:48:13.507113 splitit_web_python_sdk-2.3.0/splitit_client/model/refund_strategy.pyi
+-rw-r--r--   0        0        0     4246 2023-06-12 15:48:13.507300 splitit_web_python_sdk-2.3.0/splitit_client/model/refund_summary.py
+-rw-r--r--   0        0        0     4246 2023-06-12 15:48:13.507496 splitit_web_python_sdk-2.3.0/splitit_client/model/refund_summary.pyi
+-rw-r--r--   0        0        0    14808 2023-06-12 15:48:13.507692 splitit_web_python_sdk-2.3.0/splitit_client/model/search_installment_plan_response_item.py
+-rw-r--r--   0        0        0    14808 2023-06-12 15:48:13.507928 splitit_web_python_sdk-2.3.0/splitit_client/model/search_installment_plan_response_item.pyi
+-rw-r--r--   0        0        0     1075 2023-06-12 15:48:13.508123 splitit_web_python_sdk-2.3.0/splitit_client/model/shipping_status.py
+-rw-r--r--   0        0        0      906 2023-06-12 15:48:13.508270 splitit_web_python_sdk-2.3.0/splitit_client/model/shipping_status.pyi
+-rw-r--r--   0        0        0      958 2023-06-12 15:48:13.508444 splitit_web_python_sdk-2.3.0/splitit_client/model/shipping_status2.py
+-rw-r--r--   0        0        0      823 2023-06-12 15:48:13.508653 splitit_web_python_sdk-2.3.0/splitit_client/model/shipping_status2.pyi
+-rw-r--r--   0        0        0     3874 2023-06-12 15:48:13.508873 splitit_web_python_sdk-2.3.0/splitit_client/model/shopper_data.py
+-rw-r--r--   0        0        0     3874 2023-06-12 15:48:13.509029 splitit_web_python_sdk-2.3.0/splitit_client/model/shopper_data.pyi
+-rw-r--r--   0        0        0     1168 2023-06-12 15:48:13.509179 splitit_web_python_sdk-2.3.0/splitit_client/model/test_modes.py
+-rw-r--r--   0        0        0      975 2023-06-12 15:48:13.509385 splitit_web_python_sdk-2.3.0/splitit_client/model/test_modes.pyi
+-rw-r--r--   0        0        0     4386 2023-06-12 15:48:13.509582 splitit_web_python_sdk-2.3.0/splitit_client/model/three_ds_redirect_data_v3.py
+-rw-r--r--   0        0        0     4386 2023-06-12 15:48:13.509769 splitit_web_python_sdk-2.3.0/splitit_client/model/three_ds_redirect_data_v3.pyi
+-rw-r--r--   0        0        0     4223 2023-06-12 15:48:13.509928 splitit_web_python_sdk-2.3.0/splitit_client/model/update_order_request.py
+-rw-r--r--   0        0        0     4223 2023-06-12 15:48:13.510109 splitit_web_python_sdk-2.3.0/splitit_client/model/update_order_request.pyi
+-rw-r--r--   0        0        0     3409 2023-06-12 15:48:13.510276 splitit_web_python_sdk-2.3.0/splitit_client/model/ux_settings_model.py
+-rw-r--r--   0        0        0     3409 2023-06-12 15:48:13.510427 splitit_web_python_sdk-2.3.0/splitit_client/model/ux_settings_model.pyi
+-rw-r--r--   0        0        0     3864 2023-06-12 15:48:13.510596 splitit_web_python_sdk-2.3.0/splitit_client/model/verify_authorization_response.py
+-rw-r--r--   0        0        0     3864 2023-06-12 15:48:13.510761 splitit_web_python_sdk-2.3.0/splitit_client/model/verify_authorization_response.pyi
+-rw-r--r--   0        0        0     4366 2023-06-12 15:48:13.510935 splitit_web_python_sdk-2.3.0/splitit_client/models/__init__.py
+-rw-r--r--   0        0        0     1223 2023-06-12 15:48:13.511111 splitit_web_python_sdk-2.3.0/splitit_client/paths/__init__.py
+-rw-r--r--   0        0        0      327 2023-06-12 15:48:13.511286 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans/__init__.py
+-rw-r--r--   0        0        0    26820 2023-06-12 15:48:37.972500 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans/post.py
+-rw-r--r--   0        0        0    26371 2023-06-12 15:48:37.972801 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans/post.pyi
+-rw-r--r--   0        0        0      362 2023-06-12 15:48:13.512042 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
+-rw-r--r--   0        0        0    20400 2023-06-12 15:48:37.973118 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py
+-rw-r--r--   0        0        0    20174 2023-06-12 15:48:37.973427 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi
+-rw-r--r--   0        0        0      345 2023-06-12 15:48:13.512653 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_initiate/__init__.py
+-rw-r--r--   0        0        0    26091 2023-06-12 15:48:37.974030 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_initiate/post.py
+-rw-r--r--   0        0        0    25642 2023-06-12 15:48:37.974408 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_initiate/post.pyi
+-rw-r--r--   0        0        0      375 2023-06-12 15:48:13.513309 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number/__init__.py
+-rw-r--r--   0        0        0    18061 2023-06-12 15:48:37.974738 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py
+-rw-r--r--   0        0        0    17835 2023-06-12 15:48:37.975065 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi
+-rw-r--r--   0        0        0      389 2023-06-12 15:48:13.513892 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/__init__.py
+-rw-r--r--   0        0        0    18138 2023-06-12 15:48:37.975436 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py
+-rw-r--r--   0        0        0    17912 2023-06-12 15:48:37.975800 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi
+-rw-r--r--   0        0        0      389 2023-06-12 15:48:13.514381 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/__init__.py
+-rw-r--r--   0        0        0    21980 2023-06-12 15:48:37.976205 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py
+-rw-r--r--   0        0        0    21754 2023-06-12 15:48:37.976537 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi
+-rw-r--r--   0        0        0      399 2023-06-12 15:48:13.514898 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/__init__.py
+-rw-r--r--   0        0        0    23072 2023-06-12 15:48:37.976812 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py
+-rw-r--r--   0        0        0    22846 2023-06-12 15:48:37.977075 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi
+-rw-r--r--   0        0        0      415 2023-06-12 15:48:13.515492 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
+-rw-r--r--   0        0        0    18306 2023-06-12 15:48:37.977342 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py
+-rw-r--r--   0        0        0    18080 2023-06-12 15:48:37.977605 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi
+-rw-r--r--   0        0        0      341 2023-06-12 15:48:13.516057 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_search/__init__.py
+-rw-r--r--   0        0        0    21475 2023-06-12 15:48:37.977877 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_search/get.py
+-rw-r--r--   0        0        0    21249 2023-06-12 15:48:37.978367 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_search/get.pyi
+-rw-r--r--   0        0        0      351 2023-06-12 15:48:13.516682 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_updateorder/__init__.py
+-rw-r--r--   0        0        0    21523 2023-06-12 15:48:37.978723 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_updateorder/put.py
+-rw-r--r--   0        0        0    21297 2023-06-12 15:48:37.979047 splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi
+-rw-r--r--   0        0        0      639 2023-06-12 15:48:13.517351 splitit_web_python_sdk-2.3.0/splitit_client/request_after_hook.py
+-rw-r--r--   0        0        0      640 2023-06-12 15:48:13.517576 splitit_web_python_sdk-2.3.0/splitit_client/request_before_hook.py
+-rw-r--r--   0        0        0    10957 2023-06-12 15:48:13.517755 splitit_web_python_sdk-2.3.0/splitit_client/rest.py
+-rw-r--r--   0        0        0    95571 2023-06-12 15:48:13.518183 splitit_web_python_sdk-2.3.0/splitit_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-12 15:48:13.518346 splitit_web_python_sdk-2.3.0/splitit_client/type/__init__.py
+-rw-r--r--   0        0        0      561 2023-06-12 15:48:13.518433 splitit_web_python_sdk-2.3.0/splitit_client/type/address_data.py
+-rw-r--r--   0        0        0      587 2023-06-12 15:48:13.518532 splitit_web_python_sdk-2.3.0/splitit_client/type/address_data_model.py
+-rw-r--r--   0        0        0      887 2023-06-12 15:48:13.518670 splitit_web_python_sdk-2.3.0/splitit_client/type/authorization_model.py
+-rw-r--r--   0        0        0      398 2023-06-12 15:48:13.518801 splitit_web_python_sdk-2.3.0/splitit_client/type/card_brand.py
+-rw-r--r--   0        0        0      705 2023-06-12 15:48:13.518947 splitit_web_python_sdk-2.3.0/splitit_client/type/card_data.py
+-rw-r--r--   0        0        0      388 2023-06-12 15:48:13.519865 splitit_web_python_sdk-2.3.0/splitit_client/type/card_type.py
+-rw-r--r--   0        0        0      816 2023-06-12 15:48:13.520026 splitit_web_python_sdk-2.3.0/splitit_client/type/check_installments_eligibility_request.py
+-rw-r--r--   0        0        0      481 2023-06-12 15:48:13.520170 splitit_web_python_sdk-2.3.0/splitit_client/type/error.py
+-rw-r--r--   0        0        0      452 2023-06-12 15:48:13.520285 splitit_web_python_sdk-2.3.0/splitit_client/type/error_extended.py
+-rw-r--r--   0        0        0      524 2023-06-12 15:48:13.520384 splitit_web_python_sdk-2.3.0/splitit_client/type/events_endpoints_model.py
+-rw-r--r--   0        0        0      573 2023-06-12 15:48:13.520478 splitit_web_python_sdk-2.3.0/splitit_client/type/failed_response.py
+-rw-r--r--   0        0        0      359 2023-06-12 15:48:13.521176 splitit_web_python_sdk-2.3.0/splitit_client/type/gw_authorization_status.py
+-rw-r--r--   0        0        0      588 2023-06-12 15:48:13.521325 splitit_web_python_sdk-2.3.0/splitit_client/type/identifier_contract.py
+-rw-r--r--   0        0        0     1018 2023-06-12 15:48:13.521476 splitit_web_python_sdk-2.3.0/splitit_client/type/initiate_plan_response.py
+-rw-r--r--   0        0        0      617 2023-06-12 15:48:13.521631 splitit_web_python_sdk-2.3.0/splitit_client/type/initiate_redirection_endpoints_model.py
+-rw-r--r--   0        0        0      640 2023-06-12 15:48:13.522576 splitit_web_python_sdk-2.3.0/splitit_client/type/installment.py
+-rw-r--r--   0        0        0      575 2023-06-12 15:48:13.523340 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_cancel_response.py
+-rw-r--r--   0        0        0     1257 2023-06-12 15:48:13.523487 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_create_request.py
+-rw-r--r--   0        0        0     1510 2023-06-12 15:48:13.523625 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_create_response.py
+-rw-r--r--   0        0        0     1591 2023-06-12 15:48:13.523763 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_get_response.py
+-rw-r--r--   0        0        0     1242 2023-06-12 15:48:13.523915 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_initiate_request.py
+-rw-r--r--   0        0        0      665 2023-06-12 15:48:13.524059 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_refund_request.py
+-rw-r--r--   0        0        0      805 2023-06-12 15:48:13.524198 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_refund_response.py
+-rw-r--r--   0        0        0      709 2023-06-12 15:48:13.524339 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_search_response.py
+-rw-r--r--   0        0        0      709 2023-06-12 15:48:13.524484 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_update_request.py
+-rw-r--r--   0        0        0      622 2023-06-12 15:48:13.524626 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_update_request_by_identifier.py
+-rw-r--r--   0        0        0      768 2023-06-12 15:48:13.524773 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_update_response.py
+-rw-r--r--   0        0        0      348 2023-06-12 15:48:13.524908 splitit_web_python_sdk-2.3.0/splitit_client/type/installment_status.py
+-rw-r--r--   0        0        0      725 2023-06-12 15:48:37.979307 splitit_web_python_sdk-2.3.0/splitit_client/type/installments_eligibility_response.py
+-rw-r--r--   0        0        0      532 2023-06-12 15:48:13.525165 splitit_web_python_sdk-2.3.0/splitit_client/type/links_data.py
+-rw-r--r--   0        0        0      530 2023-06-12 15:48:13.525299 splitit_web_python_sdk-2.3.0/splitit_client/type/links_model.py
+-rw-r--r--   0        0        0      664 2023-06-12 15:48:13.525435 splitit_web_python_sdk-2.3.0/splitit_client/type/payment_method_model.py
+-rw-r--r--   0        0        0      336 2023-06-12 15:48:13.525544 splitit_web_python_sdk-2.3.0/splitit_client/type/payment_method_type.py
+-rw-r--r--   0        0        0      828 2023-06-12 15:48:37.979608 splitit_web_python_sdk-2.3.0/splitit_client/type/payment_plan_option_model.py
+-rw-r--r--   0        0        0      838 2023-06-12 15:48:13.525927 splitit_web_python_sdk-2.3.0/splitit_client/type/plan_data.py
+-rw-r--r--   0        0        0      824 2023-06-12 15:48:13.526081 splitit_web_python_sdk-2.3.0/splitit_client/type/plan_data_model.py
+-rw-r--r--   0        0        0      484 2023-06-12 15:48:13.526227 splitit_web_python_sdk-2.3.0/splitit_client/type/plan_error_response.py
+-rw-r--r--   0        0        0      371 2023-06-12 15:48:13.526402 splitit_web_python_sdk-2.3.0/splitit_client/type/plan_status.py
+-rw-r--r--   0        0        0      347 2023-06-12 15:48:13.526575 splitit_web_python_sdk-2.3.0/splitit_client/type/purchase_method.py
+-rw-r--r--   0        0        0      615 2023-06-12 15:48:13.526704 splitit_web_python_sdk-2.3.0/splitit_client/type/redirection_endpoints_model.py
+-rw-r--r--   0        0        0      719 2023-06-12 15:48:13.526865 splitit_web_python_sdk-2.3.0/splitit_client/type/refund_model.py
+-rw-r--r--   0        0        0      341 2023-06-12 15:48:13.527016 splitit_web_python_sdk-2.3.0/splitit_client/type/refund_status.py
+-rw-r--r--   0        0        0      423 2023-06-12 15:48:13.527195 splitit_web_python_sdk-2.3.0/splitit_client/type/refund_strategy.py
+-rw-r--r--   0        0        0      642 2023-06-12 15:48:13.527372 splitit_web_python_sdk-2.3.0/splitit_client/type/refund_summary.py
+-rw-r--r--   0        0        0     1626 2023-06-12 15:48:13.527532 splitit_web_python_sdk-2.3.0/splitit_client/type/search_installment_plan_response_item.py
+-rw-r--r--   0        0        0      344 2023-06-12 15:48:13.527691 splitit_web_python_sdk-2.3.0/splitit_client/type/shipping_status.py
+-rw-r--r--   0        0        0      334 2023-06-12 15:48:13.527856 splitit_web_python_sdk-2.3.0/splitit_client/type/shipping_status2.py
+-rw-r--r--   0        0        0      528 2023-06-12 15:48:13.528022 splitit_web_python_sdk-2.3.0/splitit_client/type/shopper_data.py
+-rw-r--r--   0        0        0      345 2023-06-12 15:48:13.528185 splitit_web_python_sdk-2.3.0/splitit_client/type/test_modes.py
+-rw-r--r--   0        0        0      567 2023-06-12 15:48:13.528351 splitit_web_python_sdk-2.3.0/splitit_client/type/three_ds_redirect_data_v3.py
+-rw-r--r--   0        0        0      656 2023-06-12 15:48:13.528521 splitit_web_python_sdk-2.3.0/splitit_client/type/update_order_request.py
+-rw-r--r--   0        0        0      524 2023-06-12 15:48:13.528684 splitit_web_python_sdk-2.3.0/splitit_client/type/ux_settings_model.py
+-rw-r--r--   0        0        0      708 2023-06-12 15:48:13.528862 splitit_web_python_sdk-2.3.0/splitit_client/type/verify_authorization_response.py
+-rw-r--r--   0        0        0      491 2023-06-12 15:48:13.529019 splitit_web_python_sdk-2.3.0/splitit_client/type_util.py
+-rw-r--r--   0        0        0     3170 2023-06-12 15:48:13.529175 splitit_web_python_sdk-2.3.0/splitit_client/validation_metadata.py
+-rw-r--r--   0        0        0     9244 1970-01-01 00:00:00.000000 splitit_web_python_sdk-2.3.0/PKG-INFO
```

### Comparing `splitit_web_python_sdk-2.2.0/LICENSE` & `splitit_web_python_sdk-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/README.md` & `splitit_web_python_sdk-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# splitit-web-python-sdk@2.2.0
+# splitit-web-python-sdk@2.3.0
 Splitit's Web API
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install splitit-web-python-sdk==2.2.0
+pip install splitit-web-python-sdk==2.3.0
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from splitit_client import Splitit, ApiException
```

### Comparing `splitit_web_python_sdk-2.2.0/pyproject.toml` & `splitit_web_python_sdk-2.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splitit-web-python-sdk"
-version = "2.2.0"
+version = "2.3.0"
 description = "Client for splitit-web-api-v3"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "splitit_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/__init__.py` & `splitit_web_python_sdk-2.3.0/splitit_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Splitit's Web API
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 # import ApiClient
 from splitit_client.api_client import ApiClient
 
 # import Configuration
 from splitit_client.configuration import Configuration
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/api_client.py` & `splitit_web_python_sdk-2.3.0/splitit_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2738,15 +2738,15 @@
 0000ab10: 6465 725f 6e61 6d65 5d20 3d20 6865 6164  der_name] = head
 0000ab20: 6572 5f76 616c 7565 0a20 2020 2020 2020  er_value.       
 0000ab30: 2073 656c 662e 636f 6f6b 6965 203d 2063   self.cookie = c
 0000ab40: 6f6f 6b69 650a 2020 2020 2020 2020 2320  ookie.        # 
 0000ab50: 5365 7420 6465 6661 756c 7420 5573 6572  Set default User
 0000ab60: 2d41 6765 6e74 2e0a 2020 2020 2020 2020  -Agent..        
 0000ab70: 7365 6c66 2e75 7365 725f 6167 656e 7420  self.user_agent 
-0000ab80: 3d20 274b 6f6e 6669 672f 322e 322e 302f  = 'Konfig/2.2.0/
+0000ab80: 3d20 274b 6f6e 6669 672f 322e 332e 302f  = 'Konfig/2.3.0/
 0000ab90: 7079 7468 6f6e 270a 0a20 2020 2064 6566  python'..    def
 0000aba0: 205f 5f65 6e74 6572 5f5f 2873 656c 6629   __enter__(self)
 0000abb0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
 0000abc0: 2073 656c 660a 0a20 2020 2064 6566 205f   self..    def _
 0000abd0: 5f65 7869 745f 5f28 7365 6c66 2c20 6578  _exit__(self, ex
 0000abe0: 635f 7479 7065 2c20 6578 635f 7661 6c75  c_type, exc_valu
 0000abf0: 652c 2074 7261 6365 6261 636b 293a 0a20  e, traceback):.
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/api_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/api_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/apis/path_to_api.py` & `splitit_web_python_sdk-2.3.0/splitit_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/apis/tags/installment_plan_api.py` & `splitit_web_python_sdk-2.3.0/splitit_client/apis/tags/installment_plan_api.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/client.py` & `splitit_web_python_sdk-2.3.0/splitit_client/client.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/client.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/client.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/client_custom.py` & `splitit_web_python_sdk-2.3.0/splitit_client/client_custom.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/configuration.py` & `splitit_web_python_sdk-2.3.0/splitit_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 2.2.0".\
+               "SDK Package Version: 2.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/exceptions.py` & `splitit_web_python_sdk-2.3.0/splitit_client/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,25 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
+class ApiStreamingException(OpenApiException):
+
+    def __init__(self, status=None, reason=None):
+        self.status = status
+        self.reason = reason
+
+    def __str__(self):
+        """Custom error messages for exception"""
+        return "({0})\n Reason: {1}\n".format(self.status, self.reason)
+
+
 class ApiException(OpenApiException):
 
     def __init__(self, status=None, reason=None, api_response: typing.Optional[typing.Union[ApiResponse, AsyncApiResponse]] = None):
         if api_response:
             self.status = api_response.status
             self.reason = api_response.response.reason
             self.body = api_response.body
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/exceptions_base.py` & `splitit_web_python_sdk-2.3.0/splitit_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/address_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/address_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/address_data.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/address_data.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/address_data_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/address_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/address_data_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/address_data_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/authorization_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/authorization_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/authorization_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/authorization_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/card_brand.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/card_brand.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/card_brand.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/card_brand.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/card_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/card_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/card_data.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/card_data.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/card_type.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/card_type.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/card_type.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/card_type.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/check_installments_eligibility_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/check_installments_eligibility_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/check_installments_eligibility_request.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/check_installments_eligibility_request.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/error.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/error.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/error.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/error.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/error_extended.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/error_extended.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/error_extended.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/error_extended.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/events_endpoints_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/events_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/events_endpoints_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/events_endpoints_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/failed_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/failed_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/failed_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/failed_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/gw_authorization_status.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/gw_authorization_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/gw_authorization_status.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/gw_authorization_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/identifier_contract.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/identifier_contract.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/identifier_contract.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/identifier_contract.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_plan_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/initiate_plan_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_plan_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/initiate_plan_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_redirection_endpoints_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/initiate_redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_redirection_endpoints_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/initiate_redirection_endpoints_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_cancel_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_cancel_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_cancel_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_cancel_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_create_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_request.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_create_request.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_create_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_create_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_get_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_get_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_get_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_get_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_initiate_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_initiate_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_initiate_request.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_initiate_request.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_refund_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_request.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_refund_request.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_refund_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_refund_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_search_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_search_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_search_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_search_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_request.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request_by_identifier.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_request_by_identifier.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_plan_update_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_status.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_status.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/installment_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installments_eligibility_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/payment_method_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,85 +19,92 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class InstallmentsEligibilityResponse(
+class PaymentMethodModel(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
+        required = {
+            "Type",
+        }
         
         class properties:
-            
-            
-            class PaymentPlanOptions(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['PaymentPlanOptionModel']:
-                        return PaymentPlanOptionModel
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['PaymentPlanOptionModel'], typing.List['PaymentPlanOptionModel']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'PaymentPlanOptions':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'PaymentPlanOptionModel':
-                    return super().__getitem__(i)
+        
+            @staticmethod
+            def Type() -> typing.Type['PaymentMethodType']:
+                return PaymentMethodType
+        
+            @staticmethod
+            def Card() -> typing.Type['CardData']:
+                return CardData
+            Token = schemas.StrSchema
             __annotations__ = {
-                "PaymentPlanOptions": PaymentPlanOptions,
+                "Type": Type,
+                "Card": Card,
+                "Token": Token,
             }
     
+    Type: 'PaymentMethodType'
+    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["PaymentPlanOptions"]) -> MetaOapg.properties.PaymentPlanOptions: ...
+    def __getitem__(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["Card"]) -> 'CardData': ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["Token"]) -> MetaOapg.properties.Token: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["PaymentPlanOptions", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["PaymentPlanOptions"]) -> typing.Union[MetaOapg.properties.PaymentPlanOptions, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Card"]) -> typing.Union['CardData', schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Token"]) -> typing.Union[MetaOapg.properties.Token, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["PaymentPlanOptions", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        PaymentPlanOptions: typing.Union[MetaOapg.properties.PaymentPlanOptions, list, tuple, schemas.Unset] = schemas.unset,
+        Type: 'PaymentMethodType',
+        Card: typing.Union['CardData', schemas.Unset] = schemas.unset,
+        Token: typing.Union[MetaOapg.properties.Token, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'InstallmentsEligibilityResponse':
+    ) -> 'PaymentMethodModel':
         return super().__new__(
             cls,
             *args,
-            PaymentPlanOptions=PaymentPlanOptions,
+            Type=Type,
+            Card=Card,
+            Token=Token,
             _configuration=_configuration,
             **kwargs,
         )
 
-from splitit_client.model.payment_plan_option_model import PaymentPlanOptionModel
+from splitit_client.model.card_data import CardData
+from splitit_client.model.payment_method_type import PaymentMethodType
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/installments_eligibility_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/payment_method_model.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -19,85 +19,92 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class InstallmentsEligibilityResponse(
+class PaymentMethodModel(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
+        required = {
+            "Type",
+        }
         
         class properties:
-            
-            
-            class PaymentPlanOptions(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['PaymentPlanOptionModel']:
-                        return PaymentPlanOptionModel
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['PaymentPlanOptionModel'], typing.List['PaymentPlanOptionModel']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'PaymentPlanOptions':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'PaymentPlanOptionModel':
-                    return super().__getitem__(i)
+        
+            @staticmethod
+            def Type() -> typing.Type['PaymentMethodType']:
+                return PaymentMethodType
+        
+            @staticmethod
+            def Card() -> typing.Type['CardData']:
+                return CardData
+            Token = schemas.StrSchema
             __annotations__ = {
-                "PaymentPlanOptions": PaymentPlanOptions,
+                "Type": Type,
+                "Card": Card,
+                "Token": Token,
             }
     
+    Type: 'PaymentMethodType'
+    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["PaymentPlanOptions"]) -> MetaOapg.properties.PaymentPlanOptions: ...
+    def __getitem__(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["Card"]) -> 'CardData': ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["Token"]) -> MetaOapg.properties.Token: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["PaymentPlanOptions", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["PaymentPlanOptions"]) -> typing.Union[MetaOapg.properties.PaymentPlanOptions, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Card"]) -> typing.Union['CardData', schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Token"]) -> typing.Union[MetaOapg.properties.Token, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["PaymentPlanOptions", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        PaymentPlanOptions: typing.Union[MetaOapg.properties.PaymentPlanOptions, list, tuple, schemas.Unset] = schemas.unset,
+        Type: 'PaymentMethodType',
+        Card: typing.Union['CardData', schemas.Unset] = schemas.unset,
+        Token: typing.Union[MetaOapg.properties.Token, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'InstallmentsEligibilityResponse':
+    ) -> 'PaymentMethodModel':
         return super().__new__(
             cls,
             *args,
-            PaymentPlanOptions=PaymentPlanOptions,
+            Type=Type,
+            Card=Card,
+            Token=Token,
             _configuration=_configuration,
             **kwargs,
         )
 
-from splitit_client.model.payment_plan_option_model import PaymentPlanOptionModel
+from splitit_client.model.card_data import CardData
+from splitit_client.model.payment_method_type import PaymentMethodType
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/links_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/links_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/links_data.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/links_data.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/links_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/links_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/links_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/links_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/shopper_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,92 +19,88 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PaymentMethodModel(
+class ShopperData(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
-        required = {
-            "Type",
-        }
         
         class properties:
-        
-            @staticmethod
-            def Type() -> typing.Type['PaymentMethodType']:
-                return PaymentMethodType
-        
-            @staticmethod
-            def Card() -> typing.Type['CardData']:
-                return CardData
-            Token = schemas.StrSchema
+            FullName = schemas.StrSchema
+            Email = schemas.StrSchema
+            PhoneNumber = schemas.StrSchema
+            Culture = schemas.StrSchema
             __annotations__ = {
-                "Type": Type,
-                "Card": Card,
-                "Token": Token,
+                "FullName": FullName,
+                "Email": Email,
+                "PhoneNumber": PhoneNumber,
+                "Culture": Culture,
             }
     
-    Type: 'PaymentMethodType'
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["FullName"]) -> MetaOapg.properties.FullName: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    def __getitem__(self, name: typing_extensions.Literal["Email"]) -> MetaOapg.properties.Email: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Card"]) -> 'CardData': ...
+    def __getitem__(self, name: typing_extensions.Literal["PhoneNumber"]) -> MetaOapg.properties.PhoneNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Token"]) -> MetaOapg.properties.Token: ...
+    def __getitem__(self, name: typing_extensions.Literal["Culture"]) -> MetaOapg.properties.Culture: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["FullName"]) -> typing.Union[MetaOapg.properties.FullName, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Card"]) -> typing.Union['CardData', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Email"]) -> typing.Union[MetaOapg.properties.Email, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Token"]) -> typing.Union[MetaOapg.properties.Token, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["PhoneNumber"]) -> typing.Union[MetaOapg.properties.PhoneNumber, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Culture"]) -> typing.Union[MetaOapg.properties.Culture, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        Type: 'PaymentMethodType',
-        Card: typing.Union['CardData', schemas.Unset] = schemas.unset,
-        Token: typing.Union[MetaOapg.properties.Token, str, schemas.Unset] = schemas.unset,
+        FullName: typing.Union[MetaOapg.properties.FullName, str, schemas.Unset] = schemas.unset,
+        Email: typing.Union[MetaOapg.properties.Email, str, schemas.Unset] = schemas.unset,
+        PhoneNumber: typing.Union[MetaOapg.properties.PhoneNumber, str, schemas.Unset] = schemas.unset,
+        Culture: typing.Union[MetaOapg.properties.Culture, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PaymentMethodModel':
+    ) -> 'ShopperData':
         return super().__new__(
             cls,
             *args,
-            Type=Type,
-            Card=Card,
-            Token=Token,
+            FullName=FullName,
+            Email=Email,
+            PhoneNumber=PhoneNumber,
+            Culture=Culture,
             _configuration=_configuration,
             **kwargs,
         )
-
-from splitit_client.model.card_data import CardData
-from splitit_client.model.payment_method_type import PaymentMethodType
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/shopper_data.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -19,92 +19,88 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PaymentMethodModel(
+class ShopperData(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
-        required = {
-            "Type",
-        }
         
         class properties:
-        
-            @staticmethod
-            def Type() -> typing.Type['PaymentMethodType']:
-                return PaymentMethodType
-        
-            @staticmethod
-            def Card() -> typing.Type['CardData']:
-                return CardData
-            Token = schemas.StrSchema
+            FullName = schemas.StrSchema
+            Email = schemas.StrSchema
+            PhoneNumber = schemas.StrSchema
+            Culture = schemas.StrSchema
             __annotations__ = {
-                "Type": Type,
-                "Card": Card,
-                "Token": Token,
+                "FullName": FullName,
+                "Email": Email,
+                "PhoneNumber": PhoneNumber,
+                "Culture": Culture,
             }
     
-    Type: 'PaymentMethodType'
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["FullName"]) -> MetaOapg.properties.FullName: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    def __getitem__(self, name: typing_extensions.Literal["Email"]) -> MetaOapg.properties.Email: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Card"]) -> 'CardData': ...
+    def __getitem__(self, name: typing_extensions.Literal["PhoneNumber"]) -> MetaOapg.properties.PhoneNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Token"]) -> MetaOapg.properties.Token: ...
+    def __getitem__(self, name: typing_extensions.Literal["Culture"]) -> MetaOapg.properties.Culture: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["FullName"]) -> typing.Union[MetaOapg.properties.FullName, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Card"]) -> typing.Union['CardData', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Email"]) -> typing.Union[MetaOapg.properties.Email, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Token"]) -> typing.Union[MetaOapg.properties.Token, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["PhoneNumber"]) -> typing.Union[MetaOapg.properties.PhoneNumber, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Culture"]) -> typing.Union[MetaOapg.properties.Culture, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        Type: 'PaymentMethodType',
-        Card: typing.Union['CardData', schemas.Unset] = schemas.unset,
-        Token: typing.Union[MetaOapg.properties.Token, str, schemas.Unset] = schemas.unset,
+        FullName: typing.Union[MetaOapg.properties.FullName, str, schemas.Unset] = schemas.unset,
+        Email: typing.Union[MetaOapg.properties.Email, str, schemas.Unset] = schemas.unset,
+        PhoneNumber: typing.Union[MetaOapg.properties.PhoneNumber, str, schemas.Unset] = schemas.unset,
+        Culture: typing.Union[MetaOapg.properties.Culture, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PaymentMethodModel':
+    ) -> 'ShopperData':
         return super().__new__(
             cls,
             *args,
-            Type=Type,
-            Card=Card,
-            Token=Token,
+            FullName=FullName,
+            Email=Email,
+            PhoneNumber=PhoneNumber,
+            Culture=Culture,
             _configuration=_configuration,
             **kwargs,
         )
-
-from splitit_client.model.card_data import CardData
-from splitit_client.model.payment_method_type import PaymentMethodType
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_type.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_type.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/payment_method_type.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/plan_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/plan_data.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/plan_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/plan_data_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_error_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/plan_error_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_error_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/plan_error_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_status.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/plan_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_status.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/plan_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/purchase_method.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/purchase_method.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/purchase_method.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/purchase_method.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/redirection_endpoints_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/redirection_endpoints_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/redirection_endpoints_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/refund_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/refund_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_status.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/refund_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_status.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/refund_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_strategy.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/refund_strategy.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_strategy.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/refund_strategy.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_summary.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/refund_summary.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_summary.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/refund_summary.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/search_installment_plan_response_item.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/search_installment_plan_response_item.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/search_installment_plan_response_item.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/search_installment_plan_response_item.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/shipping_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/shipping_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status2.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/shipping_status2.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status2.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/shipping_status2.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/shopper_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/update_order_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,88 +19,93 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class ShopperData(
+class UpdateOrderRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
-            FullName = schemas.StrSchema
-            Email = schemas.StrSchema
-            PhoneNumber = schemas.StrSchema
-            Culture = schemas.StrSchema
+            TrackingNumber = schemas.StrSchema
+            RefOrderNumber = schemas.StrSchema
+        
+            @staticmethod
+            def ShippingStatus() -> typing.Type['ShippingStatus']:
+                return ShippingStatus
+            Capture = schemas.BoolSchema
             __annotations__ = {
-                "FullName": FullName,
-                "Email": Email,
-                "PhoneNumber": PhoneNumber,
-                "Culture": Culture,
+                "TrackingNumber": TrackingNumber,
+                "RefOrderNumber": RefOrderNumber,
+                "ShippingStatus": ShippingStatus,
+                "Capture": Capture,
             }
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["FullName"]) -> MetaOapg.properties.FullName: ...
+    def __getitem__(self, name: typing_extensions.Literal["TrackingNumber"]) -> MetaOapg.properties.TrackingNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Email"]) -> MetaOapg.properties.Email: ...
+    def __getitem__(self, name: typing_extensions.Literal["RefOrderNumber"]) -> MetaOapg.properties.RefOrderNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["PhoneNumber"]) -> MetaOapg.properties.PhoneNumber: ...
+    def __getitem__(self, name: typing_extensions.Literal["ShippingStatus"]) -> 'ShippingStatus': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Culture"]) -> MetaOapg.properties.Culture: ...
+    def __getitem__(self, name: typing_extensions.Literal["Capture"]) -> MetaOapg.properties.Capture: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TrackingNumber", "RefOrderNumber", "ShippingStatus", "Capture", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["FullName"]) -> typing.Union[MetaOapg.properties.FullName, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["TrackingNumber"]) -> typing.Union[MetaOapg.properties.TrackingNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Email"]) -> typing.Union[MetaOapg.properties.Email, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["RefOrderNumber"]) -> typing.Union[MetaOapg.properties.RefOrderNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["PhoneNumber"]) -> typing.Union[MetaOapg.properties.PhoneNumber, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ShippingStatus"]) -> typing.Union['ShippingStatus', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Culture"]) -> typing.Union[MetaOapg.properties.Culture, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Capture"]) -> typing.Union[MetaOapg.properties.Capture, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TrackingNumber", "RefOrderNumber", "ShippingStatus", "Capture", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        FullName: typing.Union[MetaOapg.properties.FullName, str, schemas.Unset] = schemas.unset,
-        Email: typing.Union[MetaOapg.properties.Email, str, schemas.Unset] = schemas.unset,
-        PhoneNumber: typing.Union[MetaOapg.properties.PhoneNumber, str, schemas.Unset] = schemas.unset,
-        Culture: typing.Union[MetaOapg.properties.Culture, str, schemas.Unset] = schemas.unset,
+        TrackingNumber: typing.Union[MetaOapg.properties.TrackingNumber, str, schemas.Unset] = schemas.unset,
+        RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
+        ShippingStatus: typing.Union['ShippingStatus', schemas.Unset] = schemas.unset,
+        Capture: typing.Union[MetaOapg.properties.Capture, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ShopperData':
+    ) -> 'UpdateOrderRequest':
         return super().__new__(
             cls,
             *args,
-            FullName=FullName,
-            Email=Email,
-            PhoneNumber=PhoneNumber,
-            Culture=Culture,
+            TrackingNumber=TrackingNumber,
+            RefOrderNumber=RefOrderNumber,
+            ShippingStatus=ShippingStatus,
+            Capture=Capture,
             _configuration=_configuration,
             **kwargs,
         )
+
+from splitit_client.model.shipping_status import ShippingStatus
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/shopper_data.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/update_order_request.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -19,88 +19,93 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class ShopperData(
+class UpdateOrderRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
-            FullName = schemas.StrSchema
-            Email = schemas.StrSchema
-            PhoneNumber = schemas.StrSchema
-            Culture = schemas.StrSchema
+            TrackingNumber = schemas.StrSchema
+            RefOrderNumber = schemas.StrSchema
+        
+            @staticmethod
+            def ShippingStatus() -> typing.Type['ShippingStatus']:
+                return ShippingStatus
+            Capture = schemas.BoolSchema
             __annotations__ = {
-                "FullName": FullName,
-                "Email": Email,
-                "PhoneNumber": PhoneNumber,
-                "Culture": Culture,
+                "TrackingNumber": TrackingNumber,
+                "RefOrderNumber": RefOrderNumber,
+                "ShippingStatus": ShippingStatus,
+                "Capture": Capture,
             }
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["FullName"]) -> MetaOapg.properties.FullName: ...
+    def __getitem__(self, name: typing_extensions.Literal["TrackingNumber"]) -> MetaOapg.properties.TrackingNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Email"]) -> MetaOapg.properties.Email: ...
+    def __getitem__(self, name: typing_extensions.Literal["RefOrderNumber"]) -> MetaOapg.properties.RefOrderNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["PhoneNumber"]) -> MetaOapg.properties.PhoneNumber: ...
+    def __getitem__(self, name: typing_extensions.Literal["ShippingStatus"]) -> 'ShippingStatus': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Culture"]) -> MetaOapg.properties.Culture: ...
+    def __getitem__(self, name: typing_extensions.Literal["Capture"]) -> MetaOapg.properties.Capture: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TrackingNumber", "RefOrderNumber", "ShippingStatus", "Capture", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["FullName"]) -> typing.Union[MetaOapg.properties.FullName, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["TrackingNumber"]) -> typing.Union[MetaOapg.properties.TrackingNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Email"]) -> typing.Union[MetaOapg.properties.Email, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["RefOrderNumber"]) -> typing.Union[MetaOapg.properties.RefOrderNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["PhoneNumber"]) -> typing.Union[MetaOapg.properties.PhoneNumber, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ShippingStatus"]) -> typing.Union['ShippingStatus', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Culture"]) -> typing.Union[MetaOapg.properties.Culture, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Capture"]) -> typing.Union[MetaOapg.properties.Capture, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TrackingNumber", "RefOrderNumber", "ShippingStatus", "Capture", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        FullName: typing.Union[MetaOapg.properties.FullName, str, schemas.Unset] = schemas.unset,
-        Email: typing.Union[MetaOapg.properties.Email, str, schemas.Unset] = schemas.unset,
-        PhoneNumber: typing.Union[MetaOapg.properties.PhoneNumber, str, schemas.Unset] = schemas.unset,
-        Culture: typing.Union[MetaOapg.properties.Culture, str, schemas.Unset] = schemas.unset,
+        TrackingNumber: typing.Union[MetaOapg.properties.TrackingNumber, str, schemas.Unset] = schemas.unset,
+        RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
+        ShippingStatus: typing.Union['ShippingStatus', schemas.Unset] = schemas.unset,
+        Capture: typing.Union[MetaOapg.properties.Capture, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ShopperData':
+    ) -> 'UpdateOrderRequest':
         return super().__new__(
             cls,
             *args,
-            FullName=FullName,
-            Email=Email,
-            PhoneNumber=PhoneNumber,
-            Culture=Culture,
+            TrackingNumber=TrackingNumber,
+            RefOrderNumber=RefOrderNumber,
+            ShippingStatus=ShippingStatus,
+            Capture=Capture,
             _configuration=_configuration,
             **kwargs,
         )
+
+from splitit_client.model.shipping_status import ShippingStatus
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/test_modes.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/test_modes.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/test_modes.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/test_modes.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/three_ds_redirect_data_v3.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/three_ds_redirect_data_v3.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/three_ds_redirect_data_v3.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/three_ds_redirect_data_v3.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/ux_settings_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/ux_settings_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/ux_settings_model.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/ux_settings_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/verify_authorization_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/model/verify_authorization_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/model/verify_authorization_response.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/model/verify_authorization_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/models/__init__.py` & `splitit_web_python_sdk-2.3.0/splitit_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/__init__.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans/post.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,14 +418,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans/post.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans/post.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_initiate/post.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_initiate/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_initiate/post.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_initiate/post.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -393,14 +393,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,17 @@
             method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,17 @@
             method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 
 from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
 from splitit_client.model.installment_plan_cancel_response import InstallmentPlanCancelResponse as InstallmentPlanCancelResponseSchema
 
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.installment_plan_cancel_response import InstallmentPlanCancelResponse
 
-from . import path
-
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
@@ -86,17 +84,14 @@
 
 request_path_installment_plan_number = api_client.PathParameter(
     name="installmentPlanNumber",
     style=api_client.ParameterStyle.SIMPLE,
     schema=InstallmentPlanNumberSchema,
     required=True,
 )
-_auth = [
-    'oauth',
-]
 SchemaFor200ResponseBodyTextPlain = InstallmentPlanCancelResponseSchema
 SchemaFor200ResponseBodyApplicationJson = InstallmentPlanCancelResponseSchema
 SchemaFor200ResponseBodyTextJson = InstallmentPlanCancelResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -224,21 +219,14 @@
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '401': _response_for_401,
-    '403': _response_for_403,
-    '404': _response_for_404,
-    '500': _response_for_500,
-}
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
@@ -314,14 +302,17 @@
             method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
 from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
 from splitit_client.model.installment_plan_cancel_response import InstallmentPlanCancelResponse as InstallmentPlanCancelResponseSchema
 
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.installment_plan_cancel_response import InstallmentPlanCancelResponse
 
+from . import path
+
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
@@ -84,14 +86,17 @@
 
 request_path_installment_plan_number = api_client.PathParameter(
     name="installmentPlanNumber",
     style=api_client.ParameterStyle.SIMPLE,
     schema=InstallmentPlanNumberSchema,
     required=True,
 )
+_auth = [
+    'oauth',
+]
 SchemaFor200ResponseBodyTextPlain = InstallmentPlanCancelResponseSchema
 SchemaFor200ResponseBodyApplicationJson = InstallmentPlanCancelResponseSchema
 SchemaFor200ResponseBodyTextJson = InstallmentPlanCancelResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -219,14 +224,21 @@
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '401': _response_for_401,
+    '403': _response_for_403,
+    '404': _response_for_404,
+    '500': _response_for_500,
+}
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
@@ -302,14 +314,17 @@
             method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,14 @@
 from splitit_client.model.installment_plan_refund_request import InstallmentPlanRefundRequest as InstallmentPlanRefundRequestSchema
 
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.installment_plan_refund_response import InstallmentPlanRefundResponse
 from splitit_client.type.refund_strategy import RefundStrategy
 from splitit_client.type.installment_plan_refund_request import InstallmentPlanRefundRequest
 
-from . import path
-
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
@@ -110,17 +108,14 @@
         'text/json': api_client.MediaType(
             schema=SchemaForRequestBodyTextJson),
         'application/*+json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'oauth',
-]
 SchemaFor200ResponseBodyTextPlain = InstallmentPlanRefundResponseSchema
 SchemaFor200ResponseBodyApplicationJson = InstallmentPlanRefundResponseSchema
 SchemaFor200ResponseBodyTextJson = InstallmentPlanRefundResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -248,21 +243,14 @@
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '401': _response_for_401,
-    '403': _response_for_403,
-    '404': _response_for_404,
-    '500': _response_for_500,
-}
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
@@ -362,14 +350,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 from splitit_client.model.installment_plan_refund_request import InstallmentPlanRefundRequest as InstallmentPlanRefundRequestSchema
 
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.installment_plan_refund_response import InstallmentPlanRefundResponse
 from splitit_client.type.refund_strategy import RefundStrategy
 from splitit_client.type.installment_plan_refund_request import InstallmentPlanRefundRequest
 
+from . import path
+
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
@@ -108,14 +110,17 @@
         'text/json': api_client.MediaType(
             schema=SchemaForRequestBodyTextJson),
         'application/*+json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
+_auth = [
+    'oauth',
+]
 SchemaFor200ResponseBodyTextPlain = InstallmentPlanRefundResponseSchema
 SchemaFor200ResponseBodyApplicationJson = InstallmentPlanRefundResponseSchema
 SchemaFor200ResponseBodyTextJson = InstallmentPlanRefundResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -243,14 +248,21 @@
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '401': _response_for_401,
+    '403': _response_for_403,
+    '404': _response_for_404,
+    '500': _response_for_500,
+}
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
@@ -350,14 +362,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,14 +368,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,17 @@
             method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,17 @@
             method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/get.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_search/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,14 +367,17 @@
             headers=_headers,
             auth_settings=_auth,
             prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/get.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_search/get.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,17 @@
             headers=_headers,
             auth_settings=_auth,
             prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_updateorder/put.py` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,14 @@
 
 from splitit_client.type.installment_plan_update_request_by_identifier import InstallmentPlanUpdateRequestByIdentifier
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.identifier_contract import IdentifierContract
 from splitit_client.type.installment_plan_update_response import InstallmentPlanUpdateResponse
 from splitit_client.type.shipping_status2 import ShippingStatus2
 
-from . import path
-
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
@@ -86,17 +84,14 @@
         'text/json': api_client.MediaType(
             schema=SchemaForRequestBodyTextJson),
         'application/*+json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'oauth',
-]
 SchemaFor200ResponseBodyTextPlain = InstallmentPlanUpdateResponseSchema
 SchemaFor200ResponseBodyApplicationJson = InstallmentPlanUpdateResponseSchema
 SchemaFor200ResponseBodyTextJson = InstallmentPlanUpdateResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -224,21 +219,14 @@
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '401': _response_for_401,
-    '403': _response_for_403,
-    '404': _response_for_404,
-    '500': _response_for_500,
-}
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
@@ -327,14 +315,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi` & `splitit_web_python_sdk-2.3.0/splitit_client/paths/api_installmentplans_updateorder/put.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 from splitit_client.type.installment_plan_update_request_by_identifier import InstallmentPlanUpdateRequestByIdentifier
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.identifier_contract import IdentifierContract
 from splitit_client.type.installment_plan_update_response import InstallmentPlanUpdateResponse
 from splitit_client.type.shipping_status2 import ShippingStatus2
 
+from . import path
+
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
@@ -84,14 +86,17 @@
         'text/json': api_client.MediaType(
             schema=SchemaForRequestBodyTextJson),
         'application/*+json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
+_auth = [
+    'oauth',
+]
 SchemaFor200ResponseBodyTextPlain = InstallmentPlanUpdateResponseSchema
 SchemaFor200ResponseBodyApplicationJson = InstallmentPlanUpdateResponseSchema
 SchemaFor200ResponseBodyTextJson = InstallmentPlanUpdateResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -219,14 +224,21 @@
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '401': _response_for_401,
+    '403': _response_for_403,
+    '404': _response_for_404,
+    '500': _response_for_500,
+}
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
@@ -315,14 +327,17 @@
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
+            if not 200 <= response.http_response.status <= 299:
+                raise exceptions.ApiStreamingException(status=response.http_response.status, reason=response.http_response.reason)
+        
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
                 """
                 async for line in response.http_response.content:
                     if line == b'\r\n':
                         continue
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/request_after_hook.py` & `splitit_web_python_sdk-2.3.0/splitit_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/request_before_hook.py` & `splitit_web_python_sdk-2.3.0/splitit_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/rest.py` & `splitit_web_python_sdk-2.3.0/splitit_client/rest.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/schemas.py` & `splitit_web_python_sdk-2.3.0/splitit_client/schemas.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/address_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/address_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/address_data_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/address_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/authorization_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/authorization_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/card_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/card_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/check_installments_eligibility_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/check_installments_eligibility_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/events_endpoints_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/events_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/failed_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/failed_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/identifier_contract.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/identifier_contract.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/initiate_plan_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/initiate_plan_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/initiate_redirection_endpoints_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/initiate_redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_cancel_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_cancel_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_create_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_create_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_create_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_create_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_get_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_get_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_initiate_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_initiate_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_refund_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_refund_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_refund_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_refund_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_search_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_search_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_update_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_request_by_identifier.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_update_request_by_identifier.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/installment_plan_update_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/links_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/links_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/links_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/links_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/payment_method_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/payment_method_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/payment_plan_option_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/payment_plan_option_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,9 +24,13 @@
     InstallmentAmount: typing.Union[int, float]
 
     LastInstallmentAmount: typing.Union[int, float]
 
 class OptionalPaymentPlanOptionModel(TypedDict, total=False):
     Links: LinksModel
 
+    TermsAndConditionsBrief: str
+
+    InstallmentFrequency: str
+
 class PaymentPlanOptionModel(RequiredPaymentPlanOptionModel, OptionalPaymentPlanOptionModel):
     pass
```

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/plan_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/plan_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/plan_data_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/plan_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/redirection_endpoints_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/refund_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/refund_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/refund_summary.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/refund_summary.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/search_installment_plan_response_item.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/search_installment_plan_response_item.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/shopper_data.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/shopper_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/three_ds_redirect_data_v3.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/three_ds_redirect_data_v3.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/update_order_request.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/update_order_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/ux_settings_model.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/ux_settings_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/type/verify_authorization_response.py` & `splitit_web_python_sdk-2.3.0/splitit_client/type/verify_authorization_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/splitit_client/validation_metadata.py` & `splitit_web_python_sdk-2.3.0/splitit_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.2.0/PKG-INFO` & `splitit_web_python_sdk-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitit-web-python-sdk
-Version: 2.2.0
+Version: 2.3.0
 Summary: Client for splitit-web-api-v3
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,26 +18,26 @@
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
-# splitit-web-python-sdk@2.2.0
+# splitit-web-python-sdk@2.3.0
 Splitit's Web API
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install splitit-web-python-sdk==2.2.0
+pip install splitit-web-python-sdk==2.3.0
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from splitit_client import Splitit, ApiException
```

