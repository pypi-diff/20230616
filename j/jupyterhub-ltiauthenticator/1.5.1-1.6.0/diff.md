# Comparing `tmp/jupyterhub_ltiauthenticator-1.5.1.tar.gz` & `tmp/jupyterhub_ltiauthenticator-1.6.0.tar.gz`

## Comparing `jupyterhub_ltiauthenticator-1.5.1.tar` & `jupyterhub_ltiauthenticator-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/_version.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/__init__.py
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/auth.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/constants.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/handlers.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/templates.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/__init__.py
--rw-r--r--   0        0        0     6984 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/auth.py
--rw-r--r--   0        0        0    14762 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/constants.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/error.py
--rw-r--r--   0        0        0    17269 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/handlers.py
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/validator.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/.gitignore
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/LICENSE
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/README.md
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/_version.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/__init__.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/auth.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/constants.py
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/handlers.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/templates.py
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/__init__.py
+-rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/auth.py
+-rw-r--r--   0        0        0    14762 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/constants.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/error.py
+-rw-r--r--   0        0        0    20090 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/handlers.py
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/validator.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/README.md
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 jupyterhub_ltiauthenticator-1.6.0/PKG-INFO
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/utils.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import logging
 import os
 from typing import Any, Dict, List
 
-from tornado.web import RequestHandler
+from tornado.httputil import HTTPServerRequest
 
 from .lti13.constants import (
     DEFAULT_ROLE_NAMES_FOR_INSTRUCTOR,
     DEFAULT_ROLE_NAMES_FOR_STUDENT,
 )
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
-def get_client_protocol(handler: RequestHandler) -> Dict[str, str]:
-    """
-    This is a copy of the jupyterhub-ltiauthenticator logic to get the first
-    protocol value from the x-forwarded-proto list, assuming there is more than
-    one value. Otherwise, this returns the value as-is.
-
-    Extracted as a method to facilitate testing.
+try:
+    from jupyterhub.utils import get_browser_protocol  # type: ignore
 
-    Args:
-        handler: a tornado.web.RequestHandler object
+# if we are on jupyterhub < 2.0.2
+except ImportError:
 
-    Returns:
-        A decoded dict with keys/values extracted from the request's arguments
-    """
-    if "x-forwarded-proto" in handler.request.headers:
-        hops = [
-            h.strip() for h in handler.request.headers["x-forwarded-proto"].split(",")
-        ]
-        protocol = hops[0]
-    else:
-        protocol = handler.request.protocol
+    def get_browser_protocol(request: HTTPServerRequest) -> str:
+        """
+        This is a copy of the jupyterhub-ltiauthenticator logic to get the first
+        protocol value from the X-Scheme or X-Forwarded-Proto list, assuming there is more than
+        one value. Otherwise, this returns the value as-is.
+
+        Extracted as a method to facilitate testing.
+
+        Args:
+            handler: a tornado.web.RequestHandler object
+
+        Returns:
+            str of protocol seen by browser
+        """
+        proto_header = request.headers.get(
+            "X-Scheme", request.headers.get("X-Forwarded-Proto", None)
+        )
+        if proto_header:
+            hops = [h.strip() for h in proto_header.split(",")]
+            return hops[0]
 
-    return protocol
+        return request.protocol
 
 
 def convert_request_to_dict(arguments: Dict[str, List[bytes]]) -> Dict[str, Any]:
     """
     Converts the arguments obtained from a request to a dict.
 
     Args:
@@ -50,38 +55,38 @@
     """
     args = {}
     for k, values in arguments.items():
         args[k] = values[0].decode()
     return args
 
 
-def user_is_a_student(user_role: str) -> str:
+def user_is_a_student(user_role: str) -> bool:
     """Determins if the user has a Student/Learner role.
 
     Args:
         user_role: the user's rule
 
     Returns:
         Lower case student string
     """
     if not user_role:
         raise ValueError("user_role must have a value")
     return user_role.lower() in DEFAULT_ROLE_NAMES_FOR_STUDENT
 
 
-def user_is_an_instructor(user_role: str) -> str:
+def user_is_an_instructor(user_role: str) -> bool:
     """Determins if the user has a Instructor/Teacher role.
 
     Args:
         user_role: the user's rule
 
     Returns:
         Lower case instructor string
     """
     if not user_role:
         raise ValueError("user_role must have a value")
     # find the extra role names to recognize an instructor (to be added in the grader group)
