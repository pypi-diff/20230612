# Comparing `tmp/candidhealth-0.2.0.tar.gz` & `tmp/candidhealth-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candidhealth-0.2.0.tar", max compression
+gzip compressed data, was "candidhealth-0.2.1.tar", max compression
```

## Comparing `candidhealth-0.2.0.tar` & `candidhealth-0.2.1.tar`

### file list

```diff
@@ -1,255 +1,265 @@
--rw-r--r--   0        0        0      257 2023-06-05 17:07:20.463629 candidhealth-0.2.0/README.md
--rw-r--r--   0        0        0      373 2023-06-05 17:07:20.463629 candidhealth-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5809 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/__init__.py
--rw-r--r--   0        0        0     3166 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/candid_api_client.py
--rw-r--r--   0        0        0     2274 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/client.py
--rw-r--r--   0        0        0      348 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      227 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/environment.py
--rw-r--r--   0        0        0        0 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/py.typed
--rw-r--r--   0        0        0     5975 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/__init__.py
--rw-r--r--   0        0        0      111 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/__init__.py
--rw-r--r--   0        0        0      820 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/client.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/__init__.py
--rw-r--r--   0        0        0      304 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/__init__.py
--rw-r--r--   0        0        0     3502 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/client.py
--rw-r--r--   0        0        0      159 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/errors/__init__.py
--rw-r--r--   0        0        0      330 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      333 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      785 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
--rw-r--r--   0        0        0      806 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
--rw-r--r--   0        0        0      765 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
--rw-r--r--   0        0        0      191 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/__init__.py
--rw-r--r--   0        0        0     2831 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/client.py
--rw-r--r--   0        0        0      256 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/types/__init__.py
--rw-r--r--   0        0        0     1136 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note.py
--rw-r--r--   0        0        0      813 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note_base.py
--rw-r--r--   0        0        0      104 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note_id.py
--rw-r--r--   0        0        0      139 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/claims/__init__.py
--rw-r--r--   0        0        0      164 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/claims/types/__init__.py
--rw-r--r--   0        0        0     1151 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/claims/types/claim.py
--rw-r--r--   0        0        0     2605 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/claims/types/claim_status.py
--rw-r--r--   0        0        0     1445 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/__init__.py
--rw-r--r--   0        0        0     2150 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/__init__.py
--rw-r--r--   0        0        0       79 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/auth_0_id.py
--rw-r--r--   0        0        0       98 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/claim_id.py
--rw-r--r--   0        0        0      905 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/contact_info.py
--rw-r--r--   0        0        0       90 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/content_download_url.py
--rw-r--r--   0        0        0       76 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/date.py
--rw-r--r--   0        0        0       77 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/email.py
--rw-r--r--   0        0        0       91 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/encounter_external_id.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/encounter_id.py
--rw-r--r--   0        0        0    11148 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/facility_type_code.py
--rw-r--r--   0        0        0    15447 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/insurance_type_code.py
--rw-r--r--   0        0        0       79 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/link_url.py
--rw-r--r--   0        0        0       75 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/npi.py
--rw-r--r--   0        0        0      105 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/organization_id.py
--rw-r--r--   0        0        0       81 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/page_token.py
--rw-r--r--   0        0        0       89 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/patient_external_id.py
--rw-r--r--   0        0        0     4686 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
--rw-r--r--   0        0        0      822 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      620 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/phone_number_type.py
--rw-r--r--   0        0        0    79514 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/procedure_modifier.py
--rw-r--r--   0        0        0      735 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/region_national.py
--rw-r--r--   0        0        0      790 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/region_states.py
--rw-r--r--   0        0        0      633 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/regions.py
--rw-r--r--   0        0        0      864 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/resource_page.py
--rw-r--r--   0        0        0      104 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/service_line_id.py
--rw-r--r--   0        0        0      432 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/service_line_units.py
--rw-r--r--   0        0        0     5065 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/source_of_payment_code.py
--rw-r--r--   0        0        0     6264 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/state.py
--rw-r--r--   0        0        0     1037 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/street_address_base.py
--rw-r--r--   0        0        0      985 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/street_address_long_zip.py
--rw-r--r--   0        0        0     1003 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/street_address_short_zip.py
--rw-r--r--   0        0        0       83 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/work_queue_id.py
--rw-r--r--   0        0        0      251 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/__init__.py
--rw-r--r--   0        0        0      365 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/__init__.py
--rw-r--r--   0        0        0      940 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/authorized_signatory.py
--rw-r--r--   0        0        0     1430 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/contract.py
--rw-r--r--   0        0        0     1517 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/contract_base.py
--rw-r--r--   0        0        0      101 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/contract_id.py
--rw-r--r--   0        0        0      986 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/contract_status.py
--rw-r--r--   0        0        0     1125 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/credentialing/__init__.py
--rw-r--r--   0        0        0     1472 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/credentialing/types/__init__.py
--rw-r--r--   0        0        0      886 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
--rw-r--r--   0        0        0      846 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialing_span_dates.py
--rw-r--r--   0        0        0      977 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialing_span_status.py
--rw-r--r--   0        0        0      809 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
--rw-r--r--   0        0        0      864 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
--rw-r--r--   0        0        0     2210 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span.py
--rw-r--r--   0        0        0      958 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
--rw-r--r--   0        0        0      118 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
--rw-r--r--   0        0        0      827 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/required_credentialing_dates.py
--rw-r--r--   0        0        0      279 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/__init__.py
--rw-r--r--   0        0        0      409 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/__init__.py
--rw-r--r--   0        0        0      958 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis.py
--rw-r--r--   0        0        0     1904 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_create.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_id.py
--rw-r--r--   0        0        0     1974 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py
--rw-r--r--   0        0        0      903 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
--rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/__init__.py
--rw-r--r--   0        0        0      381 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      516 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
--rw-r--r--   0        0        0     1092 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
--rw-r--r--   0        0        0     1260 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
--rw-r--r--   0        0        0      101 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
--rw-r--r--   0        0        0     1244 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
--rw-r--r--   0        0        0     1244 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
--rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/__init__.py
--rw-r--r--   0        0        0      832 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/client.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/__init__.py
--rw-r--r--   0        0        0     2694 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/__init__.py
--rw-r--r--   0        0        0    34265 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/client.py
--rw-r--r--   0        0        0      202 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/errors/__init__.py
--rw-r--r--   0        0        0      387 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/errors/encounter_external_id_uniqueness_error.py
--rw-r--r--   0        0        0     3794 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/__init__.py
--rw-r--r--   0        0        0      103 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
--rw-r--r--   0        0        0     1206 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
--rw-r--r--   0        0        0      944 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
--rw-r--r--   0        0        0      874 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
--rw-r--r--   0        0        0      944 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
--rw-r--r--   0        0        0      894 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
--rw-r--r--   0        0        0      659 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
--rw-r--r--   0        0        0      713 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
--rw-r--r--   0        0        0     2992 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter.py
--rw-r--r--   0        0        0      920 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
--rw-r--r--   0        0        0      388 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
--rw-r--r--   0        0        0     4498 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
--rw-r--r--   0        0        0      889 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py
--rw-r--r--   0        0        0      885 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
--rw-r--r--   0        0        0     1025 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
--rw-r--r--   0        0        0      568 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      855 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
--rw-r--r--   0        0        0      845 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
--rw-r--r--   0        0        0       88 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
--rw-r--r--   0        0        0      969 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py
--rw-r--r--   0        0        0       88 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
--rw-r--r--   0        0        0      891 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
--rw-r--r--   0        0        0     1303 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intervention.py
--rw-r--r--   0        0        0      865 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
--rw-r--r--   0        0        0      855 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/lab.py
--rw-r--r--   0        0        0      457 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
--rw-r--r--   0        0        0      834 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
--rw-r--r--   0        0        0      953 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/medication.py
--rw-r--r--   0        0        0      880 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/network_status.py
--rw-r--r--   0        0        0     1164 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
--rw-r--r--   0        0        0     2615 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/note_category.py
--rw-r--r--   0        0        0      900 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
--rw-r--r--   0        0        0     1012 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
--rw-r--r--   0        0        0      885 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
--rw-r--r--   0        0        0       96 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
--rw-r--r--   0        0        0       77 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
--rw-r--r--   0        0        0      898 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      544 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
--rw-r--r--   0        0        0      893 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/vitals.py
--rw-r--r--   0        0        0      143 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/__init__.py
--rw-r--r--   0        0        0      181 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/types/__init__.py
--rw-r--r--   0        0        0      817 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/types/era.py
--rw-r--r--   0        0        0      811 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/types/era_base.py
--rw-r--r--   0        0        0       96 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/types/era_id.py
--rw-r--r--   0        0        0      207 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/__init__.py
--rw-r--r--   0        0        0     5547 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/client.py
--rw-r--r--   0        0        0      270 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/types/__init__.py
--rw-r--r--   0        0        0      729 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/types/expected_network_status.py
--rw-r--r--   0        0        0      981 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py
--rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/__init__.py
--rw-r--r--   0        0        0      830 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/client.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/__init__.py
--rw-r--r--   0        0        0      215 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/__init__.py
--rw-r--r--   0        0        0     8114 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/client.py
--rw-r--r--   0        0        0      300 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0      867 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py
--rw-r--r--   0        0        0     1020 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py
--rw-r--r--   0        0        0      804 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_id.py
--rw-r--r--   0        0        0      435 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/__init__.py
--rw-r--r--   0        0        0      602 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/__init__.py
--rw-r--r--   0        0        0      871 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/gender.py
--rw-r--r--   0        0        0      821 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/individual_base.py
--rw-r--r--   0        0        0      103 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/individual_id.py
--rw-r--r--   0        0        0      861 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/patient.py
--rw-r--r--   0        0        0     1614 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/patient_base.py
--rw-r--r--   0        0        0      794 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/patient_create.py
--rw-r--r--   0        0        0      972 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/subscriber.py
--rw-r--r--   0        0        0     1200 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/subscriber_base.py
--rw-r--r--   0        0        0      925 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/subscriber_create.py
--rw-r--r--   0        0        0      247 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/__init__.py
--rw-r--r--   0        0        0      352 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/__init__.py
--rw-r--r--   0        0        0     1106 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card.py
--rw-r--r--   0        0        0     1122 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_base.py
--rw-r--r--   0        0        0     1026 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_create.py
--rw-r--r--   0        0        0      106 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_id.py
--rw-r--r--   0        0        0      199 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/__init__.py
--rw-r--r--   0        0        0      276 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/__init__.py
--rw-r--r--   0        0        0     1397 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/invoice.py
--rw-r--r--   0        0        0      100 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_id.py
--rw-r--r--   0        0        0      849 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_item.py
--rw-r--r--   0        0        0      908 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_status.py
--rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/__init__.py
--rw-r--r--   0        0        0      501 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      704 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      334 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
--rw-r--r--   0        0        0      492 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
--rw-r--r--   0        0        0     2857 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
--rw-r--r--   0        0        0     1562 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
--rw-r--r--   0        0        0     1062 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
--rw-r--r--   0        0        0     2853 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
--rw-r--r--   0        0        0      113 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
--rw-r--r--   0        0        0      510 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
--rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/__init__.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/__init__.py
--rw-r--r--   0        0        0      259 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/__init__.py
--rw-r--r--   0        0        0      370 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/__init__.py
--rw-r--r--   0        0        0     1682 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py
--rw-r--r--   0        0        0       88 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_id.py
--rw-r--r--   0        0        0     2035 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py
--rw-r--r--   0        0        0     2055 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py
--rw-r--r--   0        0        0      135 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/payers/__init__.py
--rw-r--r--   0        0        0     4709 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/payers/client.py
--rw-r--r--   0        0        0      158 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/payers/types/__init__.py
--rw-r--r--   0        0        0     1043 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/payers/types/payer.py
--rw-r--r--   0        0        0      865 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/payers/types/payer_page.py
--rw-r--r--   0        0        0      251 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/__init__.py
--rw-r--r--   0        0        0      348 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/types/__init__.py
--rw-r--r--   0        0        0      975 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/types/encounter_service_facility.py
--rw-r--r--   0        0        0     1574 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py
--rw-r--r--   0        0        0      108 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/types/service_facility_id.py
--rw-r--r--   0        0        0      671 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/__init__.py
--rw-r--r--   0        0        0      978 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/__init__.py
--rw-r--r--   0        0        0     6559 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/denial_reason_content.py
--rw-r--r--   0        0        0     1104 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/drug_identification.py
--rw-r--r--   0        0        0      996 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/measurement_unit_code.py
--rw-r--r--   0        0        0     1659 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_id_qualifier.py
--rw-r--r--   0        0        0     1144 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line.py
--rw-r--r--   0        0        0      960 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_adjustment.py
--rw-r--r--   0        0        0      866 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_base.py
--rw-r--r--   0        0        0     1899 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
--rw-r--r--   0        0        0     1618 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_create.py
--rw-r--r--   0        0        0     1099 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_denial_reason.py
--rw-r--r--   0        0        0      917 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_era_data.py
--rw-r--r--   0        0        0      177 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/__init__.py
--rw-r--r--   0        0        0      244 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/__init__.py
--rw-r--r--   0        0        0      799 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/tag.py
--rw-r--r--   0        0        0     1527 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/tag_color_enum.py
--rw-r--r--   0        0        0      861 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/tag_create.py
--rw-r--r--   0        0        0       77 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/tag_id.py
--rw-r--r--   0        0        0      113 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tasks/__init__.py
--rw-r--r--   0        0        0      115 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tasks/types/__init__.py
--rw-r--r--   0        0        0       97 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tasks/types/task_id.py
--rw-r--r--   0        0        0      109 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/users/__init__.py
--rw-r--r--   0        0        0      108 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/users/types/__init__.py
--rw-r--r--   0        0        0      916 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/users/types/user.py
--rw-r--r--   0        0        0      111 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/__init__.py
--rw-r--r--   0        0        0      102 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/__init__.py
--rw-r--r--   0        0        0      207 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/__init__.py
--rw-r--r--   0        0        0      281 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0     1052 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
--rw-r--r--   0        0        0      893 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
--rw-r--r--   0        0        0     1242 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 candidhealth-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      257 2023-06-12 17:45:51.368255 candidhealth-0.2.1/README.md
+-rw-r--r--   0        0        0      373 2023-06-12 17:45:51.368255 candidhealth-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5791 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/__init__.py
+-rw-r--r--   0        0        0     3166 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/candid_api_client.py
+-rw-r--r--   0        0        0     2274 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/client.py
+-rw-r--r--   0        0        0      348 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      227 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/environment.py
+-rw-r--r--   0        0        0        0 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/py.typed
+-rw-r--r--   0        0        0     5939 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/client.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/resources/__init__.py
+-rw-r--r--   0        0        0      304 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     3502 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/client.py
+-rw-r--r--   0        0        0      159 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/errors/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      333 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      785 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
+-rw-r--r--   0        0        0      806 2023-06-12 17:45:51.368255 candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
+-rw-r--r--   0        0        0      765 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
+-rw-r--r--   0        0        0      191 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/billing_notes/__init__.py
+-rw-r--r--   0        0        0     2831 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/billing_notes/client.py
+-rw-r--r--   0        0        0      256 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/billing_notes/types/__init__.py
+-rw-r--r--   0        0        0     1136 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/billing_notes/types/billing_note.py
+-rw-r--r--   0        0        0      813 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/billing_notes/types/billing_note_base.py
+-rw-r--r--   0        0        0      104 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/billing_notes/types/billing_note_id.py
+-rw-r--r--   0        0        0      139 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/claims/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/claims/types/__init__.py
+-rw-r--r--   0        0        0     1151 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/claims/types/claim.py
+-rw-r--r--   0        0        0     2605 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/claims/types/claim_status.py
+-rw-r--r--   0        0        0     1417 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/__init__.py
+-rw-r--r--   0        0        0     2104 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0       98 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/claim_id.py
+-rw-r--r--   0        0        0      905 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/contact_info.py
+-rw-r--r--   0        0        0       90 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/content_download_url.py
+-rw-r--r--   0        0        0       76 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/date.py
+-rw-r--r--   0        0        0       77 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/email.py
+-rw-r--r--   0        0        0       91 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/encounter_external_id.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/encounter_id.py
+-rw-r--r--   0        0        0    11148 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/facility_type_code.py
+-rw-r--r--   0        0        0    15447 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/insurance_type_code.py
+-rw-r--r--   0        0        0       79 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/link_url.py
+-rw-r--r--   0        0        0       75 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/npi.py
+-rw-r--r--   0        0        0      105 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/organization_id.py
+-rw-r--r--   0        0        0       81 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/page_token.py
+-rw-r--r--   0        0        0       89 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/patient_external_id.py
+-rw-r--r--   0        0        0     4686 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
+-rw-r--r--   0        0        0      822 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      620 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/phone_number_type.py
+-rw-r--r--   0        0        0    79514 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/procedure_modifier.py
+-rw-r--r--   0        0        0      735 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/region_national.py
+-rw-r--r--   0        0        0      790 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/region_states.py
+-rw-r--r--   0        0        0      633 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/regions.py
+-rw-r--r--   0        0        0      864 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/resource_page.py
+-rw-r--r--   0        0        0      104 2023-06-12 17:45:51.372256 candidhealth-0.2.1/src/candid/resources/commons/types/service_line_id.py
+-rw-r--r--   0        0        0      432 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/commons/types/service_line_units.py
+-rw-r--r--   0        0        0     5065 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/commons/types/source_of_payment_code.py
+-rw-r--r--   0        0        0     6264 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/commons/types/state.py
+-rw-r--r--   0        0        0     1037 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/commons/types/street_address_base.py
+-rw-r--r--   0        0        0      985 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/commons/types/street_address_long_zip.py
+-rw-r--r--   0        0        0     1003 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/commons/types/street_address_short_zip.py
+-rw-r--r--   0        0        0       83 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/commons/types/work_queue_id.py
+-rw-r--r--   0        0        0      251 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/contracts/__init__.py
+-rw-r--r--   0        0        0      365 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/contracts/types/__init__.py
+-rw-r--r--   0        0        0      940 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/contracts/types/authorized_signatory.py
+-rw-r--r--   0        0        0     1430 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/contracts/types/contract.py
+-rw-r--r--   0        0        0     1517 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/contracts/types/contract_base.py
+-rw-r--r--   0        0        0      101 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/contracts/types/contract_id.py
+-rw-r--r--   0        0        0      986 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/contracts/types/contract_status.py
+-rw-r--r--   0        0        0     1125 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/__init__.py
+-rw-r--r--   0        0        0     1472 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/__init__.py
+-rw-r--r--   0        0        0      886 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
+-rw-r--r--   0        0        0      846 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/credentialing_span_dates.py
+-rw-r--r--   0        0        0      977 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/credentialing_span_status.py
+-rw-r--r--   0        0        0      809 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
+-rw-r--r--   0        0        0      864 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
+-rw-r--r--   0        0        0     2210 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/provider_credentialing_span.py
+-rw-r--r--   0        0        0      958 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
+-rw-r--r--   0        0        0      118 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
+-rw-r--r--   0        0        0      827 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/credentialing/types/required_credentialing_dates.py
+-rw-r--r--   0        0        0      279 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/diagnoses/__init__.py
+-rw-r--r--   0        0        0      409 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/diagnoses/types/__init__.py
+-rw-r--r--   0        0        0      958 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/diagnoses/types/diagnosis.py
+-rw-r--r--   0        0        0     1904 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/diagnoses/types/diagnosis_create.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/diagnoses/types/diagnosis_id.py
+-rw-r--r--   0        0        0     1974 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/diagnoses/types/diagnosis_type_code.py
+-rw-r--r--   0        0        0      903 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
+-rw-r--r--   0        0        0      111 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
+-rw-r--r--   0        0        0     1092 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
+-rw-r--r--   0        0        0     1260 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
+-rw-r--r--   0        0        0      101 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
+-rw-r--r--   0        0        0     1244 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
+-rw-r--r--   0        0        0     1244 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
+-rw-r--r--   0        0        0      111 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/client.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/__init__.py
+-rw-r--r--   0        0        0     2694 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/__init__.py
+-rw-r--r--   0        0        0    34265 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/client.py
+-rw-r--r--   0        0        0      202 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/errors/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/errors/encounter_external_id_uniqueness_error.py
+-rw-r--r--   0        0        0     3794 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
+-rw-r--r--   0        0        0     1206 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
+-rw-r--r--   0        0        0      944 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
+-rw-r--r--   0        0        0      874 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
+-rw-r--r--   0        0        0      944 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
+-rw-r--r--   0        0        0      894 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
+-rw-r--r--   0        0        0      659 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
+-rw-r--r--   0        0        0      713 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
+-rw-r--r--   0        0        0     2992 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter.py
+-rw-r--r--   0        0        0      920 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
+-rw-r--r--   0        0        0      388 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
+-rw-r--r--   0        0        0     4498 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
+-rw-r--r--   0        0        0      889 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py
+-rw-r--r--   0        0        0      885 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
+-rw-r--r--   0        0        0     1025 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
+-rw-r--r--   0        0        0      568 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      855 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
+-rw-r--r--   0        0        0      845 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
+-rw-r--r--   0        0        0       88 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
+-rw-r--r--   0        0        0      969 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intake_question.py
+-rw-r--r--   0        0        0       88 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
+-rw-r--r--   0        0        0      891 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
+-rw-r--r--   0        0        0     1303 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intervention.py
+-rw-r--r--   0        0        0      865 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
+-rw-r--r--   0        0        0      855 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/lab.py
+-rw-r--r--   0        0        0      457 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
+-rw-r--r--   0        0        0      834 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
+-rw-r--r--   0        0        0      953 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/medication.py
+-rw-r--r--   0        0        0      880 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/network_status.py
+-rw-r--r--   0        0        0     1164 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
+-rw-r--r--   0        0        0     2615 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/note_category.py
+-rw-r--r--   0        0        0      900 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
+-rw-r--r--   0        0        0     1012 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
+-rw-r--r--   0        0        0      885 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
+-rw-r--r--   0        0        0       96 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
+-rw-r--r--   0        0        0       77 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
+-rw-r--r--   0        0        0      898 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      544 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
+-rw-r--r--   0        0        0      893 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/vitals.py
+-rw-r--r--   0        0        0      143 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/era/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-12 17:45:51.376256 candidhealth-0.2.1/src/candid/resources/era/types/__init__.py
+-rw-r--r--   0        0        0      817 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/era/types/era.py
+-rw-r--r--   0        0        0      811 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/era/types/era_base.py
+-rw-r--r--   0        0        0       96 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/era/types/era_id.py
+-rw-r--r--   0        0        0      207 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/expected_network_status/__init__.py
+-rw-r--r--   0        0        0     5547 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/expected_network_status/client.py
+-rw-r--r--   0        0        0      270 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/expected_network_status/types/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/expected_network_status/types/expected_network_status.py
+-rw-r--r--   0        0        0      981 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/expected_network_status/types/expected_network_status_response.py
+-rw-r--r--   0        0        0      111 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/client.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/resources/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/__init__.py
+-rw-r--r--   0        0        0     8114 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/client.py
+-rw-r--r--   0        0        0      300 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0      867 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/types/guarantor.py
+-rw-r--r--   0        0        0     1020 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py
+-rw-r--r--   0        0        0      804 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/types/guarantor_id.py
+-rw-r--r--   0        0        0      435 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/__init__.py
+-rw-r--r--   0        0        0      871 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/gender.py
+-rw-r--r--   0        0        0      821 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/individual_base.py
+-rw-r--r--   0        0        0      103 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/individual_id.py
+-rw-r--r--   0        0        0      861 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/patient.py
+-rw-r--r--   0        0        0     1614 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/patient_base.py
+-rw-r--r--   0        0        0      794 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/patient_create.py
+-rw-r--r--   0        0        0      972 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/subscriber.py
+-rw-r--r--   0        0        0     1200 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/subscriber_base.py
+-rw-r--r--   0        0        0      925 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/individual/types/subscriber_create.py
+-rw-r--r--   0        0        0      247 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/insurance_card/__init__.py
+-rw-r--r--   0        0        0      352 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/insurance_card/types/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/insurance_card/types/insurance_card.py
+-rw-r--r--   0        0        0     1122 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/insurance_card/types/insurance_card_base.py
+-rw-r--r--   0        0        0     1026 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/insurance_card/types/insurance_card_create.py
+-rw-r--r--   0        0        0      106 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/insurance_card/types/insurance_card_id.py
+-rw-r--r--   0        0        0      199 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/invoices/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/invoices/types/__init__.py
+-rw-r--r--   0        0        0     1397 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/invoices/types/invoice.py
+-rw-r--r--   0        0        0      100 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/invoices/types/invoice_id.py
+-rw-r--r--   0        0        0      849 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/invoices/types/invoice_item.py
+-rw-r--r--   0        0        0      908 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/invoices/types/invoice_status.py
+-rw-r--r--   0        0        0      111 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/__init__.py
+-rw-r--r--   0        0        0      501 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
+-rw-r--r--   0        0        0      492 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
+-rw-r--r--   0        0        0     2857 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
+-rw-r--r--   0        0        0     1562 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
+-rw-r--r--   0        0        0     1062 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
+-rw-r--r--   0        0        0     2853 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
+-rw-r--r--   0        0        0      113 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
+-rw-r--r--   0        0        0      510 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
+-rw-r--r--   0        0        0      111 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/patient_payments/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/patient_payments/resources/__init__.py
+-rw-r--r--   0        0        0      259 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/__init__.py
+-rw-r--r--   0        0        0      370 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/types/__init__.py
+-rw-r--r--   0        0        0     1682 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py
+-rw-r--r--   0        0        0       88 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_id.py
+-rw-r--r--   0        0        0     2035 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py
+-rw-r--r--   0        0        0     2055 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py
+-rw-r--r--   0        0        0      159 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/payers/__init__.py
+-rw-r--r--   0        0        0     4737 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/payers/client.py
+-rw-r--r--   0        0        0      205 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/payers/types/__init__.py
+-rw-r--r--   0        0        0     1048 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/payers/types/payer.py
+-rw-r--r--   0        0        0      865 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/payers/types/payer_page.py
+-rw-r--r--   0        0        0      100 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/payers/types/payer_uuid.py
+-rw-r--r--   0        0        0      251 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_facility/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_facility/types/__init__.py
+-rw-r--r--   0        0        0      975 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_facility/types/encounter_service_facility.py
+-rw-r--r--   0        0        0     1574 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_facility/types/encounter_service_facility_base.py
+-rw-r--r--   0        0        0      108 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_facility/types/service_facility_id.py
+-rw-r--r--   0        0        0      671 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/__init__.py
+-rw-r--r--   0        0        0      978 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/__init__.py
+-rw-r--r--   0        0        0     6559 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/denial_reason_content.py
+-rw-r--r--   0        0        0     1104 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/drug_identification.py
+-rw-r--r--   0        0        0      996 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/measurement_unit_code.py
+-rw-r--r--   0        0        0     1659 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/service_id_qualifier.py
+-rw-r--r--   0        0        0     1144 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line.py
+-rw-r--r--   0        0        0      960 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_adjustment.py
+-rw-r--r--   0        0        0      866 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_base.py
+-rw-r--r--   0        0        0     1899 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
+-rw-r--r--   0        0        0     1618 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_create.py
+-rw-r--r--   0        0        0     1099 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_denial_reason.py
+-rw-r--r--   0        0        0      917 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_era_data.py
+-rw-r--r--   0        0        0      177 2023-06-12 17:45:51.380256 candidhealth-0.2.1/src/candid/resources/tags/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/tags/types/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/tags/types/tag.py
+-rw-r--r--   0        0        0     1527 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/tags/types/tag_color_enum.py
+-rw-r--r--   0        0        0      861 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/tags/types/tag_create.py
+-rw-r--r--   0        0        0       77 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/tags/types/tag_id.py
+-rw-r--r--   0        0        0      113 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/tasks/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/tasks/types/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/tasks/types/task_id.py
+-rw-r--r--   0        0        0      111 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/__init__.py
+-rw-r--r--   0        0        0      869 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     1069 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      840 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/auth_zero_metadata.py
+-rw-r--r--   0        0        0      766 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/google_apps_metadata.py
+-rw-r--r--   0        0        0      780 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/human_user_metadata.py
+-rw-r--r--   0        0        0     1057 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/idp_user_metadata.py
+-rw-r--r--   0        0        0      757 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/machine_user_metadata.py
+-rw-r--r--   0        0        0      765 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/other_idp_metadata.py
+-rw-r--r--   0        0        0       97 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/user_id.py
+-rw-r--r--   0        0        0      760 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/user_metadata.py
+-rw-r--r--   0        0        0     1111 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/user_v_2.py
+-rw-r--r--   0        0        0      111 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/work_queues/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/work_queues/resources/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/work_queues/resources/v_1/__init__.py
+-rw-r--r--   0        0        0      281 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/work_queues/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1074 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
+-rw-r--r--   0        0        0      893 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
+-rw-r--r--   0        0        0     1242 2023-06-12 17:45:51.384256 candidhealth-0.2.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 candidhealth-0.2.1/PKG-INFO
```

### Comparing `candidhealth-0.2.0/src/candid/__init__.py` & `candidhealth-0.2.1/src/candid/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .environment import CandidApiEnvironment
 from .resources import (
-    Auth0Id,
     AuthorizedSignatory,
     BillingNote,
     BillingNoteBase,
     BillingNoteId,
     Claim,
     ClaimId,
     ClaimStatus,
@@ -63,14 +62,15 @@
     Patient,
     PatientBase,
     PatientCreate,
     PatientExternalId,
     PatientRelationshipToInsuredCodeAll,
     Payer,
     PayerPage,
+    PayerUuid,
     PhoneNumber,
     PhoneNumberType,
     ProcedureModifier,
     ProviderCredentialingSpan,
     ProviderCredentialingSpanBase,
     ProviderCredentialingSpanId,
     RegionNational,
@@ -101,15 +101,14 @@
     SubscriberBase,
     SubscriberCreate,
     Tag,
     TagColorEnum,
     TagCreate,
     TagId,
     TaskId,
-    User,
     WorkQueueId,
     auth,
     billing_notes,
     claims,
     commons,
     contracts,
     credentialing,
@@ -130,15 +129,14 @@
     tags,
     tasks,
     users,
     work_queues,
 )
 
 __all__ = [
-    "Auth0Id",
     "AuthorizedSignatory",
     "BillingNote",
     "BillingNoteBase",
     "BillingNoteId",
     "CandidApiEnvironment",
     "Claim",
     "ClaimId",
@@ -196,14 +194,15 @@
     "Patient",
     "PatientBase",
     "PatientCreate",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
     "Payer",
     "PayerPage",
+    "PayerUuid",
     "PhoneNumber",
     "PhoneNumberType",
     "ProcedureModifier",
     "ProviderCredentialingSpan",
     "ProviderCredentialingSpanBase",
     "ProviderCredentialingSpanId",
     "RegionNational",
@@ -234,15 +233,14 @@
     "SubscriberBase",
     "SubscriberCreate",
     "Tag",
     "TagColorEnum",
     "TagCreate",
     "TagId",
     "TaskId",
-    "User",
     "WorkQueueId",
     "auth",
     "billing_notes",
     "claims",
     "commons",
     "contracts",
     "credentialing",
```

### Comparing `candidhealth-0.2.0/src/candid/candid_api_client.py` & `candidhealth-0.2.1/src/candid/candid_api_client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/client.py` & `candidhealth-0.2.1/src/candid/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/core/datetime_utils.py` & `candidhealth-0.2.1/src/candid/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/core/jsonable_encoder.py` & `candidhealth-0.2.1/src/candid/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/__init__.py` & `candidhealth-0.2.1/src/candid/resources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     tasks,
     users,
     work_queues,
 )
 from .billing_notes import BillingNote, BillingNoteBase, BillingNoteId
 from .claims import Claim, ClaimStatus
 from .commons import (
-    Auth0Id,
     ClaimId,
     ContactInfo,
     ContentDownloadUrl,
     Date,
     Email,
     EncounterExternalId,
     EncounterId,
@@ -91,15 +90,15 @@
     PatientCreate,
     Subscriber,
     SubscriberBase,
     SubscriberCreate,
 )
 from .insurance_card import InsuranceCard, InsuranceCardBase, InsuranceCardCreate, InsuranceCardId
 from .invoices import Invoice, InvoiceId, InvoiceItem, InvoiceStatus
