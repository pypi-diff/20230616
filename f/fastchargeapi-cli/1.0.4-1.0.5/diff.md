# Comparing `tmp/fastchargeapi_cli-1.0.4.tar.gz` & `tmp/fastchargeapi_cli-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchargeapi_cli-1.0.4.tar", max compression
+gzip compressed data, was "fastchargeapi_cli-1.0.5.tar", max compression
```

## Comparing `fastchargeapi_cli-1.0.4.tar` & `fastchargeapi_cli-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2023-03-17 09:53:33.031435 fastchargeapi_cli-1.0.4/fastchargeapi_cli/__generated__/__init__.py
--rw-r--r--   0        0        0    36816 2023-06-01 08:04:00.159129 fastchargeapi_cli-1.0.4/fastchargeapi_cli/__generated__/gql_operations.py
--rw-r--r--   0        0        0       22 2023-06-01 08:03:20.827205 fastchargeapi_cli-1.0.4/fastchargeapi_cli/__init__.py
--rw-r--r--   0        0        0     3299 2023-06-01 07:11:42.392468 fastchargeapi_cli-1.0.4/fastchargeapi_cli/account.py
--rw-r--r--   0        0        0     8063 2023-05-06 05:16:53.948507 fastchargeapi_cli-1.0.4/fastchargeapi_cli/auth_file.py
--rw-r--r--   0        0        0      884 2023-04-23 16:48:06.408480 fastchargeapi_cli-1.0.4/fastchargeapi_cli/config.py
--rw-r--r--   0        0        0      123 2023-04-23 16:48:08.170800 fastchargeapi_cli-1.0.4/fastchargeapi_cli/context_obj.py
--rw-r--r--   0        0        0     1064 2023-05-07 18:21:01.191960 fastchargeapi_cli-1.0.4/fastchargeapi_cli/exceptions.py
--rw-r--r--   0        0        0     1280 2023-05-07 17:06:26.549181 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_account.py
--rw-r--r--   0        0        0     1405 2023-05-07 17:06:26.575798 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_api.py
--rw-r--r--   0        0        0     5140 2023-05-07 18:28:23.129772 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_subscription.py
--rw-r--r--   0        0        0     4921 2023-05-07 17:06:31.983616 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_account.py
--rw-r--r--   0        0        0     6932 2023-05-07 20:32:44.869011 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_api.py
--rw-r--r--   0        0        0     6105 2023-05-30 03:27:23.172124 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_app.py
--rw-r--r--   0        0        0     7193 2023-05-07 17:06:31.446962 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_pricing.py
--rw-r--r--   0        0        0      967 2023-05-07 17:06:32.061592 fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_stripe.py
--rw-r--r--   0        0        0     2806 2023-05-07 19:30:33.999971 fastchargeapi_cli-1.0.4/fastchargeapi_cli/graphql_client.py
--rw-r--r--   0        0        0      789 2023-05-07 17:06:31.940160 fastchargeapi_cli-1.0.4/fastchargeapi_cli/groups.py
--rw-r--r--   0        0        0      811 2023-04-23 16:48:40.243041 fastchargeapi_cli-1.0.4/fastchargeapi_cli/http.py
--rw-r--r--   0        0        0     3637 2023-04-23 16:48:41.984143 fastchargeapi_cli-1.0.4/fastchargeapi_cli/local_server.py
--rw-r--r--   0        0        0     3867 2023-06-01 08:02:52.106455 fastchargeapi_cli-1.0.4/fastchargeapi_cli/login.py
--rw-r--r--   0        0        0      718 2023-05-07 17:06:31.932263 fastchargeapi_cli-1.0.4/fastchargeapi_cli/main.py
--rw-r--r--   0        0        0     6023 2023-05-28 22:41:24.242247 fastchargeapi_cli-1.0.4/fastchargeapi_cli/operations.graphql
--rw-r--r--   0        0        0     6594 2023-05-06 01:26:22.394837 fastchargeapi_cli-1.0.4/fastchargeapi_cli/remote_secret.py
--rw-r--r--   0        0        0     2574 2023-05-07 18:42:52.499981 fastchargeapi_cli-1.0.4/fastchargeapi_cli/token.py
--rw-r--r--   0        0        0     1503 2023-06-01 07:46:03.922199 fastchargeapi_cli-1.0.4/fastchargeapi_cli/version.py
--rw-r--r--   0        0        0     1448 2023-06-01 08:03:18.495466 fastchargeapi_cli-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 fastchargeapi_cli-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-17 09:53:33.031435 fastchargeapi_cli-1.0.5/fastchargeapi_cli/__generated__/__init__.py
+-rw-r--r--   0        0        0    37858 2023-06-16 20:18:55.699457 fastchargeapi_cli-1.0.5/fastchargeapi_cli/__generated__/gql_operations.py
+-rw-r--r--   0        0        0       22 2023-06-01 08:03:20.827205 fastchargeapi_cli-1.0.5/fastchargeapi_cli/__init__.py
+-rw-r--r--   0        0        0     3299 2023-06-01 07:11:42.392468 fastchargeapi_cli-1.0.5/fastchargeapi_cli/account.py
+-rw-r--r--   0        0        0     8063 2023-06-02 03:55:47.709199 fastchargeapi_cli-1.0.5/fastchargeapi_cli/auth_file.py
+-rw-r--r--   0        0        0     1088 2023-06-02 04:32:11.329560 fastchargeapi_cli-1.0.5/fastchargeapi_cli/config.py
+-rw-r--r--   0        0        0      123 2023-04-23 16:48:08.170800 fastchargeapi_cli-1.0.5/fastchargeapi_cli/context_obj.py
+-rw-r--r--   0        0        0     1064 2023-05-07 18:21:01.191960 fastchargeapi_cli-1.0.5/fastchargeapi_cli/exceptions.py
+-rw-r--r--   0        0        0     1280 2023-05-07 17:06:26.549181 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_account.py
+-rw-r--r--   0        0        0     1433 2023-06-02 03:40:08.819412 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_api.py
+-rw-r--r--   0        0        0     5145 2023-06-15 16:46:02.385383 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_subscription.py
+-rw-r--r--   0        0        0     5166 2023-06-15 20:28:24.635264 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_account.py
+-rw-r--r--   0        0        0     6960 2023-06-02 03:40:08.819797 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_api.py
+-rw-r--r--   0        0        0     6105 2023-05-30 03:27:23.172124 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_app.py
+-rw-r--r--   0        0        0     7193 2023-05-07 17:06:31.446962 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_pricing.py
+-rw-r--r--   0        0        0      967 2023-05-07 17:06:32.061592 fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_stripe.py
+-rw-r--r--   0        0        0     2806 2023-05-07 19:30:33.999971 fastchargeapi_cli-1.0.5/fastchargeapi_cli/graphql_client.py
+-rw-r--r--   0        0        0      789 2023-05-07 17:06:31.940160 fastchargeapi_cli-1.0.5/fastchargeapi_cli/groups.py
+-rw-r--r--   0        0        0      811 2023-04-23 16:48:40.243041 fastchargeapi_cli-1.0.5/fastchargeapi_cli/http.py
+-rw-r--r--   0        0        0     3637 2023-04-23 16:48:41.984143 fastchargeapi_cli-1.0.5/fastchargeapi_cli/local_server.py
+-rw-r--r--   0        0        0     3867 2023-06-01 18:11:35.119022 fastchargeapi_cli-1.0.5/fastchargeapi_cli/login.py
+-rw-r--r--   0        0        0      718 2023-05-07 17:06:31.932263 fastchargeapi_cli-1.0.5/fastchargeapi_cli/main.py
+-rw-r--r--   0        0        0     6164 2023-06-15 19:51:12.068426 fastchargeapi_cli-1.0.5/fastchargeapi_cli/operations.graphql
+-rw-r--r--   0        0        0     6594 2023-05-06 01:26:22.394837 fastchargeapi_cli-1.0.5/fastchargeapi_cli/remote_secret.py
+-rw-r--r--   0        0        0     2574 2023-05-07 18:42:52.499981 fastchargeapi_cli-1.0.5/fastchargeapi_cli/token.py
+-rw-r--r--   0        0        0     1503 2023-06-01 07:46:03.922199 fastchargeapi_cli-1.0.5/fastchargeapi_cli/version.py
+-rw-r--r--   0        0        0     1448 2023-06-16 20:18:53.114637 fastchargeapi_cli-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 fastchargeapi_cli-1.0.5/PKG-INFO
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/__generated__/gql_operations.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/__generated__/gql_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List, Literal, Optional
+from typing import Any, List, Literal, Optional
 
 from gql import Client
 from pydantic import BaseModel, Field
 
 from fastchargeapi_cli.graphql_client import gql_execute
 
 
