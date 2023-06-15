# Comparing `tmp/fern_moneykit-0.0.4.tar.gz` & `tmp/fern_moneykit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_moneykit-0.0.4.tar", max compression
+gzip compressed data, was "fern_moneykit-0.0.5.tar", max compression
```

## Comparing `fern_moneykit-0.0.4.tar` & `fern_moneykit-0.0.5.tar`

### file list

```diff
@@ -1,117 +1,118 @@
--rw-r--r--   0        0        0     1294 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/README.md
--rw-r--r--   0        0        0      376 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4947 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/__init__.py
--rw-r--r--   0        0        0     3782 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/client.py
--rw-r--r--   0        0        0      348 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      538 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/errors/forbidden_error.py
--rw-r--r--   0        0        0      246 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/errors/not_found_error.py
--rw-r--r--   0        0        0      354 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      250 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/errors/unauthorized_error.py
--rw-r--r--   0        0        0      333 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/py.typed
--rw-r--r--   0        0        0      292 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/resources/access_token/__init__.py
--rw-r--r--   0        0        0     7944 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/resources/access_token/client.py
--rw-r--r--   0        0        0       65 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/resources/accounts/__init__.py
--rw-r--r--   0        0        0    15357 2023-06-15 23:37:48.666844 fern_moneykit-0.0.4/src/moneykit/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/identity/__init__.py
--rw-r--r--   0        0        0     5196 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/identity/client.py
--rw-r--r--   0        0        0       65 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/institutions/__init__.py
--rw-r--r--   0        0        0     7301 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/institutions/client.py
--rw-r--r--   0        0        0       65 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/link_session/__init__.py
--rw-r--r--   0        0        0     8866 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/link_session/client.py
--rw-r--r--   0        0        0       65 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/links/__init__.py
--rw-r--r--   0        0        0    14788 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/links/client.py
--rw-r--r--   0        0        0       65 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/products/__init__.py
--rw-r--r--   0        0        0     4987 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/products/client.py
--rw-r--r--   0        0        0       65 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/transactions/__init__.py
--rw-r--r--   0        0        0    14247 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/resources/transactions/client.py
--rw-r--r--   0        0        0     6819 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/__init__.py
--rw-r--r--   0        0        0     2708 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account.py
--rw-r--r--   0        0        0     2223 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account_balances.py
--rw-r--r--   0        0        0      964 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account_group.py
--rw-r--r--   0        0        0     2854 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account_identity.py
--rw-r--r--   0        0        0     1327 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account_numbers.py
--rw-r--r--   0        0        0     1204 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account_numbers_link_product.py
--rw-r--r--   0        0        0     1187 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account_numbers_product_settings.py
--rw-r--r--   0        0        0     2154 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account_type.py
--rw-r--r--   0        0        0     2872 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/account_with_account_numbers.py
--rw-r--r--   0        0        0     1078 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/accounts_link_product.py
--rw-r--r--   0        0        0      996 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/ach_number.py
--rw-r--r--   0        0        0     1380 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/address.py
--rw-r--r--   0        0        0     1015 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/api_error_auth_expired_access_token_response.py
--rw-r--r--   0        0        0      984 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/api_error_auth_unauthorized_response.py
--rw-r--r--   0        0        0     1004 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/api_error_rate_limit_exceeded_response.py
--rw-r--r--   0        0        0      880 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/bacs_number.py
--rw-r--r--   0        0        0     1328 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/basic_account_details.py
--rw-r--r--   0        0        0     1432 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/body_generate_access_token_auth_token_post.py
--rw-r--r--   0        0        0      560 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/country.py
--rw-r--r--   0        0        0      855 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/create_link_session_response.py
--rw-r--r--   0        0        0    21806 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/currency.py
--rw-r--r--   0        0        0      851 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/cursor_pagination.py
--rw-r--r--   0        0        0      934 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/customer_app.py
--rw-r--r--   0        0        0      975 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/eft_number.py
--rw-r--r--   0        0        0      973 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/email.py
--rw-r--r--   0        0        0      953 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/exchange_token_response.py
--rw-r--r--   0        0        0     1058 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/generate_access_token_response.py
--rw-r--r--   0        0        0      923 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/get_account_numbers_response.py
--rw-r--r--   0        0        0      923 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/get_account_response.py
--rw-r--r--   0        0        0      994 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/get_accounts_response.py
--rw-r--r--   0        0        0     1037 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/get_institutions_response.py
--rw-r--r--   0        0        0     1480 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/get_transactions_response.py
--rw-r--r--   0        0        0     1000 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/get_user_accounts_response.py
--rw-r--r--   0        0        0      956 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/get_user_links_response.py
--rw-r--r--   0        0        0     1222 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/get_user_transactions_response.py
--rw-r--r--   0        0        0     1094 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/http_validation_error.py
--rw-r--r--   0        0        0     1179 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/identity_link_product.py
--rw-r--r--   0        0        0     1181 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/identity_product_settings.py
--rw-r--r--   0        0        0      977 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/identity_response.py
--rw-r--r--   0        0        0     1950 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/institution.py
--rw-r--r--   0        0        0      951 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/institution_error_not_found_response.py
--rw-r--r--   0        0        0      857 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/international_number.py
--rw-r--r--   0        0        0     1358 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/introspect_client_response.py
--rw-r--r--   0        0        0      877 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/jwk_set.py
--rw-r--r--   0        0        0     2109 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_common.py
--rw-r--r--   0        0        0      978 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_error_bad_state_response.py
--rw-r--r--   0        0        0      978 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_error_deleted_response.py
--rw-r--r--   0        0        0      984 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_error_forbidden_action_response.py
--rw-r--r--   0        0        0      937 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_error_not_found_response.py
--rw-r--r--   0        0        0      957 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_error_unauthorized_access_response.py
--rw-r--r--   0        0        0      985 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_permission_scope.py
--rw-r--r--   0        0        0      850 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_permissions.py
--rw-r--r--   0        0        0     1198 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_products.py
--rw-r--r--   0        0        0     2544 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_response.py
--rw-r--r--   0        0        0     1784 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_session_customer_user.py
--rw-r--r--   0        0        0     1364 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_session_customer_user_email.py
--rw-r--r--   0        0        0     1744 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_session_customer_user_phone.py
--rw-r--r--   0        0        0      999 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_session_error_forbidden_config_response.py
--rw-r--r--   0        0        0     1002 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_session_error_invalid_token_exchange.py
--rw-r--r--   0        0        0     1972 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_session_setting_overrides.py
--rw-r--r--   0        0        0     1262 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/link_state_changed_webhook.py
--rw-r--r--   0        0        0     1104 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/money_link_features.py
--rw-r--r--   0        0        0     1347 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/owner.py
--rw-r--r--   0        0        0     1103 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/phone_number.py
--rw-r--r--   0        0        0      792 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/phone_number_type.py
--rw-r--r--   0        0        0      895 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/product.py
--rw-r--r--   0        0        0     1132 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/products_settings.py
--rw-r--r--   0        0        0      910 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/provider.py
--rw-r--r--   0        0        0     1292 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/public_link_error.py
--rw-r--r--   0        0        0     1077 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/public_link_state.py
--rw-r--r--   0        0        0     1689 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/requested_link_permission.py
--rw-r--r--   0        0        0       88 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/supported_version.py
--rw-r--r--   0        0        0     3097 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/transaction.py
--rw-r--r--   0        0        0     1298 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/transaction_diff.py
--rw-r--r--   0        0        0     1499 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/transaction_sync_response.py
--rw-r--r--   0        0        0      501 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/transaction_type.py
--rw-r--r--   0        0        0      519 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/transaction_type_filter.py
--rw-r--r--   0        0        0     1195 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/transactions_link_product.py
--rw-r--r--   0        0        0     1525 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/transactions_product_settings.py
--rw-r--r--   0        0        0      893 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/validation_error.py
--rw-r--r--   0        0        0      133 2023-06-15 23:37:48.670844 fern_moneykit-0.0.4/src/moneykit/types/validation_error_location_item.py
--rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 fern_moneykit-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1593 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/README.md
+-rw-r--r--   0        0        0      376 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5027 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/__init__.py
+-rw-r--r--   0        0        0     4045 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/base_client.py
+-rw-r--r--   0        0        0      348 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      217 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/environment.py
+-rw-r--r--   0        0        0      538 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/errors/forbidden_error.py
+-rw-r--r--   0        0        0      246 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/errors/not_found_error.py
+-rw-r--r--   0        0        0      354 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      250 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      333 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/py.typed
+-rw-r--r--   0        0        0      292 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/access_token/__init__.py
+-rw-r--r--   0        0        0     8239 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/access_token/client.py
+-rw-r--r--   0        0        0       65 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    15664 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/identity/__init__.py
+-rw-r--r--   0        0        0     5467 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/identity/client.py
+-rw-r--r--   0        0        0       65 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/institutions/__init__.py
+-rw-r--r--   0        0        0     7584 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/institutions/client.py
+-rw-r--r--   0        0        0       65 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/link_session/__init__.py
+-rw-r--r--   0        0        0     9149 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/link_session/client.py
+-rw-r--r--   0        0        0       65 2023-06-15 23:57:10.634540 fern_moneykit-0.0.5/src/moneykit/resources/links/__init__.py
+-rw-r--r--   0        0        0    15095 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/resources/links/client.py
+-rw-r--r--   0        0        0       65 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/resources/products/__init__.py
+-rw-r--r--   0        0        0     5258 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/resources/products/client.py
+-rw-r--r--   0        0        0       65 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    14542 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/resources/transactions/client.py
+-rw-r--r--   0        0        0     6819 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/__init__.py
+-rw-r--r--   0        0        0     2708 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account.py
+-rw-r--r--   0        0        0     2223 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account_balances.py
+-rw-r--r--   0        0        0      964 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account_group.py
+-rw-r--r--   0        0        0     2854 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account_identity.py
+-rw-r--r--   0        0        0     1327 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account_numbers.py
+-rw-r--r--   0        0        0     1204 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account_numbers_link_product.py
+-rw-r--r--   0        0        0     1187 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account_numbers_product_settings.py
+-rw-r--r--   0        0        0     2154 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account_type.py
+-rw-r--r--   0        0        0     2872 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/account_with_account_numbers.py
+-rw-r--r--   0        0        0     1078 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/accounts_link_product.py
+-rw-r--r--   0        0        0      996 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/ach_number.py
+-rw-r--r--   0        0        0     1380 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/address.py
+-rw-r--r--   0        0        0     1015 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/api_error_auth_expired_access_token_response.py
+-rw-r--r--   0        0        0      984 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/api_error_auth_unauthorized_response.py
+-rw-r--r--   0        0        0     1004 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/api_error_rate_limit_exceeded_response.py
+-rw-r--r--   0        0        0      880 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/bacs_number.py
+-rw-r--r--   0        0        0     1328 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/basic_account_details.py
+-rw-r--r--   0        0        0     1432 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/body_generate_access_token_auth_token_post.py
+-rw-r--r--   0        0        0      560 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/country.py
+-rw-r--r--   0        0        0      855 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/create_link_session_response.py
+-rw-r--r--   0        0        0    21806 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/currency.py
+-rw-r--r--   0        0        0      851 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/cursor_pagination.py
+-rw-r--r--   0        0        0      934 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/customer_app.py
+-rw-r--r--   0        0        0      975 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/eft_number.py
+-rw-r--r--   0        0        0      973 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/email.py
+-rw-r--r--   0        0        0      953 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/exchange_token_response.py
+-rw-r--r--   0        0        0     1058 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/generate_access_token_response.py
+-rw-r--r--   0        0        0      923 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/get_account_numbers_response.py
+-rw-r--r--   0        0        0      923 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/get_account_response.py
+-rw-r--r--   0        0        0      994 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/get_accounts_response.py
+-rw-r--r--   0        0        0     1037 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/get_institutions_response.py
+-rw-r--r--   0        0        0     1480 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/get_transactions_response.py
+-rw-r--r--   0        0        0     1000 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/get_user_accounts_response.py
+-rw-r--r--   0        0        0      956 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/get_user_links_response.py
+-rw-r--r--   0        0        0     1222 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/get_user_transactions_response.py
+-rw-r--r--   0        0        0     1094 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/http_validation_error.py
+-rw-r--r--   0        0        0     1179 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/identity_link_product.py
+-rw-r--r--   0        0        0     1181 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/identity_product_settings.py
+-rw-r--r--   0        0        0      977 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/identity_response.py
+-rw-r--r--   0        0        0     1950 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/institution.py
+-rw-r--r--   0        0        0      951 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/institution_error_not_found_response.py
+-rw-r--r--   0        0        0      857 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/international_number.py
+-rw-r--r--   0        0        0     1358 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/introspect_client_response.py
+-rw-r--r--   0        0        0      877 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/jwk_set.py
+-rw-r--r--   0        0        0     2109 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_common.py
+-rw-r--r--   0        0        0      978 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_error_bad_state_response.py
+-rw-r--r--   0        0        0      978 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_error_deleted_response.py
+-rw-r--r--   0        0        0      984 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_error_forbidden_action_response.py
+-rw-r--r--   0        0        0      937 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_error_not_found_response.py
+-rw-r--r--   0        0        0      957 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_error_unauthorized_access_response.py
+-rw-r--r--   0        0        0      985 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_permission_scope.py
+-rw-r--r--   0        0        0      850 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_permissions.py
+-rw-r--r--   0        0        0     1198 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_products.py
+-rw-r--r--   0        0        0     2544 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_response.py
+-rw-r--r--   0        0        0     1784 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_session_customer_user.py
+-rw-r--r--   0        0        0     1364 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_session_customer_user_email.py
+-rw-r--r--   0        0        0     1744 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_session_customer_user_phone.py
+-rw-r--r--   0        0        0      999 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_session_error_forbidden_config_response.py
+-rw-r--r--   0        0        0     1002 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_session_error_invalid_token_exchange.py
+-rw-r--r--   0        0        0     1972 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_session_setting_overrides.py
+-rw-r--r--   0        0        0     1262 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/link_state_changed_webhook.py
+-rw-r--r--   0        0        0     1104 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/money_link_features.py
+-rw-r--r--   0        0        0     1347 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/owner.py
+-rw-r--r--   0        0        0     1103 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/phone_number.py
+-rw-r--r--   0        0        0      792 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/phone_number_type.py
+-rw-r--r--   0        0        0      895 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/product.py
+-rw-r--r--   0        0        0     1132 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/products_settings.py
+-rw-r--r--   0        0        0      910 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/provider.py
+-rw-r--r--   0        0        0     1292 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/public_link_error.py
+-rw-r--r--   0        0        0     1077 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/public_link_state.py
+-rw-r--r--   0        0        0     1689 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/requested_link_permission.py
+-rw-r--r--   0        0        0       88 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/supported_version.py
+-rw-r--r--   0        0        0     3097 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/transaction.py
+-rw-r--r--   0        0        0     1298 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/transaction_diff.py
+-rw-r--r--   0        0        0     1499 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/transaction_sync_response.py
+-rw-r--r--   0        0        0      501 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/transaction_type.py
+-rw-r--r--   0        0        0      519 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/transaction_type_filter.py
+-rw-r--r--   0        0        0     1195 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/transactions_link_product.py
+-rw-r--r--   0        0        0     1525 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/transactions_product_settings.py
+-rw-r--r--   0        0        0      893 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/validation_error.py
+-rw-r--r--   0        0        0      133 2023-06-15 23:57:10.638540 fern_moneykit-0.0.5/src/moneykit/types/validation_error_location_item.py
+-rw-r--r--   0        0        0     2103 1970-01-01 00:00:00.000000 fern_moneykit-0.0.5/PKG-INFO
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/__init__.py` & `fern_moneykit-0.0.5/src/moneykit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .environment import BaseMoneyKitEnvironment
 from .errors import (
     BadRequestError,
     ForbiddenError,
     NotFoundError,
     TooManyRequestsError,
     UnauthorizedError,
     UnprocessableEntityError,
@@ -107,14 +108,15 @@
     "AchNumber",
     "Address",
     "ApiErrorAuthExpiredAccessTokenResponse",
     "ApiErrorAuthUnauthorizedResponse",
     "ApiErrorRateLimitExceededResponse",
     "BacsNumber",
     "BadRequestError",
+    "BaseMoneyKitEnvironment",
     "BasicAccountDetails",
     "BodyGenerateAccessTokenAuthTokenPost",
     "Country",
     "CreateLinkSessionResponse",
     "Currency",
     "CursorPagination",
     "CustomerApp",
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/client.py` & `fern_moneykit-0.0.5/src/moneykit/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
+from .environment import BaseMoneyKitEnvironment
 from .resources.access_token.client import AccessTokenClient, AsyncAccessTokenClient
 from .resources.accounts.client import AccountsClient, AsyncAccountsClient
 from .resources.identity.client import AsyncIdentityClient, IdentityClient
 from .resources.institutions.client import AsyncInstitutionsClient, InstitutionsClient
 from .resources.link_session.client import AsyncLinkSessionClient, LinkSessionClient
 from .resources.links.client import AsyncLinksClient, LinksClient
 from .resources.products.client import AsyncProductsClient, ProductsClient
 from .resources.transactions.client import AsyncTransactionsClient, TransactionsClient
 from .types.supported_version import SupportedVersion
 
 
-class MoneyKit:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+class BaseMoneyKit:
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
         self.accounts = AccountsClient(
             environment=self._environment, moneykit_version=self.moneykit_version, token=self._token
         )
         self.access_token = AccessTokenClient(
@@ -40,16 +47,22 @@
             environment=self._environment, moneykit_version=self.moneykit_version, token=self._token
         )
         self.products = ProductsClient(
             environment=self._environment, moneykit_version=self.moneykit_version, token=self._token
         )
 
 
-class AsyncMoneyKit:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+class AsyncBaseMoneyKit:
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
         self.accounts = AsyncAccountsClient(
             environment=self._environment, moneykit_version=self.moneykit_version, token=self._token
         )
         self.access_token = AsyncAccessTokenClient(
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/core/datetime_utils.py` & `fern_moneykit-0.0.5/src/moneykit/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/core/jsonable_encoder.py` & `fern_moneykit-0.0.5/src/moneykit/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/errors/__init__.py` & `fern_moneykit-0.0.5/src/moneykit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/resources/access_token/client.py` & `fern_moneykit-0.0.5/src/moneykit/resources/access_token/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,32 +5,39 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import BaseMoneyKitEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.generate_access_token_response import GenerateAccessTokenResponse
 from ...types.introspect_client_response import IntrospectClientResponse
 from ...types.jwk_set import JwkSet
 from ...types.supported_version import SupportedVersion
 
 
 class AccessTokenClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     def generate_access_token(self) -> GenerateAccessTokenResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "auth/token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "auth/token"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -46,15 +53,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def instrospect_client(self) -> IntrospectClientResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "auth/introspect"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "auth/introspect"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -68,15 +75,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_well_known_jwks(self) -> JwkSet:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", ".well-known/jwks.json"),
+            urllib.parse.urljoin(f"{self._environment.value}/", ".well-known/jwks.json"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -89,24 +96,30 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAccessTokenClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     async def generate_access_token(self) -> GenerateAccessTokenResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "auth/token"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "auth/token"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
@@ -123,15 +136,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def instrospect_client(self) -> IntrospectClientResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "auth/introspect"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "auth/introspect"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
@@ -146,15 +159,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_well_known_jwks(self) -> JwkSet:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", ".well-known/jwks.json"),
+                urllib.parse.urljoin(f"{self._environment.value}/", ".well-known/jwks.json"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/resources/accounts/client.py` & `fern_moneykit-0.0.5/src/moneykit/resources/accounts/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import BaseMoneyKitEnvironment
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.not_found_error import NotFoundError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.api_error_rate_limit_exceeded_response import ApiErrorRateLimitExceededResponse
 from ...types.get_account_numbers_response import GetAccountNumbersResponse
@@ -20,25 +21,31 @@
 from ...types.get_accounts_response import GetAccountsResponse
 from ...types.get_user_accounts_response import GetUserAccountsResponse
 from ...types.link_error_bad_state_response import LinkErrorBadStateResponse
 from ...types.supported_version import SupportedVersion
 
 
 class AccountsClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     def get_accounts(
         self, id: str, *, account_ids: typing.Union[typing.Optional[str], typing.List[str]]
     ) -> GetAccountsResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/accounts"),
             params={"account_ids": account_ids},
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -65,15 +72,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_account_numbers(self, id: str) -> GetAccountNumbersResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/accounts/numbers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/accounts/numbers"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -99,15 +106,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_account(self, id: str, account_id: str) -> GetAccountResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/accounts/{account_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/accounts/{account_id}"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -139,15 +146,15 @@
         id: str,
         *,
         account_id: typing.Union[typing.Optional[str], typing.List[str]],
         institution_id: typing.Union[typing.Optional[str], typing.List[str]],
     ) -> GetUserAccountsResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"users/{id}/accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}/accounts"),
             params={"account_id": account_id, "institution_id": institution_id},
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -161,26 +168,32 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAccountsClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     async def get_accounts(
         self, id: str, *, account_ids: typing.Union[typing.Optional[str], typing.List[str]]
     ) -> GetAccountsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/accounts"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/accounts"),
                 params={"account_ids": account_ids},
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
@@ -208,15 +221,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_account_numbers(self, id: str) -> GetAccountNumbersResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/accounts/numbers"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/accounts/numbers"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
@@ -243,15 +256,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_account(self, id: str, account_id: str) -> GetAccountResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/accounts/{account_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/accounts/{account_id}"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
@@ -284,15 +297,15 @@
         *,
         account_id: typing.Union[typing.Optional[str], typing.List[str]],
         institution_id: typing.Union[typing.Optional[str], typing.List[str]],
     ) -> GetUserAccountsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"users/{id}/accounts"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}/accounts"),
                 params={"account_id": account_id, "institution_id": institution_id},
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/resources/identity/client.py` & `fern_moneykit-0.0.5/src/moneykit/resources/identity/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,37 +5,44 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import BaseMoneyKitEnvironment
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.not_found_error import NotFoundError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.api_error_rate_limit_exceeded_response import ApiErrorRateLimitExceededResponse
 from ...types.identity_response import IdentityResponse
 from ...types.link_error_bad_state_response import LinkErrorBadStateResponse
 from ...types.supported_version import SupportedVersion
 
 
 class IdentityClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     def get_identities(
         self, id: str, *, account_ids: typing.Union[typing.Optional[str], typing.List[str]]
     ) -> IdentityResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/identity"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/identity"),
             params={"account_ids": account_ids},
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -61,26 +68,32 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncIdentityClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     async def get_identities(
         self, id: str, *, account_ids: typing.Union[typing.Optional[str], typing.List[str]]
     ) -> IdentityResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/identity"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/identity"),
                 params={"account_ids": account_ids},
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/resources/institutions/client.py` & `fern_moneykit-0.0.5/src/moneykit/resources/institutions/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,40 +5,47 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import BaseMoneyKitEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.api_error_rate_limit_exceeded_response import ApiErrorRateLimitExceededResponse
 from ...types.get_institutions_response import GetInstitutionsResponse
 from ...types.institution import Institution
 from ...types.supported_version import SupportedVersion
 
 
 class InstitutionsClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     def get_institutions(
         self,
         *,
         name: typing.Optional[str] = None,
         featured: typing.Optional[bool] = None,
         cursor: typing.Optional[str] = None,
         limit: typing.Optional[int] = None,
     ) -> GetInstitutionsResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "institutions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "institutions"),
             params={"name": name, "featured": featured, "cursor": cursor, "limit": limit},
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -57,15 +64,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_institution(self, institution_id: str) -> Institution:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"institutions/{institution_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"institutions/{institution_id}"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -84,15 +91,21 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncInstitutionsClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     async def get_institutions(
         self,
         *,
