# Comparing `tmp/smpp_gateway-1.0.4.tar.gz` & `tmp/smpp_gateway-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpp_gateway-1.0.4.tar", max compression
+gzip compressed data, was "smpp_gateway-1.1.0.tar", max compression
```

## Comparing `smpp_gateway-1.0.4.tar` & `smpp_gateway-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1085 2023-05-15 01:52:32.518883 smpp_gateway-1.0.4/LICENSE
--rw-r--r--   0        0        0     1082 2023-05-15 01:52:32.518883 smpp_gateway-1.0.4/README.md
--rw-r--r--   0        0        0     1282 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/__init__.py
--rw-r--r--   0        0        0     2452 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/admin.py
--rw-r--r--   0        0        0      189 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/apps.py
--rw-r--r--   0        0        0     9550 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/client.py
--rw-r--r--   0        0        0      404 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/management/commands/listen_mo_messages.py
--rw-r--r--   0        0        0     1993 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/management/commands/smpp_client.py
--rw-r--r--   0        0        0     2975 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0001_initial.py
--rw-r--r--   0        0        0     2303 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0002_mtmessagestatus.py
--rw-r--r--   0        0        0     2173 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0003_big_pks_and_help_texts.py
--rw-r--r--   0        0        0     5435 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0004_translations.py
--rw-r--r--   0        0        0     3660 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/0005_alter_mtmessagestatus_command_status.py
--rw-r--r--   0        0        0        0 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/migrations/__init__.py
--rw-r--r--   0        0        0     4351 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/models.py
--rw-r--r--   0        0        0     1846 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/outgoing.py
--rw-r--r--   0        0        0     2616 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/queries.py
--rw-r--r--   0        0        0     1563 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/smpp.py
--rw-r--r--   0        0        0     2218 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/subscribers.py
--rw-r--r--   0        0        0     1894 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/src/smpp_gateway/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1697 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/factories.py
--rw-r--r--   0        0        0      450 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/settings.py
--rw-r--r--   0        0        0     4648 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/test_client.py
--rw-r--r--   0        0        0     7435 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/test_queries.py
--rw-r--r--   0        0        0       93 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/test_smpp_gateway.py
--rw-r--r--   0        0        0     2633 2023-05-15 01:52:32.522883 smpp_gateway-1.0.4/tests/test_subscribers.py
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 smpp_gateway-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1611 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/README.md
+-rw-r--r--   0        0        0     1282 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/__init__.py
+-rw-r--r--   0        0        0     2452 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/admin.py
+-rw-r--r--   0        0        0      189 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/apps.py
+-rw-r--r--   0        0        0     9760 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/client.py
+-rw-r--r--   0        0        0      404 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/management/commands/listen_mo_messages.py
+-rw-r--r--   0        0        0     2828 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/management/commands/smpp_client.py
+-rw-r--r--   0        0        0     2975 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2303 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/migrations/0002_mtmessagestatus.py
+-rw-r--r--   0        0        0     2173 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/migrations/0003_big_pks_and_help_texts.py
+-rw-r--r--   0        0        0     5435 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/migrations/0004_translations.py
+-rw-r--r--   0        0        0     3660 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/migrations/0005_alter_mtmessagestatus_command_status.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/migrations/__init__.py
+-rw-r--r--   0        0        0     4351 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/models.py
+-rw-r--r--   0        0        0     2246 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/monitoring.py
+-rw-r--r--   0        0        0     1846 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/outgoing.py
+-rw-r--r--   0        0        0     2616 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/queries.py
+-rw-r--r--   0        0        0     2050 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/smpp.py
+-rw-r--r--   0        0        0     2218 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/subscribers.py
+-rw-r--r--   0        0        0     1894 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/src/smpp_gateway/utils.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1697 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/tests/factories.py
+-rw-r--r--   0        0        0      450 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/tests/settings.py
+-rw-r--r--   0        0        0     5104 2023-06-16 19:31:55.937596 smpp_gateway-1.1.0/tests/test_client.py
+-rw-r--r--   0        0        0     7435 2023-06-16 19:31:55.941596 smpp_gateway-1.1.0/tests/test_queries.py
+-rw-r--r--   0        0        0       93 2023-06-16 19:31:55.941596 smpp_gateway-1.1.0/tests/test_smpp_gateway.py
+-rw-r--r--   0        0        0     2633 2023-06-16 19:31:55.941596 smpp_gateway-1.1.0/tests/test_subscribers.py
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 smpp_gateway-1.1.0/PKG-INFO
```

### Comparing `smpp_gateway-1.0.4/LICENSE` & `smpp_gateway-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/pyproject.toml` & `smpp_gateway-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smpp_gateway"
-version = "1.0.4"
+version = "1.1.0"
 description = ""
 authors = [ "Caktus Group <team@caktusgroup.com>" ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/caktus/rapidsms-smpp-gateway"
 
 packages = [ { include = "smpp_gateway", from = "src" } ]
```

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/admin.py` & `smpp_gateway-1.1.0/src/smpp_gateway/admin.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/client.py` & `smpp_gateway-1.1.0/src/smpp_gateway/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import smpplib.gsm
 
 from django.utils import timezone
 from rapidsms.models import Backend
 from smpplib.command import Command, DeliverSM, SubmitSMResp
 
 from smpp_gateway.models import MOMessage, MTMessage, MTMessageStatus
+from smpp_gateway.monitoring import HealthchecksIoWorker
 from smpp_gateway.queries import get_mt_messages_to_send, pg_listen, pg_notify
 from smpp_gateway.utils import decoded_params, set_exit_signals
 
 logger = logging.getLogger(__name__)
 
 
 class PgSmppSequenceGenerator(smpplib.client.SimpleSequenceGenerator):
@@ -64,21 +65,23 @@
     https://gist.github.com/pkese/2790749
     """
 
     def __init__(
         self,
         notify_mo_channel: str,
         backend: Backend,
+        hc_worker: HealthchecksIoWorker,
         submit_sm_params: Dict,
         *args,
         **kwargs,
     ):
         self.exit_signal_received = set_exit_signals()
         self.notify_mo_channel = notify_mo_channel
         self.backend = backend
+        self.hc_worker = hc_worker
         self.submit_sm_params = submit_sm_params
         super().__init__(*args, **kwargs)
         self._pg_conn = pg_listen(self.backend.name)
 
     # ############### Handlers ################
 
     def message_received_handler(self, pdu: DeliverSM):
@@ -239,14 +242,16 @@
                 # backwards-compatible with existing behavior
                 raise socket.timeout()
             for ready_socket in rlist:
                 if ready_socket is self._socket:
                     self.read_once(ignore_error_codes, auto_send_enquire_link)
                 else:
                     self.receive_pg_notifies()
+            if self.hc_worker:
+                self.hc_worker.success_ping()
             if self.exit_signal_received():
                 self.logger.info("Got exit signal, leaving listen loop")
                 self.safe_disconnect()
                 return
 
     def safe_disconnect(self):
         if self._socket is not None:
```

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/management/commands/smpp_client.py` & `smpp_gateway-1.1.0/src/smpp_gateway/management/commands/smpp_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,10 +58,28 @@
         parser.add_argument("--log-file")
         parser.add_argument(
             "--send-bulksms",
             type=int,
             help="Sends the specified number of SMSes in bulk on startup. "
             "Not intended for use with a real MNO.",
         )
+        parser.add_argument(
+            "--hc-check-uuid",
+            default=os.environ.get("HEALTHCHECKS_IO_CHECK_UUID"),
+            help="Pings healthchecks.io with the specified check UUID. "
+            "If set, --hc-ping-key and --hc-check-slug will be ignored.",
+        )
+        parser.add_argument(
+            "--hc-ping-key",
+            default=os.environ.get("HEALTHCHECKS_IO_PING_KEY"),
+            help="Pings healthchecks.io with the specified ping key and check slug. "
+            "If set, --hc-check-slug must also be set.",
+        )
+        parser.add_argument(
+            "--hc-check-slug",
+            default=os.environ.get("HEALTHCHECKS_IO_CHECK_SLUG"),
+            help="Pings healthchecks.io with the specified ping key and check slug. "
+            "If set, --hc-ping-key must also be set.",
+        )
 
     def handle(self, *args, **options):
         start_smpp_client(options)
```

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0001_initial.py` & `smpp_gateway-1.1.0/src/smpp_gateway/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0002_mtmessagestatus.py` & `smpp_gateway-1.1.0/src/smpp_gateway/migrations/0002_mtmessagestatus.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0003_big_pks_and_help_texts.py` & `smpp_gateway-1.1.0/src/smpp_gateway/migrations/0003_big_pks_and_help_texts.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0004_translations.py` & `smpp_gateway-1.1.0/src/smpp_gateway/migrations/0004_translations.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/migrations/0005_alter_mtmessagestatus_command_status.py` & `smpp_gateway-1.1.0/src/smpp_gateway/migrations/0005_alter_mtmessagestatus_command_status.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/models.py` & `smpp_gateway-1.1.0/src/smpp_gateway/models.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/outgoing.py` & `smpp_gateway-1.1.0/src/smpp_gateway/outgoing.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/queries.py` & `smpp_gateway-1.1.0/src/smpp_gateway/queries.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/smpp.py` & `smpp_gateway-1.1.0/src/smpp_gateway/smpp.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,40 @@
 
 from typing import Dict, Optional
 
 from django.db import connection as db_conn
 from rapidsms.models import Backend
 
 from smpp_gateway.client import PgSmppClient, PgSmppSequenceGenerator
+from smpp_gateway.monitoring import HealthchecksIoWorker
 
 logger = logging.getLogger(__name__)
 
 
 def get_smpplib_client(
     host: str,
     port: int,
     notify_mo_channel: str,
     backend: Backend,
     submit_sm_params: Dict,
+    hc_check_uuid: str,
+    hc_ping_key: str,
+    hc_check_slug: str,
 ) -> PgSmppClient:
     sequence_generator = PgSmppSequenceGenerator(db_conn, backend.name)
+    if hc_check_uuid:
+        hc_worker = HealthchecksIoWorker(uuid=hc_check_uuid)
+    elif hc_ping_key and hc_check_slug:
+        hc_worker = HealthchecksIoWorker(ping_key=hc_ping_key, slug=hc_check_slug)
+    else:
+        hc_worker = None
     client = PgSmppClient(
         notify_mo_channel,
         backend,
+        hc_worker,
         submit_sm_params,
         host,
         port,
         allow_unknown_opt_params=True,
         sequence_generator=sequence_generator,
     )
     return client
@@ -52,14 +63,17 @@
     backend, _ = Backend.objects.get_or_create(name=options["backend_name"])
     client = get_smpplib_client(
         options["host"],
         options["port"],
         options["notify_mo_channel"],
         backend,
         json.loads(options["submit_sm_params"]),
+        options["hc_check_uuid"],
+        options["hc_ping_key"],
+        options["hc_check_slug"],
     )
     smpplib_main_loop(
         client,
         options["system_id"],
         options["password"],
         options["interface_version"],
         options["system_type"],
```

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/subscribers.py` & `smpp_gateway-1.1.0/src/smpp_gateway/subscribers.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/src/smpp_gateway/utils.py` & `smpp_gateway-1.1.0/src/smpp_gateway/utils.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/tests/factories.py` & `smpp_gateway-1.1.0/tests/factories.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/tests/test_client.py` & `smpp_gateway-1.1.0/tests/test_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,18 @@
         """
         backend = BackendFactory()
         client = get_smpplib_client(
             "127.0.0.1",
             8000,
             "notify_mo_channel",
             backend,
-            {},
+            {},  # submit_sm_params
+            "",  # hc_check_uuid
+            "",  # hc_ping_key
+            "",  # hc_check_slug
         )
 
         pdu = DeliverSM("deliver_sm")
         pdu.short_message = b"this is a short message"
         pdu.source_addr = "+46166371876"
 
         listen_conn = pg_listen("notify_mo_channel")
@@ -49,15 +52,18 @@
         """
         backend = BackendFactory()
         client = get_smpplib_client(
             "127.0.0.1",
             8000,
             "notify_mo_channel",
             backend,
-            {},
+            {},  # submit_sm_params
+            "",  # hc_check_uuid
+            "",  # hc_ping_key
+            "",  # hc_check_slug
         )
         outbound_msg = MTMessageFactory(status=MTMessage.Status.SENT, backend=backend)
         outbound_msg_status = MTMessageStatusFactory(
             mt_message=outbound_msg, message_id="abcdefg"
         )
 
         pdu = DeliverSM("deliver_sm")
@@ -87,15 +93,18 @@
         and notify the MO listener."""
         backend = BackendFactory()
         client = get_smpplib_client(
             "127.0.0.1",
             8000,
             "notify_mo_channel",
             backend,
-            {},
+            {},  # submit_sm_params
+            "",  # hc_check_uuid
+            "",  # hc_ping_key
+            "",  # hc_check_slug
         )
 
         pdu = DeliverSM("deliver_sm")
         pdu.short_message = None
         pdu.source_addr = "+46166371876"
 
         listen_conn = pg_listen("notify_mo_channel")
@@ -121,15 +130,18 @@
     """
     backend = BackendFactory()
     client = get_smpplib_client(
         "127.0.0.1",
         8000,
         "notify_mo_channel",
         backend,
-        {},
+        {},  # submit_sm_params
+        "",  # hc_check_uuid
+        "",  # hc_ping_key
+        "",  # hc_check_slug
     )
     outbound_msg = MTMessageFactory(status=MTMessage.Status.SENT, backend=backend)
     outbound_msg_status = MTMessageStatusFactory(mt_message=outbound_msg)
 
     pdu = SubmitSMResp("submit_sm_resp")
     pdu.sequence = outbound_msg_status.sequence_number
     pdu.status = smpplib_consts.SMPP_ESME_RSUBMITFAIL
```

### Comparing `smpp_gateway-1.0.4/tests/test_queries.py` & `smpp_gateway-1.1.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/tests/test_subscribers.py` & `smpp_gateway-1.1.0/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `smpp_gateway-1.0.4/PKG-INFO` & `smpp_gateway-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smpp-gateway
-Version: 1.0.4
+Version: 1.1.0
 Summary: 
 Home-page: https://github.com/caktus/rapidsms-smpp-gateway
 License: MIT
 Author: Caktus Group
 Author-email: team@caktusgroup.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -42,14 +42,26 @@
 export SMPPLIB_HOST=localhost
 export SMPPLIB_PORT=2775
 export SMPPLIB_SYSTEM_ID=smppclient1
 export SMPPLIB_PASSWORD=password
 export SMPPLIB_SUBMIT_SM_PARAMS='{"foo": "bar"}'
 ```
 
+#### healthchecks.io support
+
+An integration with healthchecks.io can be enabled by passing the `--hc-uuid` option or setting the `HEALTHCHECKS_IO_UUID` environment variables, for example:
+
+```shell
+export HEALTHCHECKS_IO_UUID=c0c6...
+```
+
+If enabled, the `smpp_client` management command will send a success ping to healthchecks.io for the configured check at most every minute from the main listen loop.
+
+This functionality requires the [healthchecks-io](https://github.com/andrewthetechie/py-healthchecks.io) Python package.
+
 ### `listen_mo_messages`
 
 Listen for mobile-originated (MO) messages:
 
 ```shell
 python manage.py listen_mo_messages --channel new_mo_msg
 ```
```

