# Comparing `tmp/reactpy_router-0.0.1-py2.py3-none-any.whl.zip` & `tmp/reactpy_router-0.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 52174 bytes, number of entries: 10
--rw-r--r--  2.0 unx      434 b- defN 23-May-11 04:05 reactpy_router/__init__.py
--rw-r--r--  2.0 unx   143875 b- defN 23-May-11 04:05 reactpy_router/bundle.js
--rw-r--r--  2.0 unx     3685 b- defN 23-May-11 04:05 reactpy_router/core.py
--rw-r--r--  2.0 unx     2299 b- defN 23-May-11 04:05 reactpy_router/simple.py
--rw-r--r--  2.0 unx     1265 b- defN 23-May-11 04:05 reactpy_router/types.py
--rw-r--r--  2.0 unx     1083 b- defN 23-May-11 04:05 reactpy_router-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2611 b- defN 23-May-11 04:05 reactpy_router-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-11 04:05 reactpy_router-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-11 04:05 reactpy_router-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      827 b- defN 23-May-11 04:05 reactpy_router-0.0.1.dist-info/RECORD
-10 files, 156204 bytes uncompressed, 50766 bytes compressed:  67.5%
+Zip file size: 52153 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      434 b- defN 23-Jun-16 16:21 reactpy_router/__init__.py
+-rw-r--r--  2.0 unx   144285 b- defN 23-Jun-16 16:21 reactpy_router/bundle.js
+-rw-r--r--  2.0 unx     4116 b- defN 23-Jun-16 16:21 reactpy_router/core.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-16 16:21 reactpy_router/py.typed
+-rw-r--r--  2.0 unx     2737 b- defN 23-Jun-16 16:21 reactpy_router/simple.py
+-rw-r--r--  2.0 unx     1482 b- defN 23-Jun-16 16:21 reactpy_router/types.py
+-rw-r--r--  2.0 unx     1083 b- defN 23-Jun-16 16:21 reactpy_router-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      984 b- defN 23-Jun-16 16:21 reactpy_router-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-16 16:21 reactpy_router-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-16 16:21 reactpy_router-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-Jun-16 16:21 reactpy_router-0.1.0.dist-info/RECORD
+11 files, 156176 bytes uncompressed, 50623 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -3,29 +3,32 @@
 
 Filename: reactpy_router/bundle.js
 Comment: 
 
 Filename: reactpy_router/core.py
 Comment: 
 
+Filename: reactpy_router/py.typed
+Comment: 
+
 Filename: reactpy_router/simple.py
 Comment: 
 
 Filename: reactpy_router/types.py
 Comment: 
 
-Filename: reactpy_router-0.0.1.dist-info/LICENSE
+Filename: reactpy_router-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: reactpy_router-0.0.1.dist-info/METADATA
+Filename: reactpy_router-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: reactpy_router-0.0.1.dist-info/WHEEL
+Filename: reactpy_router-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: reactpy_router-0.0.1.dist-info/top_level.txt
+Filename: reactpy_router-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: reactpy_router-0.0.1.dist-info/RECORD
+Filename: reactpy_router-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reactpy_router/__init__.py

```diff
@@ -1,9 +1,9 @@
 # the version is statically loaded by setup.py
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 
 from . import simple
 from .core import create_router, link, route, router_component, use_params, use_query
 from .types import Route, RouteCompiler, RouteResolver
 
 __all__ = (
     "create_router",
```

## reactpy_router/bundle.js

### js-beautify {}