@@ -100,15 +113,15 @@
         featured: typing.Optional[bool] = None,
         cursor: typing.Optional[str] = None,
         limit: typing.Optional[int] = None,
     ) -> GetInstitutionsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "institutions"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "institutions"),
                 params={"name": name, "featured": featured, "cursor": cursor, "limit": limit},
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
@@ -128,15 +141,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_institution(self, institution_id: str) -> Institution:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"institutions/{institution_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"institutions/{institution_id}"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/resources/link_session/client.py` & `fern_moneykit-0.0.5/src/moneykit/resources/link_session/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import BaseMoneyKitEnvironment
 from ...errors.bad_request_error import BadRequestError
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.create_link_session_response import CreateLinkSessionResponse
 from ...types.exchange_token_response import ExchangeTokenResponse
 from ...types.link_session_customer_user import LinkSessionCustomerUser
 from ...types.link_session_setting_overrides import LinkSessionSettingOverrides
@@ -21,15 +22,21 @@
 from ...types.supported_version import SupportedVersion
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class LinkSessionClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     def create_link_session(
         self,
         *,
@@ -52,15 +59,15 @@
             _request["webhook"] = webhook
         if link_tags is not OMIT:
             _request["link_tags"] = link_tags
         if moneylink_features is not OMIT:
             _request["moneylink_features"] = moneylink_features
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "link-session"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "link-session"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -77,15 +84,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def exchange_token(self, *, exchangeable_token: str) -> ExchangeTokenResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "link-session/exchange-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "link-session/exchange-token"),
             json=jsonable_encoder({"exchangeable_token": exchangeable_token}),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -101,15 +108,21 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncLinkSessionClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     async def create_link_session(
         self,
         *,
@@ -133,15 +146,15 @@
         if link_tags is not OMIT:
             _request["link_tags"] = link_tags
         if moneylink_features is not OMIT:
             _request["moneylink_features"] = moneylink_features
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "link-session"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "link-session"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
@@ -159,15 +172,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def exchange_token(self, *, exchangeable_token: str) -> ExchangeTokenResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "link-session/exchange-token"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "link-session/exchange-token"),
                 json=jsonable_encoder({"exchangeable_token": exchangeable_token}),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/resources/links/client.py` & `fern_moneykit-0.0.5/src/moneykit/resources/links/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import BaseMoneyKitEnvironment
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.not_found_error import NotFoundError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.api_error_rate_limit_exceeded_response import ApiErrorRateLimitExceededResponse
 from ...types.get_user_links_response import GetUserLinksResponse
@@ -22,23 +23,29 @@
 from ...types.supported_version import SupportedVersion
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class LinksClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     def get_link(self, id: str) -> LinkResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -71,15 +78,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if webhook is not OMIT:
             _request["webhook"] = webhook
         if tags is not OMIT:
             _request["tags"] = tags
         _response = httpx.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -106,15 +113,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def disconnect(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -140,15 +147,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_user_links(self, id: str) -> GetUserLinksResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"users/{id}/links"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}/links"),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
             timeout=60,
@@ -161,24 +168,30 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncLinksClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     async def get_link(self, id: str) -> LinkResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
@@ -212,15 +225,15 @@
         if webhook is not OMIT:
             _request["webhook"] = webhook
         if tags is not OMIT:
             _request["tags"] = tags
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
@@ -248,15 +261,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def disconnect(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
@@ -283,15 +296,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_user_links(self, id: str) -> GetUserLinksResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"users/{id}/links"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}/links"),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
                 timeout=60,
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/resources/products/client.py` & `fern_moneykit-0.0.5/src/moneykit/resources/products/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,35 +6,42 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import BaseMoneyKitEnvironment
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.not_found_error import NotFoundError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.api_error_rate_limit_exceeded_response import ApiErrorRateLimitExceededResponse
 from ...types.link_error_bad_state_response import LinkErrorBadStateResponse
 from ...types.product import Product
 from ...types.supported_version import SupportedVersion
 
 
 class ProductsClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     def refresh_products(self, id: str, *, products: typing.List[Product]) -> None:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/products"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/products"),
             json=jsonable_encoder({"products": products}),
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -60,24 +67,30 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncProductsClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     async def refresh_products(self, id: str, *, products: typing.List[Product]) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/products"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/products"),
                 json=jsonable_encoder({"products": products}),
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/resources/transactions/client.py` & `fern_moneykit-0.0.5/src/moneykit/resources/transactions/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import BaseMoneyKitEnvironment
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.not_found_error import NotFoundError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.api_error_rate_limit_exceeded_response import ApiErrorRateLimitExceededResponse
 from ...types.get_transactions_response import GetTransactionsResponse
