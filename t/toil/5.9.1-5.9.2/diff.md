# Comparing `tmp/toil-5.9.1.tar.gz` & `tmp/toil-5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toil-5.9.1.tar", last modified: Sat Feb  4 03:38:31 2023, max compression
+gzip compressed data, was "toil-5.9.2.tar", last modified: Sat Feb  4 04:55:25 2023, max compression
```

## Comparing `toil-5.9.1.tar` & `toil-5.9.2.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.907590 toil-5.9.1/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    11516 2023-02-04 03:35:58.000000 toil-5.9.1/LICENSE
--rw-rw-r--   0 quokka    (1000) quokka    (1000)       26 2023-02-04 03:35:58.000000 toil-5.9.1/MANIFEST.in
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1670 2023-02-04 03:38:31.907590 toil-5.9.1/PKG-INFO
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1348 2023-02-04 03:35:58.000000 toil-5.9.1/README.rst
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      162 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-aws.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      176 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-cwl.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      372 2023-02-04 03:36:07.000000 toil-5.9.1/requirements-dev.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)       17 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-encryption.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)       58 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-google.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)       27 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-htcondor.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      328 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-kubernetes.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)       21 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-mesos.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      169 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-server.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)       16 2023-02-04 03:35:58.000000 toil-5.9.1/requirements-wdl.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      196 2023-02-04 03:35:58.000000 toil-5.9.1/requirements.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1091 2023-02-04 03:38:31.911590 toil-5.9.1/setup.cfg
--rwxrwxr-x   0 quokka    (1000) quokka    (1000)     6593 2023-02-04 03:35:58.000000 toil-5.9.1/setup.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.883590 toil-5.9.1/src/
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.891590 toil-5.9.1/src/toil/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    30914 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/__init__.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.895590 toil-5.9.1/src/toil/batchSystems/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1035 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    24725 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/abstractBatchSystem.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    19630 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/abstractGridEngineBatchSystem.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    25379 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/awsBatch.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     3738 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/cleanup_support.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     5165 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/contained_executor.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     7685 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/gridengine.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    13690 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/htcondor.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    76468 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/kubernetes.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     3826 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/local_support.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    16993 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/lsf.py
--rwxrwxr-x   0 quokka    (1000) quokka    (1000)     7205 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/lsfHelper.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.895590 toil-5.9.1/src/toil/batchSystems/mesos/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     3354 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/mesos/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    37842 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/mesos/batchSystem.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      836 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/mesos/conftest.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    12376 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/mesos/executor.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.895590 toil-5.9.1/src/toil/batchSystems/mesos/test/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     4690 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/mesos/test/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     8885 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/options.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    17504 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/parasol.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     4532 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/registry.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    42967 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/singleMachine.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    17608 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/slurm.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    19945 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/tes.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    11599 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/batchSystems/torque.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    28009 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/bus.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    92439 2023-02-04 03:36:07.000000 toil-5.9.1/src/toil/common.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.895590 toil-5.9.1/src/toil/cwl/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2190 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/cwl/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      848 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/cwl/conftest.py
--rwxrwxr-x   0 quokka    (1000) quokka    (1000)   151473 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/cwl/cwltoil.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     6366 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/cwl/utils.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    13740 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/deferred.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.895590 toil-5.9.1/src/toil/fileStores/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2376 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/fileStores/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    26660 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/fileStores/abstractFileStore.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    88712 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/fileStores/cachingFileStore.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    12443 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/fileStores/nonCachingFileStore.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)   139947 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/job.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.895590 toil-5.9.1/src/toil/jobStores/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/jobStores/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    73331 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/jobStores/abstractJobStore.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.899590 toil-5.9.1/src/toil/jobStores/aws/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/jobStores/aws/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    77468 2023-02-04 03:36:07.000000 toil-5.9.1/src/toil/jobStores/aws/jobStore.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    19342 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/jobStores/aws/utils.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      834 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/jobStores/conftest.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    43482 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/jobStores/fileJobStore.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    22417 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/jobStores/googleJobStore.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    15224 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/jobStores/utils.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    76977 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/leader.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.899590 toil-5.9.1/src/toil/lib/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     3780 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/accelerators.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.903590 toil-5.9.1/src/toil/lib/aws/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     6537 2023-02-04 03:36:07.000000 toil-5.9.1/src/toil/lib/aws/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     4679 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/aws/ami.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    11841 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/aws/iam.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     7987 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/aws/session.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    18892 2023-02-04 03:36:07.000000 toil-5.9.1/src/toil/lib/aws/utils.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2328 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/bioio.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1540 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/compatibility.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     4093 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/conversions.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    19580 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/docker.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    22000 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/ec2.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    13204 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/ec2nodes.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.903590 toil-5.9.1/src/toil/lib/encryption/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      705 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/encryption/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1070 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/encryption/_dummy.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     3769 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/encryption/_nacl.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      226 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/encryption/conftest.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2271 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/exceptions.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2925 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/expando.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)   138076 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/generatedEC2Lists.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1239 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/humanize.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     7464 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/io.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     3429 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/iterables.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     3223 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/memoize.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     5238 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/misc.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     5384 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/objects.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2183 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/resources.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    22399 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/retry.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    21002 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/threading.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     4977 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/lib/throttle.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.903590 toil-5.9.1/src/toil/provisioners/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     9067 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/provisioners/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    55376 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/provisioners/abstractProvisioner.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.903590 toil-5.9.1/src/toil/provisioners/aws/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     8623 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/provisioners/aws/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    80914 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/provisioners/aws/awsProvisioner.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    62079 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/provisioners/clusterScaler.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    23550 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/provisioners/gceProvisioner.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    13777 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/provisioners/node.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     9723 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/realtimeLogger.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    23314 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/resource.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.903590 toil-5.9.1/src/toil/server/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/__init__.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.903590 toil-5.9.1/src/toil/server/api_spec/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/api_spec/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    25377 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/api_spec/workflow_execution_service.swagger.yaml
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     7176 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/app.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      649 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/celery_app.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.903590 toil-5.9.1/src/toil/server/cli/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/cli/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    18372 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/cli/wes_cwl_runner.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    21832 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/utils.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.903590 toil-5.9.1/src/toil/server/wes/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/wes/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     9717 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/wes/abstract_backend.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    10380 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/wes/amazon_wes_utils.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    24420 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/wes/tasks.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    27850 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/wes/toil_backend.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1936 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/server/wsgi_app.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    18446 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/serviceManager.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    13056 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/statsAndLogging.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.907590 toil-5.9.1/src/toil/test/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    44074 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/test/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    14607 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/toilState.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.907590 toil-5.9.1/src/toil/utils/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1500 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilClean.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     5468 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilDebugFile.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2173 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilDebugJob.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1401 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilDestroyCluster.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2698 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilKill.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    12188 2023-02-04 03:36:07.000000 toil-5.9.1/src/toil/utils/toilLaunchCluster.py
--rwxrwxr-x   0 quokka    (1000) quokka    (1000)     2394 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilMain.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2032 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilRsyncCluster.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1178 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilServer.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     2653 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilSshCluster.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    23311 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilStats.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    16408 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilStatus.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1273 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/utils/toilUpdateEC2Instances.py
--rw-------   0 quokka    (1000) quokka    (1000)      419 2023-02-04 03:36:45.000000 toil-5.9.1/src/toil/version.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.907590 toil-5.9.1/src/toil/wdl/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     6213 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/toilwdl.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     5724 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/utils.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.907590 toil-5.9.1/src/toil/wdl/versions/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/versions/__init__.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     4098 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/versions/dev.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    39731 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/versions/draft2.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    27957 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/versions/v1.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     3762 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/wdl_analysis.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    35267 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/wdl_functions.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    45505 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/wdl_synthesis.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     6503 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/wdl/wdl_types.py
--rw-rw-r--   0 quokka    (1000) quokka    (1000)    31731 2023-02-04 03:35:58.000000 toil-5.9.1/src/toil/worker.py
-drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 03:38:31.891590 toil-5.9.1/src/toil.egg-info/
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1670 2023-02-04 03:38:31.000000 toil-5.9.1/src/toil.egg-info/PKG-INFO
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     4552 2023-02-04 03:38:31.000000 toil-5.9.1/src/toil.egg-info/SOURCES.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        1 2023-02-04 03:38:31.000000 toil-5.9.1/src/toil.egg-info/dependency_links.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)      430 2023-02-04 03:38:31.000000 toil-5.9.1/src/toil.egg-info/entry_points.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)     1739 2023-02-04 03:38:31.000000 toil-5.9.1/src/toil.egg-info/requires.txt
--rw-rw-r--   0 quokka    (1000) quokka    (1000)        5 2023-02-04 03:38:31.000000 toil-5.9.1/src/toil.egg-info/top_level.txt
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.688779 toil-5.9.2/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    11516 2023-02-04 04:49:49.000000 toil-5.9.2/LICENSE
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)       26 2023-02-04 04:49:49.000000 toil-5.9.2/MANIFEST.in
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1670 2023-02-04 04:55:25.688779 toil-5.9.2/PKG-INFO
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1348 2023-02-04 04:49:49.000000 toil-5.9.2/README.rst
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      162 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-aws.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      176 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-cwl.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      372 2023-02-04 04:49:57.000000 toil-5.9.2/requirements-dev.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)       17 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-encryption.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)       58 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-google.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)       27 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-htcondor.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      328 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-kubernetes.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)       21 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-mesos.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      169 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-server.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)       16 2023-02-04 04:49:49.000000 toil-5.9.2/requirements-wdl.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      196 2023-02-04 04:49:49.000000 toil-5.9.2/requirements.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1091 2023-02-04 04:55:25.688779 toil-5.9.2/setup.cfg
+-rwxrwxr-x   0 quokka    (1000) quokka    (1000)     6593 2023-02-04 04:49:49.000000 toil-5.9.2/setup.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.660779 toil-5.9.2/src/
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.668779 toil-5.9.2/src/toil/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    30914 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/__init__.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.672779 toil-5.9.2/src/toil/batchSystems/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1035 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    24725 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/abstractBatchSystem.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    19630 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/abstractGridEngineBatchSystem.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    25379 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/awsBatch.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     3738 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/cleanup_support.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     5165 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/contained_executor.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     7685 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/gridengine.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    13690 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/htcondor.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    76468 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/kubernetes.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     3826 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/local_support.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    16993 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/lsf.py
+-rwxrwxr-x   0 quokka    (1000) quokka    (1000)     7205 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/lsfHelper.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.672779 toil-5.9.2/src/toil/batchSystems/mesos/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     3354 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/mesos/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    37842 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/mesos/batchSystem.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      836 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/mesos/conftest.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    12376 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/mesos/executor.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.672779 toil-5.9.2/src/toil/batchSystems/mesos/test/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     4690 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/mesos/test/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     8885 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/options.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    17504 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/parasol.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     4532 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/registry.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    42967 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/singleMachine.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    17608 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/slurm.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    19945 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/tes.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    11599 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/batchSystems/torque.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    28009 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/bus.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    92512 2023-02-04 04:49:57.000000 toil-5.9.2/src/toil/common.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.672779 toil-5.9.2/src/toil/cwl/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2190 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/cwl/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      848 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/cwl/conftest.py
+-rwxrwxr-x   0 quokka    (1000) quokka    (1000)   151473 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/cwl/cwltoil.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     6366 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/cwl/utils.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    13740 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/deferred.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.676779 toil-5.9.2/src/toil/fileStores/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2376 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/fileStores/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    26660 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/fileStores/abstractFileStore.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    88712 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/fileStores/cachingFileStore.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    12443 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/fileStores/nonCachingFileStore.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)   139947 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/job.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.676779 toil-5.9.2/src/toil/jobStores/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/jobStores/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    73331 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/jobStores/abstractJobStore.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.676779 toil-5.9.2/src/toil/jobStores/aws/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/jobStores/aws/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    77460 2023-02-04 04:49:57.000000 toil-5.9.2/src/toil/jobStores/aws/jobStore.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    19342 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/jobStores/aws/utils.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      834 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/jobStores/conftest.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    43482 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/jobStores/fileJobStore.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    22417 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/jobStores/googleJobStore.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    15224 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/jobStores/utils.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    76977 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/leader.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.680779 toil-5.9.2/src/toil/lib/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     3780 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/accelerators.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.680779 toil-5.9.2/src/toil/lib/aws/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     7338 2023-02-04 04:49:57.000000 toil-5.9.2/src/toil/lib/aws/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     4679 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/aws/ami.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    11841 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/aws/iam.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     7987 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/aws/session.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    18106 2023-02-04 04:49:57.000000 toil-5.9.2/src/toil/lib/aws/utils.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2328 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/bioio.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1540 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/compatibility.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     4093 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/conversions.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    19580 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/docker.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    22000 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/ec2.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    13204 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/ec2nodes.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.680779 toil-5.9.2/src/toil/lib/encryption/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      705 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/encryption/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1070 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/encryption/_dummy.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     3769 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/encryption/_nacl.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      226 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/encryption/conftest.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2271 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/exceptions.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2925 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/expando.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)   138076 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/generatedEC2Lists.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1239 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/humanize.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     7464 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/io.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     3429 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/iterables.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     3223 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/memoize.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     5238 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/misc.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     5384 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/objects.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2183 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/resources.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    22399 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/retry.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    21002 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/threading.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     4977 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/lib/throttle.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.680779 toil-5.9.2/src/toil/provisioners/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     9067 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/provisioners/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    55376 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/provisioners/abstractProvisioner.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.680779 toil-5.9.2/src/toil/provisioners/aws/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     8623 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/provisioners/aws/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    80914 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/provisioners/aws/awsProvisioner.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    62079 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/provisioners/clusterScaler.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    23550 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/provisioners/gceProvisioner.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    13777 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/provisioners/node.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     9723 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/realtimeLogger.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    23314 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/resource.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.680779 toil-5.9.2/src/toil/server/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/__init__.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.684779 toil-5.9.2/src/toil/server/api_spec/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/api_spec/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    25377 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/api_spec/workflow_execution_service.swagger.yaml
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     7176 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/app.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      649 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/celery_app.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.684779 toil-5.9.2/src/toil/server/cli/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/cli/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    18372 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/cli/wes_cwl_runner.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    21832 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/utils.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.684779 toil-5.9.2/src/toil/server/wes/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/wes/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     9717 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/wes/abstract_backend.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    10380 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/wes/amazon_wes_utils.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    24420 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/wes/tasks.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    27850 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/wes/toil_backend.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1936 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/server/wsgi_app.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    18446 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/serviceManager.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    13056 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/statsAndLogging.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.684779 toil-5.9.2/src/toil/test/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    44074 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/test/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    14607 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/toilState.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.684779 toil-5.9.2/src/toil/utils/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1500 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilClean.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     5468 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilDebugFile.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2173 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilDebugJob.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1401 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilDestroyCluster.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2698 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilKill.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    12182 2023-02-04 04:49:57.000000 toil-5.9.2/src/toil/utils/toilLaunchCluster.py
+-rwxrwxr-x   0 quokka    (1000) quokka    (1000)     2394 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilMain.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2032 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilRsyncCluster.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1178 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilServer.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     2653 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilSshCluster.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    23311 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilStats.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    16408 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilStatus.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1273 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/utils/toilUpdateEC2Instances.py
+-rw-------   0 quokka    (1000) quokka    (1000)      419 2023-02-04 04:52:28.000000 toil-5.9.2/src/toil/version.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.688779 toil-5.9.2/src/toil/wdl/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     6213 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/toilwdl.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     5724 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/utils.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.688779 toil-5.9.2/src/toil/wdl/versions/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/versions/__init__.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     4098 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/versions/dev.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    39731 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/versions/draft2.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    27957 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/versions/v1.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     3762 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/wdl_analysis.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    35267 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/wdl_functions.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    45505 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/wdl_synthesis.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     6503 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/wdl/wdl_types.py
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)    31731 2023-02-04 04:49:49.000000 toil-5.9.2/src/toil/worker.py
+drwxrwxr-x   0 quokka    (1000) quokka    (1000)        0 2023-02-04 04:55:25.668779 toil-5.9.2/src/toil.egg-info/
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1670 2023-02-04 04:55:25.000000 toil-5.9.2/src/toil.egg-info/PKG-INFO
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     4552 2023-02-04 04:55:25.000000 toil-5.9.2/src/toil.egg-info/SOURCES.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        1 2023-02-04 04:55:25.000000 toil-5.9.2/src/toil.egg-info/dependency_links.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)      430 2023-02-04 04:55:25.000000 toil-5.9.2/src/toil.egg-info/entry_points.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)     1739 2023-02-04 04:55:25.000000 toil-5.9.2/src/toil.egg-info/requires.txt
+-rw-rw-r--   0 quokka    (1000) quokka    (1000)        5 2023-02-04 04:55:25.000000 toil-5.9.2/src/toil.egg-info/top_level.txt
```

### Comparing `toil-5.9.1/LICENSE` & `toil-5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/PKG-INFO` & `toil-5.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toil
-Version: 5.9.1
+Version: 5.9.2
 Summary: Pipeline management software for clusters.
 Home-page: https://github.com/DataBiosphere/toil
 Author: Benedict Paten and the Toil community
 Author-email: toil-community@googlegroups.com
 License: Apache License v2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `toil-5.9.1/README.rst` & `toil-5.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/setup.cfg` & `toil-5.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/setup.py` & `toil-5.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/__init__.py` & `toil-5.9.2/src/toil/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/__init__.py` & `toil-5.9.2/src/toil/batchSystems/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/abstractBatchSystem.py` & `toil-5.9.2/src/toil/batchSystems/abstractBatchSystem.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/abstractGridEngineBatchSystem.py` & `toil-5.9.2/src/toil/batchSystems/abstractGridEngineBatchSystem.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/awsBatch.py` & `toil-5.9.2/src/toil/batchSystems/awsBatch.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/cleanup_support.py` & `toil-5.9.2/src/toil/batchSystems/cleanup_support.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/contained_executor.py` & `toil-5.9.2/src/toil/batchSystems/contained_executor.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/gridengine.py` & `toil-5.9.2/src/toil/batchSystems/gridengine.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/htcondor.py` & `toil-5.9.2/src/toil/batchSystems/htcondor.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/kubernetes.py` & `toil-5.9.2/src/toil/batchSystems/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/local_support.py` & `toil-5.9.2/src/toil/batchSystems/local_support.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/lsf.py` & `toil-5.9.2/src/toil/batchSystems/lsf.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/lsfHelper.py` & `toil-5.9.2/src/toil/batchSystems/lsfHelper.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/mesos/__init__.py` & `toil-5.9.2/src/toil/batchSystems/mesos/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/mesos/batchSystem.py` & `toil-5.9.2/src/toil/batchSystems/mesos/batchSystem.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/mesos/conftest.py` & `toil-5.9.2/src/toil/batchSystems/mesos/conftest.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/mesos/executor.py` & `toil-5.9.2/src/toil/batchSystems/mesos/executor.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/mesos/test/__init__.py` & `toil-5.9.2/src/toil/batchSystems/mesos/test/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/options.py` & `toil-5.9.2/src/toil/batchSystems/options.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/parasol.py` & `toil-5.9.2/src/toil/batchSystems/parasol.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/registry.py` & `toil-5.9.2/src/toil/batchSystems/registry.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/singleMachine.py` & `toil-5.9.2/src/toil/batchSystems/singleMachine.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/slurm.py` & `toil-5.9.2/src/toil/batchSystems/slurm.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/tes.py` & `toil-5.9.2/src/toil/batchSystems/tes.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/batchSystems/torque.py` & `toil-5.9.2/src/toil/batchSystems/torque.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/bus.py` & `toil-5.9.2/src/toil/bus.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/common.py` & `toil-5.9.2/src/toil/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import json
 import logging
 import os
 import pickle
 import re
 import signal
 import subprocess
 import sys
@@ -32,14 +33,15 @@
 from typing import (IO,
                     TYPE_CHECKING,
                     Any,
                     Callable,
                     ContextManager,
                     Dict,
                     List,
+                    MutableMapping,
                     Optional,
                     Set,
                     Tuple,
                     Type,
                     TypeVar,
                     Union,
                     cast,
@@ -63,15 +65,15 @@
                       JobFailedMessage,
                       JobIssuedMessage,
                       JobMissingMessage,
                       MessageBus,
                       QueueSizeMessage,
                       gen_message_bus_path)
 from toil.fileStores import FileID
-from toil.lib.aws import zone_to_region
+from toil.lib.aws import zone_to_region, build_tag_dict_from_env
 from toil.lib.compatibility import deprecated
 from toil.lib.conversions import bytes2human, human2bytes
 from toil.lib.io import try_path
 from toil.lib.retry import retry
 from toil.provisioners import (add_provisioner_options,
                                cluster_factory,
                                parse_node_types)
```