-from .payers import Payer, PayerPage
+from .payers import Payer, PayerPage, PayerUuid
 from .service_facility import EncounterServiceFacility, EncounterServiceFacilityBase, ServiceFacilityId
 from .service_lines import (
     DenialReasonContent,
     DrugIdentification,
     MeasurementUnitCode,
     ServiceIdQualifier,
     ServiceLine,
@@ -108,18 +107,16 @@
     ServiceLineBaseWithOptionals,
     ServiceLineCreate,
     ServiceLineDenialReason,
     ServiceLineEraData,
 )
 from .tags import Tag, TagColorEnum, TagCreate, TagId
 from .tasks import TaskId
-from .users import User
 
 __all__ = [
-    "Auth0Id",
     "AuthorizedSignatory",
     "BillingNote",
     "BillingNoteBase",
     "BillingNoteId",
     "Claim",
     "ClaimId",
     "ClaimStatus",
@@ -176,14 +173,15 @@
     "Patient",
     "PatientBase",
     "PatientCreate",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
     "Payer",
     "PayerPage",
+    "PayerUuid",
     "PhoneNumber",
     "PhoneNumberType",
     "ProcedureModifier",
     "ProviderCredentialingSpan",
     "ProviderCredentialingSpanBase",
     "ProviderCredentialingSpanId",
     "RegionNational",
@@ -214,15 +212,14 @@
     "SubscriberBase",
     "SubscriberCreate",
     "Tag",
     "TagColorEnum",
     "TagCreate",
     "TagId",
     "TaskId",
-    "User",
     "WorkQueueId",
     "auth",
     "billing_notes",
     "claims",
     "commons",
     "contracts",
     "credentialing",
```

### Comparing `candidhealth-0.2.0/src/candid/resources/auth/client.py` & `candidhealth-0.2.1/src/candid/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/client.py` & `candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py` & `candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py` & `candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py` & `candidhealth-0.2.1/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/billing_notes/client.py` & `candidhealth-0.2.1/src/candid/resources/billing_notes/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note.py` & `candidhealth-0.2.1/src/candid/resources/billing_notes/types/billing_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note_base.py` & `candidhealth-0.2.1/src/candid/resources/billing_notes/types/billing_note_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/claims/types/claim.py` & `candidhealth-0.2.1/src/candid/resources/claims/types/claim.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/claims/types/claim_status.py` & `candidhealth-0.2.1/src/candid/resources/claims/types/claim_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/__init__.py` & `candidhealth-0.2.1/src/candid/resources/commons/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
-    Auth0Id,
     ClaimId,
     ContactInfo,
     ContentDownloadUrl,
     Date,
     Email,
     EncounterExternalId,
     EncounterId,
@@ -33,15 +32,14 @@
     StreetAddressBase,
     StreetAddressLongZip,
     StreetAddressShortZip,
     WorkQueueId,
 )
 
 __all__ = [
-    "Auth0Id",
     "ClaimId",
     "ContactInfo",
     "ContentDownloadUrl",
     "Date",
     "Email",
     "EncounterExternalId",
     "EncounterId",
```

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/__init__.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .auth_0_id import Auth0Id
 from .claim_id import ClaimId
 from .contact_info import ContactInfo
 from .content_download_url import ContentDownloadUrl
 from .date import Date
 from .email import Email
 from .encounter_external_id import EncounterExternalId
 from .encounter_id import EncounterId
@@ -29,15 +28,14 @@
 from .state import State
 from .street_address_base import StreetAddressBase
 from .street_address_long_zip import StreetAddressLongZip
 from .street_address_short_zip import StreetAddressShortZip
 from .work_queue_id import WorkQueueId
 
 __all__ = [
-    "Auth0Id",
     "ClaimId",
     "ContactInfo",
     "ContentDownloadUrl",
     "Date",
     "Email",
     "EncounterExternalId",
     "EncounterId",
```

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/contact_info.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/contact_info.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/facility_type_code.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/facility_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/insurance_type_code.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/insurance_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/phone_number.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/phone_number_type.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/phone_number_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/procedure_modifier.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/procedure_modifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/region_national.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/region_national.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/region_states.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/region_states.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/regions.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/regions.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/resource_page.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/resource_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/source_of_payment_code.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/source_of_payment_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/state.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/state.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/street_address_base.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/street_address_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/street_address_long_zip.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/street_address_long_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/commons/types/street_address_short_zip.py` & `candidhealth-0.2.1/src/candid/resources/commons/types/street_address_short_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/contracts/types/authorized_signatory.py` & `candidhealth-0.2.1/src/candid/resources/contracts/types/authorized_signatory.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/contracts/types/contract.py` & `candidhealth-0.2.1/src/candid/resources/contracts/types/contract.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/contracts/types/contract_base.py` & `candidhealth-0.2.1/src/candid/resources/contracts/types/contract_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/contracts/types/contract_status.py` & `candidhealth-0.2.1/src/candid/resources/contracts/types/contract_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/__init__.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/__init__.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialing_span_dates.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/credentialing_span_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialing_span_status.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/credentialing_span_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/non_required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/provider_credentialing_span.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/provider_credentialing_span_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/credentialing/types/required_credentialing_dates.py` & `candidhealth-0.2.1/src/candid/resources/credentialing/types/required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis.py` & `candidhealth-0.2.1/src/candid/resources/diagnoses/types/diagnosis.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_create.py` & `candidhealth-0.2.1/src/candid/resources/diagnoses/types/diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py` & `candidhealth-0.2.1/src/candid/resources/diagnoses/types/diagnosis_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py` & `candidhealth-0.2.1/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py` & `candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py` & `candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py` & `candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py` & `candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py` & `candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py` & `candidhealth-0.2.1/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/client.py` & `candidhealth-0.2.1/src/candid/resources/encounters/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/__init__.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/client.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/__init__.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/base_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/clinical_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         description=(
             "Whether you have accepted the patient's authorization for insurance payments\n"
             "to be made to you, not them.\n"
             "Box 27 on the CMS-1500 claim form.\n"
         )
     )
     appointment_type: typing.Optional[str] = pydantic.Field(
-        description=('Human-readable description of the appointment time (ex: "Acupuncture - Headaches")\n')
+        description=('Human-readable description of the appointment type (ex: "Acupuncture - Headaches")\n')
     )
     do_not_bill: typing.Optional[bool] = pydantic.Field(
         description=(
             "Should be set to true if Candid should not create or submit a claim but you'd\n"
             "like us to track this encounter anyway (ex: patient is paying cash)\n"
         )
     )
