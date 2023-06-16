# Comparing `tmp/citizenk-0.1.47.tar.gz` & `tmp/citizenk-0.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.47.tar", max compression
+gzip compressed data, was "citizenk-0.1.48.tar", max compression
```

## Comparing `citizenk-0.1.47.tar` & `citizenk-0.1.48.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    18767 2023-05-27 09:09:22.290086 citizenk-0.1.47/README.md
--rw-r--r--   0        0        0      382 2023-05-25 17:44:44.985810 citizenk-0.1.47/citizenk/__init__.py
--rw-r--r--   0        0        0     8805 2023-05-25 17:44:44.985906 citizenk-0.1.47/citizenk/agent.py
--rw-r--r--   0        0        0    20655 2023-05-25 17:44:44.986069 citizenk-0.1.47/citizenk/citizenk.py
--rw-r--r--   0        0        0    20928 2023-05-25 17:44:44.986229 citizenk-0.1.47/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-05-25 17:44:44.986302 citizenk-0.1.47/citizenk/murmur2.py
--rw-r--r--   0        0        0     5448 2023-05-25 17:44:44.986393 citizenk-0.1.47/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-05-25 17:44:44.986451 citizenk-0.1.47/citizenk/utils.py
--rw-r--r--   0        0        0     1542 2023-05-27 09:08:35.537133 citizenk-0.1.47/pyproject.toml
--rw-r--r--   0        0        0    20075 2023-05-27 09:09:22.827184 citizenk-0.1.47/setup.py
--rw-r--r--   0        0        0    19885 2023-05-27 09:09:22.828151 citizenk-0.1.47/PKG-INFO
+-rw-r--r--   0        0        0    18975 2023-06-16 13:57:46.346216 citizenk-0.1.48/README.md
+-rw-r--r--   0        0        0      382 2023-06-11 19:27:45.145664 citizenk-0.1.48/citizenk/__init__.py
+-rw-r--r--   0        0        0     8805 2023-06-11 19:27:45.145758 citizenk-0.1.48/citizenk/agent.py
+-rw-r--r--   0        0        0    20706 2023-06-16 13:36:58.623566 citizenk-0.1.48/citizenk/citizenk.py
+-rw-r--r--   0        0        0    24505 2023-06-16 13:36:28.101104 citizenk-0.1.48/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-06-11 19:27:45.146160 citizenk-0.1.48/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5664 2023-06-16 13:50:06.593517 citizenk-0.1.48/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-06-11 19:27:45.146294 citizenk-0.1.48/citizenk/utils.py
+-rw-r--r--   0        0        0     1799 2023-06-16 13:57:45.883745 citizenk-0.1.48/pyproject.toml
+-rw-r--r--   0        0        0    20639 1970-01-01 00:00:00.000000 citizenk-0.1.48/PKG-INFO
```

### Comparing `citizenk-0.1.47/README.md` & `citizenk-0.1.48/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -365,14 +365,18 @@
 - target_service_consumer_group: The service consumer group to delete when replication is enabled
 
 ## Topic Level Mapping
 Topic level mappings allows mapping of key/values when replicating a topic. This might be useful if for example the schema / enums / keys are different between the environments
 
 To support this, the replicator supports value mappings for each topic that it consumes from the source in the following JSON format:
 
+There are two mapping formats:
+- value.payload.product_id : map source product_id to target product_id
+- key:partition: map source key to target partition (drop entire msg if partition equals -1000)
+
 ```json
 {
     "key":{
         "1":10,
         "2":12
     },
     "value.payload.product_id":{
@@ -381,21 +385,21 @@
         "1003":14
     },
     "value.payload.user_name":{
         "A":"A name",
         "B":"B name",
         "C":"C name"
     },
-    "partition":{
-        "0":0,
+    "key:partition":{
         "1":0,
         "2":0,
-        "3":1,
+        "3":-1000,
         "4":1,
         "5":1,
+        "6":1,
     }
 }
 ```
 
 ## Stats
 Returns a list of JSON stats for each mapping in the following format:
 ```json
```

### Comparing `citizenk-0.1.47/citizenk/agent.py` & `citizenk-0.1.48/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.47/citizenk/citizenk.py` & `citizenk-0.1.48/citizenk/citizenk.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,15 @@
                         num_messages=self.total_batch_size, timeout=0.1
                     )
                     if len(msgs) > 0:
                         processed = True
                         events = Agent.validate_messages(msgs, self.topics)
                         for agent in self.agents.values():
                             await agent.process(events)
+                        self.consumer.commit(msgs)
 
                 # Consume from websocket agents consumers (no group)
                 for agent in self.websocket_agents.values():
                     if await agent.consume():
                         processed = True
 
                 duration = 1000 * (time.time() - start_time)
```

### Comparing `citizenk-0.1.47/citizenk/kafka_adapter.py` & `citizenk-0.1.48/citizenk/kafka_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import certifi
 from confluent_kafka import (
     Consumer,
+    ConsumerGroupTopicPartitions,
     KafkaError,
     KafkaException,
     Message,
     Producer,
     TopicPartition,
 )
 from confluent_kafka.admin import AdminClient, NewTopic
-
 from .murmur2 import murmur2_partition
 
 logger = logging.getLogger(__name__)
 
 
 class KafkaRole(Enum):
     ADMIN = 1
@@ -48,17 +48,20 @@
 
     def __init__(
         self,
         config: KafkaConfig,
         role: KafkaRole = KafkaRole.ADMIN,
         consumer_group_name: Optional[str] = None,
         consumer_group_init_offset: Optional[str] = "latest",
+        consumer_group_auto_commit: Optional[bool] = True,
+        extra_config: Optional[Dict[str, str]] = None,
     ):
         self.role = role
         self.consumer_group_name = consumer_group_name
+        self.consumer_group_auto_commit = consumer_group_auto_commit
         self.consumer_started = False
         self.consumer_topics = {}
         self.assigned_partitions = defaultdict(set)
         self.kafka_error = None
         self.last_stats = {}
         self.topic_stats = defaultdict(int)
 
@@ -80,24 +83,28 @@
                 "statistics.interval.ms": 15 * 60 * 1000,
                 "error_cb": self._on_kafka_error,
                 "stats_cb": self._on_kafka_stats,
             }
         else:
             raise ValueError("Unsupported sasl_mechanism")
         self.config["bootstrap.servers"] = config.bootstrap_servers
+
+        # Add additional config
         if config.extra_config is not None:
             self.config.update(config.extra_config)
+        if extra_config is not None:
+            self.config.update(extra_config)
 
         self.admin_config = self.config.copy()
         if self.role == KafkaRole.CONSUMER:
             self.config["auto.offset.reset"] = consumer_group_init_offset
             self.config["on_commit"] = self._on_kafka_commit
             if self.consumer_group_name is not None:
                 self.config["group.id"] = self.consumer_group_name
-                self.config["enable.auto.commit"] = True
+                self.config["enable.auto.commit"] = consumer_group_auto_commit
             else:
                 logger.info("Starting consumer without a consumer group")
                 self.config["enable.auto.commit"] = False
                 self.config["group.id"] = "dummy_shouldnt_be_used"
             self.connection = Consumer(self.config, logger=logger)
         elif self.role == KafkaRole.PRODUCER:
             self.config["partitioner"] = "murmur2"