### Comparing `toil-5.9.1/src/toil/cwl/__init__.py` & `toil-5.9.2/src/toil/cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/cwl/conftest.py` & `toil-5.9.2/src/toil/cwl/conftest.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/cwl/cwltoil.py` & `toil-5.9.2/src/toil/cwl/cwltoil.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/cwl/utils.py` & `toil-5.9.2/src/toil/cwl/utils.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/deferred.py` & `toil-5.9.2/src/toil/deferred.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/fileStores/__init__.py` & `toil-5.9.2/src/toil/fileStores/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/fileStores/abstractFileStore.py` & `toil-5.9.2/src/toil/fileStores/abstractFileStore.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/fileStores/cachingFileStore.py` & `toil-5.9.2/src/toil/fileStores/cachingFileStore.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/fileStores/nonCachingFileStore.py` & `toil-5.9.2/src/toil/fileStores/nonCachingFileStore.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/job.py` & `toil-5.9.2/src/toil/job.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/jobStores/abstractJobStore.py` & `toil-5.9.2/src/toil/jobStores/abstractJobStore.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/jobStores/aws/jobStore.py` & `toil-5.9.2/src/toil/jobStores/aws/jobStore.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 import boto.s3.connection
 import boto.sdb
 from boto.exception import SDBResponseError
 from botocore.exceptions import ClientError
 
 import toil.lib.encryption as encryption