@@ -89,14 +89,20 @@
     settled = "settled"
 
 
 class AccountActivityIndex(str, Enum):
     indexByStatus_settleAt__onlyPK = "indexByStatus_settleAt__onlyPK"
 
 
+class SiteMetaDataKey(str, Enum):
+    pricingPerRequestCharge = "pricingPerRequestCharge"
+    pricingStripePercentageFee = "pricingStripePercentageFee"
+    pricingStripeFlatFee = "pricingStripeFlatFee"
+
+
 class DateRangeInput(BaseModel):
     start: Optional[int]
     end: Optional[int]
 
 
 class GetCurrentSubscriptionSubscriptionPricing(BaseModel):
     typename: Optional[Literal["Pricing"]] = Field(alias="__typename")
@@ -713,14 +719,30 @@
     class Arguments(BaseModel):
         user: str
 
     class Meta:
         document = "query GetUserAccountInfo($user: ID!) {\n  user(pk: $user) {\n    balance\n    author\n    email\n  }\n}"
 
 
+class GetStripePricingDataSitemetadata(BaseModel):
+    typename: Optional[Literal["SiteMetaData"]] = Field(alias="__typename")
+    key: SiteMetaDataKey
+    value: Any
+
+
+class GetStripePricingData(BaseModel):
+    siteMetaData: List[GetStripePricingDataSitemetadata]
+
+    class Arguments(BaseModel):
+        pass
+
+    class Meta:
+        document = "query GetStripePricingData {\n  siteMetaData(keys: [pricingStripeFlatFee, pricingStripePercentageFee]) {\n    key\n    value\n  }\n}"
+
+
 def get_current_subscription(
     client: Client, user: Optional[str] = None, app_name: Optional[str] = None
 ) -> GetCurrentSubscriptionSubscription:
     """GetCurrentSubscription
 
 
 
@@ -1266,7 +1288,20 @@
     Arguments:
         client (gql.Client): The client we want to use to execute the operation
         user (str): user
 
     Returns:
         GetUserAccountInfoUser"""
     return gql_execute(client, GetUserAccountInfo, {"user": user}).user