-    extra_roles = os.environ.get("EXTRA_ROLE_NAMES_FOR_INSTRUCTOR") or []
+    extra_roles: str = os.environ.get("EXTRA_ROLE_NAMES_FOR_INSTRUCTOR") or ""
     if extra_roles:
         extra_roles = extra_roles.lower().split(",")
         DEFAULT_ROLE_NAMES_FOR_INSTRUCTOR.extend(extra_roles)
     return user_role.lower() in DEFAULT_ROLE_NAMES_FOR_INSTRUCTOR
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/auth.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from textwrap import dedent
 
-from jupyterhub.app import JupyterHub
-from jupyterhub.auth import Authenticator
-from jupyterhub.handlers import BaseHandler
-from jupyterhub.utils import url_path_join
+from jupyterhub.app import JupyterHub  # type: ignore
+from jupyterhub.auth import Authenticator  # type: ignore
+from jupyterhub.handlers import BaseHandler  # type: ignore
+from jupyterhub.utils import url_path_join  # type: ignore
 from tornado.web import HTTPError
-from traitlets.config import Dict, Unicode
+from traitlets import CaselessStrEnum, Dict, Unicode
 
-from ..utils import convert_request_to_dict, get_client_protocol
+from ..utils import convert_request_to_dict, get_browser_protocol
 from .handlers import LTI11AuthenticateHandler, LTI11ConfigHandler
 from .validator import LTI11LaunchValidator
 
 
 class LTI11Authenticator(Authenticator):
     """
     JupyterHub LTI 1.1 Authenticator which extends the ltiauthenticator.LTIAuthenticator class.
@@ -83,14 +83,29 @@
         To preserve legacy behavior, if custom_canvas_user_id is present in the LTI
         request, it is used as the username. If not, user_id is used. In the future,
         the default will be just user_id - if you want to use custom_canvas_user_id,
         you must explicitly set username_key to custom_canvas_user_id.
         """,
     )
 
+    uri_scheme = CaselessStrEnum(
+        ("auto", "https", "http"),
+        default_value="auto",
+        config=True,
+        help="""
+        Scheme to use for endpoint URLs offered by this authenticator.
+
+        Possible values are "auto", "https" and "http", where "auto" is the default.
+        When "auto" is chosen, the scheme is inferred from the incomming request's header.
+        Since this may lead to unreliable results in some deployment scenarios (in particular
+        when several different versions of forwarding headers are mixed), manually specifying it
+        here is kept as an escape hatch.
+        """,
+    )
+
     def login_url(self, base_url: str) -> str:
         return url_path_join(base_url, "/lti/launch")
 
     def get_handlers(self, app: JupyterHub) -> BaseHandler:
         return [
             ("/lti/launch", LTI11AuthenticateHandler),
             ("/lti11/config", LTI11ConfigHandler),
@@ -128,15 +143,15 @@
         )
 
         # extract the request arguments to a dict
         args = convert_request_to_dict(handler.request.arguments)
         self.log.debug(f"Decoded args from request: {args}")
 
         # get the origin protocol
-        protocol = get_client_protocol(handler)
+        protocol = self.get_uri_scheme(handler.request)
         self.log.debug(f"Origin protocol is: {protocol}")
 
         # build the full launch url value required for oauth1 signatures
         launch_url = f"{protocol}://{handler.request.host}{handler.request.uri}"
         self.log.debug(f"Launch url is: {launch_url}")
 
         if validator.validate_launch_request(launch_url, handler.request.headers, args):
@@ -162,7 +177,14 @@
             # except for the oauth_* arguments.
             return {
                 "name": username,
                 "auth_state": {
                     k: v for k, v in args.items() if not k.startswith("oauth_")
                 },
             }
+
+    def get_uri_scheme(self, request) -> str:
+        """Return scheme to use for endpoint URLs of this authenticator."""
+        if self.uri_scheme == "auto":
+            return get_browser_protocol(request)
+        # manually specified https or http
+        return self.uri_scheme
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/constants.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/handlers.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from jupyterhub.handlers import BaseHandler
+from jupyterhub.handlers import BaseHandler  # type: ignore
 from tornado import gen
 