+from toil.lib.aws import build_tag_dict_from_env
 from toil.fileStores import FileID
 from toil.jobStores.abstractJobStore import (AbstractJobStore,
                                              ConcurrentFileModificationException,
                                              JobStoreExistsException,
                                              NoSuchFileException,
                                              NoSuchJobException,
                                              NoSuchJobStoreException)
@@ -52,16 +53,15 @@
                                       sdb_unavailable,
                                       uploadFile,
                                       uploadFromPath)
 from toil.jobStores.utils import (ReadablePipe,
                                   ReadableTransformingPipe,
                                   WritablePipe)
 from toil.lib.aws.session import establish_boto3_session
-from toil.lib.aws.utils import (build_tag_dict_from_env,
-                                create_s3_bucket,
+from toil.lib.aws.utils import (create_s3_bucket,
                                 flatten_tags,
                                 get_bucket_region,
                                 get_object_for_url,
                                 list_objects_for_url,
                                 retry_s3,
                                 retryable_s3_errors)
 from toil.lib.compatibility import compat_bytes
```

### Comparing `toil-5.9.1/src/toil/jobStores/aws/utils.py` & `toil-5.9.2/src/toil/jobStores/aws/utils.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/jobStores/conftest.py` & `toil-5.9.2/src/toil/jobStores/conftest.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/jobStores/fileJobStore.py` & `toil-5.9.2/src/toil/jobStores/fileJobStore.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/jobStores/googleJobStore.py` & `toil-5.9.2/src/toil/jobStores/googleJobStore.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/jobStores/utils.py` & `toil-5.9.2/src/toil/jobStores/utils.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/leader.py` & `toil-5.9.2/src/toil/leader.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/accelerators.py` & `toil-5.9.2/src/toil/lib/accelerators.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/aws/__init__.py` & `toil-5.9.2/src/toil/lib/aws/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import threading
 from functools import lru_cache
 from typing import (Any,
                     Callable,
                     Dict,
                     Iterable,
                     List,
+                    MutableMapping,
                     Optional,
                     TypeVar,
                     Union)
 from urllib.error import URLError
 from urllib.request import urlopen
 
 logger = logging.getLogger(__name__)
@@ -168,7 +169,27 @@
 
 def running_on_ecs() -> bool:
     """
     Return True if we are currently running on Amazon ECS, and false otherwise.
     """
     # We only care about relatively current ECS
     return 'ECS_CONTAINER_METADATA_URI_V4' in os.environ
+
+def build_tag_dict_from_env(environment: MutableMapping[str, str] = os.environ) -> Dict[str, str]:
+    tags = dict()
+    owner_tag = environment.get('TOIL_OWNER_TAG')
+    if owner_tag:
+        tags.update({'Owner': owner_tag})
+
+    user_tags = environment.get('TOIL_AWS_TAGS')
+    if user_tags:
+        try:
+            json_user_tags = json.loads(user_tags)
+            if isinstance(json_user_tags, dict):
+                tags.update(json.loads(user_tags))
+            else:
+                logger.error('TOIL_AWS_TAGS must be in JSON format: {"key" : "value", ...}')
+                exit(1)
+        except json.decoder.JSONDecodeError:
+            logger.error('TOIL_AWS_TAGS must be in JSON format: {"key" : "value", ...}')
+            exit(1)
+    return tags
```

### Comparing `toil-5.9.1/src/toil/lib/aws/ami.py` & `toil-5.9.2/src/toil/lib/aws/ami.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/aws/iam.py` & `toil-5.9.2/src/toil/lib/aws/iam.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/aws/session.py` & `toil-5.9.2/src/toil/lib/aws/session.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/aws/utils.py` & `toil-5.9.2/src/toil/lib/aws/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,31 +24,30 @@
                     Hashable,
                     Iterable,
                     Iterator,
                     List,
                     Optional,
                     Set,
                     Union,
-                    cast)
+                    cast,
+                    MutableMapping)
 from urllib.parse import ParseResult
 
 from toil.lib.aws import session
 from toil.lib.misc import printq
 from toil.lib.retry import (DEFAULT_DELAYS,
                             DEFAULT_TIMEOUT,
                             get_error_code,
                             get_error_status,
                             old_retry,
                             retry)
 
 if sys.version_info >= (3, 8):