+
+
+def get_stripe_pricing_data(client: Client) -> List[GetStripePricingDataSitemetadata]:
+    """GetStripePricingData
+
+
+
+    Arguments:
+        client (gql.Client): The client we want to use to execute the operation
+
+    Returns:
+        List[GetStripePricingDataSitemetadata]"""
+    return gql_execute(client, GetStripePricingData, {}).siteMetaData
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/account.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/auth_file.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/auth_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,18 +37,18 @@
     if auth_file_path.exists():
         auth_file_path.unlink()
 
 
 @dataclass
 class AuthFileContent:
     id_token: str
-    refresh_token: Union[Literal["firebase"], Literal["fastchargeapi"]]
+    refresh_token: str
     user_pk: str
     email: str
-    issuer: str
+    issuer: Union[Literal["firebase"], Literal["fastchargeapi"]]
 
 
 def write_to_auth_file(
     *,
     profile: Optional[str] = None,
     issuer: Optional[str] = "firebase",
     id_token: Optional[str] = None,
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/config.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import os
 
-graphql_host = "https://api.graphql.fastchargeapi.com"
-payment_service_host = "https://api.v2.payment.fastchargeapi.com"
-auth_service_host = "https://api.v2.auth.fastchargeapi.com"
-react_host = "https://fastchargeapi.com"
+base_domain = (
+    "devfastchargeapi.com"
+    if os.environ.get("DEV_DOMAIN") == "1"
+    else "fastchargeapi.com"
+)
+aws_account_id = (
+    "209991057786" if os.environ.get("DEV_DOMAIN") == "1" else "887279901853"
+)
+graphql_host = f"https://api.graphql.{base_domain}"
+payment_service_host = f"https://api.v2.payment.{base_domain}"
+auth_service_host = f"https://api.v2.auth.{base_domain}"
+react_host = f"https://{base_domain}"
 
 if os.environ.get("TEST") == "1":
     graphql_host = "http://localhost:4001"
     payment_service_host = "http://localhost:3001"
     react_host = "http://localhost:8001"
 
 if os.environ.get("LOCAL_GRAPHQL") == "1":
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/exceptions.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_account.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_account.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_api.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 from blessings import Terminal
 from click import echo
 from click_aliases import ClickAliasedGroup
 
 from .__generated__ import gql_operations as GQL
+from .config import base_domain
 from .context_obj import ContextObject
 from .fastcharge_app import get_app_or_prompt_exit
 from .graphql_client import get_client_info
 from .groups import fastapi
 
 terminal = Terminal()
 
@@ -27,15 +28,15 @@
     client, auth = get_client_info(ctx_obj.profile)
     app = get_app_or_prompt_exit(client, app_name)
     app = GQL.get_app_endpoints(client, app_name)
     echo(terminal.blue + terminal.bold + f'"{app.name}" endpoints:\n' + terminal.normal)
     # echo(f"\n Gateway mode: {app['gatewayMode']}\n")
     if app.endpoints:
         for endpoint in app.endpoints:
-            url = f"https://{app.name}.fastchargeapi.com{endpoint.path}"
+            url = f"https://{app.name}.{base_domain}{endpoint.path}"
             echo(" ID:\t\t" + endpoint.pk)
             echo(" HTTP Method:\t" + endpoint.method)
             echo(" Endpoint:\t" + url)
             echo(terminal.dim(f" {endpoint.description or 'No description.'}"))
             echo()
     else:
         echo("No API available.")
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastapi_subscription.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastapi_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         echo(
             f"  ${float(pricing.minMonthlyCharge):.2f} during active month + additional ${pricing.chargePerRequest} per request"
         )
         echo("  First 1000 requests are free of charge.")
         echo()
 
 
-@fastapi_subscribe.command("add", aliases=[])
+@fastapi_subscribe.command("add", aliases=["sub"])
 @click.argument("app_name", required=True)
 @click.option("-p", "--plan", help="Name of the plan to subscribe to.")
 @click.pass_obj
 def subscription_add(ctx_obj: ContextObject, app_name: str, plan: Optional[str] = None):
     """Subscribe to an app."""
     client, auth = get_client_info(ctx_obj.profile)
     # Get the pricing plan the user is currently subscribed to, to provide a better output.
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_account.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from blessings import Terminal
 from click import echo
 from click_aliases import ClickAliasedGroup
 
 from . import config
 from .__generated__ import gql_operations as GQL
 from .account import do_account_info, do_account_topup, do_account_update
+from .config import base_domain
 from .context_obj import ContextObject
 from .graphql_client import get_client_info
 from .groups import fastcharge
 from .http import HttpClient
 
 terminal = Terminal()
 
@@ -86,35 +87,40 @@
         + f"${balance:.2f}"
         + terminal.normal
     )
     echo()
     echo(
         "Note that it may take up to 1 busines day for the funds to arrive to your Stripe account."
     )