@@ -206,15 +213,15 @@
                     TopicPartition(topic, p)
                     for p in metadata.topics[topic].partitions
                     if p in partition_filter
                 ]
             filtered_partitions += partitions
 
         # for time strategy lookup offset for time
-        if strategy == "time":
+        if epoch > 0:
             epoch = int(epoch)
             for p in filtered_partitions:
                 p.offset = epoch
             return self.connection.offsets_for_times(filtered_partitions, timeout=10)
         else:
             for p in filtered_partitions:
                 (lo, hi) = self.connection.get_watermark_offsets(
@@ -251,32 +258,32 @@
             )
         ]
         fs = self.connection.create_topics(new_topics)
         for topic, f in fs.items():
             try:
                 f.result()  # The result itself is None
                 logger.debug("Topic %s created", topic)
-            except KafkaException as e:
-                logger.error("Failed to create topic %s: %s", topic, e)
+            except KafkaException as ex:
+                logger.error("Failed to create topic %s: %s", topic, ex)
 
     def get_own_group_topics(self) -> List[str]:
         """Get a list of all the topics in the replicator consumer group"""
         if self.role != KafkaRole.CONSUMER or self.consumer_group_name is None:
             return []
 
         group_topics = set()
         partitions = self.get_all_broker_partitions()
         # Find which topic has stored offset for the group
         try:
             committed = self.connection.committed(partitions, timeout=10)
-        except KafkaException as e:
+        except KafkaException as ex:
             logger.error(
                 "Failed to get group committed offsets %s %s",
                 self.consumer_group_name,
-                e,
+                ex,
             )
             return []
 
         for p in committed:
             if p.offset > 0:
                 group_topics.add(p.topic)
         return list(group_topics)
@@ -299,43 +306,144 @@
                         continue
                     topic = p.topic
                     lag = hi - p.offset
                     group_topics[topic] += lag
             logger.debug(
                 "Topics Lag for %s group are %s", self.consumer_group_name, group_topics
             )
-        except KafkaException as e:
+        except KafkaException as ex:
             logger.error(
                 "Failed to get group committed offsets %s %s",
                 self.consumer_group_name,
-                e,
+                ex,
             )
             return group_topics
 
         return group_topics
 
     def delete_groups(self, groups: List[str]) -> int:
-        current_groups = self.get_all_broker_groups()
+        """Delete the given consumer groups"""
+        if len(groups) == 0:
+            return 0
+        connection = AdminClient(self.admin_config)
+        future_map = connection.delete_consumer_groups(groups, request_timeout=10)
         count = 0
-        for group in groups:
-            if group in current_groups:
-                self.delete_offset_for_group(group)
+        for group_id, future in future_map.items():
+            try:
+                future.result()
+                logger.debug("Deleted consumer groups %s", group_id)
                 count += 1
+            except KafkaException as ex:
+                logger.error("Failed to delete consumer groups %s %s", group_id, ex)
         return count
 
+    def delete_offset_for_group_api(
+        self, group: str, topic: Optional[str] = None
+    ) -> int:
+        """Delete the offset of the given topic from  (Not working) !!"""
+        if topic is None:
+            return 0
+        connection = AdminClient(self.admin_config)
+        topics = connection.list_topics(topic, timeout=15).topics
+        if len(topics) == 0:
+            logger.error("Can't find topic %s in broker", topic)
+            return 0
+        group_request = [
+            ConsumerGroupTopicPartitions(
+                group, [TopicPartition(topic, p, 0) for p in topics[topic].partitions]
+            )
+        ]
+        print(topic, topics[topic].partitions)
+        print(group_request)
+        future_map = connection.alter_consumer_group_offsets(
+            group_request, request_timeout=15
+        )
+        count = 0
+        for future in future_map.values():
+            try:
+                future.result()
+                logger.debug("Deleted offset of topic %s group %s", topic, group)
+                count += 1
+            except KafkaException as ex:
+                logger.error(
+                    "Failed to delete offset of topic %s from consumer groups %s %s",
+                    group,
+                    topic,
+                    ex,
+                )
+        return count
+
+    def reset_offset_for_group(self, group: str, topic: Optional[str] = None) -> int:
+        """
+        Resets the offset of a topic for the group to latest.
+        """
+        params = {"--reset-offsets": "", "--to-latest": ""}
+        if topic is None:
+            params["--all-topics"] = ""
+        else:
+            params["--topic"] = topic
+
+        error_code = self.group_ops(group, params)
+        if error_code != 0:
+            logger.error(
+                "Failed to reset offsets for group using kafka CLI %s", error_code
+            )
+        else:
+            logger.debug(
+                "Successfully reset offsets for group %s topic %s", group, topic
+            )
+        return error_code
+
     def delete_offset_for_group(self, group: str, topic: Optional[str] = None) -> int:
         """
-        Delete the offset of a topic for the group. If topic is not given,
-        deletes the entire group
+        Deletes the offset of a topic for the group.
         """
         # When we stop replicating a topic, we want to delete the offsets of the consumer group
         # So that when we replicate the same topic back, we will start from latest and not the stored
         # offset. I coulnd't find a way to delete the offsets using the API, so I had to use the
         # Standard kafka cli for this
         # kafka-consumer-groups.sh --bootstrap-server 'localhost:9092' --group replicator --command-config local.config --topic globalvia.ap53.dev.camera.video.ocr - 1  --delete-offsets
+        params = {"--delete-offsets": ""}
+        if topic is None:
+            params["--all-topics"] = ""
+        else:
+            params["--topic"] = topic
+
+        error_code = self.group_ops(group, params)
+        if error_code != 0:
+            logger.error(
+                "Failed to delete offsets for group using kafka CLI %s", error_code
+            )
+        else:
+            logger.debug(
+                "Successfully deleted offsets for group %s topic %s", group, topic
+            )
+        return error_code
+
+    def group_ops(self, group: str, ops_params: Dict[str, str]) -> int:
+        """
+        Perform the given ops on the group
+
+        Which op:
+        --describe
+        --delete to delete the group
+        --delete-offsets to delete offsets for a topic / all topics
+        --reset-offsets to reset offsets for a topic / all topics
+
+        Which topic:
+        --topic <name>
+        --all-topics
+
+        Which offset
+        --to-earliest
+        --to-latest
+        --to-offset
+        --shift-by
+        --to-datetime
+        """
         temp_config_filename = tempfile.NamedTemporaryFile(
             suffix=".config", delete=False
         ).name
 
         config_string = "\n".join([f"{k}={v}" for k, v in self.config.items()])
         if self.sasl_mechanism == "PLAIN":
             config_string += "\nsasl.jaas.config=org.apache.kafka.common.security.plain.PlainLoginModule"
@@ -349,41 +457,27 @@
             f.write(config_string)
 
         command = "kafka-consumer-groups.sh"
         params = {
             "--bootstrap-server": self.config["bootstrap.servers"],
             "--command-config": temp_config_filename,
             "--group": group,
+            "--execute": "",
         }