-    from typing import Literal, MutableMapping
+    from typing import Literal
 else:
-    from typing import MutableMapping
-
     from typing_extensions import Literal
 
 try:
     from boto.exception import BotoServerError, S3ResponseError
     from botocore.exceptions import ClientError
     from mypy_boto3_iam import IAMClient, IAMServiceResource
     from mypy_boto3_s3 import S3Client, S3ServiceResource
@@ -399,34 +398,12 @@
                         # Ignore folder name itself
                         continue
                     listing.append(content_item['Key'][len(key_name):])
 
         logger.debug('Found in %s items: %s', url, listing)
         return listing
 
-
-def build_tag_dict_from_env(environment: MutableMapping[str, str] = os.environ) -> Dict[str, str]:
-    tags = dict()
-    owner_tag = environment.get('TOIL_OWNER_TAG')
-    if owner_tag:
-        tags.update({'Owner': owner_tag})
-
-    user_tags = environment.get('TOIL_AWS_TAGS')
-    if user_tags:
-        try:
-            json_user_tags = json.loads(user_tags)
-            if isinstance(json_user_tags, dict):
-                tags.update(json.loads(user_tags))
-            else:
-                logger.error('TOIL_AWS_TAGS must be in JSON format: {"key" : "value", ...}')
-                exit(1)
-        except json.decoder.JSONDecodeError:
-            logger.error('TOIL_AWS_TAGS must be in JSON format: {"key" : "value", ...}')
-            exit(1)
-    return tags
-
-
 def flatten_tags(tags: Dict[str, str]) -> List[Dict[str, str]]:
     """
     Convert tags from a key to value dict into a list of 'Key': xxx, 'Value': xxx dicts.
     """
     return [{'Key': k, 'Value': v} for k, v in tags.items()]