@@ -20,15 +21,21 @@
 from ...types.link_error_bad_state_response import LinkErrorBadStateResponse
 from ...types.supported_version import SupportedVersion
 from ...types.transaction_sync_response import TransactionSyncResponse
 from ...types.transaction_type_filter import TransactionTypeFilter
 
 
 class TransactionsClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     def get_transactions(
         self,
         id: str,
@@ -37,15 +44,15 @@
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
         start_date: typing.Optional[str] = None,
         end_date: typing.Optional[str] = None,
     ) -> GetTransactionsResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/transactions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/transactions"),
             params={
                 "account_ids": account_ids,
                 "page": page,
                 "size": size,
                 "start_date": start_date,
                 "end_date": end_date,
             },
@@ -80,15 +87,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_transactions_diff(
         self, id: str, *, cursor: typing.Optional[str] = None, size: typing.Optional[int] = None
     ) -> TransactionSyncResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/transactions/sync"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/transactions/sync"),
             params={"cursor": cursor, "size": size},
             headers=remove_none_from_headers(
                 {
                     "moneykit-version": self.moneykit_version,
                     "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                 }
             ),
@@ -127,15 +134,15 @@
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
         start_date: typing.Optional[str] = None,
         end_date: typing.Optional[str] = None,
     ) -> GetUserTransactionsResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"users/{id}/transactions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}/transactions"),
             params={
                 "transaction_type": transaction_type,
                 "category": category,
                 "account_id": account_id,
                 "institution_id": institution_id,
                 "page": page,
                 "size": size,
@@ -158,15 +165,21 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTransactionsClient:
-    def __init__(self, *, environment: str, moneykit_version: typing.Optional[SupportedVersion] = None, token: str):
+    def __init__(
+        self,
+        *,
+        environment: BaseMoneyKitEnvironment = BaseMoneyKitEnvironment.PRODUCTION,
+        moneykit_version: typing.Optional[SupportedVersion] = None,
+        token: str,
+    ):
         self._environment = environment
         self.moneykit_version = moneykit_version
         self._token = token
 
     async def get_transactions(
         self,
         id: str,
@@ -176,15 +189,15 @@
         size: typing.Optional[int] = None,
         start_date: typing.Optional[str] = None,
         end_date: typing.Optional[str] = None,
     ) -> GetTransactionsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/transactions"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/transactions"),
                 params={
                     "account_ids": account_ids,
                     "page": page,
                     "size": size,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
@@ -220,15 +233,15 @@
 
     async def get_transactions_diff(
         self, id: str, *, cursor: typing.Optional[str] = None, size: typing.Optional[int] = None
     ) -> TransactionSyncResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"links/{id}/transactions/sync"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"links/{id}/transactions/sync"),
                 params={"cursor": cursor, "size": size},
                 headers=remove_none_from_headers(
                     {
                         "moneykit-version": self.moneykit_version,
                         "Authorization": f"Bearer {self._token}" if self._token is not None else None,
                     }
                 ),