-    stripe_charges_percent = 2.9 + 0.25 + 0.5
-    stripe_charges_flat = 2 + 0.5 + 0.25
+    stripe_pricing = {x.key: x.value for x in GQL.get_stripe_pricing_data(client)}
+    stripe_charges_percent = float(
+        stripe_pricing[GQL.SiteMetaDataKey.pricingStripePercentageFee]
+    )
+    stripe_charges_flat = float(
+        stripe_pricing[GQL.SiteMetaDataKey.pricingStripeFlatFee]
+    )
     echo(
         "\n".join(
             textwrap.wrap(
-                f"Stripe Express account charges a fee for the transfer, which is {terminal.blue}${stripe_charges_flat:.2f} + {stripe_charges_percent:.2f}%{terminal.normal} of the transferred amout. "
+                f"Stripe Express account charges a fee for the transfer, which is {terminal.blue}${stripe_charges_flat:.2f} + {(stripe_charges_percent * 100):.2f}%{terminal.normal} of the transferred amout. "
                 "As a result, you may recieve less than the transferred amount.",
             )
         )
     )
-    stripe_fee = stripe_charges_flat + stripe_charges_percent / 100 * withdraw
+    stripe_fee = stripe_charges_flat + stripe_charges_percent * withdraw
     receive_amount = max(0, withdraw - stripe_fee)
     echo()
     echo(
         "Estimated received amount to your Stripe account: "
         + terminal.yellow
         + f"${receive_amount * 0.9975:.2f}"
         + terminal.normal
     )
     echo(
-        "Your FastchargeAPI account estimated new balance: "
+        "Your FastchargeAPI account new estimated balance: "
         + terminal.green
         + f"${balance - withdraw:.2f}"
         + terminal.normal
     )
     echo()
     if yes or input("Continue? (y/N)").strip().lower() == "y":
         response = HttpClient(ctx_obj.profile).post(
@@ -129,15 +135,15 @@
             terminal.green
             + terminal.bold
             + "Payout request was sent."
             + terminal.normal
         )
         echo("Note that it may take up to 1 business day for the funds to arrive.")
         echo("Login to the account dashboard to view your payout status:")