```

### Comparing `toil-5.9.1/src/toil/lib/bioio.py` & `toil-5.9.2/src/toil/lib/bioio.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/compatibility.py` & `toil-5.9.2/src/toil/lib/compatibility.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/conversions.py` & `toil-5.9.2/src/toil/lib/conversions.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/docker.py` & `toil-5.9.2/src/toil/lib/docker.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/ec2.py` & `toil-5.9.2/src/toil/lib/ec2.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/ec2nodes.py` & `toil-5.9.2/src/toil/lib/ec2nodes.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/encryption/__init__.py` & `toil-5.9.2/src/toil/lib/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/encryption/_dummy.py` & `toil-5.9.2/src/toil/lib/encryption/_dummy.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/encryption/_nacl.py` & `toil-5.9.2/src/toil/lib/encryption/_nacl.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/exceptions.py` & `toil-5.9.2/src/toil/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/expando.py` & `toil-5.9.2/src/toil/lib/expando.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/generatedEC2Lists.py` & `toil-5.9.2/src/toil/lib/generatedEC2Lists.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/humanize.py` & `toil-5.9.2/src/toil/lib/humanize.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/io.py` & `toil-5.9.2/src/toil/lib/io.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/iterables.py` & `toil-5.9.2/src/toil/lib/iterables.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/memoize.py` & `toil-5.9.2/src/toil/lib/memoize.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/misc.py` & `toil-5.9.2/src/toil/lib/misc.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/objects.py` & `toil-5.9.2/src/toil/lib/objects.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/resources.py` & `toil-5.9.2/src/toil/lib/resources.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/retry.py` & `toil-5.9.2/src/toil/lib/retry.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/threading.py` & `toil-5.9.2/src/toil/lib/threading.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/lib/throttle.py` & `toil-5.9.2/src/toil/lib/throttle.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/provisioners/__init__.py` & `toil-5.9.2/src/toil/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/provisioners/abstractProvisioner.py` & `toil-5.9.2/src/toil/provisioners/abstractProvisioner.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/provisioners/aws/__init__.py` & `toil-5.9.2/src/toil/provisioners/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/provisioners/aws/awsProvisioner.py` & `toil-5.9.2/src/toil/provisioners/aws/awsProvisioner.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/provisioners/clusterScaler.py` & `toil-5.9.2/src/toil/provisioners/clusterScaler.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/provisioners/gceProvisioner.py` & `toil-5.9.2/src/toil/provisioners/gceProvisioner.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/provisioners/node.py` & `toil-5.9.2/src/toil/provisioners/node.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/realtimeLogger.py` & `toil-5.9.2/src/toil/realtimeLogger.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/resource.py` & `toil-5.9.2/src/toil/resource.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/api_spec/workflow_execution_service.swagger.yaml` & `toil-5.9.2/src/toil/server/api_spec/workflow_execution_service.swagger.yaml`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/app.py` & `toil-5.9.2/src/toil/server/app.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/celery_app.py` & `toil-5.9.2/src/toil/server/celery_app.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/cli/wes_cwl_runner.py` & `toil-5.9.2/src/toil/server/cli/wes_cwl_runner.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/utils.py` & `toil-5.9.2/src/toil/server/utils.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/wes/abstract_backend.py` & `toil-5.9.2/src/toil/server/wes/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/wes/amazon_wes_utils.py` & `toil-5.9.2/src/toil/server/wes/amazon_wes_utils.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/wes/tasks.py` & `toil-5.9.2/src/toil/server/wes/tasks.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/wes/toil_backend.py` & `toil-5.9.2/src/toil/server/wes/toil_backend.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/server/wsgi_app.py` & `toil-5.9.2/src/toil/server/wsgi_app.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/serviceManager.py` & `toil-5.9.2/src/toil/serviceManager.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/statsAndLogging.py` & `toil-5.9.2/src/toil/statsAndLogging.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/test/__init__.py` & `toil-5.9.2/src/toil/test/__init__.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/toilState.py` & `toil-5.9.2/src/toil/toilState.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilClean.py` & `toil-5.9.2/src/toil/utils/toilClean.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilDebugFile.py` & `toil-5.9.2/src/toil/utils/toilDebugFile.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilDebugJob.py` & `toil-5.9.2/src/toil/utils/toilDebugJob.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilDestroyCluster.py` & `toil-5.9.2/src/toil/utils/toilDestroyCluster.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilKill.py` & `toil-5.9.2/src/toil/utils/toilKill.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilLaunchCluster.py` & `toil-5.9.2/src/toil/utils/toilLaunchCluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import logging
 import os
 from typing import Dict, List, Tuple, Union
 
 from toil import applianceSelf
 from toil.common import parser_with_common_options
-from toil.lib.aws.utils import build_tag_dict_from_env
+from toil.lib.aws import build_tag_dict_from_env
 from toil.provisioners import (check_valid_node_types,
                                cluster_factory,
                                parse_node_types)
 from toil.statsAndLogging import set_logging_from_options
 
 logger = logging.getLogger(__name__)
```