-from ..utils import get_client_protocol
 from .templates import LTI11_CONFIG_TEMPLATE
 
 
 class LTI11AuthenticateHandler(BaseHandler):
     """
     Implements v1.1 of the LTI protocol for passing authentication information
     through.
@@ -73,15 +72,15 @@
     def get(self) -> None:
         """
         Renders the XML config which is used by LTI consumers to install the external tool.
         """
         self.set_header("Content-Type", "application/xml")
 
         # get the launch url from the client request
-        protocol = get_client_protocol(self)
+        protocol = self.authenticator.get_uri_scheme(self.request)
         launch_url = f"{protocol}://{self.request.host}{self.application.settings['base_url']}hub/lti/launch"
         self.log.debug(f"Calculated launch URL is: {launch_url}")
 
         # build the configuration XML
         config_xml = LTI11_CONFIG_TEMPLATE.format(
             description=self.authenticator.config_description,
             icon=self.authenticator.config_icon,
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/templates.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/templates.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti11/validator.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti11/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from collections import OrderedDict
 from typing import Any, Dict
 from typing import OrderedDict as OrderedDictType
 
-from oauthlib.common import safe_string_equals
-from oauthlib.oauth1.rfc5849 import Client, signature
+from oauthlib.common import safe_string_equals  # type: ignore
+from oauthlib.oauth1.rfc5849 import Client, signature  # type: ignore
 from tornado.web import HTTPError
 from traitlets.config import LoggingConfigurable
 
 from .constants import LTI11_LAUNCH_PARAMS_REQUIRED, LTI11_OAUTH_ARGS
 
 
 class LTI11LaunchValidator(LoggingConfigurable):
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/auth.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 import logging
 from typing import Any, Dict, List
 
-from jupyterhub.app import JupyterHub
-from jupyterhub.auth import LocalAuthenticator
-from jupyterhub.handlers import BaseHandler
-from jupyterhub.utils import url_path_join
-from oauthenticator.oauth2 import OAuthenticator
+from jupyterhub.app import JupyterHub  # type: ignore
+from jupyterhub.auth import Authenticator  # type: ignore
+from jupyterhub.handlers import BaseHandler  # type: ignore
+from jupyterhub.utils import url_path_join  # type: ignore
+from traitlets import CaselessStrEnum
 from traitlets import List as TraitletsList
+from traitlets import Set as TraitletsSet
 from traitlets import Unicode
 
+from ..utils import get_browser_protocol
 from .constants import LTI13_CUSTOM_CLAIM
 from .error import LoginError
 from .handlers import LTI13CallbackHandler, LTI13ConfigHandler, LTI13LoginInitHandler
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
-class LTI13Authenticator(OAuthenticator):
+class LTI13Authenticator(Authenticator):
     """
-    JupyterHub LTI 1.3 Authenticator which extends the `OAuthenticator` class. (LTI 1.3
-    is basically an extension of OIDC/OAuth2). Messages sent to this authenticator are sent
-    from a LTI 1.3 Platform, such as an LMS. JupyterHub, as the authenticator, works as the
-    LTI 1.3 External Tool. The basic login flow is authentication using the implicit flow. As such,
-    the client id is always required.
-
-    This class utilizes the following required configurables defined in the `OAuthenticator` base class:
-
-        - authorize_url
-        - client_id
+    JupyterHub LTI 1.3 Authenticator. LTI 1.3 is basically an extension of OIDC/OAuth2.
+    Messages sent to this authenticator are sent from a LTI 1.3 Platform, such as an LMS.
+    JupyterHub, as the authenticator, works as the LTI 1.3 External Tool.
+    The basic login flow is authentication using the implicit flow.
+    As such, at least one client id is required.
 
     Ref:
-      - https://github.com/jupyterhub/oauthenticator/blob/master/oauthenticator/oauth2.py
       - http://www.imsglobal.org/spec/lti/v1p3/
       - https://openid.net/specs/openid-connect-core-1_0.html#ImplicitFlowAuth
     """
 
     login_service = "LTI 1.3"
 
-    # handlers used for login, callback, and jwks endpoints
+    # handlers used for login, callback, and json config endpoints
     login_handler = LTI13LoginInitHandler
     callback_handler = LTI13CallbackHandler
+    config_handler = LTI13ConfigHandler
+
+    authorize_url = Unicode(
+        config=True,
+        help="""Authorization end-point of the platforms identity provider.""",
+    )
+
+    client_id = TraitletsSet(
+        trait=Unicode(),
+        config=True,
+        help="""
+        The client ID or a list of client IDs identifying the JuyterHub within the LMS platform.
+        Must contain the client IDs created when registering the tool on the LMS platform.
+
+        Possible values are of type str or iterables thereof.
+        """,
+    )
 
     jwks_algorithms = TraitletsList(
         default_value=["RS256"],
         config=True,
         help="""
         Supported algorithms for signing JWT. The actual algorithm is declared by the authenticator
         in the `id_token_signed_response_alg` parameter during out-of-band registration.
