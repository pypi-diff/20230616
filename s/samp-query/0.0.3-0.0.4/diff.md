# Comparing `tmp/samp_query-0.0.3.tar.gz` & `tmp/samp_query-0.0.4.tar.gz`

## Comparing `samp_query-0.0.3.tar` & `samp_query-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 samp_query-0.0.3/.coverage
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 samp_query-0.0.3/main.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 samp_query-0.0.3/requirements-test.txt
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 samp_query-0.0.3/requirements.txt
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.0.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 samp_query-0.0.3/samp_query/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.3/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.3/test/conftest.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 samp_query-0.0.3/test/test_client.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.0.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.0.3/LICENSE
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.0.3/README.md
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 samp_query-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 samp_query-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 samp_query-0.0.4/.coverage
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 samp_query-0.0.4/main.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 samp_query-0.0.4/requirements-test.txt
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 samp_query-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 samp_query-0.0.4/samp_query/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.4/test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.4/test/conftest.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 samp_query-0.0.4/test/test_client.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.0.4/LICENSE
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.0.4/README.md
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 samp_query-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 samp_query-0.0.4/PKG-INFO
```

### Comparing `samp_query-0.0.3/.coverage` & `samp_query-0.0.4/.coverage`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.3/.github/workflows/ci.yml` & `samp_query-0.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.3/samp_query/__init__.py` & `samp_query-0.0.4/samp_query/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import random
 from dataclasses import dataclass, field
 
 import cchardet as chardet  # type: ignore
 import trio
 
 
-def unpack_string(data: bytes, len_type: str = 'I') -> tuple[str, bytes]:
+def unpack_string(data: bytes, len_type: str) -> tuple[str, bytes]:
     format = f'<{len_type}'
     size = struct.calcsize(format)
     str_len, data = *struct.unpack_from(format, data), data[size:]
     string, data = data[:str_len], data[str_len:]
     encoding: str = chardet.detect(string)['encoding']
     return string.decode(encoding), data
 
@@ -25,17 +25,17 @@
     gamemode: str
     language: str
 
     @classmethod
     def from_data(cls, data: bytes) -> ServerInfo:
         password, players, max_players = struct.unpack_from('<?HH', data)
         data = data[5:]  # _Bool + short + short, see above
-        name, data = unpack_string(data)
-        gamemode, data = unpack_string(data)
-        language, data = unpack_string(data)
+        name, data = unpack_string(data, 'I')
+        gamemode, data = unpack_string(data, 'I')
+        language, data = unpack_string(data, 'I')
 
         assert not data  # We consumed all the buffer
 
         return cls(
             name=name,
             password=password,
             players=players,
@@ -78,67 +78,121 @@
 
         assert not data  # We consumed all the buffer
 
         return cls(players=players)
 
 
 @dataclass
+class Rule:
+    name: str
+    value: str
+
+    @classmethod
+    def from_data(cls, data: bytes) -> tuple[Rule, bytes]:
+        name, data = unpack_string(data, 'B')
+        value, data = unpack_string(data, 'B')
+
+        return cls(
+            name=name,
+            value=value,
+        ), data
+
+
+@dataclass
+class RuleList:
+    rules: list[Rule]
+
+    @classmethod
+    def from_data(cls, data: bytes) -> RuleList:
+        rule_count = struct.unpack_from('<H', data)[0]
+        data = data[2:]  # short, see above
+        rules = []
+
+        for _ in range(rule_count):
+            rule, data = Rule.from_data(data)
+            rules.append(rule)
+
+        assert not data  # We consumed all the buffer
+
+        return cls(rules=rules)
+
+
+@dataclass
 class Client:
     ip: str
     port: int
     rcon_password: str | None = field(default=None, repr=False)
 
+    prefix: bytes | None = field(default=None, repr=False)
     _socket: trio.socket.SocketType | None = field(default=None, repr=False)
-    _prefix: bytes | None = field(default=None, repr=False)
 
     async def connect(self) -> None:
         family, type, proto, _, (ip, *_) = (await trio.socket.getaddrinfo(
             self.ip,
             self.port,
             family=trio.socket.AF_INET,
             proto=trio.socket.IPPROTO_UDP,
         ))[0]
         self.ip = ip
         self._socket = socket = trio.socket.socket(family, type, proto)
         await socket.connect((self.ip, self.port))
-        self._prefix = (
+        self.prefix = (
             b'SAMP'
             + trio.socket.inet_aton(self.ip)
             + self.port.to_bytes(2, 'little')
         )
 
     async def send(self, opcode: bytes, payload: bytes = b'') -> None:
         if not self._socket:
             await self.connect()
 
-        assert self._socket and self._prefix
-        await self._socket.send(self._prefix + opcode + payload)
+        assert self._socket and self.prefix
+        await self._socket.send(self.prefix + opcode + payload)
 
     async def receive(self, header: bytes = b'') -> bytes:
         assert self._socket
 
         while True:
             data = await self._socket.recv(4096)
 
             if data.startswith(header):
                 return data[len(header):]
 
     async def ping(self) -> float:
         payload = random.getrandbits(32).to_bytes(4, 'little')
         start_time = trio.current_time()
         await self.send(b'p', payload)
-        assert self._prefix
-        data = await self.receive(header=self._prefix + b'p' + payload)
+        assert self.prefix
+        data = await self.receive(header=self.prefix + b'p' + payload)
         assert not data  # No data beyond expected header
         return trio.current_time() - start_time
 
+    async def is_omp(self) -> bool:
+        ping = await self.ping()
+        payload = random.getrandbits(32).to_bytes(4, 'little')
+
+        # Assuming latency variance is less than 100%
+        with trio.move_on_after(2 * ping):
+            await self.send(b'o', payload)
+            assert self.prefix
+            await self.receive(header=self.prefix + b'o' + payload)
+            return True
+
+        return False
+
     async def info(self) -> ServerInfo:
         await self.send(b'i')
-        assert self._prefix
-        data = await self.receive(header=self._prefix + b'i')
+        assert self.prefix
+        data = await self.receive(header=self.prefix + b'i')
         return ServerInfo.from_data(data)
 
     async def players(self) -> PlayerList:
         await self.send(b'c')
-        assert self._prefix
-        data = await self.receive(header=self._prefix + b'c')
+        assert self.prefix
+        data = await self.receive(header=self.prefix + b'c')
         return PlayerList.from_data(data)
+
+    async def rules(self) -> RuleList:
+        await self.send(b'r')
+        assert self.prefix
+        data = await self.receive(header=self.prefix + b'r')
+        return RuleList.from_data(data)
```

### Comparing `samp_query-0.0.3/LICENSE` & `samp_query-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.3/pyproject.toml` & `samp_query-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "samp_query"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="The Cheaterman", email="the.cheaterman@gmail.com" },
 ]
 description = "A SAMP query/RCON client for Python using trio."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `samp_query-0.0.3/PKG-INFO` & `samp_query-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samp_query
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SAMP query/RCON client for Python using trio.
 Project-URL: Homepage, https://github.com/Cheaterman/samp-query
 Project-URL: Bug Tracker, https://github.com/Cheaterman/samp-query/issues
 Author-email: The Cheaterman <the.cheaterman@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