-        if topic is None:
-            params["--delete"] = ""
-        else:
-            params["--delete-offsets"] = ""
-            params["--topic"] = topic
-
+        params.update(ops_params)
         command_with_params = command + "".join(
             [f" {k} {v}" for k, v in params.items()]
         )
         error_code = subprocess.call(
             command_with_params,
             shell=True,
             stderr=sys.stderr,
             stdout=sys.stdout,
             timeout=15,
         )
-        if error_code != 0:
-            logger.error(
-                "Failed to delete offsets for group using kafka CLI %s", error_code
-            )
-        if topic is None:
-            logger.debug("Successfully deleted group %s", group)
-        else:
-            logger.debug(
-                "Successfully deleted offsets for group %s topic %s", group, topic
-            )
         os.remove(temp_config_filename)
         return error_code
 
     def delete_old_offsets_for_group(self) -> int:
         if self.role != KafkaRole.CONSUMER:
             return 0
         if not self.consumer_started:
@@ -477,14 +571,21 @@
                 msgs.append(msg)
             else:
                 self._on_kafka_error(error)
             self.topic_stats[msg.topic()] += 1
         logger.debug("Consumed %s Kafka messages", len(msgs))
         return msgs
 
+    def commit(self,msgs:List[Message]):
+        if self.consumer_group_name is None:
+            return
+        if self.consumer_group_auto_commit:
+            return
+        self.connection.commit(msgs)
+
     def produce(
         self,
         topic: str,
         value: Any,
         key: Optional[Any] = None,
         partition: int = -1,
         headers: Optional[Dict[str, bytes]] = None,
@@ -518,14 +619,17 @@
             self.assigned_partitions[p.topic].discard(p.partition)
 
     def _on_kafka_lost(self, consumer, partitions: List[TopicPartition]):
         logger.info("Group rebalancing. Partitions lost %s", partitions)
         for p in partitions:
             self.assigned_partitions[p.topic].discard(p.partition)
 
+    def is_assigned(self, topic):
+        return len(self.assigned_partitions[topic]) > 0
+
     def get_topic_stats(self) -> Dict[str, int]:
         result = self.topic_stats
         self.topic_stats = defaultdict(int)
         return result
 
     def messages_in_queue(self) -> int:
         if self.role != KafkaRole.PRODUCER:
```

### Comparing `citizenk-0.1.47/citizenk/murmur2.py` & `citizenk-0.1.48/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.47/citizenk/topic.py` & `citizenk-0.1.48/citizenk/topic.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,22 +69,26 @@
         if self.name in assignments:
             topic_info["assignments"] = assignments[self.name]
         return topic_info
 
     def _generate_apis(self):
         if self.topic_dir in [TopicDir.OUTPUT, TopicDir.BIDIR]:
 
-            def f(value: int, key: str = ""):
-                self.send(value, key)
+            def f(value: int, key: str = "", count: int = 1, partition: int = -1):
+                for n in range(count):
+                    if key == "":
+                        self.send(value, str(n), partition)
+                    else:
+                        self.send(value, key, partition)
                 return value
 
             annotate_function(
                 f,
                 name=f"send_to_topic_{self.name}",
-                doc=f"This endpoint send value to topic {self.name}",
+                doc=f"This endpoint sends value to topic {self.name}",
                 argument_types={"value": self.value_type},
             )
             self.app.add_api_route(
                 path=f"{self.app.api_router_prefix}/topic/{self.name}",
                 response_class=JSONResponse,
                 methods=["POST"],
                 endpoint=f,
```

### Comparing `citizenk-0.1.47/pyproject.toml` & `citizenk-0.1.48/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.47"
+version = "0.1.48"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
-keywords = ["kafka", "fastapi"]
+keywords = ["kafka", "fastapi", "confluent", "pydantic", "distributed", "real-time"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
-    "Development Status :: 4 - Beta",
-    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Framework :: FastAPI"
+    "Framework :: FastAPI",
+    "Topic :: System :: Distributed Computing",
+    "Topic :: Software Development",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 confluent-kafka = {extras = ["schema-registry"], version = "2.0.2"}
 certifi = "^2022.12.7"
 fastapi = "^0.92.0"
```

### Comparing `citizenk-0.1.47/setup.py` & `citizenk-0.1.48/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,476 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: citizenk
+Version: 0.1.48
+Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
+Home-page: https://pypi.org/user/valerann/
+License: Apache-2.0
+Keywords: kafka,fastapi,confluent,pydantic,distributed,real-time
+Author: Valerann
+Author-email: info@valerann.com
+Maintainer: Valerann
+Maintainer-email: info@valerann.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: FastAPI
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Distributed Computing
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: confluent-kafka[schema-registry] (==2.0.2)
+Requires-Dist: fastapi (>=0.92.0,<0.93.0)
+Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: websockets (>=10.4,<11.0)
+Project-URL: Repository, https://github.com/Valerann/citizenk
+Description-Content-Type: text/markdown
 
-packages = \
-['citizenk']
+# CitizenK
+**CitizienK** is a simple but powerful Python Library for developing reactive async Kafka microservices, built on top of [Confluent Kafka Python](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html), [FastAPI](https://fastapi.tiangolo.com/) and [Pydantic](https://docs.pydantic.dev/).
 
-package_data = \
-{'': ['*']}
+**CitizenK Replicator** is an additional tool that we developed using the same technology to simplify data transfer between production and staging environments. It's not a substitution for Confluent's replicator which is a much more robust tool for replicating data between multiple production environments
 
-install_requires = \
-['certifi>=2022.12.7,<2023.0.0',
- 'confluent-kafka[schema-registry]==2.0.2',
- 'fastapi-utils>=0.2.1,<0.3.0',
- 'fastapi>=0.92.0,<0.93.0',
- 'httpx>=0.23.3,<0.24.0',
- 'websockets>=10.4,<11.0']
-
-setup_kwargs = {
-    'name': 'citizenk',
-    'version': '0.1.47',
-    'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
-    'long_description': '# CitizenK\n**CitizienK** is a simple but powerful Python Library for developing reactive async Kafka microservices, built on top of [Confluent Kafka Python](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html), [FastAPI](https://fastapi.tiangolo.com/) and [Pydantic](https://docs.pydantic.dev/).\n\n**CitizenK Replicator** is an additional tool that we developed using the same technology to simplify data transfer between production and staging environments. It\'s not a substitution for Confluent\'s replicator which is a much more robust tool for replicating data between multiple production environments\n\n------------------------------------------------------------------------\n------------------------------------------------------------------------\n\n## How we got here...\nWe are a Python shop. We develop web services in Python, write ETL code in Python, and obviously use Python for data science. A few years ago, when we started working on Lanternn, we were looking for a python library that can help us build distributed, scalable processing pipelines on top of Kafka with stateless and stateful microservices. The best solution that we could find at the time was Faust. Faust is a stream processing library, porting ideas from Kafka Streams to Python. Additionally, Faust includes a powerful web server, schema validation and management, and is based on an agents/actors approach. With so many goodies, how could we resist?\n\n\nWe built dozens of services using Faust, and all in all, we were pretty happy with it. however, over time we realized that Kafka Streams is not really working for us, it\'s just too complex to manage and other alternatives for state management like Redis are simpler. We were also worried that Faust without the spirit of its creator Ask Solem, and its underlying Kafka library: aiokafka and python-kafka don\'t have a large enough community to support the stability issues that we had experienced. In parallel, frameworks like FastAPI and Confluent Kafka that we used anyway had large community backing, and we felt like we can use them together to build an alternative foundation for our pipelines.\n\n\nThe name CitizenK was chosen to reflect the idea that Python should be a first-class citizen in the Kafka world.\n\nIt is also related to Kafka\'s most famous novel: The Trial, which tells the story of Josef K. a man arrested and prosecuted by a remote, inaccessible authority, with the nature of his crime revealed neither to him nor to the reader.\n\n## Existing tools\n- Faust\n- Fastkafka\n\n------------------------------------------------------------------------\n\n## Tutorial\n\nYou can see an example of how to use CitizenK in the demo app\n\n### Creating a CitizienK app\n\nFirst, we create a CitizenK app similar to how we create a FastAPI app, but with additional arguments:\n\n- kafka_config: provides configuration for connecting and configuring the Kafka client\n- app_name: Mainly used as the consumer group name\n- app_type: SINK (consumer only), SOURCE(producer only) or TRANSFORM(producer-consumer)\n- auto_generate_apis: Will auto generate FastAPI to consume and produce to workers and topics\n- agents_in_thread: Will run the consumer agents in a thread and not in an async loop\n\n``` python\napp = CitizenK(\n    kafka_config=config.source_kafka,\n    app_name="citizenk",\n    app_type=AppType.TRANSFORM,\n    debug=True,\n    title="CitizenK Demo App",\n    auto_generate_apis=True,\n    agents_in_thread=config.AGENTS_IN_THREAD,\n    api_router_prefix=prefix,\n    api_port=config.API_PORT,\n    schema_registry_url=config.KAFKA_SOURCE_SCHEMA_REGISTRY,\n    version=config.VERSION,\n    openapi_url=prefix + "/openapi.json",\n    docs_url=prefix + "/docs",\n    license_info={\n        "name": "Apache 2.0",\n        "url": "https://www.apache.org/licenses/LICENSE-2.0.html",\n    },\n)\n```\n\n### Creating CitizienK topics\nNext, we create topics for the app and define the model for the topics using Pydantic\n\nTopics can be either INPUT, OUTPUT or BIDIR\n\n``` python\nclass Video(JSONSchema):\n    camera_id: int\n    path: str\n    timestamp: datetime\n\n\nclass ProcessedVideo(JSONSchema):\n    camera_id: int\n    path: str\n    timestamp: datetime\n    valid: bool\n\n\nt1 = app.topic(name="B", value_type=Video, topic_dir=TopicDir.BIDIR)\nt2 = app.topic(name="C", value_type=ProcessedVideo, topic_dir=TopicDir.BIDIR)\nt3 = app.topic(name="D", value_type=ProcessedVideo, topic_dir=TopicDir.OUTPUT)\n```\n\n### Creating CitizienK agents\nAnd lastly, we create gents that process the Kafka messages.\n\nAgents can listen to multiple topics and accept either values or the entire Kafka event (key, value, offset, partition, timestamp...)\n\n``` python\n@app.agent(topics=t1, batch_size=100)\nasync def process_videos_t1(events: List[KafkaEvent]):\n    # Process incoming video\n    for event in events:\n        camera_id = event.value.camera_id\n        video_counts[camera_id] += 1\n        v = ProcessedVideo(\n            camera_id=camera_id,\n            path=event.value.path,\n            timestamp=event.value.timestamp,\n            valid=bool(camera_id % 2),\n        )\n        t2.send(value=v, key=str(v.camera_id))\n\n\n@app.agent(topics=t2, batch_size=100)\nasync def process_videos_t2(values: List[BaseModel]):\n    # Process incoming video\n    for value in values:\n        if value.valid:\n            t3.send(value=value, key=str(value.camera_id))\n\n```\n\n### Auto endpoints\nTo help debug and evaluate the service, CitizenK automatically creates web endpoints that help you send messages to topics and agents.\n\n- info: get service info\n- topics: send events to topics\n- agents: send events directly to agents, bypassing topics\n- stats: get Kafka stats for producer and consumer\n\n![CitizenK Demo API](docs/citizenk_demo_api.jpg)\n\n\n### Creating additional CitizienK endpoints\nJust like any other FastAPI app, you can create get, post and put endpoints that either interact with Kafka or perform some other tasks, non Kafka related\n\n``` python\n@router.post("/events", response_class=JSONResponse)\nasync def produce_video_events(\n    values: List[Video],\n    topic: str = Query(),\n):\n    """Sends events to the given topic"""\n    if topic not in app.topics:\n        raise HTTPException(status_code=400, detail="Topic not supported by app")\n    t = app.topics[topic]\n    for v in values:\n        t.send(value=v, key=str(v.camera_id))\n    return {"status": "ok"}\n\n\n@router.get("/topics", response_class=JSONResponse)\nasync def get_source_topics():\n    """Returns the list of topics from the source kafka"""\n    admin = KafkaAdapter(config.source_kafka)\n    topics = sorted(list(admin.get_all_broker_topics().keys()))\n    return {"topics": topics}\n```\n\n### Multiple workers behind a load balancer\nCitizenK includes two special decorators for scenarios where the service has multiple workers behind a load balancer and the web request needs to reach a specific worker that holds a partition.\n\n- topic_router: forwards the request based on the topic and key (JSON / HTML)\n- broadcast_router: aggregates the responses from all workers into a single JSON\n\nBoth routers support GET, POST, PUT and DELETE commands\n\n``` python\n@router.get("/topic_test", response_class=JSONResponse)\n@app.topic_router(topic=t1, match_info="camera_id")\nasync def test_topic_router(request: Request, camera_id: int):\n    """Returns the list of groups from the target kafka"""\n    return {"key": camera_id, "count": video_counts[camera_id]}\n\n\n@router.get("/broadcast_test", response_class=JSONResponse)\n@app.broadcast_router()\nasync def test_broadcast_router(request: Request):\n    """Returns the list of groups from the target kafka"""\n    return video_counts\n```\n\n### Websocket\nCitizenK support for Websocket agents\n\n``` python\n@app.agent(topics=t2, batch_size=100, websocket_route=prefix + "/ws")\nasync def websocket_agent(values: List[BaseModel]) -> str:\n    values = [json.loads(v.json()) for v in values if not v.valid]\n    return json.dumps(values, indent=4)\n```\n\nThis agent exposes a WebSocket endpoint for one or more clients to connect to. It then processes incoming Kafka messages from topic t2 and sends the returned string value to all the existing live WebSocket "/ws" connections. The main use case for this is to bridge between Kafka and Websocket. One possible use case for this feature is to send filtered Kafka events to a web app or mobile app.\n\n\nThe other direction frontend --> Kafka is probably easier to implement with a normal REST post endpoint and is not supported yet.\n\n## Things to be aware of...\nCitizenK is a single-threaded async app. i.e. If a coroutine spends too much time in processing without awaiting IO, it will block other coroutines from running. Specifically, when using a load balancer with health checks, it\'s important to pay attention to the time between health checks and see that it\'s higher than the longest-running agent. Fixed using:agents_in_thread\n\n\nTo help tune the service. CitizenK includes the concept of batch size:i.e. how many events to consume and process every batch across all agents.\n\nAdditionally like any other Kafka service. it\'s important to tune several kafka [consumer](https://docs.confluent.io/platform/current/installation/configuration/consumer-configs.html#fetch-max-bytes) and [producer](https://docs.confluent.io/platform/current/installation/configuration/producer-configs.html) configs. Specifically ensure rebalancing is not triggered unintentionally:\n\n\nConsumer:\n- fetch.max.bytes (50 Mbytes): The maximum amount of data the server should return for a fetch request. Reduce if processing each record takes significant time.\n- max.poll.records(500): The maximum number of records returned in a single call to poll().\n- max.poll.interval.ms (5 min): The maximum delay between invocations of poll() when using consumer group management\n\nProducer:\n- linger.ms(0): Important to set to 0/5/10/50/200 on moderate/high load\n- batch.size(16K): Increase if sending large buffers to Kafka\n\nBoth:\n- compression.type(none): gzip, snappy, or lz4\n\nMore explanation in here: [Solving My Weird Kafka Rebalancing Problems & Explaining What Is Happening and Why?](https://medium.com/bakdata/solving-my-weird-kafka-rebalancing-problems-c05e99535435)\n\n## Limitations\nAt the moment the library only supports JSON schema\n\n------------------------------------------------------------------------\n\n\n# CitizenK Replicator\n## Scenarios\n\n### Staging environment\n1. I have a staging environment and I want to replicate some production topics to it\n\n2. At some point I want to produce the staging topics in the staging environment using a staging service. So I switch off the replication and populate the same staging topic with real data.\n\n3. When I finish the testing in staging, I want to switch back to production, so that I can save on costs.\n\n4. If the workload is high, I want to replicate most (i.e. 90%) of the messages from production and only produce just a little (i.e. 10%) of the data from staging. This way in the same topic, I will have mixed data and potential schema from the two environments\n\n5. When switching between environments (i.e. on configuration change), I want to change the offset to the latest on the new topic, so that the handover is not too chaotic\n\n6. I also want to delete the consumer group of the service in staging, so that when it come back up again, it won\'t see a lag.\n\n7. Additionally sometimes, I want to migrate data between production and staging due to schema change or different identities.\n\n![Replicator](docs/replicator.jpg)\n\n### Dev environment + live data\n1. When I test a service locally or in a dev environment, possibly with a local Kafka, I want the local Kafka to have real data, so that I can test the service for a long period of time with live data.\n\n2. Theoretically, I can connect the dev service to the staging or production Kafka cluster, however, this presents a stability/security risk to the remote cluster. There is also a risk that the service will join a consumer group and participate accidentally in the remote workload. This approach also prevents parallel testing as there can be a conflict between the consumers.\n\n3. So one solution would be to replicate the topics from staging to the local/dev Kafka, maybe with some filtering to reduce the load, so that the local service is not overwhelmed with too much data\n\n### On premise kafka -- cloud kafka bridge\n1. I have a local Kafka and I want to replicate some topics to the remote cloud\n\n2. You can use this tool for this scenario, however Confluent replicator or Kafka MirrorMaker are probably more suitable\n\n### Dev environment + replayed data\n1. When I test a service locally or in a dev environment, possibly with a local Kafka, I want the local Kafka to replay historical/simulated messages from a file.\n\n2. this scenario is a bit different from the previous ones, as there is no Kafka consumer, just a producer. And you can say that it is more of a tool than a service.\n\n3. The messages are read from a file with a timestamp (one file for each topic), and injected into the right topic with the correct timing keeping the same gap between now, and the initial timestamp.\n\n\n### Cluster -- Cluster replication\n1. You can use this tool for this scenario, however Confluent replicator or Kafka MirrorMaker are probably more suitable\n\n## Existing tools\n1. Confluent replicator: Looks like a good tool, but not open source, expensive\n2. Kafka Mirror Maker: Open source but doesn\'t support filtering\n3. kcat: Nice tool, but not for these scenarios\n\n\n## Implementation details\n1. Using containerised python\n2. Based on Confluent Kafka API + FastAP\n3. Does not create the topics or partitions automatically. It assumes they exists and configured\n3. Deployed as a distributed service\n4. Filter based on JMESPath for JSON messages\n5. Allow two consumer options: with consumer group, without consumer group\n6. write code following DDD principles\n\n## Configuration\n- LOG_LEVEL: service log level\n- JSON_LOGGING: Use json logging\n- API_PREFIX: API prefix\n- FILE_DATA_PATH: Location of json files when reading and writing topics from file\n- KAFKA_SOURCE_SERVER_URL: Source Bootstrap Servers\n- KAFKA_SOURCE_USE_TLS: Enable Source SSL: 0,1\n- KAFKA_SOURCE_SASL_MECHANISM: Source SASL mechanism: PLAIN, SCRAM-SHA-256, SCRAM-SHA-512\n- KAFKA_SOURCE_SASL_USERNAME: Source SASL username\n- KAFKA_SOURCE_SASL_PASSWORD: Source SASL password\n- KAFKA_SOURCE_GROUP_NAME: Source group name, or leave empty to consume without a consumer group\n- KAFKA_SOURCE_EXTRA_CONFIG_<KAFKA_CONFIG_KEY>: Any valid kafka consumer config (uppercase, replace . with _)\n- KAFKA_TARGET_SERVER_URL: Target Bootstrap Servers\n- KAFKA_TARGET_USE_TLS: Enable Target SSL\n- KAFKA_TARGET_SASL_MECHANISM: Target SASL mechanism: PLAIN, SCRAM-SHA-256, SCRAM-SHA-512\n- KAFKA_TARGET_SASL_USERNAME: Target SASL username\n- KAFKA_TARGET_SASL_PASSWORD: Target SASL password\n- KAFKA_TARGET_EXTRA_CONFIG_<KAFKA_CONFIG_KEY>: Any valid kafka producer config (uppercase, replace . with _)\n- READ_MAPPINGS_EVERY_SECONDS: How often to check for new mappings in the file system\n- CACULATE_STATS_EVERY_SECONDS: How often to calculate stats\n- DELETE_GROUPS_EVERY_SECONDS: How often to check for new group deletion\n\n## Current solution limitations\n1. Currently only supports JSON schema.\n\n## API\n[API Description](docs/replicator_openapi.md)\n\n![Replicator API](docs/replicator_api.jpg)\n\n## User Interface\n![Replicator User Interface](docs/replicator_ui.jpg)\n\nThe user interface allows you to add a new mapping and edit/delete an existing mapping.\n\n## Usage\nProvide a JSON list of topic mappings in this format:\n```json\n[\n    {\n        "name": "File A to B",\n        "source_topic_name": "A",\n        "target_topic_name": "B",\n        "source_is_file": true\n    },\n    {\n        "name": "Topic B to C",\n        "source_topic_name": "B",\n        "target_topic_name": "C"\n    },\n    {\n        "name": "Topic C to D Using filter",\n        "source_topic_name": "C",\n        "target_topic_name": "D",\n        "valid_jmespath": "key == \'hello\' && value.msg == \'world\'",\n        "enabled": true\n    },\n    {\n        "name": "TopicCtoD",\n        "source_topic_name": "C",\n        "target_topic_name": "D",\n        "enabled": false,\n        "target_service_consumer_group": "service"\n    },\n    {\n        "name": "Topic D to File E",\n        "source_topic_name": "D",\n        "target_topic_name": "E",\n        "target_is_file": true\n    },\n    {\n        "name": "Disabled Topic U to File V",\n        "source_topic_name": "U",\n        "target_topic_name": "V",\n        "target_is_file": true,\n        "enabled": false\n    }\n]\n```\n\n- name: The mapping name\n- enabled: Enable / disable mapping\n- source_topic_name: The topic to read from in the source cluster\n- target_topic_name: The topic to write to in the target cluster\n- valid_jmespath: filter criteria\n- source_is_file: If the source is a json file\n- target_is_file: If the target is a json file\n- target_service_consumer_group: The service consumer group to delete when replication is enabled\n\n## Topic Level Mapping\nTopic level mappings allows mapping of key/values when replicating a topic. This might be useful if for example the schema / enums / keys are different between the environments\n\nTo support this, the replicator supports value mappings for each topic that it consumes from the source in the following JSON format:\n\n```json\n{\n    "key":{\n        "1":10,\n        "2":12\n    },\n    "value.payload.product_id":{\n        "1001":1,\n        "1002":12,\n        "1003":14\n    },\n    "value.payload.user_name":{\n        "A":"A name",\n        "B":"B name",\n        "C":"C name"\n    },\n    "partition":{\n        "0":0,\n        "1":0,\n        "2":0,\n        "3":1,\n        "4":1,\n        "5":1,\n    }\n}\n```\n\n## Stats\nReturns a list of JSON stats for each mapping in the following format:\n```json\n{\n    "time": "2023-05-25 18:20:43.875557",\n    "started": "2023-05-25 08:08:35.728313",\n    "queue": 180,\n    "mappings": [\n        {\n            "name": "Topic B to C",\n            "source_topic_name": "B",\n            "target_topic_name": "C",\n            "valid_jmespath": null,\n            "target_service_consumer_group": null,\n            "consumer_group_up": false,\n            "assignments": [0,1,2],\n            "lag": 1258,\n            "source_count": 27739,\n            "target_count": 27739\n        }\n    ]\n}\n```\n\n## Grafana Integration\nTo view the stats in Grafana, use the Infinity data source with the following settings:\n\n![Replicator Grafana Interface](docs/replicator_grafana.jpg)\n\n## Consumer API\nTo simplify debug and to support other use cases, the replicator also includes an end point to consume messages from a given topic.\n\n\n## License\n[Apache License v2.0](https://www.apache.org/licenses/LICENSE-2.0)\n',
-    'author': 'Valerann',
-    'author_email': 'info@valerann.com',
-    'maintainer': 'Valerann',
-    'maintainer_email': 'info@valerann.com',
-    'url': 'https://pypi.org/user/valerann/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+------------------------------------------------------------------------
+------------------------------------------------------------------------
+
+## How we got here...
+We are a Python shop. We develop web services in Python, write ETL code in Python, and obviously use Python for data science. A few years ago, when we started working on Lanternn, we were looking for a python library that can help us build distributed, scalable processing pipelines on top of Kafka with stateless and stateful microservices. The best solution that we could find at the time was Faust. Faust is a stream processing library, porting ideas from Kafka Streams to Python. Additionally, Faust includes a powerful web server, schema validation and management, and is based on an agents/actors approach. With so many goodies, how could we resist?
+
+
+We built dozens of services using Faust, and all in all, we were pretty happy with it. however, over time we realized that Kafka Streams is not really working for us, it's just too complex to manage and other alternatives for state management like Redis are simpler. We were also worried that Faust without the spirit of its creator Ask Solem, and its underlying Kafka library: aiokafka and python-kafka don't have a large enough community to support the stability issues that we had experienced. In parallel, frameworks like FastAPI and Confluent Kafka that we used anyway had large community backing, and we felt like we can use them together to build an alternative foundation for our pipelines.
+
+
+The name CitizenK was chosen to reflect the idea that Python should be a first-class citizen in the Kafka world.
+
+It is also related to Kafka's most famous novel: The Trial, which tells the story of Josef K. a man arrested and prosecuted by a remote, inaccessible authority, with the nature of his crime revealed neither to him nor to the reader.
+
+## Existing tools
+- Faust
+- Fastkafka
+
+------------------------------------------------------------------------
+
+## Tutorial
+
+You can see an example of how to use CitizenK in the demo app
+
+### Creating a CitizienK app
+
+First, we create a CitizenK app similar to how we create a FastAPI app, but with additional arguments:
+
+- kafka_config: provides configuration for connecting and configuring the Kafka client
+- app_name: Mainly used as the consumer group name
+- app_type: SINK (consumer only), SOURCE(producer only) or TRANSFORM(producer-consumer)
+- auto_generate_apis: Will auto generate FastAPI to consume and produce to workers and topics
+- agents_in_thread: Will run the consumer agents in a thread and not in an async loop
+
+``` python
+app = CitizenK(
+    kafka_config=config.source_kafka,
+    app_name="citizenk",
+    app_type=AppType.TRANSFORM,
+    debug=True,
+    title="CitizenK Demo App",
+    auto_generate_apis=True,
+    agents_in_thread=config.AGENTS_IN_THREAD,
+    api_router_prefix=prefix,
+    api_port=config.API_PORT,
+    schema_registry_url=config.KAFKA_SOURCE_SCHEMA_REGISTRY,
+    version=config.VERSION,
+    openapi_url=prefix + "/openapi.json",
+    docs_url=prefix + "/docs",
+    license_info={
+        "name": "Apache 2.0",
+        "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
+    },
+)
+```
+
+### Creating CitizienK topics
+Next, we create topics for the app and define the model for the topics using Pydantic
+
+Topics can be either INPUT, OUTPUT or BIDIR
+
+``` python
+class Video(JSONSchema):
+    camera_id: int
+    path: str
+    timestamp: datetime
+
+
+class ProcessedVideo(JSONSchema):
+    camera_id: int
+    path: str
+    timestamp: datetime
+    valid: bool
+
+
+t1 = app.topic(name="B", value_type=Video, topic_dir=TopicDir.BIDIR)
+t2 = app.topic(name="C", value_type=ProcessedVideo, topic_dir=TopicDir.BIDIR)
+t3 = app.topic(name="D", value_type=ProcessedVideo, topic_dir=TopicDir.OUTPUT)
+```
+
+### Creating CitizienK agents
+And lastly, we create gents that process the Kafka messages.
+
+Agents can listen to multiple topics and accept either values or the entire Kafka event (key, value, offset, partition, timestamp...)
+
+``` python
+@app.agent(topics=t1, batch_size=100)
+async def process_videos_t1(events: List[KafkaEvent]):
+    # Process incoming video
+    for event in events:
+        camera_id = event.value.camera_id
+        video_counts[camera_id] += 1
+        v = ProcessedVideo(
+            camera_id=camera_id,
+            path=event.value.path,
+            timestamp=event.value.timestamp,
+            valid=bool(camera_id % 2),
+        )
+        t2.send(value=v, key=str(v.camera_id))
+
+
+@app.agent(topics=t2, batch_size=100)
+async def process_videos_t2(values: List[BaseModel]):
+    # Process incoming video
+    for value in values:
+        if value.valid:
+            t3.send(value=value, key=str(value.camera_id))
+
+```
+
+### Auto endpoints
+To help debug and evaluate the service, CitizenK automatically creates web endpoints that help you send messages to topics and agents.
+
+- info: get service info
+- topics: send events to topics
+- agents: send events directly to agents, bypassing topics
+- stats: get Kafka stats for producer and consumer
+
+![CitizenK Demo API](docs/citizenk_demo_api.jpg)
+
+
+### Creating additional CitizienK endpoints
+Just like any other FastAPI app, you can create get, post and put endpoints that either interact with Kafka or perform some other tasks, non Kafka related
+
+``` python
+@router.post("/events", response_class=JSONResponse)
+async def produce_video_events(
+    values: List[Video],
+    topic: str = Query(),
+):
+    """Sends events to the given topic"""
+    if topic not in app.topics:
+        raise HTTPException(status_code=400, detail="Topic not supported by app")
+    t = app.topics[topic]
+    for v in values:
+        t.send(value=v, key=str(v.camera_id))
+    return {"status": "ok"}
+
+
+@router.get("/topics", response_class=JSONResponse)
+async def get_source_topics():
+    """Returns the list of topics from the source kafka"""
+    admin = KafkaAdapter(config.source_kafka)
+    topics = sorted(list(admin.get_all_broker_topics().keys()))
+    return {"topics": topics}
+```
+
+### Multiple workers behind a load balancer
+CitizenK includes two special decorators for scenarios where the service has multiple workers behind a load balancer and the web request needs to reach a specific worker that holds a partition.
+
+- topic_router: forwards the request based on the topic and key (JSON / HTML)
+- broadcast_router: aggregates the responses from all workers into a single JSON
+
+Both routers support GET, POST, PUT and DELETE commands
+
+``` python
+@router.get("/topic_test", response_class=JSONResponse)
+@app.topic_router(topic=t1, match_info="camera_id")
+async def test_topic_router(request: Request, camera_id: int):
+    """Returns the list of groups from the target kafka"""
+    return {"key": camera_id, "count": video_counts[camera_id]}
+
+
+@router.get("/broadcast_test", response_class=JSONResponse)
+@app.broadcast_router()
+async def test_broadcast_router(request: Request):
+    """Returns the list of groups from the target kafka"""
+    return video_counts
+```
+
+### Websocket
+CitizenK support for Websocket agents
+
+``` python
+@app.agent(topics=t2, batch_size=100, websocket_route=prefix + "/ws")
+async def websocket_agent(values: List[BaseModel]) -> str:
+    values = [json.loads(v.json()) for v in values if not v.valid]
+    return json.dumps(values, indent=4)
+```
+
+This agent exposes a WebSocket endpoint for one or more clients to connect to. It then processes incoming Kafka messages from topic t2 and sends the returned string value to all the existing live WebSocket "/ws" connections. The main use case for this is to bridge between Kafka and Websocket. One possible use case for this feature is to send filtered Kafka events to a web app or mobile app.
+
+
+The other direction frontend --> Kafka is probably easier to implement with a normal REST post endpoint and is not supported yet.
+
+## Things to be aware of...
+CitizenK is a single-threaded async app. i.e. If a coroutine spends too much time in processing without awaiting IO, it will block other coroutines from running. Specifically, when using a load balancer with health checks, it's important to pay attention to the time between health checks and see that it's higher than the longest-running agent. Fixed using:agents_in_thread
+
+
+To help tune the service. CitizenK includes the concept of batch size:i.e. how many events to consume and process every batch across all agents.
+
+Additionally like any other Kafka service. it's important to tune several kafka [consumer](https://docs.confluent.io/platform/current/installation/configuration/consumer-configs.html#fetch-max-bytes) and [producer](https://docs.confluent.io/platform/current/installation/configuration/producer-configs.html) configs. Specifically ensure rebalancing is not triggered unintentionally:
+
+
+Consumer:
+- fetch.max.bytes (50 Mbytes): The maximum amount of data the server should return for a fetch request. Reduce if processing each record takes significant time.
+- max.poll.records(500): The maximum number of records returned in a single call to poll().
+- max.poll.interval.ms (5 min): The maximum delay between invocations of poll() when using consumer group management
+
+Producer:
+- linger.ms(0): Important to set to 0/5/10/50/200 on moderate/high load
+- batch.size(16K): Increase if sending large buffers to Kafka
+
+Both:
+- compression.type(none): gzip, snappy, or lz4
+
+More explanation in here: [Solving My Weird Kafka Rebalancing Problems & Explaining What Is Happening and Why?](https://medium.com/bakdata/solving-my-weird-kafka-rebalancing-problems-c05e99535435)
+
+## Limitations
+At the moment the library only supports JSON schema
+
+------------------------------------------------------------------------
+
+
+# CitizenK Replicator
+## Scenarios
+
+### Staging environment
+1. I have a staging environment and I want to replicate some production topics to it
+
+2. At some point I want to produce the staging topics in the staging environment using a staging service. So I switch off the replication and populate the same staging topic with real data.
+
+3. When I finish the testing in staging, I want to switch back to production, so that I can save on costs.
+
+4. If the workload is high, I want to replicate most (i.e. 90%) of the messages from production and only produce just a little (i.e. 10%) of the data from staging. This way in the same topic, I will have mixed data and potential schema from the two environments
+
+5. When switching between environments (i.e. on configuration change), I want to change the offset to the latest on the new topic, so that the handover is not too chaotic
+
+6. I also want to delete the consumer group of the service in staging, so that when it come back up again, it won't see a lag.
+
+7. Additionally sometimes, I want to migrate data between production and staging due to schema change or different identities.
+
+![Replicator](docs/replicator.jpg)
+
+### Dev environment + live data
+1. When I test a service locally or in a dev environment, possibly with a local Kafka, I want the local Kafka to have real data, so that I can test the service for a long period of time with live data.
+
+2. Theoretically, I can connect the dev service to the staging or production Kafka cluster, however, this presents a stability/security risk to the remote cluster. There is also a risk that the service will join a consumer group and participate accidentally in the remote workload. This approach also prevents parallel testing as there can be a conflict between the consumers.
+
+3. So one solution would be to replicate the topics from staging to the local/dev Kafka, maybe with some filtering to reduce the load, so that the local service is not overwhelmed with too much data
+
+### On premise kafka -- cloud kafka bridge
+1. I have a local Kafka and I want to replicate some topics to the remote cloud
+
+2. You can use this tool for this scenario, however Confluent replicator or Kafka MirrorMaker are probably more suitable
+
+### Dev environment + replayed data
+1. When I test a service locally or in a dev environment, possibly with a local Kafka, I want the local Kafka to replay historical/simulated messages from a file.
+
+2. this scenario is a bit different from the previous ones, as there is no Kafka consumer, just a producer. And you can say that it is more of a tool than a service.
+
+3. The messages are read from a file with a timestamp (one file for each topic), and injected into the right topic with the correct timing keeping the same gap between now, and the initial timestamp.
+
+
+### Cluster -- Cluster replication
+1. You can use this tool for this scenario, however Confluent replicator or Kafka MirrorMaker are probably more suitable
+
+## Existing tools
+1. Confluent replicator: Looks like a good tool, but not open source, expensive
+2. Kafka Mirror Maker: Open source but doesn't support filtering
+3. kcat: Nice tool, but not for these scenarios
+
+
+## Implementation details
+1. Using containerised python
+2. Based on Confluent Kafka API + FastAP
+3. Does not create the topics or partitions automatically. It assumes they exists and configured
+3. Deployed as a distributed service
+4. Filter based on JMESPath for JSON messages
+5. Allow two consumer options: with consumer group, without consumer group
+6. write code following DDD principles
+
+## Configuration
+- LOG_LEVEL: service log level
+- JSON_LOGGING: Use json logging
+- API_PREFIX: API prefix
+- FILE_DATA_PATH: Location of json files when reading and writing topics from file
+- KAFKA_SOURCE_SERVER_URL: Source Bootstrap Servers
+- KAFKA_SOURCE_USE_TLS: Enable Source SSL: 0,1
+- KAFKA_SOURCE_SASL_MECHANISM: Source SASL mechanism: PLAIN, SCRAM-SHA-256, SCRAM-SHA-512
+- KAFKA_SOURCE_SASL_USERNAME: Source SASL username
+- KAFKA_SOURCE_SASL_PASSWORD: Source SASL password
+- KAFKA_SOURCE_GROUP_NAME: Source group name, or leave empty to consume without a consumer group
+- KAFKA_SOURCE_EXTRA_CONFIG_<KAFKA_CONFIG_KEY>: Any valid kafka consumer config (uppercase, replace . with _)
+- KAFKA_TARGET_SERVER_URL: Target Bootstrap Servers
+- KAFKA_TARGET_USE_TLS: Enable Target SSL
+- KAFKA_TARGET_SASL_MECHANISM: Target SASL mechanism: PLAIN, SCRAM-SHA-256, SCRAM-SHA-512
+- KAFKA_TARGET_SASL_USERNAME: Target SASL username
+- KAFKA_TARGET_SASL_PASSWORD: Target SASL password
+- KAFKA_TARGET_EXTRA_CONFIG_<KAFKA_CONFIG_KEY>: Any valid kafka producer config (uppercase, replace . with _)
+- READ_MAPPINGS_EVERY_SECONDS: How often to check for new mappings in the file system
+- CACULATE_STATS_EVERY_SECONDS: How often to calculate stats
+- DELETE_GROUPS_EVERY_SECONDS: How often to check for new group deletion
+
+## Current solution limitations
+1. Currently only supports JSON schema.
+
+## API
+[API Description](docs/replicator_openapi.md)
+
+![Replicator API](docs/replicator_api.jpg)
+
+## User Interface
+![Replicator User Interface](docs/replicator_ui.jpg)
+
+The user interface allows you to add a new mapping and edit/delete an existing mapping.
+
+## Usage
+Provide a JSON list of topic mappings in this format:
+```json
+[
+    {
+        "name": "File A to B",
+        "source_topic_name": "A",
+        "target_topic_name": "B",
+        "source_is_file": true
+    },
+    {
+        "name": "Topic B to C",
+        "source_topic_name": "B",
+        "target_topic_name": "C"
+    },
+    {
+        "name": "Topic C to D Using filter",
+        "source_topic_name": "C",
+        "target_topic_name": "D",
+        "valid_jmespath": "key == 'hello' && value.msg == 'world'",
+        "enabled": true
+    },
+    {
+        "name": "TopicCtoD",
+        "source_topic_name": "C",
+        "target_topic_name": "D",
+        "enabled": false,
+        "target_service_consumer_group": "service"
+    },
+    {
+        "name": "Topic D to File E",
+        "source_topic_name": "D",
+        "target_topic_name": "E",
+        "target_is_file": true
+    },
+    {
+        "name": "Disabled Topic U to File V",
+        "source_topic_name": "U",
+        "target_topic_name": "V",
+        "target_is_file": true,
+        "enabled": false
+    }
+]
+```
+
+- name: The mapping name
+- enabled: Enable / disable mapping
+- source_topic_name: The topic to read from in the source cluster
+- target_topic_name: The topic to write to in the target cluster
+- valid_jmespath: filter criteria
+- source_is_file: If the source is a json file
+- target_is_file: If the target is a json file
+- target_service_consumer_group: The service consumer group to delete when replication is enabled
+
+## Topic Level Mapping
+Topic level mappings allows mapping of key/values when replicating a topic. This might be useful if for example the schema / enums / keys are different between the environments
+
+To support this, the replicator supports value mappings for each topic that it consumes from the source in the following JSON format:
+
+There are two mapping formats:
+- value.payload.product_id : map source product_id to target product_id
+- key:partition: map source key to target partition (drop entire msg if partition equals -1000)
+
+```json
+{
+    "key":{
+        "1":10,
+        "2":12
+    },
+    "value.payload.product_id":{
+        "1001":1,
+        "1002":12,
+        "1003":14
+    },
+    "value.payload.user_name":{
+        "A":"A name",
+        "B":"B name",
+        "C":"C name"
+    },
+    "key:partition":{
+        "1":0,
+        "2":0,
+        "3":-1000,
+        "4":1,
+        "5":1,
+        "6":1,
+    }
 }
+```
+
+## Stats
+Returns a list of JSON stats for each mapping in the following format:
+```json
+{
+    "time": "2023-05-25 18:20:43.875557",
+    "started": "2023-05-25 08:08:35.728313",
+    "queue": 180,
+    "mappings": [
+        {
+            "name": "Topic B to C",
+            "source_topic_name": "B",
+            "target_topic_name": "C",
+            "valid_jmespath": null,
+            "target_service_consumer_group": null,
+            "consumer_group_up": false,
+            "assignments": [0,1,2],
+            "lag": 1258,
+            "source_count": 27739,
+            "target_count": 27739
+        }
+    ]
+}
+```
+
+## Grafana Integration
+To view the stats in Grafana, use the Infinity data source with the following settings:
+
+![Replicator Grafana Interface](docs/replicator_grafana.jpg)
+
+## Consumer API
+To simplify debug and to support other use cases, the replicator also includes an end point to consume messages from a given topic.
+
 
+## License
+[Apache License v2.0](https://www.apache.org/licenses/LICENSE-2.0)
 
-setup(**setup_kwargs)
```