```

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intake_question.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intervention.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intervention.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/intervention_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/lab.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/lab.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/medication.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/medication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/network_status.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/note_category.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/vitals.py` & `candidhealth-0.2.1/src/candid/resources/encounters/resources/v_4/types/vitals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/era/types/era.py` & `candidhealth-0.2.1/src/candid/resources/era/types/era.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/era/types/era_base.py` & `candidhealth-0.2.1/src/candid/resources/era/types/era_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/expected_network_status/client.py` & `candidhealth-0.2.1/src/candid/resources/expected_network_status/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/expected_network_status/types/expected_network_status.py` & `candidhealth-0.2.1/src/candid/resources/expected_network_status/types/expected_network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py` & `candidhealth-0.2.1/src/candid/resources/expected_network_status/types/expected_network_status_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/guarantor/client.py` & `candidhealth-0.2.1/src/candid/resources/guarantor/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/client.py` & `candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py` & `candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/types/guarantor.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py` & `candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py` & `candidhealth-0.2.1/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/__init__.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/gender.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/gender.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/individual_base.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/individual_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/patient.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/patient.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/patient_base.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/patient_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/patient_create.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/patient_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/subscriber.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/subscriber.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/subscriber_base.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/individual/types/subscriber_create.py` & `candidhealth-0.2.1/src/candid/resources/individual/types/subscriber_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card.py` & `candidhealth-0.2.1/src/candid/resources/insurance_card/types/insurance_card.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_base.py` & `candidhealth-0.2.1/src/candid/resources/insurance_card/types/insurance_card_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_create.py` & `candidhealth-0.2.1/src/candid/resources/insurance_card/types/insurance_card_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/invoices/types/invoice.py` & `candidhealth-0.2.1/src/candid/resources/invoices/types/invoice.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_item.py` & `candidhealth-0.2.1/src/candid/resources/invoices/types/invoice_item.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_status.py` & `candidhealth-0.2.1/src/candid/resources/invoices/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py` & `candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py` & `candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/license_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py` & `candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py` & `candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py` & `candidhealth-0.2.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py` & `candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py` & `candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py` & `candidhealth-0.2.1/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/payers/client.py` & `candidhealth-0.2.1/src/candid/resources/payers/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
-import uuid
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import CandidApiEnvironment
 from ..commons.types.page_token import PageToken
 from .types.payer import Payer
 from .types.payer_page import PayerPage
+from .types.payer_uuid import PayerUuid
 
 
 class PayersClient:
     def __init__(
         self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def get(self, payer_uuid: uuid.UUID) -> Payer:
+    def get(self, payer_uuid: PayerUuid) -> Payer:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/payers/v3/{payer_uuid}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
@@ -68,15 +68,15 @@
 class AsyncPayersClient:
     def __init__(
         self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def get(self, payer_uuid: uuid.UUID) -> Payer:
+    async def get(self, payer_uuid: PayerUuid) -> Payer:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/payers/v3/{payer_uuid}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
```