-        echo(terminal.blue + " https://fastchargeapi.com/account" + terminal.normal)
+        echo(terminal.blue + f" https://{base_domain}/account/" + terminal.normal)
 
 
 @fastcharge_account.command("topup")
 @click.help_option("-h", "--help")
 @click.argument("amount", type=float, required=True)
 @click.option("--browser/--no-browser", is_flag=True, default=True)
 @click.pass_obj
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_api.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .__generated__ import gql_operations as GQL
 from .context_obj import ContextObject
 from .exceptions import AlreadyExists, BadUserInput, NotFound, PermissionDenied
 from .fastcharge_app import get_app_or_prompt_exit
 from .graphql_client import get_client_info
 from .groups import fastcharge
+from .config import base_domain
 
 terminal = Terminal()
 
 
 @fastcharge.group("api", cls=ClickAliasedGroup)
 @click.help_option("-h", "--help")
 def fastcharge_api():
@@ -115,15 +116,15 @@
         echo(terminal.red(f'You do not have permission to manage "{app_name}".'))
         echo("To view the endpoints as a customer, use `fastapi api list` instead.")
         exit(1)
     echo(terminal.blue + terminal.bold + f'"{app.name}" endpoints:\n' + terminal.normal)
     # echo(f"\n Gateway mode: {app['gatewayMode']}\n")
     if app.endpoints:
         for endpoint in app.endpoints:
-            url = f"https://{app.name}.fastchargeapi.com{endpoint.path}"
+            url = f"https://{app.name}.{base_domain}{endpoint.path}"
             echo(" ID:\t\t" + endpoint.pk)
             echo(" HTTP Method:\t" + endpoint.method)
             echo(" Endpoint:\t" + f"{url} ~> {endpoint.destination}")
             echo(terminal.dim(f" {endpoint.description or 'No description.'}"))
             echo()
     else:
         echo("No API available.")
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_app.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_app.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_pricing.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_pricing.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/fastcharge_stripe.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/fastcharge_stripe.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/graphql_client.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/graphql_client.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/groups.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/groups.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/http.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/http.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/local_server.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/local_server.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/login.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,23 +65,23 @@
     url = f"{config.react_host}/auth/?relogin=true&behavior=putsecret&jwe={jwe_secret.hex()}&jwt={jwt_secret.hex()}&key={key}"
     webbrowser.open_new(url)
     echo("Please authenticate in the browser.")
     echo("If the browser does not open, please visit:")
     echo(term.blue(" " + url))
     tries = 0
     while True:
-        time.sleep(5)
+        time.sleep(3)
         tries += 1
         try:
             if value := get_remote_secret(client, key, jwe_secret, jwt_secret):
                 id_token, refresh_token = value["idToken"], value["refreshToken"]
                 break
         except NotFound as e:
             pass
-        if tries > 20:
+        if tries > 40:
             input("Timed out. Press enter to retry.")
             continue
     user_email = verify_id_token(id_token)
     assert user_email is not None, "ID token is invalid. Login failed."
     user_pk = query_user_pk(id_token, user_email.email)
     write_to_auth_file(
         profile=profile,
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/main.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/main.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/operations.graphql` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/operations.graphql`

 * *Files 2% similar despite different names*

```diff
@@ -299,7 +299,14 @@
 query GetUserAccountInfo($user: ID!) {
     user(pk: $user) {
         balance
         author
         email
     }
 }
+
+query GetStripePricingData {
+    siteMetaData(keys: [pricingStripeFlatFee, pricingStripePercentageFee]) {
+        key
+        value
+    }
+}
```

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/remote_secret.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/remote_secret.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/token.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/token.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/fastchargeapi_cli/version.py` & `fastchargeapi_cli-1.0.5/fastchargeapi_cli/version.py`

 * *Files identical despite different names*

### Comparing `fastchargeapi_cli-1.0.4/pyproject.toml` & `fastchargeapi_cli-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchargeapi-cli"
-version = "1.0.4"
+version = "1.0.5"
 description = "Official CLI for managing apps and account on FastchargeAPI.com"
 authors = ["FastchargeAPI <fastchargeapi@gmail.com>"]
 license = "GNU v3.0"
 homepage = "https://fastchargeapi.com"
 repository = "https://github.com/FastchargeAPI/fastchargeapi-cli"
 packages = [{include = "fastchargeapi_cli"}]
 include = ["fastchargeapi_cli/__generated__/*"]
```

### Comparing `fastchargeapi_cli-1.0.4/PKG-INFO` & `fastchargeapi_cli-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchargeapi-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: Official CLI for managing apps and account on FastchargeAPI.com
 Home-page: https://fastchargeapi.com
 License: GNU v3.0
 Author: FastchargeAPI
 Author-email: fastchargeapi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