@@ -97,14 +110,29 @@
         your vendor's standard LTI 1.3 login initiation flow request.
 
         Reference to the IMS LTI specification on variable substitutions:
         http://www.imsglobal.org/spec/lti/v1p3/#customproperty.
         """,
     )
 
+    uri_scheme = CaselessStrEnum(
+        ("auto", "https", "http"),
+        default_value="auto",
+        config=True,
+        help="""
+        Scheme to use for endpoint URLs offered by this authenticator.
+
+        Possible values are "auto", "https" and "http", where "auto" is the default.
+        When "auto" is chosen, the scheme is inferred from the incomming request's header.
+        Since this may lead to unreliable results in some deployment scenarios (in particular
+        when several different versions of forwarding headers are mixed), manually specifying it
+        here is kept as an escape hatch.
+        """,
+    )
+
     tool_name = Unicode(
         "JupyterHub",
         config=True,
         help="""
         Name of tool provided to the LMS when installed via the config URL.
 
         This is primarily used for display purposes.
@@ -130,27 +158,26 @@
     def config_json_url(self, base_url):
         return url_path_join(base_url, "lti13", "config")
 
     def get_handlers(self, app: JupyterHub) -> List[BaseHandler]:
         return [
             (self.login_url(""), self.login_handler),
             (self.callback_url(""), self.callback_handler),
-            (self.config_json_url(""), LTI13ConfigHandler),
+            (self.config_json_url(""), self.config_handler),
         ]
 
     async def authenticate(
         self, handler: LTI13LoginInitHandler, data: Dict[str, str] = None
     ) -> Dict[str, Any]:
         """
-        Overrides authenticate from the OAuthenticator base class to handle LTI
-        1.3 launch requests based on a passed JWT.
+        Handles LTI 1.3 launch requests based on a passed JWT.
 
         Args:
           handler: handler object
-          data: authentication dictionary. The decoded, verified and validated id_token send by tehe platform
+          data: authentication dictionary. The decoded, verified and validated id_token send by the platform
 
         Returns:
           Authentication dictionary
         """
         if not data:
             data = {}
 
@@ -187,12 +214,13 @@
             username = token.get("sub")
         if not username:
             raise LoginError(
                 f"Unable to set the username with username_key {username_key}"
             )
         return username
 
-
-class LocalLTI13Authenticator(LocalAuthenticator, OAuthenticator):
-    """A version that mixes in local system user creation"""
-
-    pass
+    def get_uri_scheme(self, request) -> str:
+        """Return scheme to use for endpoint URLs of this authenticator."""
+        if self.uri_scheme == "auto":
+            return get_browser_protocol(request)
+        # manually specified https or http
+        return self.uri_scheme
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/constants.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/error.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/error.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/handlers.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/handlers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+import base64
 import hashlib
 import json
 import re
 import uuid
 from typing import Any, Dict, Optional, cast
 from urllib.parse import quote, unquote, urlparse
 
-from jupyterhub.handlers import BaseHandler
-from jupyterhub.utils import url_path_join
-from oauthenticator.oauth2 import (
-    OAuthCallbackHandler,
-    OAuthLoginHandler,
-    _serialize_state,
-)
-from oauthlib.common import generate_token
+from jupyterhub.handlers import BaseHandler  # type: ignore
+from jupyterhub.utils import url_path_join  # type: ignore
+from oauthlib.common import generate_token  # type: ignore
 from tornado.httputil import url_concat
-from tornado.web import HTTPError, RequestHandler
+from tornado.log import app_log
+from tornado.web import HTTPError, MissingArgumentError, RequestHandler
 
-from ..utils import convert_request_to_dict, get_client_protocol
+from ..utils import convert_request_to_dict
 from .error import InvalidAudienceError, LoginError, ValidationError
 from .validator import LTI13LaunchValidator
 