### Comparing `toil-5.9.1/src/toil/utils/toilMain.py` & `toil-5.9.2/src/toil/utils/toilMain.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilRsyncCluster.py` & `toil-5.9.2/src/toil/utils/toilRsyncCluster.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilServer.py` & `toil-5.9.2/src/toil/utils/toilServer.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilSshCluster.py` & `toil-5.9.2/src/toil/utils/toilSshCluster.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilStats.py` & `toil-5.9.2/src/toil/utils/toilStats.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilStatus.py` & `toil-5.9.2/src/toil/utils/toilStatus.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/utils/toilUpdateEC2Instances.py` & `toil-5.9.2/src/toil/utils/toilUpdateEC2Instances.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/toilwdl.py` & `toil-5.9.2/src/toil/wdl/toilwdl.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/utils.py` & `toil-5.9.2/src/toil/wdl/utils.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/versions/dev.py` & `toil-5.9.2/src/toil/wdl/versions/dev.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/versions/draft2.py` & `toil-5.9.2/src/toil/wdl/versions/draft2.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/versions/v1.py` & `toil-5.9.2/src/toil/wdl/versions/v1.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/wdl_analysis.py` & `toil-5.9.2/src/toil/wdl/wdl_analysis.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/wdl_functions.py` & `toil-5.9.2/src/toil/wdl/wdl_functions.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/wdl_synthesis.py` & `toil-5.9.2/src/toil/wdl/wdl_synthesis.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/wdl/wdl_types.py` & `toil-5.9.2/src/toil/wdl/wdl_types.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil/worker.py` & `toil-5.9.2/src/toil/worker.py`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil.egg-info/PKG-INFO` & `toil-5.9.2/src/toil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toil
-Version: 5.9.1
+Version: 5.9.2
 Summary: Pipeline management software for clusters.
 Home-page: https://github.com/DataBiosphere/toil
 Author: Benedict Paten and the Toil community
 Author-email: toil-community@googlegroups.com
 License: Apache License v2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `toil-5.9.1/src/toil.egg-info/SOURCES.txt` & `toil-5.9.2/src/toil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toil-5.9.1/src/toil.egg-info/requires.txt` & `toil-5.9.2/src/toil.egg-info/requires.txt`

 * *Files identical despite different names*