```diff
@@ -7762,23 +7762,42 @@
         }
         return p(), h
     }(s)), r), arguments, [])).length > 1 ? r : r[0]
 }
 
 const html = htm.bind(react.createElement);
 
-function bind(node, config) {
+function bind(node) {
     return {
         create: (type, props, children) =>
             react.createElement(type, props, ...children),
-        render: (element) => reactDom.render(element, node),
+        render: (element) => {
+            reactDom.render(element, node);
+        },
         unmount: () => reactDom.unmountComponentAtNode(node),
     };
 }
 
+function History({
+    onChange
+}) {
+    // capture changes to the browser's history
+    react.useEffect(() => {
+        const listener = () => {
+            onChange({
+                pathname: window.location.pathname,
+                search: window.location.search,
+            });
+        };
+        window.addEventListener("popstate", listener);
+        return () => window.removeEventListener("popstate", listener);
+    });
+    return null;
+}
+
 function Link({
     to,
     onClick,
     children,
     ...props
 }) {
     const handleClick = (event) => {
@@ -7790,10 +7809,11 @@
         });
     };
 
     return html`<a href=${to} onClick=${handleClick} ...${props}>${children}</a>`;
 }
 
 export {
+    History,
     Link,
     bind
 };
```

## reactpy_router/core.py

```diff
@@ -1,17 +1,20 @@
+"""Core functionality for the reactpy-router package."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, replace
 from pathlib import Path
 from typing import Any, Callable, Iterator, Sequence, TypeVar
 from urllib.parse import parse_qs
 
 from reactpy import (
     component,
     create_context,
+    html,
     use_context,
     use_location,
     use_memo,
     use_state,
 )
 from reactpy.backend.hooks import ConnectionContext, use_connection
 from reactpy.backend.types import Connection, Location
@@ -21,14 +24,15 @@
 
 from reactpy_router.types import Route, RouteCompiler, Router, RouteResolver
 
 R = TypeVar("R", bound=Route)
 
 
 def route(path: str, element: Any | None, *routes: Route) -> Route:
+    """Create a route with the given path, element, and child routes"""
     return Route(path, element, routes)
 
 
 def create_router(compiler: RouteCompiler[R]) -> Router[R]:
     """A decorator that turns a route compiler into a router"""
 
     def wrapper(*routes: R) -> ComponentType:
@@ -37,37 +41,43 @@
     return wrapper
 
 
 @component
 def router_component(
     *routes: R,
     compiler: RouteCompiler[R],
-) -> ComponentType | None:
+) -> VdomDict | None:
+    """A component that renders the first matching route using the given compiler"""
+
     old_conn = use_connection()
     location, set_location = use_state(old_conn.location)
 
     resolvers = use_memo(
         lambda: tuple(map(compiler, _iter_routes(routes))),
         dependencies=(compiler, hash(routes)),
     )
 
     match = use_memo(lambda: _match_route(resolvers, location))
 
     if match is not None:
         element, params = match
-        return ConnectionContext(
-            _route_state_context(element, value=_RouteState(set_location, params)),
-            value=Connection(old_conn.scope, location, old_conn.carrier),
+        return html._(
+            ConnectionContext(
+                _route_state_context(element, value=_RouteState(set_location, params)),
+                value=Connection(old_conn.scope, location, old_conn.carrier),
+            ),
+            _history({"on_change": lambda event: set_location(Location(**event))}),
         )
 
     return None
 
 
 @component
 def link(*children: VdomChild, to: str, **attributes: Any) -> VdomDict:
+    """A component that renders a link to the given path"""
     set_location = _use_route_state().set_location
     attrs = {
         **attributes,
         "to": to,
         "onClick": lambda event: set_location(Location(**event)),
     }
     return _link(attrs, *children)
@@ -109,17 +119,17 @@
     for resolver in compiled_routes:
         match = resolver.resolve(location.pathname)
         if match is not None:
             return match
     return None
 
 
-_link = export(
+_link, _history = export(
     module_from_file("reactpy-router", file=Path(__file__).parent / "bundle.js"),
-    "Link",
+    ("Link", "History"),
 )
 
 
 @dataclass
 class _RouteState:
     set_location: Callable[[Location], None]
     params: dict[str, Any]
```

## reactpy_router/simple.py