@@ -268,15 +281,15 @@
         size: typing.Optional[int] = None,
         start_date: typing.Optional[str] = None,
         end_date: typing.Optional[str] = None,
     ) -> GetUserTransactionsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"users/{id}/transactions"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}/transactions"),
                 params={
                     "transaction_type": transaction_type,
                     "category": category,
                     "account_id": account_id,
                     "institution_id": institution_id,
                     "page": page,
                     "size": size,
```

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/__init__.py` & `fern_moneykit-0.0.5/src/moneykit/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account.py` & `fern_moneykit-0.0.5/src/moneykit/types/account.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account_balances.py` & `fern_moneykit-0.0.5/src/moneykit/types/account_balances.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account_group.py` & `fern_moneykit-0.0.5/src/moneykit/types/account_group.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account_identity.py` & `fern_moneykit-0.0.5/src/moneykit/types/account_identity.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account_numbers.py` & `fern_moneykit-0.0.5/src/moneykit/types/account_numbers.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account_numbers_link_product.py` & `fern_moneykit-0.0.5/src/moneykit/types/account_numbers_link_product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account_numbers_product_settings.py` & `fern_moneykit-0.0.5/src/moneykit/types/account_numbers_product_settings.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account_type.py` & `fern_moneykit-0.0.5/src/moneykit/types/account_type.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/account_with_account_numbers.py` & `fern_moneykit-0.0.5/src/moneykit/types/account_with_account_numbers.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/accounts_link_product.py` & `fern_moneykit-0.0.5/src/moneykit/types/accounts_link_product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/ach_number.py` & `fern_moneykit-0.0.5/src/moneykit/types/ach_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/address.py` & `fern_moneykit-0.0.5/src/moneykit/types/address.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/api_error_auth_expired_access_token_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/api_error_auth_expired_access_token_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/api_error_auth_unauthorized_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/api_error_auth_unauthorized_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/api_error_rate_limit_exceeded_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/api_error_rate_limit_exceeded_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/bacs_number.py` & `fern_moneykit-0.0.5/src/moneykit/types/bacs_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/basic_account_details.py` & `fern_moneykit-0.0.5/src/moneykit/types/basic_account_details.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/body_generate_access_token_auth_token_post.py` & `fern_moneykit-0.0.5/src/moneykit/types/body_generate_access_token_auth_token_post.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/country.py` & `fern_moneykit-0.0.5/src/moneykit/types/country.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/create_link_session_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/create_link_session_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/currency.py` & `fern_moneykit-0.0.5/src/moneykit/types/currency.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/cursor_pagination.py` & `fern_moneykit-0.0.5/src/moneykit/types/cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/customer_app.py` & `fern_moneykit-0.0.5/src/moneykit/types/customer_app.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/eft_number.py` & `fern_moneykit-0.0.5/src/moneykit/types/eft_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/email.py` & `fern_moneykit-0.0.5/src/moneykit/types/email.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/exchange_token_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/exchange_token_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/generate_access_token_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/generate_access_token_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/get_account_numbers_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/get_account_numbers_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/get_account_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/get_account_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/get_accounts_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/get_accounts_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/get_institutions_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/get_institutions_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/get_transactions_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/get_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/get_user_accounts_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/get_user_accounts_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/get_user_links_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/get_user_links_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/get_user_transactions_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/get_user_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/http_validation_error.py` & `fern_moneykit-0.0.5/src/moneykit/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/identity_link_product.py` & `fern_moneykit-0.0.5/src/moneykit/types/identity_link_product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/identity_product_settings.py` & `fern_moneykit-0.0.5/src/moneykit/types/identity_product_settings.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/identity_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/identity_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/institution.py` & `fern_moneykit-0.0.5/src/moneykit/types/institution.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/institution_error_not_found_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/institution_error_not_found_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/international_number.py` & `fern_moneykit-0.0.5/src/moneykit/types/international_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/introspect_client_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/introspect_client_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/jwk_set.py` & `fern_moneykit-0.0.5/src/moneykit/types/jwk_set.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_common.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_common.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_error_bad_state_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_error_bad_state_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_error_deleted_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_error_deleted_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_error_forbidden_action_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_error_forbidden_action_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_error_not_found_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_error_not_found_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_error_unauthorized_access_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_error_unauthorized_access_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_permission_scope.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_permission_scope.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_permissions.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_permissions.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_products.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_products.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_session_customer_user.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_session_customer_user.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_session_customer_user_email.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_session_customer_user_email.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_session_customer_user_phone.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_session_customer_user_phone.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_session_error_forbidden_config_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_session_error_forbidden_config_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_session_error_invalid_token_exchange.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_session_error_invalid_token_exchange.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_session_setting_overrides.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_session_setting_overrides.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/link_state_changed_webhook.py` & `fern_moneykit-0.0.5/src/moneykit/types/link_state_changed_webhook.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/money_link_features.py` & `fern_moneykit-0.0.5/src/moneykit/types/money_link_features.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/owner.py` & `fern_moneykit-0.0.5/src/moneykit/types/owner.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/phone_number.py` & `fern_moneykit-0.0.5/src/moneykit/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/phone_number_type.py` & `fern_moneykit-0.0.5/src/moneykit/types/phone_number_type.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/product.py` & `fern_moneykit-0.0.5/src/moneykit/types/product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/products_settings.py` & `fern_moneykit-0.0.5/src/moneykit/types/products_settings.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/provider.py` & `fern_moneykit-0.0.5/src/moneykit/types/provider.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/public_link_error.py` & `fern_moneykit-0.0.5/src/moneykit/types/public_link_error.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/public_link_state.py` & `fern_moneykit-0.0.5/src/moneykit/types/public_link_state.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/requested_link_permission.py` & `fern_moneykit-0.0.5/src/moneykit/types/requested_link_permission.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/transaction.py` & `fern_moneykit-0.0.5/src/moneykit/types/transaction.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/transaction_diff.py` & `fern_moneykit-0.0.5/src/moneykit/types/transaction_diff.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/transaction_sync_response.py` & `fern_moneykit-0.0.5/src/moneykit/types/transaction_sync_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/transaction_type_filter.py` & `fern_moneykit-0.0.5/src/moneykit/types/transaction_type_filter.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/transactions_link_product.py` & `fern_moneykit-0.0.5/src/moneykit/types/transactions_link_product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/transactions_product_settings.py` & `fern_moneykit-0.0.5/src/moneykit/types/transactions_product_settings.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/src/moneykit/types/validation_error.py` & `fern_moneykit-0.0.5/src/moneykit/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.4/PKG-INFO` & `fern_moneykit-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 Metadata-Version: 2.1
 Name: fern-moneykit
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (==0.23.3)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 
-# {Company} Python Library
+# MoneyKit Python Library
 
-[![pypi](https://img.shields.io/pypi/v/{company}.svg)](https://pypi.python.org/pypi/{company})
+[![pypi](https://img.shields.io/pypi/v/fern-moneykit.svg)](https://pypi.python.org/pypi/fern-moneykit)
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
 
-## Documentation
+## Installation
 
-API documentation is available at <{docs_url}>.
+Add this dependency to your project's build file:
+
+```bash
+pip install fern-moneykit
+# or
+poetry add fern-moneykit
+```
 
 ## Usage
 
-Check out the [sample app](.sample-app/app.py) which consumes this SDK!
+```python
+from moneykit.client import MoneyKit
+
+moneykit_client = MoneyKit(client_id="YOUR_CLIENT_ID", client_secret="YOUR_CLIENT_SECRET")
+```
+
+## Async Client
 
 ```python
-TODO
+from moneykit.client import AsyncMoneyKit
+
+moneykit_client = AsyncMoneyKit(client_id="YOUR_CLIENT_ID", client_secret="YOUR_CLIENT_SECRET")
 ```
 
 ## Beta status
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning the package version to a specific version in your pyproject.toml file. This way, you can install the same version each time without breaking changes unless you are intentionally looking for the latest version.
 
 ## Contributing
```