+STATE_COOKIE_NAME = "lti13authenticator-state"
 NONCE_STATE_COOKIE_NAME = "lti13authenticator-nonce-state"
 
 
 def make_nonce_state() -> str:
     """
     Create state for nonce calculation.
     """
@@ -37,14 +35,36 @@
     SHA 256 is used to create the hash. The nonce is its hexdigest.
     """
     hash = hashlib.sha256(nonce_state.encode())
     nonce = hash.hexdigest()
     return nonce
 
 
+def _serialize_state(state):
+    """Serialize OAuth state to a base64 string after passing through JSON"""
+    json_state = json.dumps(state)
+    return base64.urlsafe_b64encode(json_state.encode("utf8")).decode("ascii")
+
+
+def _deserialize_state(b64_state):
+    """Deserialize OAuth state as serialized in _serialize_state"""
+    if isinstance(b64_state, str):
+        b64_state = b64_state.encode("ascii")
+    try:
+        json_state = base64.urlsafe_b64decode(b64_state).decode("utf8")
+    except ValueError:
+        app_log.error(f"Failed to b64-decode state: {b64_state}")
+        return {}
+    try:
+        return json.loads(json_state)
+    except ValueError:
+        app_log.error(f"Failed to json-decode state: {json_state}")
+        return {}
+
+
 class LTI13ConfigHandler(BaseHandler):
     """
     Handles JSON configuration file for LTI 1.3.
     """
 
     async def get(self) -> None:
         """
@@ -59,15 +79,15 @@
         - Usernames are obtained by first attempting to get and normalize values sent when
         tools are installed with public settings. If private, the username is set using the
         anonumized user data when requests are sent with private installation settings.
         """
         self.set_header("Content-Type", "application/json")
 
         # get the origin protocol
-        protocol = get_client_protocol(self)
+        protocol = self.authenticator.get_uri_scheme(self.request)
         self.log.debug(f"Origin protocol is: {protocol}")
         # build the full target link url value required for the jwks endpoint
         target_link_url = f"{protocol}://{self.request.host}"
         self.log.debug(f"Target link url is: {target_link_url}")
         keys = {
             "title": self.authenticator.tool_name,
             "scopes": [
@@ -121,20 +141,22 @@
             "oidc_initiation_url": self.authenticator.login_url(
                 url_path_join(target_link_url, self.hub.server.base_url)
             ),
         }
         self.write(json.dumps(keys))
 
 
-class LTI13LoginInitHandler(OAuthLoginHandler):
+class LTI13LoginInitHandler(BaseHandler):
     """
     Handles JupyterHub authentication requests according to the
     LTI 1.3 standard.
     """
 
+    _state = None
+
     def check_xsrf_cookie(self):
         """
         Do not attempt to check for xsrf parameter in POST requests. LTI requests are
         meant to be cross-site, so it must not be verified.
         """
         return
 
@@ -253,50 +275,55 @@
         # would be a good way to implement this.
         # lti_deployment_id = self._get_optional_arg(args, "lti_deployment_id")
 
         redirect_uri = self.get_redirect_uri()
         self.log.debug(f"redirect_uri is: {redirect_uri}")
 
         # to prevent CSRF
-        state = self.get_state()
-        self.set_state_cookie(state)
+        state = self.generate_state()
 
         # to prevent replay attacks
         nonce = self.generate_nonce()
         self.log.debug(f"nonce value: {nonce}")
 
         self.authorize_redirect(
             client_id=client_id,
             login_hint=login_hint,
             lti_message_hint=lti_message_hint,
             nonce=nonce,
             redirect_uri=redirect_uri,
             state=state,
         )
 
-    # GET requests are also allowed by the OpenID Conect launch flow:
+    # GET requests are also allowed by the OpenID Connect launch flow:
     # https://www.imsglobal.org/spec/security/v1p0/#fig_oidcflow
     #
     get = post
 
+    def generate_state(self):
+        """Produce a state including the url of the original request."""
+        state = self.get_state()
+        self.set_state_cookie(state)
+        return state
+
     def generate_nonce(self):
         """Produce a nonce.
 
         The nonce state will be stored as a session cookie to later validate the nonce
         field of the id_token.
         """
         nonce_state = make_nonce_state()
-        self.set_nonce_cookie(nonce_state)
+        self.set_nonce_state_cookie(nonce_state)
         nonce = get_nonce(nonce_state)
         return nonce
 
     def get_redirect_uri(self) -> str:
         """Create uri to redirect user agent to after successful authorization by the LMS platform."""
         return "{proto}://{host}{path}".format(
-            proto=self.request.protocol,
+            proto=self.authenticator.get_uri_scheme(self.request),
             host=self.request.host,
             path=self.authenticator.callback_url(self.hub.server.base_url),
         )
 
     def _get_optional_arg(self, args: Dict[str, str], arg: str) -> Optional[str]:
         """
         Return value of optional argument or None if not present.