```diff
@@ -1,7 +1,9 @@
+"""A simple router implementation for ReactPy"""
+
 from __future__ import annotations
 
 import re
 import uuid
 from typing import Any, Callable
 
 from typing_extensions import TypeAlias, TypedDict
@@ -10,18 +12,21 @@
 from reactpy_router.types import Route
 
 __all__ = ["router"]
 
 ConversionFunc: TypeAlias = "Callable[[str], Any]"
 ConverterMapping: TypeAlias = "dict[str, ConversionFunc]"
 
-PARAM_REGEX = re.compile(r"{(?P<name>\w+)(?P<type>:\w+)?}")
+STAR_PATTERN = re.compile("^.*$")
+PARAM_PATTERN = re.compile(r"{(?P<name>\w+)(?P<type>:\w+)?}")
 
 
 class SimpleResolver:
+    """A simple route resolver that uses regex to match paths"""
+
     def __init__(self, route: Route) -> None:
         self.element = route.element
         self.pattern, self.converters = parse_path(route.path)
         self.key = self.pattern.pattern
 
     def resolve(self, path: str) -> tuple[Any, dict[str, Any]] | None:
         match = self.pattern.match(path)
@@ -30,18 +35,21 @@
                 self.element,
                 {k: self.converters[k](v) for k, v in match.groupdict().items()},
             )
         return None
 
 
 def parse_path(path: str) -> tuple[re.Pattern[str], ConverterMapping]:
+    if path == "*":
+        return STAR_PATTERN, {}
+
     pattern = "^"
     last_match_end = 0
     converters: ConverterMapping = {}
-    for match in PARAM_REGEX.finditer(path):
+    for match in PARAM_PATTERN.finditer(path):
         param_name = match.group("name")
         param_type = (match.group("type") or "str").lstrip(":")
         try:
             param_conv = CONVERSION_TYPES[param_type]
         except KeyError:
             raise ValueError(f"Unknown conversion type {param_type!r} in {path!r}")
         pattern += re.escape(path[last_match_end : match.start()])
@@ -49,16 +57,20 @@
         converters[param_name] = param_conv["func"]
         last_match_end = match.end()
     pattern += re.escape(path[last_match_end:]) + "$"
     return re.compile(pattern), converters
 
 
 class ConversionInfo(TypedDict):
+    """Information about a conversion type"""
+
     regex: str
+    """The regex to match the conversion type"""
     func: ConversionFunc
+    """The function to convert the matched string to the expected type"""
 
 
 CONVERSION_TYPES: dict[str, ConversionInfo] = {
     "str": {
         "regex": r"[^/]+",
         "func": str,
     },
@@ -75,10 +87,12 @@
         "func": uuid.UUID,
     },
     "path": {
         "regex": r".+",
         "func": str,
     },
 }
+"""The supported conversion types"""
 
 
 router = create_router(SimpleResolver)
+"""The simple router"""
```

## reactpy_router/types.py

```diff
@@ -1,40 +1,53 @@
+"""Types for reactpy_router"""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, Sequence, TypeVar
 
 from reactpy.core.vdom import is_vdom
 from reactpy.types import ComponentType, Key
 from typing_extensions import Protocol, Self
 
 
 @dataclass(frozen=True)
 class Route:
+    """A route that can be matched against a path"""
+
     path: str
+    """The path to match against"""
+
     element: Any = field(hash=False)
+    """The element to render if the path matches"""
+
     routes: Sequence[Self]
+    """Child routes"""
 
     def __hash__(self) -> int:
         el = self.element
         key = el["key"] if is_vdom(el) and "key" in el else getattr(el, "key", id(el))
         return hash((self.path, key, self.routes))
 
 
 R = TypeVar("R", bound=Route, contravariant=True)
 
 
 class Router(Protocol[R]):
+    """Return a component that renders the first matching route"""
+
     def __call__(self, *routes: R) -> ComponentType:
-        """Return a component that renders the first matching route"""
+        ...
 
 
 class RouteCompiler(Protocol[R]):
+    """Compile a route into a resolver that can be matched against a path"""
+
     def __call__(self, route: R) -> RouteResolver:
-        """Compile a route into a resolver that can be matched against a path"""
+        ...
 
 
 class RouteResolver(Protocol):
     """A compiled route that can be matched against a path"""
 
     @property
     def key(self) -> Key:
```

## Comparing `reactpy_router-0.0.1.dist-info/LICENSE` & `reactpy_router-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