### Comparing `candidhealth-0.2.0/src/candid/resources/payers/types/payer.py` & `candidhealth-0.2.1/src/candid/resources/payers/types/payer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
-import uuid
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .payer_uuid import PayerUuid
 
 
 class Payer(pydantic.BaseModel):
-    payer_uuid: typing.Optional[uuid.UUID] = pydantic.Field(description=("Auto-generated ID set on creation\n"))
+    payer_uuid: PayerUuid = pydantic.Field(description=("Auto-generated ID set on creation\n"))
     payer_id: str = pydantic.Field(description=("The primary national payer ID of the payer\n"))
     payer_name: str = pydantic.Field(description=("The primary display name of the payer\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `candidhealth-0.2.0/src/candid/resources/payers/types/payer_page.py` & `candidhealth-0.2.1/src/candid/resources/payers/types/payer_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_facility/types/encounter_service_facility.py` & `candidhealth-0.2.1/src/candid/resources/service_facility/types/encounter_service_facility.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py` & `candidhealth-0.2.1/src/candid/resources/service_facility/types/encounter_service_facility_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/__init__.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/__init__.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/denial_reason_content.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/denial_reason_content.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/drug_identification.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/drug_identification.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/measurement_unit_code.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/measurement_unit_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_id_qualifier.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/service_id_qualifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_adjustment.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_adjustment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_base.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_base_with_optionals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_create.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_denial_reason.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_denial_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_era_data.py` & `candidhealth-0.2.1/src/candid/resources/service_lines/types/service_line_era_data.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/tags/types/tag.py` & `candidhealth-0.2.1/src/candid/resources/tags/types/tag.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/tags/types/tag_color_enum.py` & `candidhealth-0.2.1/src/candid/resources/tags/types/tag_color_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/tags/types/tag_create.py` & `candidhealth-0.2.1/src/candid/resources/tags/types/tag_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/src/candid/resources/users/types/user.py` & `candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/auth_zero_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.auth_0_id import Auth0Id
+from ......core.datetime_utils import serialize_datetime
 
 
-class User(pydantic.BaseModel):
-    auth_0_id: Auth0Id = pydantic.Field(alias="auth0_id")
-    first_name: str
-    last_name: str
+class AuthZeroMetadata(pydantic.BaseModel):
+    auth_0_id: str = pydantic.Field(alias="auth0_id")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py` & `candidhealth-0.2.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,26 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .....commons.types.work_queue_id import WorkQueueId
-from .....users.types.user import User
-from .work_queue_category import WorkQueueCategory
+from .work_queue_category_type import WorkQueueCategoryType
 
 
-class WorkQueue(pydantic.BaseModel):
-    work_queue_id: WorkQueueId
+class WorkQueueCategory(pydantic.BaseModel):
+    type: WorkQueueCategoryType
     display_name: str
     description: typing.Optional[str]
-    category: WorkQueueCategory
-    created_at: dt.datetime
-    created_by: User
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py` & `candidhealth-0.2.1/src/candid/resources/users/resources/v_2/types/machine_user_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .work_queue_category_type import WorkQueueCategoryType
 
 
-class WorkQueueCategory(pydantic.BaseModel):
-    type: WorkQueueCategoryType
-    display_name: str
-    description: typing.Optional[str]
+class MachineUserMetadata(pydantic.BaseModel):
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py` & `candidhealth-0.2.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.2.0/PKG-INFO` & `candidhealth-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candidhealth
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

