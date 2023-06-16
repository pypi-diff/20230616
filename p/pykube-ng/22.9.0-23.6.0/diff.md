# Comparing `tmp/pykube-ng-22.9.0.tar.gz` & `tmp/pykube-ng-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykube-ng-22.9.0.tar", max compression
+gzip compressed data, was "pykube-ng-23.6.0.tar", max compression
```

## Comparing `pykube-ng-22.9.0.tar` & `pykube-ng-23.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11358 2019-03-03 09:09:47.928815 pykube-ng-22.9.0/LICENSE
--rw-r--r--   0        0        0     6574 2020-10-11 13:14:53.284204 pykube-ng-22.9.0/README.rst
--rw-r--r--   0        0        0      862 2022-09-18 13:43:33.522752 pykube-ng-22.9.0/pykube/__init__.py
--rw-r--r--   0        0        0       34 2019-04-14 11:23:34.881587 pykube-ng-22.9.0/pykube/__main__.py
--rw-r--r--   0        0        0    11036 2022-09-18 13:20:44.821981 pykube-ng-22.9.0/pykube/config.py
--rw-r--r--   0        0        0     1720 2020-10-03 11:25:05.829332 pykube-ng-22.9.0/pykube/console.py
--rw-r--r--   0        0        0      415 2020-10-03 11:25:05.829332 pykube-ng-22.9.0/pykube/exceptions.py
--rw-r--r--   0        0        0    18552 2022-09-18 13:20:44.821981 pykube-ng-22.9.0/pykube/http.py
--rw-r--r--   0        0        0      844 2020-10-03 11:25:05.829332 pykube-ng-22.9.0/pykube/mixins.py
--rw-r--r--   0        0        0    19446 2022-09-18 13:20:44.821981 pykube-ng-22.9.0/pykube/objects.py
--rw-r--r--   0        0        0     8741 2022-09-18 13:20:44.821981 pykube-ng-22.9.0/pykube/query.py
--rw-r--r--   0        0        0     2430 2020-10-03 11:25:05.829332 pykube-ng-22.9.0/pykube/utils.py
--rw-r--r--   0        0        0     1460 2022-09-18 13:43:34.090749 pykube-ng-22.9.0/pyproject.toml
--rw-r--r--   0        0        0     7648 1970-01-01 00:00:00.000000 pykube-ng-22.9.0/setup.py
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 pykube-ng-22.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2019-03-03 09:09:47.928815 pykube-ng-23.6.0/LICENSE
+-rw-r--r--   0        0        0     6574 2020-10-11 13:14:53.284204 pykube-ng-23.6.0/README.rst
+-rw-r--r--   0        0        0      862 2023-06-16 17:58:38.379356 pykube-ng-23.6.0/pykube/__init__.py
+-rw-r--r--   0        0        0       34 2019-04-14 11:23:34.881587 pykube-ng-23.6.0/pykube/__main__.py
+-rw-r--r--   0        0        0    11033 2023-04-07 13:13:30.917689 pykube-ng-23.6.0/pykube/config.py
+-rw-r--r--   0        0        0     1720 2020-10-03 11:25:05.829332 pykube-ng-23.6.0/pykube/console.py
+-rw-r--r--   0        0        0      415 2020-10-03 11:25:05.829332 pykube-ng-23.6.0/pykube/exceptions.py
+-rw-r--r--   0        0        0    18563 2023-06-16 17:55:54.639099 pykube-ng-23.6.0/pykube/http.py
+-rw-r--r--   0        0        0      843 2023-04-07 13:13:30.505690 pykube-ng-23.6.0/pykube/mixins.py
+-rw-r--r--   0        0        0    19583 2023-04-07 13:21:01.188193 pykube-ng-23.6.0/pykube/objects.py
+-rw-r--r--   0        0        0     8819 2023-04-07 13:22:13.187310 pykube-ng-23.6.0/pykube/query.py
+-rw-r--r--   0        0        0     2430 2020-10-03 11:25:05.829332 pykube-ng-23.6.0/pykube/utils.py
+-rw-r--r--   0        0        0     1460 2023-06-16 17:58:38.923356 pykube-ng-23.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7648 1970-01-01 00:00:00.000000 pykube-ng-23.6.0/setup.py
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 pykube-ng-23.6.0/PKG-INFO
```

### Comparing `pykube-ng-22.9.0/LICENSE` & `pykube-ng-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykube-ng-22.9.0/README.rst` & `pykube-ng-23.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pykube-ng-22.9.0/pykube/__init__.py` & `pykube-ng-23.6.0/pykube/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Python client for Kubernetes
 """
 
-__version__ = "22.9.0"
+__version__ = "23.6.0"
 
 from .config import KubeConfig  # noqa: F401
 from .exceptions import KubernetesError, PyKubeError, ObjectDoesNotExist  # noqa: F401
 from .http import HTTPClient  # noqa: F401
 from .objects import (  # noqa: F401
     object_factory,
     ConfigMap,
```

### Comparing `pykube-ng-22.9.0/pykube/config.py` & `pykube-ng-23.6.0/pykube/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,14 @@
     def namespace(self) -> str:
         """
         Returns the current context namespace by exposing as a read-only property.
         """
         return self.contexts[self.current_context].get("namespace", "default")
 
     def persist_doc(self):
-
         if not self.kubeconfig_path:
             # Config was provided as string, not way to persit it
             return
         with self.kubeconfig_path.open("w") as f:
             yaml.safe_dump(
                 self.doc,
                 f,
@@ -291,15 +290,14 @@
            - `data`: base64 encoded bytes
         """
         self._path = None
         self._bytes = None
         if filename is not None and data is not None:
             raise TypeError("filename or data kwarg must be specified, not both")
         elif filename is not None:
-
             path = Path(filename)
             # If relative path is given, should be made absolute with respect to the directory of the kube config
             # https://kubernetes.io/docs/concepts/configuration/organize-cluster-access-kubeconfig/#file-references
             if not path.is_absolute():
                 if kubeconfig_path:
                     path = kubeconfig_path.parent.joinpath(path)
                 else:
@@ -330,15 +328,14 @@
             return self._bytes
 
     def filename(self):
         """
         Returns the provided data as a file location.
         """
         if not self._path:
-
             m = hashlib.md5()
             m.update(self._bytes)
 
             path = Path(f"{tempfile.gettempdir()}/pykube-ng.{m.hexdigest()}.crt")
             if not path.exists() or path.stat().st_size == 0:
                 with open(path, "wb") as f:
                     f.write(self._bytes)
```

### Comparing `pykube-ng-22.9.0/pykube/console.py` & `pykube-ng-23.6.0/pykube/console.py`

 * *Files identical despite different names*

### Comparing `pykube-ng-22.9.0/pykube/http.py` & `pykube-ng-23.6.0/pykube/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 DEFAULT_HTTP_TIMEOUT = 10  # seconds
 EXPIRY_SKEW_PREVENTION_DELAY = datetime.timedelta(minutes=5)
 UTC = datetime.timezone.utc
 LOG = logging.getLogger(__name__)
 
 
 class KubernetesHTTPAdapter(requests.adapters.HTTPAdapter):
-
     # _do_send: the actual send method of HTTPAdapter
     # it can be overwritten in unit tests to mock the actual HTTP calls
     _do_send = requests.adapters.HTTPAdapter.send
 
     def __init__(self, kube_config: KubeConfig, **kwargs):
         self.kube_config = kube_config
 
@@ -222,15 +221,15 @@
                 )
 
             cmd_env_vars = dict(os.environ)
             for env_var in exec_conf.get("env") or []:
                 cmd_env_vars[env_var["name"]] = env_var["value"]
 
             output = subprocess.check_output(
-                [exec_conf["command"]] + exec_conf["args"], env=cmd_env_vars
+                [exec_conf["command"]] + (exec_conf.get("args") or []), env=cmd_env_vars
             )
 
             parsed_out = json.loads(output)
             status = parsed_out["status"]
 
             if status.get("token"):
                 token = status["token"]
```

### Comparing `pykube-ng-22.9.0/pykube/mixins.py` & `pykube-ng-23.6.0/pykube/mixins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 
 
 class ReplicatedMixin:
-
     scalable_attr = "replicas"
 
     @property
     def replicas(self):
         return self.obj["spec"]["replicas"]
 
     @replicas.setter
```

### Comparing `pykube-ng-22.9.0/pykube/objects.py` & `pykube-ng-23.6.0/pykube/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .mixins import ScalableMixin
 from .query import Query
 from .utils import join_url_path
 from .utils import obj_merge
 
 
 class ObjectManager:
-    def __call__(self, api: HTTPClient, namespace: str = None):
+    def __call__(self, api: HTTPClient, namespace: Optional[str] = None):
         if namespace is None and NamespacedAPIObject in getmro(self.api_obj_class):
             namespace = api.config.namespace
         return Query(api, self.api_obj_class, namespace=namespace)
 
     def __get__(self, obj, api_obj_class: Type):
         assert obj is None, "cannot invoke objects on resource object."
         self.api_obj_class = api_obj_class