@@ -304,34 +331,41 @@
         value = args.get(arg)
         if value:
             self.log.debug(f"{arg} is {value}")
         else:
             self.log.debug(f"{arg} not present in login initiation request")
         return value
 
-    def set_nonce_cookie(self, nonce_state):
+    def set_nonce_state_cookie(self, nonce_state):
+        self._set_oauth_cookie(NONCE_STATE_COOKIE_NAME, nonce_state)
+
+    def set_state_cookie(self, state):
+        self._set_oauth_cookie(STATE_COOKIE_NAME, state)
+
+    def _set_oauth_cookie(self, key: str, value):
         self._set_cookie(
-            NONCE_STATE_COOKIE_NAME,
-            nonce_state,
+            key,
+            value,
             expires_days=1,
             httponly=True,
             encrypted=True,
         )
 
 
-class LTI13CallbackHandler(OAuthCallbackHandler):
+class LTI13CallbackHandler(BaseHandler):
     """
     Handles JupyterHub authentication requests responses according to the
     LTI 1.3 standard.
 
     References:
     https://www.imsglobal.org/spec/security/v1p0/#step-3-authentication-response
     https://www.imsglobal.org/spec/security/v1p0/#step-4-resource-is-displayed
     """
 
+    _state_cookie = None
     _nonce_state_cookie = None
 
     def check_xsrf_cookie(self):
         """
         Do not attempt to check for xsrf parameter in POST requests. LTI requests are
         meant to be cross-site, so it must not be verified.
         """
@@ -404,32 +438,76 @@
         # References:
         # https://openid.net/specs/openid-connect-core-1_0.html#NonceNotes
         # https://auth0.com/docs/get-started/authentication-and-authorization-flow/mitigate-replay-attacks-when-using-the-implicit-flow
         self.check_nonce(id_token)
 
         return id_token
 
+    def check_state(self):
+        """Verify OAuth state
+
+        compare value in cookie with redirect url param
+        """
+        cookie_state = self._get_state_cookie()
+        if not cookie_state:
+            raise HTTPError(400, "OAuth state missing from cookies")
+        url_state = self._get_state_from_url()
+        if cookie_state != url_state:
+            self.log.warning(f"OAuth state mismatch: {cookie_state} != {url_state}")
+            raise HTTPError(400, "OAuth state mismatch")
+
     def check_nonce(self, id_token: Dict[str, Any]) -> None:
         """Check if received nonce corresponds to hash of nonce state cookie"""
         received_nonce = id_token.get("nonce")
 
         nonce_state = self._get_nonce_state_cookie()
         if not nonce_state:
             raise HTTPError(400, "Missing nonce state cookie")
 
         nonce = get_nonce(nonce_state)
 
         if nonce != received_nonce:
             self.log.warning("OAuth nonce mismatch: %s != %s", nonce, received_nonce)
             raise HTTPError(400, "OAuth nonce mismatch")
 
+    def get_next_url(self, user=None):
+        """Get the redirect target from the state field"""
+        state = self._get_state_from_url()
+        next_url = _deserialize_state(state).get("next_url")
+        if next_url:
+            return next_url
+        # JupyterHub 0.8 adds default .get_next_url for a fallback
+        return super().get_next_url(user)
+
+    def _get_state_from_url(self):
+        """Get OAuth state from URL parameters
+
+        Raises HTTPError(400) if `state` argument is missing from request.
+        """
+        try:
+            return self.get_argument("state")
+        except MissingArgumentError:
+            raise HTTPError(400, "OAuth state missing from URL")
+
     def _get_nonce_state_cookie(self):
         """Get OAuth nonce state from cookies
 
         To be compared with the value in id_token
         """
         if self._nonce_state_cookie is None:
-            self._nonce_state_cookie = (
-                self.get_secure_cookie(NONCE_STATE_COOKIE_NAME) or b""
-            ).decode("utf8")
-            self.clear_cookie(NONCE_STATE_COOKIE_NAME)
+            self._nonce_state_cookie = self._get_oauth_cookie(NONCE_STATE_COOKIE_NAME)
         return self._nonce_state_cookie
+
+    def _get_state_cookie(self):
+        """Get OAuth state from cookies
+
+        To be compared with the value in redirect URL
+        """
+        if self._state_cookie is None:
+            self._state_cookie = self._get_oauth_cookie(STATE_COOKIE_NAME)
+        return self._state_cookie
+
+    def _get_oauth_cookie(self, name: str):
+        """Get OAuth state cookie."""
+        cookie = (self.get_secure_cookie(name) or b"").decode("utf8", "replace")
+        self.clear_cookie(name)
+        return cookie
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/ltiauthenticator/lti13/validator.py` & `jupyterhub_ltiauthenticator-1.6.0/ltiauthenticator/lti13/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,26 +179,28 @@
             "https://purl.imsglobal.org/spec/lti/claim/resource_link", {}
         ).get("id")
         if not id:
             raise MissingRequiredArgumentError(
                 "resource_link claim's id can't be empty"
             )
 
-    def validate_azp_claim(self, id_token: Dict[str, Any], client_id: str) -> None:
+    def validate_azp_claim(
+        self, id_token: Dict[str, Any], client_id: Iterable[str]
+    ) -> None:
         """Check if azp claim is present and matches client_id."""
         aud = id_token["aud"]
         need_azp = isinstance(id_token["aud"], list) and len(aud) > 1
         if not need_azp:
             return
         azp = id_token.get("azp")
         if not azp:
             raise MissingRequiredArgumentError(
                 "azp claim is missing although multiple values for aud are given."
             )
-        if azp != client_id:
+        if azp not in client_id:
             raise InvalidAudienceError("azp claim does not match client_id.")
 
     def _check_if_iat_is_too_old(self, id_token: Dict[str, Any]) -> None:
         """Raise TokenError if iat is too old."""
         iat = id_token["iat"]
         if iat < now() - self.max_age - self.time_leeway:
             raise TokenError("id_token issued too long ago.")
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/.gitignore` & `jupyterhub_ltiauthenticator-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.1/LICENSE` & `jupyterhub_ltiauthenticator-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.1/README.md` & `jupyterhub_ltiauthenticator-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_ltiauthenticator-1.5.1/pyproject.toml` & `jupyterhub_ltiauthenticator-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     {name = "Jupyter Contributors", email = "jupyter@googlegroups.com"},
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
+    "traitlets>=5.1.0",
     "escapism>=1.0.1",
     "jupyterhub>=1.2",
-    "oauthenticator>=15.1.0",
     "oauthlib>=3.2.2",
     "PyJWT[crypto]>=2.7.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
@@ -121,15 +121,15 @@
 #
 # ref: https://github.com/your-tools/tbump#readme
 #
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/ltiauthenticator"
 
 [tool.tbump.version]
-current = "1.5.1"
+current = "1.6.0"
 regex = '''
     (?P<major>\d+)
     \.
     (?P<minor>\d+)
     \.
     (?P<patch>\d+)
     (?P<pre>((a|b|rc)\d+)|)
```

### Comparing `jupyterhub_ltiauthenticator-1.5.1/PKG-INFO` & `jupyterhub_ltiauthenticator-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-ltiauthenticator
-Version: 1.5.1
+Version: 1.6.0
 Summary: JupyterHub authenticator implementing LTI v1.1 and LTI v1.3
 Project-URL: Documentation, https://ltiauthenticator.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/ltiauthenticator
 Project-URL: Issues, https://github.com/jupyterhub/ltiauthenticator/issues
 Author-email: Yuvi Panda <yuvipanda@gmail.com>, Jupyter Contributors <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -38,17 +38,17 @@
 License-File: LICENSE
 Keywords: authenticator,jupyterhub
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: escapism>=1.0.1
 Requires-Dist: jupyterhub>=1.2
-Requires-Dist: oauthenticator>=15.1.0
 Requires-Dist: oauthlib>=3.2.2
 Requires-Dist: pyjwt[crypto]>=2.7.0
+Requires-Dist: traitlets>=5.1.0
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