@@ -160,15 +160,15 @@
     def update(self, is_strategic=True, *, subresource=None):
         """
         Update the Kubernetes resource by calling the API (patch)
         """
         self.obj = obj_merge(self.obj, self._original_obj, is_strategic)
         self.patch(self.obj, subresource=subresource)
 
-    def delete(self, propagation_policy: str = None):
+    def delete(self, propagation_policy: Optional[str] = None):
         """
         Delete the Kubernetes resource by calling the API.
 
         The parameter propagation_policy defines whether to cascade the delete. It can be "Foreground", "Background" or "Orphan".
         See https://kubernetes.io/docs/concepts/workloads/controllers/garbage-collection/#setting-the-cascading-deletion-policy
         """
         if propagation_policy:
@@ -230,15 +230,15 @@
 class ConfigMap(NamespacedAPIObject):
     version = "v1"
     endpoint = "configmaps"
     kind = "ConfigMap"
 
 
 class CronJob(NamespacedAPIObject):
-    version = "batch/v1beta1"
+    version = "batch/v1"
     endpoint = "cronjobs"
     kind = "CronJob"
 
 
 class DaemonSet(NamespacedAPIObject):
     version = "apps/v1"
     endpoint = "daemonsets"
@@ -553,15 +553,15 @@
 class PersistentVolumeClaim(NamespacedAPIObject):
     version = "v1"
     endpoint = "persistentvolumeclaims"
     kind = "PersistentVolumeClaim"
 
 
 class HorizontalPodAutoscaler(NamespacedAPIObject):
-    version = "autoscaling/v1"
+    version = "autoscaling/v2"
     endpoint = "horizontalpodautoscalers"
     kind = "HorizontalPodAutoscaler"
 
 
 class StatefulSet(NamespacedAPIObject, ReplicatedMixin, ScalableMixin):
     version = "apps/v1"
     endpoint = "statefulsets"
@@ -588,22 +588,24 @@
 
 class ClusterRoleBinding(APIObject):
     version = "rbac.authorization.k8s.io/v1"
     endpoint = "clusterrolebindings"
     kind = "ClusterRoleBinding"
 
 
+# PodSecurityPolicy no longer exists in v1.25
+# see https://kubernetes.io/docs/reference/using-api/deprecation-guide/#psp-v125
 class PodSecurityPolicy(APIObject):
     version = "policy/v1beta1"
     endpoint = "podsecuritypolicies"
     kind = "PodSecurityPolicy"
 
 
 class PodDisruptionBudget(NamespacedAPIObject):
-    version = "policy/v1beta1"
+    version = "policy/v1"
     endpoint = "poddisruptionbudgets"
     kind = "PodDisruptionBudget"
 
 
 class CustomResourceDefinition(APIObject):
     version = "apiextensions.k8s.io/v1"
     endpoint = "customresourcedefinitions"
```

### Comparing `pykube-ng-22.9.0/pykube/query.py` & `pykube-ng-23.6.0/pykube/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from collections import namedtuple
+from typing import Optional
 from typing import Union
 from urllib.parse import urlencode
 
 from .exceptions import HTTPError
 from .exceptions import ObjectDoesNotExist
 from .http import HTTPClient
 
@@ -35,15 +36,15 @@
 
     @property
     def rows(self):
         return self.obj["rows"]
 
 
 class BaseQuery:
-    def __init__(self, api: HTTPClient, api_obj_class, namespace: str = None):
+    def __init__(self, api: HTTPClient, api_obj_class, namespace: Optional[str] = None):
         self.api = api
         self.api_obj_class = api_obj_class
         self.namespace = namespace
         self.selector = everything
         self.field_selector = everything
 
     def __repr__(self) -> str:
@@ -52,17 +53,17 @@
         )
 
     def all(self) -> "BaseQuery":
         return self._clone()
 
     def filter(
         self,
-        namespace: str = None,
-        selector: Union[str, dict] = None,
-        field_selector: Union[str, dict] = None,
+        namespace: Optional[str] = None,
+        selector: Optional[Union[str, dict]] = None,
+        field_selector: Optional[Union[str, dict]] = None,
     ) -> "BaseQuery":
         """
         Filter objects by namespace, labels, or fields
 
         :param namespace: Namespace to filter by (pass pykube.all to get objects in all namespaces)
         :param selector: Label selector, can be a dictionary of label names/values
         """
@@ -79,15 +80,15 @@
         if cls is None:
             cls = self.__class__
         clone = cls(self.api, self.api_obj_class, namespace=self.namespace)
         clone.selector = self.selector
         clone.field_selector = self.field_selector
         return clone
 
-    def _build_api_url(self, params: dict = None):
+    def _build_api_url(self, params: Optional[dict] = None):
         if params is None:
             params = {}
         if self.selector is not everything:
             params["labelSelector"] = as_selector(self.selector)  # type: ignore
         if self.field_selector is not everything:
             params["fieldSelector"] = as_selector(self.field_selector)  # type: ignore
         query_string = urlencode(params)
```

### Comparing `pykube-ng-22.9.0/pykube/utils.py` & `pykube-ng-23.6.0/pykube/utils.py`

 * *Files identical despite different names*

### Comparing `pykube-ng-22.9.0/pyproject.toml` & `pykube-ng-23.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "pykube-ng"
-version = "22.9.0"
+version = "23.6.0"
 description = "Python client library for Kubernetes"
 license = "Apache"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `pykube-ng-22.9.0/setup.py` & `pykube-ng-23.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 extras_require = \
 {'gcp': ['google-auth', 'jsonpath-ng'],
  'oidc': ['requests-oauthlib>=1.3.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'pykube-ng',
-    'version': '22.9.0',
+    'version': '23.6.0',
     'description': 'Python client library for Kubernetes',
     'long_description': 'pykube-ng\n=========\n\n.. image:: https://img.shields.io/travis/hjacobs/pykube.svg\n   :target: https://travis-ci.org/hjacobs/pykube\n   :alt: Build status\n\n.. image:: https://coveralls.io/repos/github/hjacobs/pykube/badge.svg?branch=master;_=1\n   :target: https://coveralls.io/github/hjacobs/pykube?branch=master\n   :alt: Code Coverage\n\n.. image:: https://readthedocs.org/projects/pykube/badge/?version=latest\n   :target: https://pykube.readthedocs.io/\n   :alt: Documentation\n\n.. image:: https://img.shields.io/pypi/v/pykube-ng.svg\n   :target: https://pypi.python.org/pypi/pykube-ng/\n   :alt: PyPI version\n\n.. image:: https://img.shields.io/pypi/pyversions/pykube-ng.svg\n   :target: https://pypi.python.org/pypi/pykube-ng/\n   :alt: Python versions\n\n.. image:: https://img.shields.io/badge/license-apache-blue.svg\n   :target: https://pypi.python.org/pypi/pykube-ng/\n   :alt: Apache License\n\n.. image:: https://img.shields.io/badge/calver-YY.MM.MICRO-22bfda.svg\n   :target: http://calver.org/\n   :alt: CalVer\n\nPykube (pykube-ng) is a lightweight Python 3.6+ client library for Kubernetes.\n\nThis is a fork of `kelproject/pykube <https://github.com/kelproject/pykube>`_ which is no longer maintained (archived). Here the original text of the pykube README:\n\n    Kel is an open source Platform as a Service (PaaS) from Eldarion, Inc. that\n    makes it easy to manage web application deployment and hosting through the\n    entire lifecycle from development through testing to production. It adds\n    components and tools on top of Kubernetes that help developers manage their\n    application infrastructure. Kel builds on Eldarion\'s 7+ years experience running\n    one of the leading Python and Django PaaSes.\n    For more information about Kel, see `kelproject.com`_ or follow us on Twitter\n    `@projectkel`_.\n\n.. _kelproject.com: http://kelproject.com/\n.. _@projectkel: https://twitter.com/projectkel\n\nFeatures\n--------\n\n* HTTP interface using requests using kubeconfig for authentication\n* Python native querying of Kubernetes API objects\n\nInstallation\n------------\n\nTo install pykube, use pip::\n\n    pip install pykube-ng\n\n\nInteractive Console\n-------------------\n\nThe ``pykube`` library module can be run as an interactive console locally for quick exploration.\nIt will automatically load ``~/.kube/config`` to provide the ``api`` object, and it loads pykube classes (``Deployment``, ``Pod``, ..) into local context:\n\n.. code-block:: bash\n\n    python3 -m pykube\n    >>> [d.name for d in Deployment.objects(api)]\n\n\nUsage\n-----\n\nQuery for all ready pods in a custom namespace:\n\n.. code:: python\n\n    import operator\n    import pykube\n\n    api = pykube.HTTPClient(pykube.KubeConfig.from_file())\n    pods = pykube.Pod.objects(api).filter(namespace="gondor-system")\n    ready_pods = filter(operator.attrgetter("ready"), pods)\n\nAccess any attribute of the Kubernetes object:\n\n.. code:: python\n\n    pod = pykube.Pod.objects(api).filter(namespace="gondor-system").get(name="my-pod")\n    pod.obj["spec"]["containers"][0]["image"]\n\nSelector query:\n\n.. code:: python\n\n    pods = pykube.Pod.objects(api).filter(\n        namespace="gondor-system",\n        selector={"gondor.io/name__in": {"api-web", "api-worker"}},\n    )\n    pending_pods = pykube.objects.Pod.objects(api).filter(\n        field_selector={"status.phase": "Pending"}\n    )\n\nWatch query:\n\n.. code:: python\n\n    watch = pykube.Job.objects(api, namespace="gondor-system")\n    watch = watch.filter(field_selector={"metadata.name": "my-job"}).watch()\n\n    # watch is a generator:\n    for watch_event in watch:\n        print(watch_event.type) # \'ADDED\', \'DELETED\', \'MODIFIED\'\n        print(watch_event.object) # pykube.Job object\n\nCreate a Deployment:\n\n.. code:: python\n\n    obj = {\n        "apiVersion": "apps/v1",\n        "kind": "Deployment",\n        "metadata": {\n            "name": "my-deploy",\n            "namespace": "gondor-system"\n        },\n        "spec": {\n            "replicas": 3,\n            "selector": {\n                "matchLabels": {\n                    "app": "nginx"\n                }\n            },\n            "template": {\n                "metadata": {\n                    "labels": {\n                        "app": "nginx"\n                    }\n                },\n                "spec": {\n                    "containers": [\n                        {\n                            "name": "nginx",\n                            "image": "nginx",\n                            "ports": [\n                                {"containerPort": 80}\n                            ]\n                        }\n                    ]\n                }\n            }\n        }\n    }\n    pykube.Deployment(api, obj).create()\n\nDelete a Deployment:\n\n.. code:: python\n\n    obj = {\n        "apiVersion": "apps/v1",\n        "kind": "Deployment",\n        "metadata": {\n            "name": "my-deploy",\n            "namespace": "gondor-system"\n        }\n    }\n    pykube.Deployment(api, obj).delete()\n\nCheck server version:\n\n.. code:: python\n\n    api = pykube.HTTPClient(pykube.KubeConfig.from_file())\n    api.version\n\n\nRequirements\n------------\n\n* Python 3.6+\n* requests (included in ``install_requires``)\n* PyYAML (included in ``install_requires``)\n\n\nLocal Development\n-----------------\n\nYou can run pykube against your current kubeconfig context, e.g. local Minikube_:\n\n.. code-block:: bash\n\n    poetry install\n    poetry run python3\n    >>> import pykube\n    >>> config = pykube.KubeConfig.from_file()\n    >>> api = pykube.HTTPClient(config)\n    >>> list(pykube.Deployment.objects(api))\n\nTo run PEP8 (flake8) checks and unit tests including coverage report:\n\n.. code-block:: bash\n\n    make test\n\n\nLicense\n-------\n\nThe code in this project is licensed under the Apache License, version 2.0\n(included in this repository under LICENSE).\n\n\nContributing\n------------\n\nEasiest way to contribute is to provide feedback! We would love to hear what you like and what you think is missing.\nCreate an issue or `ping try_except_ on Twitter`_.\n\nPRs are welcome. Please also have a look at `issues labeled with "help wanted"`_.\n\n\nCode of Conduct\n----------------\n\nIn order to foster a kind, inclusive, and harassment-free community, this project follows the `Contributor Covenant Code of Conduct`_.\n\n.. _Contributor Covenant Code of Conduct: http://contributor-covenant.org/version/1/4/\n\n\n.. _ping try_except_ on Twitter: https://twitter.com/try_except_\n.. _issues labeled with "help wanted": https://codeberg.org/hjacobs/pykube-ng/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22\n.. _Minikube: https://github.com/kubernetes/minikube\n',
     'author': 'Eldarion, Inc.',
     'author_email': 'development@eldarion.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/hjacobs/pykube-ng',
```

### Comparing `pykube-ng-22.9.0/PKG-INFO` & `pykube-ng-23.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykube-ng
-Version: 22.9.0
+Version: 23.6.0
 Summary: Python client library for Kubernetes
 Home-page: https://codeberg.org/hjacobs/pykube-ng
 License: Apache
 Author: Eldarion, Inc.
 Author-email: development@eldarion.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
```

