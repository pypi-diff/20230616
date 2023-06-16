# Comparing `tmp/sentinel_protobuf-0.2.0.tar.gz` & `tmp/sentinel_protobuf-0.2.1.tar.gz`

## Comparing `sentinel_protobuf-0.2.0.tar` & `sentinel_protobuf-0.2.1.tar`

### file list

```diff
@@ -1,576 +1,497 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/.pydevproject
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/requirements.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/.settings/org.eclipse.core.resources.prefs
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/.gitignore
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/auth.proto
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/auth_pb2.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/auth_pb2.pyi
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis.proto
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/query.proto
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/authz.proto
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/event.proto
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis.proto
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/query.proto
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/tx.proto
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/authz.proto
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/bank.proto
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/bank_pb2.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/bank_pb2.pyi
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis.proto
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/query.proto
--rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    15085 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/tx.proto
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci.proto
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci_pb2.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci_pb2.pyi
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv.proto
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv_pb2.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv_pb2.pyi
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination.proto
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination_pb2.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination_pb2.pyi
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection.proto
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection_pb2.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection.proto
--rw-r--r--   0        0        0    10387 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection_pb2.py
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot.proto
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info.proto
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info_pb2.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info_pb2.pyi
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening.proto
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening_pb2.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening_pb2.pyi
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query.proto
--rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    12460 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/v1beta1/coin.proto
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/v1beta1/coin_pb2.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/v1beta1/coin_pb2.pyi
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/capability.proto
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/capability_pb2.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/capability_pb2.pyi
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis.proto
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis.proto
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx.proto
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/ed25519/keys.proto
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/ed25519/keys_pb2.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/ed25519/keys_pb2.pyi
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/keys.proto
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/keys_pb2.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/keys_pb2.pyi
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig.proto
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys.proto
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys_pb2.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys_pb2.pyi
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys.proto
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys_pb2.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys_pb2.pyi
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution.proto
--rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution_pb2.py
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution_pb2.pyi
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis.proto
--rw-r--r--   0        0        0    13234 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/query.proto
--rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    18352 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx.proto
--rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence.proto
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence_pb2.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence_pb2.pyi
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis.proto
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/query.proto
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx.proto
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant.proto
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant_pb2.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis.proto
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query.proto
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx.proto
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis.proto
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis.proto
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/gov.proto
--rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/query.proto
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14598 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/tx.proto
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/ics23/v1
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis.proto
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/mint.proto
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/mint_pb2.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/mint_pb2.pyi
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/query.proto
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/params.proto
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/params_pb2.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/params_pb2.pyi
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/query.proto
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis.proto
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/query.proto
--rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6284 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing.proto
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing_pb2.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing_pb2.pyi
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx.proto
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/authz.proto
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis.proto
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0    13564 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/query.proto
--rw-r--r--   0        0        0    19200 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    11274 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    26968 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0    15834 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/staking.proto
--rw-r--r--   0        0        0    24776 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/staking_pb2.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/staking_pb2.pyi
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/tx.proto
--rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing.proto
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing_pb2.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing_pb2.pyi
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/service.proto
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2.pyi
--rw-r--r--   0        0        0     9577 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2_grpc.py
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/tx.proto
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query.proto
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade.proto
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade_pb2.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx.proto
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting.proto
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting_pb2.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting_pb2.pyi
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos_proto/cosmos.proto
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos_proto/cosmos_pb2.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos_proto/cosmos_pb2.pyi
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/gogoproto/gogo.proto
--rw-r--r--   0        0        0    14516 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/gogoproto/gogo_pb2.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/gogoproto/gogo_pb2.pyi
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/annotations.proto
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0    12099 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/http.proto
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/http_pb2.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/http_pb2.pyi
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/protobuf/any.proto
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/protobuf/any_pb2.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/protobuf/any_pb2.pyi
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller.proto
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller_pb2.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller_pb2.pyi
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query.proto
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2.pyi
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host.proto
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host_pb2.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host_pb2.pyi
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query.proto
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account.proto
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account_pb2.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account_pb2.pyi
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis.proto
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis_pb2.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata.proto
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata_pb2.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata_pb2.pyi
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet.proto
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet_pb2.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet_pb2.pyi
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis.proto
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/query.proto
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2.pyi
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer.proto
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer_pb2.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer_pb2.pyi
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/tx.proto
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/tx_pb2.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/tx_pb2.pyi
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v2/packet.proto
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v2/packet_pb2.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v2/packet_pb2.pyi
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/channel.proto
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/channel_pb2.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/channel_pb2.pyi
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/genesis.proto
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/genesis_pb2.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0    14315 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/query.proto
--rw-r--r--   0        0        0    18937 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2.py
--rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2.pyi
--rw-r--r--   0        0        0    25454 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/tx.proto
--rw-r--r--   0        0        0    20228 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/tx_pb2.py
--rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/client.proto
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/client_pb2.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/client_pb2.pyi
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/genesis.proto
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/genesis_pb2.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/query.proto
--rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/query_pb2.py
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/query_pb2.pyi
--rw-r--r--   0        0        0    15612 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/tx.proto
--rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/tx_pb2.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/commitment/v1/commitment.proto
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/connection/v1/connection.proto
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/connection/v1/genesis.proto
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/connection/v1/query.proto
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/connection/v1/tx.proto
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/types/v1/genesis.proto
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost.proto
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost_pb2.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost_pb2.pyi
--rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/solomachine/v1/solomachine.proto
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/solomachine/v2/solomachine.proto
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/tendermint/v1/tendermint.proto
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/consumer.proto
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/genesis.proto
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query.proto
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2.pyi
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/genesis.proto
--rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/provider.proto
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/query.proto
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx.proto
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx_pb2.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/ccv.proto
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/query.proto
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2.pyi
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/tx.proto
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/tx_pb2.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/tx_pb2.pyi
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/deposit.proto
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/deposit_pb2.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/deposit_pb2.pyi
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/events.proto
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/events_pb2.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/events_pb2.pyi
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/querier.proto
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/querier_pb2.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/querier_pb2.pyi
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/mint/v1/genesis.proto
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/mint/v1/genesis_pb2.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/mint/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/mint/v1/inflation.proto
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/mint/v1/inflation_pb2.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/mint/v1/inflation_pb2.pyi
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v1/node.proto
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v1/node_pb2.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v1/node_pb2.pyi
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/events.proto
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/events_pb2.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/events_pb2.pyi
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/genesis.proto
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/genesis_pb2.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/genesis_pb2.pyi
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/lease.proto
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/lease_pb2.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/lease_pb2.pyi
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/msg.proto
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/msg_pb2.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/msg_pb2.pyi
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/node.proto
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/node_pb2.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/node_pb2.pyi
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/params.proto
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/params_pb2.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/params_pb2.pyi
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/querier.proto
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/querier_pb2.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/querier_pb2.pyi
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v1/plan.proto
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v1/plan_pb2.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v1/plan_pb2.pyi
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/events.proto
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/events_pb2.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/events_pb2.pyi
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/genesis.proto
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/genesis_pb2.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/genesis_pb2.pyi
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/msg.proto
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/msg_pb2.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/msg_pb2.pyi
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/plan.proto
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/plan_pb2.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/plan_pb2.pyi
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/querier.proto
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/querier_pb2.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/querier_pb2.pyi
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v1/provider.proto
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v1/provider_pb2.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v1/provider_pb2.pyi
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/events.proto
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/events_pb2.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/events_pb2.pyi
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/genesis.proto
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/genesis_pb2.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/genesis_pb2.pyi
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/msg.proto
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/msg_pb2.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/msg_pb2.pyi
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/params.proto
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/params_pb2.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/params_pb2.pyi
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/provider.proto
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/provider_pb2.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/provider_pb2.pyi
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/querier.proto
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/querier_pb2.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/querier_pb2.pyi
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v1/session.proto
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v1/session_pb2.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v1/session_pb2.pyi
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/events.proto
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/events_pb2.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/events_pb2.pyi
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/genesis.proto
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/genesis_pb2.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/genesis_pb2.pyi
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/msg.proto
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/msg_pb2.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/msg_pb2.pyi
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/params.proto
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/params_pb2.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/params_pb2.pyi
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/proof.proto
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/proof_pb2.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/proof_pb2.pyi
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/querier.proto
--rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/querier_pb2.py
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/querier_pb2.pyi
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/session.proto
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/session_pb2.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/session_pb2.pyi
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v1/quota.proto
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v1/quota_pb2.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v1/quota_pb2.pyi
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v1/subscription.proto
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v1/subscription_pb2.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v1/subscription_pb2.pyi
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/events.proto
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/events_pb2.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/events_pb2.pyi
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/genesis.proto
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/genesis_pb2.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/genesis_pb2.pyi
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/msg.proto
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/msg_pb2.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/msg_pb2.pyi
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/params.proto
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/params_pb2.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/params_pb2.pyi
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/querier.proto
--rw-r--r--   0        0        0     9791 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/querier_pb2.py
--rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/querier_pb2.pyi
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/quota.proto
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/quota_pb2.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/quota_pb2.pyi
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/subscription.proto
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/subscription_pb2.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/subscription_pb2.pyi
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/events.proto
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/events_pb2.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/events_pb2.pyi
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/genesis.proto
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/genesis_pb2.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/msg.proto
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/msg_pb2.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/msg_pb2.pyi
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/params.proto
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/params_pb2.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/params_pb2.pyi
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/querier.proto
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/querier_pb2.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/querier_pb2.pyi
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/swap.proto
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/swap_pb2.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/swap_pb2.pyi
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/types/v1/bandwidth.proto
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/types/v1/bandwidth_pb2.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/types/v1/bandwidth_pb2.pyi
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/types/v1/status.proto
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/types/v1/status_pb2.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/types/v1/status_pb2.pyi
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/vpn/v1/genesis.proto
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/vpn/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/vpn/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0    12749 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/abci/types.proto
--rw-r--r--   0        0        0    21205 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/abci/types_pb2.py
--rw-r--r--   0        0        0    24568 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/abci/types_pb2.pyi
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/blockchain/types.proto
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/blockchain/types_pb2.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/blockchain/types_pb2.pyi
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/types.proto
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/types_pb2.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/types_pb2.pyi
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/wal.proto
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/wal_pb2.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/wal_pb2.pyi
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/keys.proto
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/keys_pb2.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/keys_pb2.pyi
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/proof.proto
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/proof_pb2.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/proof_pb2.pyi
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/libs/bits/types.proto
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/libs/bits/types_pb2.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/libs/bits/types_pb2.pyi
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/mempool/types.proto
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/mempool/types_pb2.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/mempool/types_pb2.pyi
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/conn.proto
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/conn_pb2.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/conn_pb2.pyi
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/pex.proto
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/pex_pb2.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/pex_pb2.pyi
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/types.proto
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/types_pb2.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/types_pb2.pyi
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/privval/types.proto
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/privval/types_pb2.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/privval/types_pb2.pyi
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/rpc/grpc/types.proto
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/rpc/grpc/types_pb2.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/rpc/grpc/types_pb2.pyi
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/state/types.proto
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/state/types_pb2.py
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/state/types_pb2.pyi
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/statesync/types.proto
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/statesync/types_pb2.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/statesync/types_pb2.pyi
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/store/types.proto
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/store/types_pb2.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/store/types_pb2.pyi
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/block.proto
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/block_pb2.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/block_pb2.pyi
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/canonical.proto
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/canonical_pb2.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/canonical_pb2.pyi
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/events.proto
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/events_pb2.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/events_pb2.pyi
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/evidence.proto
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/evidence_pb2.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/evidence_pb2.pyi
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/params.proto
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/params_pb2.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/params_pb2.pyi
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/types.proto
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/types_pb2.py
--rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/types_pb2.pyi
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/validator.proto
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/validator_pb2.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/validator_pb2.pyi
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/version/types.proto
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/version/types_pb2.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/version/types_pb2.pyi
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/README.md
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/.gitattributes
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/.project
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/aggregate.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/compile.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/requirements.txt
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/.github/workflows/tg-notify.yml
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/configs/cosmos.json
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/configs/osmosis.json
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/configs/sentinel.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/configs/sentinel2.json
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/configs/stargaze.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/examples/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/examples/query_bonded_tokens.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/.gitignore
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/auth.proto
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/auth_pb2.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/auth_pb2.pyi
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/query.proto
+-rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/authz.proto
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/event.proto
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/query.proto
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/tx.proto
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/authz.proto
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/bank.proto
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/bank_pb2.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/bank_pb2.pyi
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/query.proto
+-rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    15085 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/tx.proto
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci.proto
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci_pb2.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci_pb2.pyi
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv.proto
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv_pb2.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv_pb2.pyi
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination.proto
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination_pb2.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination_pb2.pyi
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection.proto
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection_pb2.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection.proto
+-rw-r--r--   0        0        0    10387 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection_pb2.py
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot.proto
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info.proto
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info_pb2.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info_pb2.pyi
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening.proto
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening_pb2.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening_pb2.pyi
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query.proto
+-rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    12460 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/v1beta1/coin.proto
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/v1beta1/coin_pb2.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/v1beta1/coin_pb2.pyi
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/capability.proto
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/capability_pb2.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/capability_pb2.pyi
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx.proto
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/ed25519/keys.proto
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/ed25519/keys_pb2.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/ed25519/keys_pb2.pyi
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/keys.proto
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/keys_pb2.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/keys_pb2.pyi
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig.proto
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys.proto
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys_pb2.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys_pb2.pyi
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys.proto
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys_pb2.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys_pb2.pyi
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution.proto
+-rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution_pb2.py
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution_pb2.pyi
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis.proto
+-rw-r--r--   0        0        0    13234 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/query.proto
+-rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    18352 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx.proto
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence.proto
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence_pb2.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence_pb2.pyi
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/query.proto
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx.proto
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant.proto
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant_pb2.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query.proto
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx.proto
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/gov.proto
+-rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/query.proto
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14598 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/tx.proto
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/ics23/v1
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/mint.proto
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/mint_pb2.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/mint_pb2.pyi
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/query.proto
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/params.proto
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/params_pb2.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/params_pb2.pyi
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/query.proto
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/query.proto
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6284 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing.proto
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing_pb2.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing_pb2.pyi
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx.proto
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/authz.proto
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis.proto
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0    13564 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/query.proto
+-rw-r--r--   0        0        0    19200 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    11274 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    26968 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    15834 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/staking.proto
+-rw-r--r--   0        0        0    24776 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/staking_pb2.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/staking_pb2.pyi
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/tx.proto
+-rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing.proto
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing_pb2.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing_pb2.pyi
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/service.proto
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2.pyi
+-rw-r--r--   0        0        0     9577 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2_grpc.py
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/tx.proto
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query.proto
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade.proto
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade_pb2.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx.proto
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting.proto
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting_pb2.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting_pb2.pyi
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos_proto/cosmos.proto
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos_proto/cosmos_pb2.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos_proto/cosmos_pb2.pyi
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/gogoproto/gogo.proto
+-rw-r--r--   0        0        0    14516 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/gogoproto/gogo_pb2.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/gogoproto/gogo_pb2.pyi
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/annotations.proto
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0    12099 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/http.proto
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/http_pb2.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/protobuf/any.proto
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/protobuf/any_pb2.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/protobuf/any_pb2.pyi
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller.proto
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller_pb2.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller_pb2.pyi
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query.proto
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host.proto
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host_pb2.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host_pb2.pyi
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query.proto
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account.proto
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account_pb2.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account_pb2.pyi
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis.proto
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata.proto
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata_pb2.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata_pb2.pyi
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet.proto
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet_pb2.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet_pb2.pyi
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis.proto
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/query.proto
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer.proto
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer_pb2.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer_pb2.pyi
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/tx.proto
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/tx_pb2.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v2/packet.proto
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v2/packet_pb2.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v2/packet_pb2.pyi
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/channel.proto
+-rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/channel_pb2.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/channel_pb2.pyi
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/genesis.proto
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0    14315 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/query.proto
+-rw-r--r--   0        0        0    18937 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2.py
+-rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    25454 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/tx.proto
+-rw-r--r--   0        0        0    20228 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/tx_pb2.py
+-rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/client.proto
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/client_pb2.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/client_pb2.pyi
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/genesis.proto
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/query.proto
+-rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/query_pb2.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    15612 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/tx.proto
+-rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/tx_pb2.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/commitment/v1/commitment.proto
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/connection/v1/connection.proto
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/connection/v1/genesis.proto
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/connection/v1/query.proto
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/connection/v1/tx.proto
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/types/v1/genesis.proto
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost.proto
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost_pb2.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost_pb2.pyi
+-rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/solomachine/v1/solomachine.proto
+-rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/solomachine/v2/solomachine.proto
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/tendermint/v1/tendermint.proto
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/consumer.proto
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/genesis.proto
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query.proto
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/genesis.proto
+-rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/provider.proto
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/query.proto
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx.proto
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx_pb2.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/ccv.proto
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/query.proto
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2.pyi
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/tx.proto
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/tx_pb2.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/deposit.proto
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/events.proto
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/genesis.proto
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/genesis_pb2.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/msg.proto
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/msg_pb2.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/msg_pb2.pyi
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/params.proto
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/params_pb2.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/params_pb2.pyi
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/querier.proto
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/mint/v1/genesis.proto
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/mint/v1/inflation.proto
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/events.proto
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/genesis.proto
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/msg.proto
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/node.proto
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/params.proto
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/querier.proto
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/events.proto
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/genesis.proto
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/msg.proto
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/params.proto
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/params_pb2.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/params_pb2.pyi
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/plan.proto
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/querier.proto
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/events.proto
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/genesis.proto
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/msg.proto
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/params.proto
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/provider.proto
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/querier.proto
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/events.proto
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/genesis.proto
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/msg.proto
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/params.proto
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/proof.proto
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/querier.proto
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/session.proto
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/events.proto
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/genesis.proto
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/msg.proto
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/params.proto
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/querier.proto
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/quota.proto
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/subscription.proto
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/swap/v1/events.proto
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/swap/v1/genesis.proto
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/swap/v1/msg.proto
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/swap/v1/params.proto
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/swap/v1/querier.proto
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/swap/v1/swap.proto
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/types/v1/bandwidth.proto
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/types/v1/status.proto
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/genesis.proto
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/msg.proto
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/msg_pb2.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/msg_pb2.pyi
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/params.proto
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/params_pb2.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/params_pb2.pyi
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/querier.proto
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/querier_pb2.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/querier_pb2.pyi
+-rw-r--r--   0        0        0    12749 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/abci/types.proto
+-rw-r--r--   0        0        0    21205 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/abci/types_pb2.py
+-rw-r--r--   0        0        0    24568 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/abci/types_pb2.pyi
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/blockchain/types.proto
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/blockchain/types_pb2.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/blockchain/types_pb2.pyi
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/types.proto
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/types_pb2.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/types_pb2.pyi
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/wal.proto
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/wal_pb2.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/wal_pb2.pyi
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/keys.proto
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/keys_pb2.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/keys_pb2.pyi
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/proof.proto
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/proof_pb2.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/proof_pb2.pyi
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/libs/bits/types.proto
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/libs/bits/types_pb2.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/libs/bits/types_pb2.pyi
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/mempool/types.proto
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/mempool/types_pb2.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/mempool/types_pb2.pyi
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/conn.proto
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/conn_pb2.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/conn_pb2.pyi
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/pex.proto
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/pex_pb2.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/pex_pb2.pyi
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/types.proto
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/types_pb2.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/types_pb2.pyi
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/privval/types.proto
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/privval/types_pb2.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/privval/types_pb2.pyi
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/rpc/grpc/types.proto
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/rpc/grpc/types_pb2.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/rpc/grpc/types_pb2.pyi
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/state/types.proto
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/state/types_pb2.py
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/state/types_pb2.pyi
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/statesync/types.proto
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/statesync/types_pb2.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/statesync/types_pb2.pyi
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/store/types.proto
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/store/types_pb2.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/store/types_pb2.pyi
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/block.proto
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/block_pb2.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/block_pb2.pyi
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/canonical.proto
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/canonical_pb2.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/canonical_pb2.pyi
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/events.proto
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/events_pb2.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/events_pb2.pyi
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/evidence.proto
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/evidence_pb2.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/evidence_pb2.pyi
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/params.proto
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/params_pb2.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/params_pb2.pyi
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/types.proto
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/types_pb2.py
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/types_pb2.pyi
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/validator.proto
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/validator_pb2.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/validator_pb2.pyi
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/version/types.proto
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/version/types_pb2.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/version/types_pb2.pyi
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/.gitignore
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/README.md
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 sentinel_protobuf-0.2.1/PKG-INFO
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/auth.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/auth.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/auth_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/auth_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/auth/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/authz.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/authz.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/authz_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/authz_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/event.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/event.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/event_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/event_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/authz/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/authz/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/authz.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/authz.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/authz_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/authz_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/bank.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/bank.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/bank_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/bank_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/bank_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/bank_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/bank/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/bank/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/abci/v1beta1/abci_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/kv/v1beta1/kv_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/query/v1beta1/pagination_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v1beta1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/commit_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/store/v1beta1/listening_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/v1beta1/coin.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/v1beta1/coin.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/v1beta1/coin_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/v1beta1/coin_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/base/v1beta1/coin_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/base/v1beta1/coin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/capability.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/capability.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/capability_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/capability_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/capability/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crisis/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/ed25519/keys.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/ed25519/keys.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/ed25519/keys_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/ed25519/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/ed25519/keys_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/ed25519/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/keys.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/keys.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/keys_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/keys_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256k1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/crypto/secp256r1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/distribution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/distribution/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/evidence/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/feegrant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/feegrant/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/genutil/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/gov.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/gov.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/gov_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/gov_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/gov_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/gov/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/gov/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/ics23/v1` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/ics23/v1`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/mint.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/mint.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/mint_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/mint_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/mint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/mint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/params.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/params.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/params_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/params_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/params/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/slashing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/slashing/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/authz.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/authz.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/authz_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/authz_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/staking.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/staking.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/staking_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/staking_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/staking_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/staking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/staking/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/staking/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/signing/v1beta1/signing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/service.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/service.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/tx/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/tx/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/upgrade/v1beta1/upgrade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos/vesting/v1beta1/vesting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos_proto/cosmos.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos_proto/cosmos.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos_proto/cosmos_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos_proto/cosmos_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/cosmos_proto/cosmos_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/cosmos_proto/cosmos_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/gogoproto/gogo.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/gogoproto/gogo.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/gogoproto/gogo_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/gogoproto/gogo_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/annotations.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/annotations_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/http.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/http_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/api/http_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/protobuf/any.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/protobuf/any_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/protobuf/any_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/google/protobuf/any_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/google/protobuf/any_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/controller_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/controller/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/host_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/host/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/interchain_accounts/v1/packet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v2/packet.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v2/packet.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v2/packet_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v2/packet_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/applications/transfer/v2/packet_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/applications/transfer/v2/packet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/channel.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/channel.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/channel_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/channel_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/channel/v1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/channel/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/client.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/client.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/client_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/client_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/client_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/genesis_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/genesis_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/client/v1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/client/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/commitment/v1/commitment.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/commitment/v1/commitment.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/connection/v1/connection.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/connection/v1/connection.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/connection/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/connection/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/connection/v1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/connection/v1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/connection/v1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/connection/v1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/core/types/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/core/types/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/localhost/v1/localhost_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/solomachine/v1/solomachine.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/solomachine/v1/solomachine.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/solomachine/v2/solomachine.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/solomachine/v2/solomachine.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/ibc/lightclients/tendermint/v1/tendermint.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/ibc/lightclients/tendermint/v1/tendermint.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/consumer.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/consumer.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/consumer/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/provider.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/provider.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/query.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/query.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/provider/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/ccv.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/ccv.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2_grpc.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/interchain_security/ccv/v1/tx_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/interchain_security/ccv/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/deposit.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/deposit.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/deposit_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/statesync/types_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/deposit/v1/deposit.proto
+# source: tendermint/statesync/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!sentinel/deposit/v1/deposit.proto\x12\x13sentinel.deposit.v1\x1a\x14gogoproto/gogo.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"v\n\x07\x44\x65posit\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12Z\n\x05\x63oins\x18\x02 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.CoinsB:Z0github.com/sentinel-official/hub/x/deposit/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tendermint/statesync/types.proto\x12\x14tendermint.statesync\"\x98\x02\n\x07Message\x12\x43\n\x11snapshots_request\x18\x01 \x01(\x0b\x32&.tendermint.statesync.SnapshotsRequestH\x00\x12\x45\n\x12snapshots_response\x18\x02 \x01(\x0b\x32\'.tendermint.statesync.SnapshotsResponseH\x00\x12;\n\rchunk_request\x18\x03 \x01(\x0b\x32\".tendermint.statesync.ChunkRequestH\x00\x12=\n\x0e\x63hunk_response\x18\x04 \x01(\x0b\x32#.tendermint.statesync.ChunkResponseH\x00\x42\x05\n\x03sum\"\x12\n\x10SnapshotsRequest\"c\n\x11SnapshotsResponse\x12\x0e\n\x06height\x18\x01 \x01(\x04\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\r\x12\x0e\n\x06\x63hunks\x18\x03 \x01(\r\x12\x0c\n\x04hash\x18\x04 \x01(\x0c\x12\x10\n\x08metadata\x18\x05 \x01(\x0c\"=\n\x0c\x43hunkRequest\x12\x0e\n\x06height\x18\x01 \x01(\x04\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\r\x12\r\n\x05index\x18\x03 \x01(\r\"^\n\rChunkResponse\x12\x0e\n\x06height\x18\x01 \x01(\x04\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\r\x12\r\n\x05index\x18\x03 \x01(\r\x12\r\n\x05\x63hunk\x18\x04 \x01(\x0c\x12\x0f\n\x07missing\x18\x05 \x01(\x08\x42=Z;github.com/tendermint/tendermint/proto/tendermint/statesyncb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.deposit.v1.deposit_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.statesync.types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z0github.com/sentinel-official/hub/x/deposit/types\250\342\036\000\310\341\036\000'
-  _DEPOSIT.fields_by_name['coins']._options = None
-  _DEPOSIT.fields_by_name['coins']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
-  _DEPOSIT._serialized_start=112
-  _DEPOSIT._serialized_end=230
+  DESCRIPTOR._serialized_options = b'Z;github.com/tendermint/tendermint/proto/tendermint/statesync'
+  _MESSAGE._serialized_start=59
+  _MESSAGE._serialized_end=339
+  _SNAPSHOTSREQUEST._serialized_start=341
+  _SNAPSHOTSREQUEST._serialized_end=359
+  _SNAPSHOTSRESPONSE._serialized_start=361
+  _SNAPSHOTSRESPONSE._serialized_end=460
+  _CHUNKREQUEST._serialized_start=462
+  _CHUNKREQUEST._serialized_end=523
+  _CHUNKRESPONSE._serialized_start=525
+  _CHUNKRESPONSE._serialized_end=619
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/deposit_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/mempool/types_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from gogoproto import gogo_pb2 as _gogo_pb2
-from cosmos.base.v1beta1 import coin_pb2 as _coin_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Deposit(_message.Message):
-    __slots__ = ["address", "coins"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    COINS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    coins: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    def __init__(self, address: _Optional[str] = ..., coins: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ...) -> None: ...
+class Message(_message.Message):
+    __slots__ = ["txs"]
+    TXS_FIELD_NUMBER: _ClassVar[int]
+    txs: Txs
+    def __init__(self, txs: _Optional[_Union[Txs, _Mapping]] = ...) -> None: ...
+
+class Txs(_message.Message):
+    __slots__ = ["txs"]
+    TXS_FIELD_NUMBER: _ClassVar[int]
+    txs: _containers.RepeatedScalarFieldContainer[bytes]
+    def __init__(self, txs: _Optional[_Iterable[bytes]] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/events.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/events.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/events_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/pex_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from cosmos.base.v1beta1 import coin_pb2 as _coin_pb2
+from tendermint.p2p import types_pb2 as _types_pb2
 from gogoproto import gogo_pb2 as _gogo_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class EventAdd(_message.Message):
-    __slots__ = ["address", "coins"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    COINS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    coins: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    def __init__(self, address: _Optional[str] = ..., coins: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ...) -> None: ...
+class Message(_message.Message):
+    __slots__ = ["pex_addrs", "pex_request"]
+    PEX_ADDRS_FIELD_NUMBER: _ClassVar[int]
+    PEX_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    pex_addrs: PexAddrs
+    pex_request: PexRequest
+    def __init__(self, pex_request: _Optional[_Union[PexRequest, _Mapping]] = ..., pex_addrs: _Optional[_Union[PexAddrs, _Mapping]] = ...) -> None: ...
 
-class EventSubtract(_message.Message):
-    __slots__ = ["address", "coins"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    COINS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    coins: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    def __init__(self, address: _Optional[str] = ..., coins: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ...) -> None: ...
+class PexAddrs(_message.Message):
+    __slots__ = ["addrs"]
+    ADDRS_FIELD_NUMBER: _ClassVar[int]
+    addrs: _containers.RepeatedCompositeFieldContainer[_types_pb2.NetAddress]
+    def __init__(self, addrs: _Optional[_Iterable[_Union[_types_pb2.NetAddress, _Mapping]]] = ...) -> None: ...
+
+class PexRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/querier.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/querier.proto`

 * *Files 1% similar despite different names*

```diff
@@ -28,10 +28,10 @@
 
 service QueryService {
   rpc QueryDeposits(QueryDepositsRequest) returns (QueryDepositsResponse) {
     option (google.api.http).get = "/sentinel/deposits";
   }
 
   rpc QueryDeposit(QueryDepositRequest) returns (QueryDepositResponse) {
-    option (google.api.http).get = "/sentinel/deposits/{address}";
+    option (google.api.http).get = "/sentinel/accounts/{address}/deposits";
   }
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/deposit/v1/querier_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/params_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/deposit/v1/querier.proto
+# source: tendermint/types/params.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.query.v1beta1 import pagination_pb2 as cosmos_dot_base_dot_query_dot_v1beta1_dot_pagination__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from sentinel.deposit.v1 import deposit_pb2 as sentinel_dot_deposit_dot_v1_dot_deposit__pb2
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!sentinel/deposit/v1/querier.proto\x12\x13sentinel.deposit.v1\x1a*cosmos/base/query/v1beta1/pagination.proto\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a!sentinel/deposit/v1/deposit.proto\"R\n\x14QueryDepositsRequest\x12:\n\npagination\x18\x01 \x01(\x0b\x32&.cosmos.base.query.v1beta1.PageRequest\"&\n\x13QueryDepositRequest\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\"\x8a\x01\n\x15QueryDepositsResponse\x12\x34\n\x08\x64\x65posits\x18\x01 \x03(\x0b\x32\x1c.sentinel.deposit.v1.DepositB\x04\xc8\xde\x1f\x00\x12;\n\npagination\x18\x02 \x01(\x0b\x32\'.cosmos.base.query.v1beta1.PageResponse\"K\n\x14QueryDepositResponse\x12\x33\n\x07\x64\x65posit\x18\x01 \x01(\x0b\x32\x1c.sentinel.deposit.v1.DepositB\x04\xc8\xde\x1f\x00\x32\x9f\x02\n\x0cQueryService\x12\x82\x01\n\rQueryDeposits\x12).sentinel.deposit.v1.QueryDepositsRequest\x1a*.sentinel.deposit.v1.QueryDepositsResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\x12\x12/sentinel/deposits\x12\x89\x01\n\x0cQueryDeposit\x12(.sentinel.deposit.v1.QueryDepositRequest\x1a).sentinel.deposit.v1.QueryDepositResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/sentinel/deposits/{address}B:Z0github.com/sentinel-official/hub/x/deposit/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtendermint/types/params.proto\x12\x10tendermint.types\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\"\xf3\x01\n\x0f\x43onsensusParams\x12\x32\n\x05\x62lock\x18\x01 \x01(\x0b\x32\x1d.tendermint.types.BlockParamsB\x04\xc8\xde\x1f\x00\x12\x38\n\x08\x65vidence\x18\x02 \x01(\x0b\x32 .tendermint.types.EvidenceParamsB\x04\xc8\xde\x1f\x00\x12:\n\tvalidator\x18\x03 \x01(\x0b\x32!.tendermint.types.ValidatorParamsB\x04\xc8\xde\x1f\x00\x12\x36\n\x07version\x18\x04 \x01(\x0b\x32\x1f.tendermint.types.VersionParamsB\x04\xc8\xde\x1f\x00\"G\n\x0b\x42lockParams\x12\x11\n\tmax_bytes\x18\x01 \x01(\x03\x12\x0f\n\x07max_gas\x18\x02 \x01(\x03\x12\x14\n\x0ctime_iota_ms\x18\x03 \x01(\x03\"~\n\x0e\x45videnceParams\x12\x1a\n\x12max_age_num_blocks\x18\x01 \x01(\x03\x12=\n\x10max_age_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xc8\xde\x1f\x00\x98\xdf\x1f\x01\x12\x11\n\tmax_bytes\x18\x03 \x01(\x03\"2\n\x0fValidatorParams\x12\x15\n\rpub_key_types\x18\x01 \x03(\t:\x08\xb8\xa0\x1f\x01\xe8\xa0\x1f\x01\".\n\rVersionParams\x12\x13\n\x0b\x61pp_version\x18\x01 \x01(\x04:\x08\xb8\xa0\x1f\x01\xe8\xa0\x1f\x01\">\n\x0cHashedParams\x12\x17\n\x0f\x62lock_max_bytes\x18\x01 \x01(\x03\x12\x15\n\rblock_max_gas\x18\x02 \x01(\x03\x42=Z7github.com/tendermint/tendermint/proto/tendermint/types\xa8\xe2\x1e\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.deposit.v1.querier_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.params_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z0github.com/sentinel-official/hub/x/deposit/types\250\342\036\000\310\341\036\000'
-  _QUERYDEPOSITSRESPONSE.fields_by_name['deposits']._options = None
-  _QUERYDEPOSITSRESPONSE.fields_by_name['deposits']._serialized_options = b'\310\336\037\000'
-  _QUERYDEPOSITRESPONSE.fields_by_name['deposit']._options = None
-  _QUERYDEPOSITRESPONSE.fields_by_name['deposit']._serialized_options = b'\310\336\037\000'
-  _QUERYSERVICE.methods_by_name['QueryDeposits']._options = None
-  _QUERYSERVICE.methods_by_name['QueryDeposits']._serialized_options = b'\202\323\344\223\002\024\022\022/sentinel/deposits'
-  _QUERYSERVICE.methods_by_name['QueryDeposit']._options = None
-  _QUERYSERVICE.methods_by_name['QueryDeposit']._serialized_options = b'\202\323\344\223\002\036\022\034/sentinel/deposits/{address}'
-  _QUERYDEPOSITSREQUEST._serialized_start=189
-  _QUERYDEPOSITSREQUEST._serialized_end=271
-  _QUERYDEPOSITREQUEST._serialized_start=273
-  _QUERYDEPOSITREQUEST._serialized_end=311
-  _QUERYDEPOSITSRESPONSE._serialized_start=314
-  _QUERYDEPOSITSRESPONSE._serialized_end=452
-  _QUERYDEPOSITRESPONSE._serialized_start=454
-  _QUERYDEPOSITRESPONSE._serialized_end=529
-  _QUERYSERVICE._serialized_start=532
-  _QUERYSERVICE._serialized_end=819
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types\250\342\036\001'
+  _CONSENSUSPARAMS.fields_by_name['block']._options = None
+  _CONSENSUSPARAMS.fields_by_name['block']._serialized_options = b'\310\336\037\000'
+  _CONSENSUSPARAMS.fields_by_name['evidence']._options = None
+  _CONSENSUSPARAMS.fields_by_name['evidence']._serialized_options = b'\310\336\037\000'
+  _CONSENSUSPARAMS.fields_by_name['validator']._options = None
+  _CONSENSUSPARAMS.fields_by_name['validator']._serialized_options = b'\310\336\037\000'
+  _CONSENSUSPARAMS.fields_by_name['version']._options = None
+  _CONSENSUSPARAMS.fields_by_name['version']._serialized_options = b'\310\336\037\000'
+  _EVIDENCEPARAMS.fields_by_name['max_age_duration']._options = None
+  _EVIDENCEPARAMS.fields_by_name['max_age_duration']._serialized_options = b'\310\336\037\000\230\337\037\001'
+  _VALIDATORPARAMS._options = None
+  _VALIDATORPARAMS._serialized_options = b'\270\240\037\001\350\240\037\001'
+  _VERSIONPARAMS._options = None
+  _VERSIONPARAMS._serialized_options = b'\270\240\037\001\350\240\037\001'
+  _CONSENSUSPARAMS._serialized_start=106
+  _CONSENSUSPARAMS._serialized_end=349
+  _BLOCKPARAMS._serialized_start=351
+  _BLOCKPARAMS._serialized_end=422
+  _EVIDENCEPARAMS._serialized_start=424
+  _EVIDENCEPARAMS._serialized_end=550
+  _VALIDATORPARAMS._serialized_start=552
+  _VALIDATORPARAMS._serialized_end=602
+  _VERSIONPARAMS._serialized_start=604
+  _VERSIONPARAMS._serialized_end=650
+  _HASHEDPARAMS._serialized_start=652
+  _HASHEDPARAMS._serialized_end=714
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/mint/v1/inflation.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/mint/v1/inflation.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v1/node.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/node.proto`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 syntax = "proto3";
 package sentinel.node.v1;
 
+option go_package = "github.com/sentinel-official/hub/x/node/types";
+
 import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 import "google/protobuf/timestamp.proto";
 import "sentinel/types/v1/status.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/node/legacy/v1/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 message Node {
   string address                          = 1;
   string provider                         = 2;
   repeated cosmos.base.v1beta1.Coin price = 3 [
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/events.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/events.proto`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 syntax = "proto3";
-package sentinel.node.v2;
+package sentinel.node.v1;
 
 import "gogoproto/gogo.proto";
 import "sentinel/types/v1/status.proto";
 
 option go_package            = "github.com/sentinel-official/hub/x/node/types";
 option (gogoproto.equal_all) = false;
 option (gogoproto.goproto_getters_all) = false;
 
 message EventRegister {
-  string address = 1 [ (gogoproto.moretags) = "yaml:\"address\"" ];
+  string address  = 1 [ (gogoproto.moretags) = "yaml:\"address\"" ];
+  string provider = 2 [ (gogoproto.moretags) = "yaml:\"provider\"" ];
 }
 
 message EventUpdate {
-  string address = 1 [ (gogoproto.moretags) = "yaml:\"address\"" ];
+  string address  = 1 [ (gogoproto.moretags) = "yaml:\"address\"" ];
+  string provider = 2 [ (gogoproto.moretags) = "yaml:\"provider\"" ];
 }
 
 message EventSetStatus {
   string address = 1 [ (gogoproto.moretags) = "yaml:\"address\"" ];
   sentinel.types.v1.Status status = 2
       [ (gogoproto.moretags) = "yaml:\"status\"" ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/events_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/version/types_pb2.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 from gogoproto import gogo_pb2 as _gogo_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class EventRegister(_message.Message):
-    __slots__ = ["address"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    def __init__(self, address: _Optional[str] = ...) -> None: ...
+class App(_message.Message):
+    __slots__ = ["protocol", "software"]
+    PROTOCOL_FIELD_NUMBER: _ClassVar[int]
+    SOFTWARE_FIELD_NUMBER: _ClassVar[int]
+    protocol: int
+    software: str
+    def __init__(self, protocol: _Optional[int] = ..., software: _Optional[str] = ...) -> None: ...
 
-class EventSetStatus(_message.Message):
-    __slots__ = ["address", "status"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    status: _status_pb2.Status
-    def __init__(self, address: _Optional[str] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ...) -> None: ...
-
-class EventUpdate(_message.Message):
-    __slots__ = ["address"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    def __init__(self, address: _Optional[str] = ...) -> None: ...
+class Consensus(_message.Message):
+    __slots__ = ["app", "block"]
+    APP_FIELD_NUMBER: _ClassVar[int]
+    BLOCK_FIELD_NUMBER: _ClassVar[int]
+    app: int
+    block: int
+    def __init__(self, block: _Optional[int] = ..., app: _Optional[int] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/lease.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/swap/v1/msg.proto`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 syntax = "proto3";
-package sentinel.node.v2;
+package sentinel.swap.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/swap/types";
 
-import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 
-option go_package            = "github.com/sentinel-official/hub/x/node/types";
-option (gogoproto.equal_all) = false;
+option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message Lease {
-  uint64 id                      = 1 [ (gogoproto.customname) = "ID" ];
-  string node_address            = 2;
-  string account_address         = 3;
-  int64 hours                    = 4;
-  cosmos.base.v1beta1.Coin price = 5 [ (gogoproto.nullable) = false ];
-}
+// MsgSwapRequest defines the SDK message for swapping an ERC-20 token to the
+// native coin
+message MsgSwapRequest {
+  string from     = 1;
+  bytes tx_hash   = 2;
+  string receiver = 3;
+  string amount   = 4 [
+    (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
+    (gogoproto.nullable)   = false
+  ];
+}
+
+// MsgSwapResponse defines the response of message MsgSwapRequest
+message MsgSwapResponse {}
+
+service MsgService { rpc MsgSwap(MsgSwapRequest) returns (MsgSwapResponse); }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/lease_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/keys_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/node/v2/lease.proto
+# source: tendermint/crypto/keys.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1csentinel/node/v2/lease.proto\x12\x10sentinel.node.v2\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\"\x89\x01\n\x05Lease\x12\x12\n\x02id\x18\x01 \x01(\x04\x42\x06\xe2\xde\x1f\x02ID\x12\x14\n\x0cnode_address\x18\x02 \x01(\t\x12\x17\n\x0f\x61\x63\x63ount_address\x18\x03 \x01(\t\x12\r\n\x05hours\x18\x04 \x01(\x03\x12.\n\x05price\x18\x05 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x42\x37Z-github.com/sentinel-official/hub/x/node/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctendermint/crypto/keys.proto\x12\x11tendermint.crypto\x1a\x14gogoproto/gogo.proto\"D\n\tPublicKey\x12\x11\n\x07\x65\x64\x32\x35\x35\x31\x39\x18\x01 \x01(\x0cH\x00\x12\x13\n\tsecp256k1\x18\x02 \x01(\x0cH\x00:\x08\xe8\xa1\x1f\x01\xe8\xa0\x1f\x01\x42\x05\n\x03sumB:Z8github.com/tendermint/tendermint/proto/tendermint/cryptob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.node.v2.lease_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.crypto.keys_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/sentinel-official/hub/x/node/types\250\342\036\000\310\341\036\000'
-  _LEASE.fields_by_name['id']._options = None
-  _LEASE.fields_by_name['id']._serialized_options = b'\342\336\037\002ID'
-  _LEASE.fields_by_name['price']._options = None
-  _LEASE.fields_by_name['price']._serialized_options = b'\310\336\037\000'
-  _LEASE._serialized_start=105
-  _LEASE._serialized_end=242
+  DESCRIPTOR._serialized_options = b'Z8github.com/tendermint/tendermint/proto/tendermint/crypto'
+  _PUBLICKEY._options = None
+  _PUBLICKEY._serialized_options = b'\350\241\037\001\350\240\037\001'
+  _PUBLICKEY._serialized_start=73
+  _PUBLICKEY._serialized_end=141
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/msg.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/msg.proto`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,55 @@
 syntax = "proto3";
-package sentinel.node.v2;
+package sentinel.node.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/node/types";
 
 import "gogoproto/gogo.proto";
 import "cosmos/base/v1beta1/coin.proto";
 import "sentinel/types/v1/status.proto";
 
-option go_package            = "github.com/sentinel-official/hub/x/node/types";
-option (gogoproto.equal_all) = false;
+option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 // MsgRegisterRequest defines the SDK message for registering a node
 message MsgRegisterRequest {
-  string from                                       = 1;
-  repeated cosmos.base.v1beta1.Coin gigabyte_prices = 2 [
-    (gogoproto.nullable)     = false,
-    (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
-  ];
-  repeated cosmos.base.v1beta1.Coin hourly_prices = 3 [
+  string from                             = 1;
+  string provider                         = 2;
+  repeated cosmos.base.v1beta1.Coin price = 3 [
     (gogoproto.nullable)     = false,
     (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
   ];
   string remote_url = 4 [ (gogoproto.customname) = "RemoteURL" ];
 }
 
-// MsgUpdateDetailsRequest defines the SDK message for updating the node details
-message MsgUpdateDetailsRequest {
-  string from                                       = 1;
-  repeated cosmos.base.v1beta1.Coin gigabyte_prices = 2 [
-    (gogoproto.nullable)     = false,
-    (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
-  ];
-  repeated cosmos.base.v1beta1.Coin hourly_prices = 3 [
+// MsgUpdateRequest defines the SDK message for updating a node
+message MsgUpdateRequest {
+  string from                             = 1;
+  string provider                         = 2;
+  repeated cosmos.base.v1beta1.Coin price = 3 [
     (gogoproto.nullable)     = false,
     (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
   ];
   string remote_url = 4 [ (gogoproto.customname) = "RemoteURL" ];
 }
 
-// MsgUpdateStatusRequest defines the SDK message for updating the node status
-message MsgUpdateStatusRequest {
+// MsgSetStatusRequest defines the SDK message for modifying the status of a
+// node
+message MsgSetStatusRequest {
   string from                     = 1;
   sentinel.types.v1.Status status = 2;
 }
 
-// MsgSubscribeRequest defines the SDK message for subscribe to a node
-message MsgSubscribeRequest {
-  string from    = 1;
-  string address = 2;
-  int64 hours    = 3;
-  string denom   = 4;
-}
-
 // MsgRegisterResponse defines the response of message MsgRegisterRequest
 message MsgRegisterResponse {}
 
-// MsgUpdateDetailsResponse defines the response of message
-// MsgUpdateDetailsRequest
-message MsgUpdateDetailsResponse {}
-
-// MsgUpdateStatusResponse defines the response of message
-// MsgUpdateStatusRequest
-message MsgUpdateStatusResponse {}
+// MsgUpdateResponse defines the response of message MsgUpdateRequest
+message MsgUpdateResponse {}
 
-// MsgSubscribeResponse defines the response of message MsgSubscribeRequest
-message MsgSubscribeResponse {}
+// MsgSetStatusResponse defines the response of message MsgSetStatusRequest
+message MsgSetStatusResponse {}
 
 service MsgService {
   rpc MsgRegister(MsgRegisterRequest) returns (MsgRegisterResponse);
-  rpc MsgUpdateDetails(MsgUpdateDetailsRequest)
-      returns (MsgUpdateDetailsResponse);
-  rpc MsgUpdateStatus(MsgUpdateStatusRequest) returns (MsgUpdateStatusResponse);
-  rpc MsgSubscribe(MsgSubscribeRequest) returns (MsgSubscribeResponse);
+  rpc MsgUpdate(MsgUpdateRequest) returns (MsgUpdateResponse);
+  rpc MsgSetStatus(MsgSetStatusRequest) returns (MsgSetStatusResponse);
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/msg_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/canonical_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,58 @@
 from gogoproto import gogo_pb2 as _gogo_pb2
-from cosmos.base.v1beta1 import coin_pb2 as _coin_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
-from google.protobuf.internal import containers as _containers
+from tendermint.types import types_pb2 as _types_pb2
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class MsgRegisterRequest(_message.Message):
-    __slots__ = ["gigabyte_prices", "hourly_prices", "remote_url"]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    GIGABYTE_PRICES_FIELD_NUMBER: _ClassVar[int]
-    HOURLY_PRICES_FIELD_NUMBER: _ClassVar[int]
-    REMOTE_URL_FIELD_NUMBER: _ClassVar[int]
-    gigabyte_prices: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    hourly_prices: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    remote_url: str
-    def __init__(self, gigabyte_prices: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ..., hourly_prices: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ..., remote_url: _Optional[str] = ..., **kwargs) -> None: ...
-
-class MsgRegisterResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MsgSubscribeRequest(_message.Message):
-    __slots__ = ["address", "denom", "hours"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    DENOM_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    HOURS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    denom: str
-    hours: int
-    def __init__(self, address: _Optional[str] = ..., hours: _Optional[int] = ..., denom: _Optional[str] = ..., **kwargs) -> None: ...
-
-class MsgSubscribeResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MsgUpdateDetailsRequest(_message.Message):
-    __slots__ = ["gigabyte_prices", "hourly_prices", "remote_url"]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    GIGABYTE_PRICES_FIELD_NUMBER: _ClassVar[int]
-    HOURLY_PRICES_FIELD_NUMBER: _ClassVar[int]
-    REMOTE_URL_FIELD_NUMBER: _ClassVar[int]
-    gigabyte_prices: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    hourly_prices: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    remote_url: str
-    def __init__(self, gigabyte_prices: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ..., hourly_prices: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ..., remote_url: _Optional[str] = ..., **kwargs) -> None: ...
-
-class MsgUpdateDetailsResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MsgUpdateStatusRequest(_message.Message):
-    __slots__ = ["status"]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    status: _status_pb2.Status
-    def __init__(self, status: _Optional[_Union[_status_pb2.Status, str]] = ..., **kwargs) -> None: ...
-
-class MsgUpdateStatusResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+class CanonicalBlockID(_message.Message):
+    __slots__ = ["hash", "part_set_header"]
+    HASH_FIELD_NUMBER: _ClassVar[int]
+    PART_SET_HEADER_FIELD_NUMBER: _ClassVar[int]
+    hash: bytes
+    part_set_header: CanonicalPartSetHeader
+    def __init__(self, hash: _Optional[bytes] = ..., part_set_header: _Optional[_Union[CanonicalPartSetHeader, _Mapping]] = ...) -> None: ...
+
+class CanonicalPartSetHeader(_message.Message):
+    __slots__ = ["hash", "total"]
+    HASH_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    hash: bytes
+    total: int
+    def __init__(self, total: _Optional[int] = ..., hash: _Optional[bytes] = ...) -> None: ...
+
+class CanonicalProposal(_message.Message):
+    __slots__ = ["block_id", "chain_id", "height", "pol_round", "round", "timestamp", "type"]
+    BLOCK_ID_FIELD_NUMBER: _ClassVar[int]
+    CHAIN_ID_FIELD_NUMBER: _ClassVar[int]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    POL_ROUND_FIELD_NUMBER: _ClassVar[int]
+    ROUND_FIELD_NUMBER: _ClassVar[int]
+    TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    block_id: CanonicalBlockID
+    chain_id: str
+    height: int
+    pol_round: int
+    round: int
+    timestamp: _timestamp_pb2.Timestamp
+    type: _types_pb2.SignedMsgType
+    def __init__(self, type: _Optional[_Union[_types_pb2.SignedMsgType, str]] = ..., height: _Optional[int] = ..., round: _Optional[int] = ..., pol_round: _Optional[int] = ..., block_id: _Optional[_Union[CanonicalBlockID, _Mapping]] = ..., timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., chain_id: _Optional[str] = ...) -> None: ...
+
+class CanonicalVote(_message.Message):
+    __slots__ = ["block_id", "chain_id", "height", "round", "timestamp", "type"]
+    BLOCK_ID_FIELD_NUMBER: _ClassVar[int]
+    CHAIN_ID_FIELD_NUMBER: _ClassVar[int]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    ROUND_FIELD_NUMBER: _ClassVar[int]
+    TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    block_id: CanonicalBlockID
+    chain_id: str
+    height: int
+    round: int
+    timestamp: _timestamp_pb2.Timestamp
+    type: _types_pb2.SignedMsgType
+    def __init__(self, type: _Optional[_Union[_types_pb2.SignedMsgType, str]] = ..., height: _Optional[int] = ..., round: _Optional[int] = ..., block_id: _Optional[_Union[CanonicalBlockID, _Mapping]] = ..., timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., chain_id: _Optional[str] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/node.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/subscription.proto`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 syntax = "proto3";
-package sentinel.node.v2;
+package sentinel.subscription.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/subscription/types";
 
 import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 import "google/protobuf/timestamp.proto";
 import "sentinel/types/v1/status.proto";
 
-option go_package            = "github.com/sentinel-official/hub/x/node/types";
-option (gogoproto.equal_all) = false;
+option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message Node {
-  string address                                    = 1;
-  repeated cosmos.base.v1beta1.Coin gigabyte_prices = 2 [
-    (gogoproto.nullable)     = false,
-    (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
-  ];
-  repeated cosmos.base.v1beta1.Coin hourly_prices = 3 [
-    (gogoproto.nullable)     = false,
-    (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
+message Subscription {
+  uint64 id                        = 1;
+  string owner                     = 2;
+  string node                      = 3;
+  cosmos.base.v1beta1.Coin price   = 4 [ (gogoproto.nullable) = false ];
+  cosmos.base.v1beta1.Coin deposit = 5 [ (gogoproto.nullable) = false ];
+  uint64 plan                      = 6;
+  string denom                     = 7;
+  google.protobuf.Timestamp expiry = 8
+      [ (gogoproto.nullable) = false, (gogoproto.stdtime) = true ];
+  string free = 9 [
+    (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
+    (gogoproto.nullable)   = false
   ];
-  string remote_url               = 4 [ (gogoproto.customname) = "RemoteURL" ];
-  sentinel.types.v1.Status status = 5;
-  google.protobuf.Timestamp status_at = 6
+  sentinel.types.v1.Status status     = 10;
+  google.protobuf.Timestamp status_at = 11
       [ (gogoproto.nullable) = false, (gogoproto.stdtime) = true ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/node_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/evidence_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,52 @@
-from cosmos.base.v1beta1 import coin_pb2 as _coin_pb2
 from gogoproto import gogo_pb2 as _gogo_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
+from tendermint.types import types_pb2 as _types_pb2
+from tendermint.types import validator_pb2 as _validator_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Node(_message.Message):
-    __slots__ = ["address", "gigabyte_prices", "hourly_prices", "remote_url", "status", "status_at"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    GIGABYTE_PRICES_FIELD_NUMBER: _ClassVar[int]
-    HOURLY_PRICES_FIELD_NUMBER: _ClassVar[int]
-    REMOTE_URL_FIELD_NUMBER: _ClassVar[int]
-    STATUS_AT_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    gigabyte_prices: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    hourly_prices: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    remote_url: str
-    status: _status_pb2.Status
-    status_at: _timestamp_pb2.Timestamp
-    def __init__(self, address: _Optional[str] = ..., gigabyte_prices: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ..., hourly_prices: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ..., remote_url: _Optional[str] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ..., status_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+class DuplicateVoteEvidence(_message.Message):
+    __slots__ = ["timestamp", "total_voting_power", "validator_power", "vote_a", "vote_b"]
+    TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_VOTING_POWER_FIELD_NUMBER: _ClassVar[int]
+    VALIDATOR_POWER_FIELD_NUMBER: _ClassVar[int]
+    VOTE_A_FIELD_NUMBER: _ClassVar[int]
+    VOTE_B_FIELD_NUMBER: _ClassVar[int]
+    timestamp: _timestamp_pb2.Timestamp
+    total_voting_power: int
+    validator_power: int
+    vote_a: _types_pb2.Vote
+    vote_b: _types_pb2.Vote
+    def __init__(self, vote_a: _Optional[_Union[_types_pb2.Vote, _Mapping]] = ..., vote_b: _Optional[_Union[_types_pb2.Vote, _Mapping]] = ..., total_voting_power: _Optional[int] = ..., validator_power: _Optional[int] = ..., timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+
+class Evidence(_message.Message):
+    __slots__ = ["duplicate_vote_evidence", "light_client_attack_evidence"]
+    DUPLICATE_VOTE_EVIDENCE_FIELD_NUMBER: _ClassVar[int]
+    LIGHT_CLIENT_ATTACK_EVIDENCE_FIELD_NUMBER: _ClassVar[int]
+    duplicate_vote_evidence: DuplicateVoteEvidence
+    light_client_attack_evidence: LightClientAttackEvidence
+    def __init__(self, duplicate_vote_evidence: _Optional[_Union[DuplicateVoteEvidence, _Mapping]] = ..., light_client_attack_evidence: _Optional[_Union[LightClientAttackEvidence, _Mapping]] = ...) -> None: ...
+
+class EvidenceList(_message.Message):
+    __slots__ = ["evidence"]
+    EVIDENCE_FIELD_NUMBER: _ClassVar[int]
+    evidence: _containers.RepeatedCompositeFieldContainer[Evidence]
+    def __init__(self, evidence: _Optional[_Iterable[_Union[Evidence, _Mapping]]] = ...) -> None: ...
+
+class LightClientAttackEvidence(_message.Message):
+    __slots__ = ["byzantine_validators", "common_height", "conflicting_block", "timestamp", "total_voting_power"]
+    BYZANTINE_VALIDATORS_FIELD_NUMBER: _ClassVar[int]
+    COMMON_HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    CONFLICTING_BLOCK_FIELD_NUMBER: _ClassVar[int]
+    TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_VOTING_POWER_FIELD_NUMBER: _ClassVar[int]
+    byzantine_validators: _containers.RepeatedCompositeFieldContainer[_validator_pb2.Validator]
+    common_height: int
+    conflicting_block: _types_pb2.LightBlock
+    timestamp: _timestamp_pb2.Timestamp
+    total_voting_power: int
+    def __init__(self, conflicting_block: _Optional[_Union[_types_pb2.LightBlock, _Mapping]] = ..., common_height: _Optional[int] = ..., byzantine_validators: _Optional[_Iterable[_Union[_validator_pb2.Validator, _Mapping]]] = ..., total_voting_power: _Optional[int] = ..., timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/params.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/node/v1/params.proto`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 syntax = "proto3";
-package sentinel.node.v2;
+package sentinel.node.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/node/types";
 
-import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 import "google/protobuf/duration.proto";
+import "cosmos/base/v1beta1/coin.proto";
 
-option go_package            = "github.com/sentinel-official/hub/x/node/types";
-option (gogoproto.equal_all) = false;
+option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 message Params {
   cosmos.base.v1beta1.Coin deposit = 1 [ (gogoproto.nullable) = false ];
   google.protobuf.Duration inactive_duration = 2
       [ (gogoproto.nullable) = false, (gogoproto.stdduration) = true ];
-  repeated cosmos.base.v1beta1.Coin max_gigabyte_prices = 3 [
-    (gogoproto.nullable)     = false,
-    (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
-  ];
-  repeated cosmos.base.v1beta1.Coin min_gigabyte_prices = 4 [
-    (gogoproto.nullable)     = false,
-    (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
-  ];
-  repeated cosmos.base.v1beta1.Coin max_hourly_prices = 5 [
+  repeated cosmos.base.v1beta1.Coin max_price = 3 [
     (gogoproto.nullable)     = false,
     (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
   ];
-  repeated cosmos.base.v1beta1.Coin min_hourly_prices = 6 [
+  repeated cosmos.base.v1beta1.Coin min_price = 4 [
     (gogoproto.nullable)     = false,
     (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
   ];
-  int64 max_lease_hours = 7;
-  int64 min_lease_hours = 8;
-  int64 max_leases      = 9;
-  string revenue_share  = 10 [
+  string staking_share = 5 [
     (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Dec",
     (gogoproto.nullable)   = false
   ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/params_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/types_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/node/v2/params.proto
+# source: tendermint/p2p/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dsentinel/node/v2/params.proto\x12\x10sentinel.node.v2\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\"\xab\x05\n\x06Params\x12\x30\n\x07\x64\x65posit\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12>\n\x11inactive_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xc8\xde\x1f\x00\x98\xdf\x1f\x01\x12h\n\x13max_gigabyte_prices\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\x12h\n\x13min_gigabyte_prices\x18\x04 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\x12\x66\n\x11max_hourly_prices\x18\x05 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\x12\x66\n\x11min_hourly_prices\x18\x06 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\x12\x17\n\x0fmax_lease_hours\x18\x07 \x01(\x03\x12\x17\n\x0fmin_lease_hours\x18\x08 \x01(\x03\x12\x12\n\nmax_leases\x18\t \x01(\x03\x12\x45\n\rrevenue_share\x18\n \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x42\x37Z-github.com/sentinel-official/hub/x/node/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1atendermint/p2p/types.proto\x12\x0etendermint.p2p\x1a\x14gogoproto/gogo.proto\"B\n\nNetAddress\x12\x12\n\x02id\x18\x01 \x01(\tB\x06\xe2\xde\x1f\x02ID\x12\x12\n\x02ip\x18\x02 \x01(\tB\x06\xe2\xde\x1f\x02IP\x12\x0c\n\x04port\x18\x03 \x01(\r\"C\n\x0fProtocolVersion\x12\x14\n\x03p2p\x18\x01 \x01(\x04\x42\x07\xe2\xde\x1f\x03P2P\x12\r\n\x05\x62lock\x18\x02 \x01(\x04\x12\x0b\n\x03\x61pp\x18\x03 \x01(\x04\"\x93\x02\n\x0f\x44\x65\x66\x61ultNodeInfo\x12?\n\x10protocol_version\x18\x01 \x01(\x0b\x32\x1f.tendermint.p2p.ProtocolVersionB\x04\xc8\xde\x1f\x00\x12*\n\x0f\x64\x65\x66\x61ult_node_id\x18\x02 \x01(\tB\x11\xe2\xde\x1f\rDefaultNodeID\x12\x13\n\x0blisten_addr\x18\x03 \x01(\t\x12\x0f\n\x07network\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\x10\n\x08\x63hannels\x18\x06 \x01(\x0c\x12\x0f\n\x07moniker\x18\x07 \x01(\t\x12\x39\n\x05other\x18\x08 \x01(\x0b\x32$.tendermint.p2p.DefaultNodeInfoOtherB\x04\xc8\xde\x1f\x00\"M\n\x14\x44\x65\x66\x61ultNodeInfoOther\x12\x10\n\x08tx_index\x18\x01 \x01(\t\x12#\n\x0brpc_address\x18\x02 \x01(\tB\x0e\xe2\xde\x1f\nRPCAddressB7Z5github.com/tendermint/tendermint/proto/tendermint/p2pb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.node.v2.params_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.p2p.types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/sentinel-official/hub/x/node/types\250\342\036\000\310\341\036\000'
-  _PARAMS.fields_by_name['deposit']._options = None
-  _PARAMS.fields_by_name['deposit']._serialized_options = b'\310\336\037\000'
-  _PARAMS.fields_by_name['inactive_duration']._options = None
-  _PARAMS.fields_by_name['inactive_duration']._serialized_options = b'\310\336\037\000\230\337\037\001'
-  _PARAMS.fields_by_name['max_gigabyte_prices']._options = None
-  _PARAMS.fields_by_name['max_gigabyte_prices']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
-  _PARAMS.fields_by_name['min_gigabyte_prices']._options = None
-  _PARAMS.fields_by_name['min_gigabyte_prices']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
-  _PARAMS.fields_by_name['max_hourly_prices']._options = None
-  _PARAMS.fields_by_name['max_hourly_prices']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
-  _PARAMS.fields_by_name['min_hourly_prices']._options = None
-  _PARAMS.fields_by_name['min_hourly_prices']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
-  _PARAMS.fields_by_name['revenue_share']._options = None
-  _PARAMS.fields_by_name['revenue_share']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _PARAMS._serialized_start=138
-  _PARAMS._serialized_end=821
+  DESCRIPTOR._serialized_options = b'Z5github.com/tendermint/tendermint/proto/tendermint/p2p'
+  _NETADDRESS.fields_by_name['id']._options = None
+  _NETADDRESS.fields_by_name['id']._serialized_options = b'\342\336\037\002ID'
+  _NETADDRESS.fields_by_name['ip']._options = None
+  _NETADDRESS.fields_by_name['ip']._serialized_options = b'\342\336\037\002IP'
+  _PROTOCOLVERSION.fields_by_name['p2p']._options = None
+  _PROTOCOLVERSION.fields_by_name['p2p']._serialized_options = b'\342\336\037\003P2P'
+  _DEFAULTNODEINFO.fields_by_name['protocol_version']._options = None
+  _DEFAULTNODEINFO.fields_by_name['protocol_version']._serialized_options = b'\310\336\037\000'
+  _DEFAULTNODEINFO.fields_by_name['default_node_id']._options = None
+  _DEFAULTNODEINFO.fields_by_name['default_node_id']._serialized_options = b'\342\336\037\rDefaultNodeID'
+  _DEFAULTNODEINFO.fields_by_name['other']._options = None
+  _DEFAULTNODEINFO.fields_by_name['other']._serialized_options = b'\310\336\037\000'
+  _DEFAULTNODEINFOOTHER.fields_by_name['rpc_address']._options = None
+  _DEFAULTNODEINFOOTHER.fields_by_name['rpc_address']._serialized_options = b'\342\336\037\nRPCAddress'
+  _NETADDRESS._serialized_start=68
+  _NETADDRESS._serialized_end=134
+  _PROTOCOLVERSION._serialized_start=136
+  _PROTOCOLVERSION._serialized_end=203
+  _DEFAULTNODEINFO._serialized_start=206
+  _DEFAULTNODEINFO._serialized_end=481
+  _DEFAULTNODEINFOOTHER._serialized_start=483
+  _DEFAULTNODEINFOOTHER._serialized_end=560
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/node/v2/querier.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/querier.proto`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,94 @@
 syntax = "proto3";
-package sentinel.node.v2;
+package sentinel.subscription.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/subscription/types";
 
 import "cosmos/base/query/v1beta1/pagination.proto";
 import "gogoproto/gogo.proto";
 import "google/api/annotations.proto";
+import "sentinel/subscription/v1/quota.proto";
 import "sentinel/types/v1/status.proto";
-import "sentinel/node/v2/lease.proto";
-import "sentinel/node/v2/node.proto";
-import "sentinel/node/v2/params.proto";
+import "sentinel/subscription/v1/subscription.proto";
+import "sentinel/subscription/v1/params.proto";
 
-option go_package            = "github.com/sentinel-official/hub/x/node/types";
-option (gogoproto.equal_all) = false;
+option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message QueryNodesRequest {
-  sentinel.types.v1.Status status                  = 1;
-  cosmos.base.query.v1beta1.PageRequest pagination = 2;
+message QuerySubscriptionsRequest {
+  cosmos.base.query.v1beta1.PageRequest pagination = 1;
 }
 
-message QueryNodesForPlanRequest {
-  uint64 id                                        = 1;
+message QuerySubscriptionsForAddressRequest {
+  string address                                   = 1;
   sentinel.types.v1.Status status                  = 2;
   cosmos.base.query.v1beta1.PageRequest pagination = 3;
 }
 
-message QueryNodeRequest { string address = 1; }
+message QuerySubscriptionRequest { uint64 id = 1; }
 
-message QueryLeasesRequest {
-  cosmos.base.query.v1beta1.PageRequest pagination = 1;
+message QueryQuotaRequest {
+  uint64 id      = 1;
+  string address = 2;
 }
 
-message QueryLeasesForAccountRequest {
-  string address                                   = 1;
-  cosmos.base.query.v1beta1.PageRequest pagination = 2;
-}
-
-message QueryLeasesForNodeRequest {
-  string address                                   = 1;
+message QueryQuotasRequest {
+  uint64 id                                        = 1;
   cosmos.base.query.v1beta1.PageRequest pagination = 2;
 }
 
-message QueryLeaseRequest { uint64 id = 1; }
-
 message QueryParamsRequest {}
 
-message QueryNodesResponse {
-  repeated Node nodes = 1 [ (gogoproto.nullable) = false ];
+message QuerySubscriptionsResponse {
+  repeated Subscription subscriptions = 1 [ (gogoproto.nullable) = false ];
   cosmos.base.query.v1beta1.PageResponse pagination = 2;
 }
 
-message QueryNodesForPlanResponse {
-  repeated Node nodes = 1 [ (gogoproto.nullable) = false ];
+message QuerySubscriptionsForAddressResponse {
+  repeated Subscription subscriptions = 1 [ (gogoproto.nullable) = false ];
   cosmos.base.query.v1beta1.PageResponse pagination = 2;
 }
 
-message QueryNodeResponse { Node node = 1 [ (gogoproto.nullable) = false ]; }
-
-message QueryLeasesResponse {
-  repeated Lease leases = 1 [ (gogoproto.nullable) = false ];
-  cosmos.base.query.v1beta1.PageResponse pagination = 2;
+message QuerySubscriptionResponse {
+  Subscription subscription = 1 [ (gogoproto.nullable) = false ];
 }
 
-message QueryLeasesForAccountResponse {
-  repeated Lease leases = 1 [ (gogoproto.nullable) = false ];
-  cosmos.base.query.v1beta1.PageResponse pagination = 2;
-}
+message QueryQuotaResponse { Quota quota = 1 [ (gogoproto.nullable) = false ]; }
 
-message QueryLeasesForNodeResponse {
-  repeated Lease leases = 1 [ (gogoproto.nullable) = false ];
+message QueryQuotasResponse {
+  repeated Quota quotas = 1 [ (gogoproto.nullable) = false ];
   cosmos.base.query.v1beta1.PageResponse pagination = 2;
 }
 
-message QueryLeaseResponse { Lease lease = 1 [ (gogoproto.nullable) = false ]; }
-
 message QueryParamsResponse {
   Params params = 1 [ (gogoproto.nullable) = false ];
 }
 
 service QueryService {
-  rpc QueryNodes(QueryNodesRequest) returns (QueryNodesResponse) {
-    option (google.api.http).get = "/sentinel/nodes";
-  }
-
-  rpc QueryNodesForPlan(QueryNodesForPlanRequest)
-      returns (QueryNodesForPlanResponse) {
-    option (google.api.http).get = "/sentinel/plans/{id}/nodes";
-  }
-
-  rpc QueryNode(QueryNodeRequest) returns (QueryNodeResponse) {
-    option (google.api.http).get = "/sentinel/nodes/{address}";
+  rpc QuerySubscriptions(QuerySubscriptionsRequest)
+      returns (QuerySubscriptionsResponse) {
+    option (google.api.http).get = "/sentinel/subscriptions";
   }
 
-  rpc QueryLeases(QueryLeasesRequest) returns (QueryLeasesResponse) {
-    option (google.api.http).get = "/sentinel/leases";
+  rpc QuerySubscriptionsForAddress(QuerySubscriptionsForAddressRequest)
+      returns (QuerySubscriptionsForAddressResponse) {
+    option (google.api.http).get = "/sentinel/accounts/{address}/subscriptions";
   }
 
-  rpc QueryLeasesForAccount(QueryLeasesForAccountRequest)
-      returns (QueryLeasesForAccountResponse) {
-    option (google.api.http).get = "/sentinel/accounts/{address}/leases";
+  rpc QuerySubscription(QuerySubscriptionRequest)
+      returns (QuerySubscriptionResponse) {
+    option (google.api.http).get = "/sentinel/subscriptions/{id}";
   }
 
-  rpc QueryLeasesForNode(QueryLeasesForNodeRequest)
-      returns (QueryLeasesForNodeResponse) {
-    option (google.api.http).get = "/sentinel/nodes/{address}/leases";
+  rpc QueryQuota(QueryQuotaRequest) returns (QueryQuotaResponse) {
+    option (google.api.http).get =
+        "/accounts/{address}/subscriptions/{id}/quotas";
   }
 
-  rpc QueryLease(QueryLeaseRequest) returns (QueryLeaseResponse) {
-    option (google.api.http).get = "/sentinel/leases/{id}";
+  rpc QueryQuotas(QueryQuotasRequest) returns (QueryQuotasResponse) {
+    option (google.api.http).get = "/sentinel/subscriptions/{id}/quotas";
   }
 
   rpc QueryParams(QueryParamsRequest) returns (QueryParamsResponse) {
-    option (google.api.http).get = "/sentinel/modules/node/params";
+    option (google.api.http).get = "/sentinel/modules/subscription/params";
   }
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v1/plan.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/plan.proto`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 syntax = "proto3";
 package sentinel.plan.v1;
 
-option go_package = "github.com/sentinel-official/hub/x/plan/legacy/v1/types";
+option go_package = "github.com/sentinel-official/hub/x/plan/types";
 
 import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 import "google/protobuf/duration.proto";
 import "google/protobuf/timestamp.proto";
 import "sentinel/types/v1/status.proto";
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v1/plan_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/conn_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/plan/v1/plan.proto
+# source: tendermint/p2p/conn.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from sentinel.types.v1 import status_pb2 as sentinel_dot_types_dot_v1_dot_status__pb2
+from tendermint.crypto import keys_pb2 as tendermint_dot_crypto_dot_keys__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bsentinel/plan/v1/plan.proto\x12\x10sentinel.plan.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1esentinel/types/v1/status.proto\"\xda\x02\n\x04Plan\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x10\n\x08provider\x18\x02 \x01(\t\x12Z\n\x05price\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\x12\x35\n\x08validity\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xc8\xde\x1f\x00\x98\xdf\x1f\x01\x12=\n\x05\x62ytes\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\x12)\n\x06status\x18\x06 \x01(\x0e\x32\x19.sentinel.types.v1.Status\x12\x37\n\tstatus_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x42\x41Z7github.com/sentinel-official/hub/x/plan/legacy/v1/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tendermint/p2p/conn.proto\x12\x0etendermint.p2p\x1a\x14gogoproto/gogo.proto\x1a\x1ctendermint/crypto/keys.proto\"\x0c\n\nPacketPing\"\x0c\n\nPacketPong\"R\n\tPacketMsg\x12!\n\nchannel_id\x18\x01 \x01(\x05\x42\r\xe2\xde\x1f\tChannelID\x12\x14\n\x03\x65of\x18\x02 \x01(\x08\x42\x07\xe2\xde\x1f\x03\x45OF\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"\xa6\x01\n\x06Packet\x12\x31\n\x0bpacket_ping\x18\x01 \x01(\x0b\x32\x1a.tendermint.p2p.PacketPingH\x00\x12\x31\n\x0bpacket_pong\x18\x02 \x01(\x0b\x32\x1a.tendermint.p2p.PacketPongH\x00\x12/\n\npacket_msg\x18\x03 \x01(\x0b\x32\x19.tendermint.p2p.PacketMsgH\x00\x42\x05\n\x03sum\"R\n\x0e\x41uthSigMessage\x12\x33\n\x07pub_key\x18\x01 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKeyB\x04\xc8\xde\x1f\x00\x12\x0b\n\x03sig\x18\x02 \x01(\x0c\x42\x37Z5github.com/tendermint/tendermint/proto/tendermint/p2pb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.plan.v1.plan_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.p2p.conn_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z7github.com/sentinel-official/hub/x/plan/legacy/v1/types\250\342\036\000\310\341\036\000'
-  _PLAN.fields_by_name['price']._options = None
-  _PLAN.fields_by_name['price']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
-  _PLAN.fields_by_name['validity']._options = None
-  _PLAN.fields_by_name['validity']._serialized_options = b'\310\336\037\000\230\337\037\001'
-  _PLAN.fields_by_name['bytes']._options = None
-  _PLAN.fields_by_name['bytes']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Int\310\336\037\000'
-  _PLAN.fields_by_name['status_at']._options = None
-  _PLAN.fields_by_name['status_at']._serialized_options = b'\310\336\037\000\220\337\037\001'
-  _PLAN._serialized_start=201
-  _PLAN._serialized_end=547
+  DESCRIPTOR._serialized_options = b'Z5github.com/tendermint/tendermint/proto/tendermint/p2p'
+  _PACKETMSG.fields_by_name['channel_id']._options = None
+  _PACKETMSG.fields_by_name['channel_id']._serialized_options = b'\342\336\037\tChannelID'
+  _PACKETMSG.fields_by_name['eof']._options = None
+  _PACKETMSG.fields_by_name['eof']._serialized_options = b'\342\336\037\003EOF'
+  _AUTHSIGMESSAGE.fields_by_name['pub_key']._options = None
+  _AUTHSIGMESSAGE.fields_by_name['pub_key']._serialized_options = b'\310\336\037\000'
+  _PACKETPING._serialized_start=97
+  _PACKETPING._serialized_end=109
+  _PACKETPONG._serialized_start=111
+  _PACKETPONG._serialized_end=123
+  _PACKETMSG._serialized_start=125
+  _PACKETMSG._serialized_end=207
+  _PACKET._serialized_start=210
+  _PACKET._serialized_end=376
+  _AUTHSIGMESSAGE._serialized_start=378
+  _AUTHSIGMESSAGE._serialized_end=460
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v1/plan_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/conn_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,43 @@
-from cosmos.base.v1beta1 import coin_pb2 as _coin_pb2
 from gogoproto import gogo_pb2 as _gogo_pb2
-from google.protobuf import duration_pb2 as _duration_pb2
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
-from google.protobuf.internal import containers as _containers
+from tendermint.crypto import keys_pb2 as _keys_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Plan(_message.Message):
-    __slots__ = ["bytes", "id", "price", "provider", "status", "status_at", "validity"]
-    BYTES_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    PRICE_FIELD_NUMBER: _ClassVar[int]
-    PROVIDER_FIELD_NUMBER: _ClassVar[int]
-    STATUS_AT_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    VALIDITY_FIELD_NUMBER: _ClassVar[int]
-    bytes: str
-    id: int
-    price: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    provider: str
-    status: _status_pb2.Status
-    status_at: _timestamp_pb2.Timestamp
-    validity: _duration_pb2.Duration
-    def __init__(self, id: _Optional[int] = ..., provider: _Optional[str] = ..., price: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ..., validity: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., bytes: _Optional[str] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ..., status_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+class AuthSigMessage(_message.Message):
+    __slots__ = ["pub_key", "sig"]
+    PUB_KEY_FIELD_NUMBER: _ClassVar[int]
+    SIG_FIELD_NUMBER: _ClassVar[int]
+    pub_key: _keys_pb2.PublicKey
+    sig: bytes
+    def __init__(self, pub_key: _Optional[_Union[_keys_pb2.PublicKey, _Mapping]] = ..., sig: _Optional[bytes] = ...) -> None: ...
+
+class Packet(_message.Message):
+    __slots__ = ["packet_msg", "packet_ping", "packet_pong"]
+    PACKET_MSG_FIELD_NUMBER: _ClassVar[int]
+    PACKET_PING_FIELD_NUMBER: _ClassVar[int]
+    PACKET_PONG_FIELD_NUMBER: _ClassVar[int]
+    packet_msg: PacketMsg
+    packet_ping: PacketPing
+    packet_pong: PacketPong
+    def __init__(self, packet_ping: _Optional[_Union[PacketPing, _Mapping]] = ..., packet_pong: _Optional[_Union[PacketPong, _Mapping]] = ..., packet_msg: _Optional[_Union[PacketMsg, _Mapping]] = ...) -> None: ...
+
+class PacketMsg(_message.Message):
+    __slots__ = ["channel_id", "data", "eof"]
+    CHANNEL_ID_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    EOF_FIELD_NUMBER: _ClassVar[int]
+    channel_id: int
+    data: bytes
+    eof: bool
+    def __init__(self, channel_id: _Optional[int] = ..., eof: bool = ..., data: _Optional[bytes] = ...) -> None: ...
+
+class PacketPing(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class PacketPong(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/events.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/events.proto`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 syntax = "proto3";
-package sentinel.plan.v2;
+package sentinel.session.v1;
 
+import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 import "sentinel/types/v1/status.proto";
 
-option go_package            = "github.com/sentinel-official/hub/x/plan/types";
-option (gogoproto.equal_all) = false;
+option go_package = "github.com/sentinel-official/hub/x/session/types";
+option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message EventCreate {
-  uint64 id = 1
-      [ (gogoproto.customname) = "ID", (gogoproto.moretags) = "yaml:\"id\"" ];
-  string provider_address = 2
-      [ (gogoproto.moretags) = "yaml:\"provider_address\"" ];
+message EventStart {
+  uint64 id           = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
+  string node         = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
+  uint64 subscription = 3 [ (gogoproto.moretags) = "yaml:\"subscription\"" ];
 }
 
-message EventUpdateStatus {
-  uint64 id = 1
-      [ (gogoproto.customname) = "ID", (gogoproto.moretags) = "yaml:\"id\"" ];
-  string provider_address = 2
-      [ (gogoproto.moretags) = "yaml:\"provider_address\"" ];
-  sentinel.types.v1.Status status = 3
-      [ (gogoproto.moretags) = "yaml:\"status\"" ];
+message EventUpdate {
+  uint64 id           = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
+  string node         = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
+  uint64 subscription = 3 [ (gogoproto.moretags) = "yaml:\"subscription\"" ];
 }
 
-message EventLinkNode {
-  uint64 id = 1
-      [ (gogoproto.customname) = "ID", (gogoproto.moretags) = "yaml:\"id\"" ];
-  string node_address = 2 [ (gogoproto.moretags) = "yaml:\"node_address\"" ];
-  string provider_address = 3
-      [ (gogoproto.moretags) = "yaml:\"provider_address\"" ];
+message EventSetStatus {
+  uint64 id           = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
+  string node         = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
+  uint64 subscription = 3 [ (gogoproto.moretags) = "yaml:\"subscription\"" ];
+  sentinel.types.v1.Status status = 4
+      [ (gogoproto.moretags) = "yaml:\"status\"" ];
 }
 
-message EventUnlinkNode {
-  uint64 id = 1
-      [ (gogoproto.customname) = "ID", (gogoproto.moretags) = "yaml:\"id\"" ];
-  string node_address = 2 [ (gogoproto.moretags) = "yaml:\"node_address\"" ];
-  string provider_address = 3
-      [ (gogoproto.moretags) = "yaml:\"provider_address\"" ];
+message EventPay {
+  uint64 id           = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
+  string node         = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
+  uint64 subscription = 3 [ (gogoproto.moretags) = "yaml:\"subscription\"" ];
+  cosmos.base.v1beta1.Coin amount = 4 [
+    (gogoproto.moretags) = "yaml:\"amount\"",
+    (gogoproto.nullable) = false
+  ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/events_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/proof_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 from gogoproto import gogo_pb2 as _gogo_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class EventCreate(_message.Message):
-    __slots__ = ["id", "provider_address"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    PROVIDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    provider_address: str
-    def __init__(self, id: _Optional[int] = ..., provider_address: _Optional[str] = ...) -> None: ...
-
-class EventLinkNode(_message.Message):
-    __slots__ = ["id", "node_address", "provider_address"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    NODE_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    PROVIDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    node_address: str
-    provider_address: str
-    def __init__(self, id: _Optional[int] = ..., node_address: _Optional[str] = ..., provider_address: _Optional[str] = ...) -> None: ...
-
-class EventUnlinkNode(_message.Message):
-    __slots__ = ["id", "node_address", "provider_address"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    NODE_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    PROVIDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    node_address: str
-    provider_address: str
-    def __init__(self, id: _Optional[int] = ..., node_address: _Optional[str] = ..., provider_address: _Optional[str] = ...) -> None: ...
-
-class EventUpdateStatus(_message.Message):
-    __slots__ = ["id", "provider_address", "status"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    PROVIDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    provider_address: str
-    status: _status_pb2.Status
-    def __init__(self, id: _Optional[int] = ..., provider_address: _Optional[str] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ...) -> None: ...
+class DominoOp(_message.Message):
+    __slots__ = ["input", "key", "output"]
+    INPUT_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_FIELD_NUMBER: _ClassVar[int]
+    input: str
+    key: str
+    output: str
+    def __init__(self, key: _Optional[str] = ..., input: _Optional[str] = ..., output: _Optional[str] = ...) -> None: ...
+
+class Proof(_message.Message):
+    __slots__ = ["aunts", "index", "leaf_hash", "total"]
+    AUNTS_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    LEAF_HASH_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    aunts: _containers.RepeatedScalarFieldContainer[bytes]
+    index: int
+    leaf_hash: bytes
+    total: int
+    def __init__(self, total: _Optional[int] = ..., index: _Optional[int] = ..., leaf_hash: _Optional[bytes] = ..., aunts: _Optional[_Iterable[bytes]] = ...) -> None: ...
+
+class ProofOp(_message.Message):
+    __slots__ = ["data", "key", "type"]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    data: bytes
+    key: bytes
+    type: str
+    def __init__(self, type: _Optional[str] = ..., key: _Optional[bytes] = ..., data: _Optional[bytes] = ...) -> None: ...
+
+class ProofOps(_message.Message):
+    __slots__ = ["ops"]
+    OPS_FIELD_NUMBER: _ClassVar[int]
+    ops: _containers.RepeatedCompositeFieldContainer[ProofOp]
+    def __init__(self, ops: _Optional[_Iterable[_Union[ProofOp, _Mapping]]] = ...) -> None: ...
+
+class ValueOp(_message.Message):
+    __slots__ = ["key", "proof"]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    PROOF_FIELD_NUMBER: _ClassVar[int]
+    key: bytes
+    proof: Proof
+    def __init__(self, key: _Optional[bytes] = ..., proof: _Optional[_Union[Proof, _Mapping]] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/msg.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/msg.proto`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,68 @@
 syntax = "proto3";
-package sentinel.plan.v2;
+package sentinel.plan.v1;
 
 option go_package = "github.com/sentinel-official/hub/x/plan/types";
 
 import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 import "google/protobuf/duration.proto";
 import "sentinel/types/v1/status.proto";
 
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-// MsgCreateRequest defines the SDK message for creating a subscription plan
-message MsgCreateRequest {
-  string from                              = 1;
-  repeated cosmos.base.v1beta1.Coin prices = 2 [
+// MsgAddRequest defines the SDK message for adding a plan
+message MsgAddRequest {
+  string from                             = 1;
+  repeated cosmos.base.v1beta1.Coin price = 2 [
     (gogoproto.nullable)     = false,
     (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
   ];
   google.protobuf.Duration validity = 3
       [ (gogoproto.stdduration) = true, (gogoproto.nullable) = false ];
   string bytes = 4 [
     (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
     (gogoproto.nullable)   = false
   ];
 }
 
-// MsgUpdateStatusRequest defines the SDK message for modifying the status of a
-// subscription plan
-message MsgUpdateStatusRequest {
+// MsgSetStatusRequest defines the SDK message for modifying the status of a
+// plan
+message MsgSetStatusRequest {
   string from                     = 1;
-  uint64 id                       = 2 [ (gogoproto.customname) = "ID" ];
+  uint64 id                       = 2;
   sentinel.types.v1.Status status = 3;
 }
 
-// MsgLinkNodeRequest defines the SDK message for adding a node to a
-// subscription plan
-message MsgLinkNodeRequest {
+// MsgAddNodeRequest defines the SDK message for adding a node to a plan
+message MsgAddNodeRequest {
   string from    = 1;
-  uint64 id      = 2 [ (gogoproto.customname) = "ID" ];
+  uint64 id      = 2;
   string address = 3;
 }
 
-// MsgUnlinkNodeRequest defines the SDK message for removing a node from a
-// subscription plan
-message MsgUnlinkNodeRequest {
+// MsgRemoveNodeRequest defines the SDK message for removing a node from a plan
+message MsgRemoveNodeRequest {
   string from    = 1;
-  uint64 id      = 2 [ (gogoproto.customname) = "ID" ];
+  uint64 id      = 2;
   string address = 3;
 }
 
-// MsgSubscribeRequest defines the SDK message for subscribing to a subscription
-// plan
-message MsgSubscribeRequest {
-  string from  = 1;
-  uint64 id    = 2 [ (gogoproto.customname) = "ID" ];
-  string denom = 3;
-}
-
-// MsgCreateResponse defines the response of message MsgCreateRequest
-message MsgCreateResponse {}
-
-// MsgUpdateStatusResponse defines the response of message
-// MsgUpdateStatusRequest
-message MsgUpdateStatusResponse {}
+// MsgAddResponse defines the response of message MsgRegisterRequest
+message MsgAddResponse {}
 
-// MsgLinkNodeResponse defines the response of message MsgLinkNodeRequest
-message MsgLinkNodeResponse {}
+// MsgSetStatusResponse defines the response of message MsgSetStatusRequest
+message MsgSetStatusResponse {}
 
-// MsgUnlinkNodeResponse defines the response of message MsgUnlinkNodeRequest
-message MsgUnlinkNodeResponse {}
+// MsgAddNodeResponse defines the response of message MsgAddNodeRequest
+message MsgAddNodeResponse {}
 
-// MsgSubscribeResponse defines the response of message MsgSubscribeRequest
-message MsgSubscribeResponse {}
+// MsgRemoveNodeResponse defines the response of message MsgRemoveNodeRequest
+message MsgRemoveNodeResponse {}
 
 service MsgService {
-  rpc MsgCreate(MsgCreateRequest) returns (MsgCreateResponse);
-  rpc MsgUpdateStatus(MsgUpdateStatusRequest) returns (MsgUpdateStatusResponse);
-  rpc MsgLinkNode(MsgLinkNodeRequest) returns (MsgLinkNodeResponse);
-  rpc MsgUnlinkNode(MsgUnlinkNodeRequest) returns (MsgUnlinkNodeResponse);
-  rpc MsgSubscribe(MsgSubscribeRequest) returns (MsgSubscribeResponse);
+  rpc MsgAdd(MsgAddRequest) returns (MsgAddResponse);
+  rpc MsgSetStatus(MsgSetStatusRequest) returns (MsgSetStatusResponse);
+  rpc MsgAddNode(MsgAddNodeRequest) returns (MsgAddNodeResponse);
+  rpc MsgRemoveNode(MsgRemoveNodeRequest) returns (MsgRemoveNodeResponse);
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/msg_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/types_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,54 @@
-from cosmos.base.v1beta1 import coin_pb2 as _coin_pb2
 from gogoproto import gogo_pb2 as _gogo_pb2
-from google.protobuf import duration_pb2 as _duration_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
-from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class MsgCreateRequest(_message.Message):
-    __slots__ = ["bytes", "prices", "validity"]
-    BYTES_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    PRICES_FIELD_NUMBER: _ClassVar[int]
-    VALIDITY_FIELD_NUMBER: _ClassVar[int]
-    bytes: str
-    prices: _containers.RepeatedCompositeFieldContainer[_coin_pb2.Coin]
-    validity: _duration_pb2.Duration
-    def __init__(self, prices: _Optional[_Iterable[_Union[_coin_pb2.Coin, _Mapping]]] = ..., validity: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., bytes: _Optional[str] = ..., **kwargs) -> None: ...
+class DefaultNodeInfo(_message.Message):
+    __slots__ = ["channels", "default_node_id", "listen_addr", "moniker", "network", "other", "protocol_version", "version"]
+    CHANNELS_FIELD_NUMBER: _ClassVar[int]
+    DEFAULT_NODE_ID_FIELD_NUMBER: _ClassVar[int]
+    LISTEN_ADDR_FIELD_NUMBER: _ClassVar[int]
+    MONIKER_FIELD_NUMBER: _ClassVar[int]
+    NETWORK_FIELD_NUMBER: _ClassVar[int]
+    OTHER_FIELD_NUMBER: _ClassVar[int]
+    PROTOCOL_VERSION_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    channels: bytes
+    default_node_id: str
+    listen_addr: str
+    moniker: str
+    network: str
+    other: DefaultNodeInfoOther
+    protocol_version: ProtocolVersion
+    version: str
+    def __init__(self, protocol_version: _Optional[_Union[ProtocolVersion, _Mapping]] = ..., default_node_id: _Optional[str] = ..., listen_addr: _Optional[str] = ..., network: _Optional[str] = ..., version: _Optional[str] = ..., channels: _Optional[bytes] = ..., moniker: _Optional[str] = ..., other: _Optional[_Union[DefaultNodeInfoOther, _Mapping]] = ...) -> None: ...
+
+class DefaultNodeInfoOther(_message.Message):
+    __slots__ = ["rpc_address", "tx_index"]
+    RPC_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    TX_INDEX_FIELD_NUMBER: _ClassVar[int]
+    rpc_address: str
+    tx_index: str
+    def __init__(self, tx_index: _Optional[str] = ..., rpc_address: _Optional[str] = ...) -> None: ...
 
-class MsgCreateResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MsgLinkNodeRequest(_message.Message):
-    __slots__ = ["address", "id"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    id: int
-    def __init__(self, id: _Optional[int] = ..., address: _Optional[str] = ..., **kwargs) -> None: ...
-
-class MsgLinkNodeResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MsgSubscribeRequest(_message.Message):
-    __slots__ = ["denom", "id"]
-    DENOM_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
+class NetAddress(_message.Message):
+    __slots__ = ["id", "ip", "port"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    denom: str
-    id: int
-    def __init__(self, id: _Optional[int] = ..., denom: _Optional[str] = ..., **kwargs) -> None: ...
-
-class MsgSubscribeResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MsgUnlinkNodeRequest(_message.Message):
-    __slots__ = ["address", "id"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    id: int
-    def __init__(self, id: _Optional[int] = ..., address: _Optional[str] = ..., **kwargs) -> None: ...
-
-class MsgUnlinkNodeResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MsgUpdateStatusRequest(_message.Message):
-    __slots__ = ["id", "status"]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    status: _status_pb2.Status
-    def __init__(self, id: _Optional[int] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ..., **kwargs) -> None: ...
-
-class MsgUpdateStatusResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+    IP_FIELD_NUMBER: _ClassVar[int]
+    PORT_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    ip: str
+    port: int
+    def __init__(self, id: _Optional[str] = ..., ip: _Optional[str] = ..., port: _Optional[int] = ...) -> None: ...
+
+class ProtocolVersion(_message.Message):
+    __slots__ = ["app", "block", "p2p"]
+    APP_FIELD_NUMBER: _ClassVar[int]
+    BLOCK_FIELD_NUMBER: _ClassVar[int]
+    P2P_FIELD_NUMBER: _ClassVar[int]
+    app: int
+    block: int
+    p2p: int
+    def __init__(self, p2p: _Optional[int] = ..., block: _Optional[int] = ..., app: _Optional[int] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/plan.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/session.proto`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 syntax = "proto3";
-package sentinel.plan.v2;
+package sentinel.session.v1;
 
-option go_package = "github.com/sentinel-official/hub/x/plan/types";
+option go_package = "github.com/sentinel-official/hub/x/session/types";
 
-import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 import "google/protobuf/duration.proto";
 import "google/protobuf/timestamp.proto";
+import "sentinel/types/v1/bandwidth.proto";
 import "sentinel/types/v1/status.proto";
 
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message Plan {
-  uint64 id               = 1 [ (gogoproto.customname) = "ID" ];
-  string provider_address = 2;
-  repeated cosmos.base.v1beta1.Coin prices = 3 [
-    (gogoproto.nullable)     = false,
-    (gogoproto.castrepeated) = "github.com/cosmos/cosmos-sdk/types.Coins"
-  ];
-  google.protobuf.Duration validity = 4
-      [ (gogoproto.nullable) = false, (gogoproto.stdduration) = true ];
-  string bytes = 5 [
-    (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
-    (gogoproto.nullable)   = false
-  ];
-  sentinel.types.v1.Status status     = 6;
-  google.protobuf.Timestamp status_at = 7
+message Session {
+  uint64 id                         = 1;
+  uint64 subscription               = 2;
+  string node                       = 3;
+  string address                    = 4;
+  google.protobuf.Duration duration = 5
+      [ (gogoproto.stdduration) = true, (gogoproto.nullable) = false ];
+  sentinel.types.v1.Bandwidth bandwidth = 6 [ (gogoproto.nullable) = false ];
+  sentinel.types.v1.Status status       = 7;
+  google.protobuf.Timestamp status_at   = 8
       [ (gogoproto.nullable) = false, (gogoproto.stdtime) = true ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/plan_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/proof_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/plan/v2/plan.proto
+# source: tendermint/crypto/proof.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from sentinel.types.v1 import status_pb2 as sentinel_dot_types_dot_v1_dot_status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bsentinel/plan/v2/plan.proto\x12\x10sentinel.plan.v2\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1esentinel/types/v1/status.proto\"\xeb\x02\n\x04Plan\x12\x12\n\x02id\x18\x01 \x01(\x04\x42\x06\xe2\xde\x1f\x02ID\x12\x18\n\x10provider_address\x18\x02 \x01(\t\x12[\n\x06prices\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\x12\x35\n\x08validity\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xc8\xde\x1f\x00\x98\xdf\x1f\x01\x12=\n\x05\x62ytes\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\x12)\n\x06status\x18\x06 \x01(\x0e\x32\x19.sentinel.types.v1.Status\x12\x37\n\tstatus_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x42\x37Z-github.com/sentinel-official/hub/x/plan/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtendermint/crypto/proof.proto\x12\x11tendermint.crypto\x1a\x14gogoproto/gogo.proto\"G\n\x05Proof\x12\r\n\x05total\x18\x01 \x01(\x03\x12\r\n\x05index\x18\x02 \x01(\x03\x12\x11\n\tleaf_hash\x18\x03 \x01(\x0c\x12\r\n\x05\x61unts\x18\x04 \x03(\x0c\"?\n\x07ValueOp\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\'\n\x05proof\x18\x02 \x01(\x0b\x32\x18.tendermint.crypto.Proof\"6\n\x08\x44ominoOp\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05input\x18\x02 \x01(\t\x12\x0e\n\x06output\x18\x03 \x01(\t\"2\n\x07ProofOp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"9\n\x08ProofOps\x12-\n\x03ops\x18\x01 \x03(\x0b\x32\x1a.tendermint.crypto.ProofOpB\x04\xc8\xde\x1f\x00\x42:Z8github.com/tendermint/tendermint/proto/tendermint/cryptob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.plan.v2.plan_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.crypto.proof_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/sentinel-official/hub/x/plan/types\250\342\036\000\310\341\036\000'
-  _PLAN.fields_by_name['id']._options = None
-  _PLAN.fields_by_name['id']._serialized_options = b'\342\336\037\002ID'
-  _PLAN.fields_by_name['prices']._options = None
-  _PLAN.fields_by_name['prices']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
-  _PLAN.fields_by_name['validity']._options = None
-  _PLAN.fields_by_name['validity']._serialized_options = b'\310\336\037\000\230\337\037\001'
-  _PLAN.fields_by_name['bytes']._options = None
-  _PLAN.fields_by_name['bytes']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Int\310\336\037\000'
-  _PLAN.fields_by_name['status_at']._options = None
-  _PLAN.fields_by_name['status_at']._serialized_options = b'\310\336\037\000\220\337\037\001'
-  _PLAN._serialized_start=201
-  _PLAN._serialized_end=564
+  DESCRIPTOR._serialized_options = b'Z8github.com/tendermint/tendermint/proto/tendermint/crypto'
+  _PROOFOPS.fields_by_name['ops']._options = None
+  _PROOFOPS.fields_by_name['ops']._serialized_options = b'\310\336\037\000'
+  _PROOF._serialized_start=74
+  _PROOF._serialized_end=145
+  _VALUEOP._serialized_start=147
+  _VALUEOP._serialized_end=210
+  _DOMINOOP._serialized_start=212
+  _DOMINOOP._serialized_end=266
+  _PROOFOP._serialized_start=268
+  _PROOFOP._serialized_end=318
+  _PROOFOPS._serialized_start=320
+  _PROOFOPS._serialized_end=377
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/querier.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/querier.proto`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 syntax = "proto3";
-package sentinel.plan.v2;
+package sentinel.plan.v1;
 
 option go_package = "github.com/sentinel-official/hub/x/plan/types";
 
 import "cosmos/base/query/v1beta1/pagination.proto";
 import "gogoproto/gogo.proto";
 import "google/api/annotations.proto";
+import "sentinel/node/v1/node.proto";
+import "sentinel/plan/v1/plan.proto";
 import "sentinel/types/v1/status.proto";
-import "sentinel/plan/v2/plan.proto";
 
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 message QueryPlansRequest {
   sentinel.types.v1.Status status                  = 1;
   cosmos.base.query.v1beta1.PageRequest pagination = 2;
@@ -21,33 +22,48 @@
   string address                                   = 1;
   sentinel.types.v1.Status status                  = 2;
   cosmos.base.query.v1beta1.PageRequest pagination = 3;
 }
 
 message QueryPlanRequest { uint64 id = 1; }
 
+message QueryNodesForPlanRequest {
+  uint64 id                                        = 1;
+  cosmos.base.query.v1beta1.PageRequest pagination = 2;
+}
+
 message QueryPlansResponse {
   repeated Plan plans = 1 [ (gogoproto.nullable) = false ];
   cosmos.base.query.v1beta1.PageResponse pagination = 2;
 }
 
 message QueryPlansForProviderResponse {
   repeated Plan plans = 1 [ (gogoproto.nullable) = false ];
   cosmos.base.query.v1beta1.PageResponse pagination = 2;
 }
 
 message QueryPlanResponse { Plan plan = 1 [ (gogoproto.nullable) = false ]; }
 
+message QueryNodesForPlanResponse {
+  repeated sentinel.node.v1.Node nodes = 1 [ (gogoproto.nullable) = false ];
+  cosmos.base.query.v1beta1.PageResponse pagination = 2;
+}
+
 service QueryService {
   rpc QueryPlans(QueryPlansRequest) returns (QueryPlansResponse) {
     option (google.api.http).get = "/sentinel/plans";
   }
 
   rpc QueryPlansForProvider(QueryPlansForProviderRequest)
       returns (QueryPlansForProviderResponse) {
     option (google.api.http).get = "/sentinel/providers/{address}/plans";
   }
 
   rpc QueryPlan(QueryPlanRequest) returns (QueryPlanResponse) {
     option (google.api.http).get = "/sentinel/plans/{id}";
   }
+
+  rpc QueryNodesForPlan(QueryNodesForPlanRequest)
+      returns (QueryNodesForPlanResponse) {
+    option (google.api.http).get = "/sentinel/plans/{id}/nodes";
+  }
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/plan/v2/querier_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/wal_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-from cosmos.base.query.v1beta1 import pagination_pb2 as _pagination_pb2
 from gogoproto import gogo_pb2 as _gogo_pb2
-from google.api import annotations_pb2 as _annotations_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
-from sentinel.plan.v2 import plan_pb2 as _plan_pb2
-from google.protobuf.internal import containers as _containers
+from tendermint.consensus import types_pb2 as _types_pb2
+from tendermint.types import events_pb2 as _events_pb2
+from google.protobuf import duration_pb2 as _duration_pb2
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class QueryPlanRequest(_message.Message):
-    __slots__ = ["id"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    def __init__(self, id: _Optional[int] = ...) -> None: ...
-
-class QueryPlanResponse(_message.Message):
-    __slots__ = ["plan"]
-    PLAN_FIELD_NUMBER: _ClassVar[int]
-    plan: _plan_pb2.Plan
-    def __init__(self, plan: _Optional[_Union[_plan_pb2.Plan, _Mapping]] = ...) -> None: ...
-
-class QueryPlansForProviderRequest(_message.Message):
-    __slots__ = ["address", "pagination", "status"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    PAGINATION_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    pagination: _pagination_pb2.PageRequest
-    status: _status_pb2.Status
-    def __init__(self, address: _Optional[str] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ..., pagination: _Optional[_Union[_pagination_pb2.PageRequest, _Mapping]] = ...) -> None: ...
-
-class QueryPlansForProviderResponse(_message.Message):
-    __slots__ = ["pagination", "plans"]
-    PAGINATION_FIELD_NUMBER: _ClassVar[int]
-    PLANS_FIELD_NUMBER: _ClassVar[int]
-    pagination: _pagination_pb2.PageResponse
-    plans: _containers.RepeatedCompositeFieldContainer[_plan_pb2.Plan]
-    def __init__(self, plans: _Optional[_Iterable[_Union[_plan_pb2.Plan, _Mapping]]] = ..., pagination: _Optional[_Union[_pagination_pb2.PageResponse, _Mapping]] = ...) -> None: ...
-
-class QueryPlansRequest(_message.Message):
-    __slots__ = ["pagination", "status"]
-    PAGINATION_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    pagination: _pagination_pb2.PageRequest
-    status: _status_pb2.Status
-    def __init__(self, status: _Optional[_Union[_status_pb2.Status, str]] = ..., pagination: _Optional[_Union[_pagination_pb2.PageRequest, _Mapping]] = ...) -> None: ...
-
-class QueryPlansResponse(_message.Message):
-    __slots__ = ["pagination", "plans"]
-    PAGINATION_FIELD_NUMBER: _ClassVar[int]
-    PLANS_FIELD_NUMBER: _ClassVar[int]
-    pagination: _pagination_pb2.PageResponse
-    plans: _containers.RepeatedCompositeFieldContainer[_plan_pb2.Plan]
-    def __init__(self, plans: _Optional[_Iterable[_Union[_plan_pb2.Plan, _Mapping]]] = ..., pagination: _Optional[_Union[_pagination_pb2.PageResponse, _Mapping]] = ...) -> None: ...
+class EndHeight(_message.Message):
+    __slots__ = ["height"]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    height: int
+    def __init__(self, height: _Optional[int] = ...) -> None: ...
+
+class MsgInfo(_message.Message):
+    __slots__ = ["msg", "peer_id"]
+    MSG_FIELD_NUMBER: _ClassVar[int]
+    PEER_ID_FIELD_NUMBER: _ClassVar[int]
+    msg: _types_pb2.Message
+    peer_id: str
+    def __init__(self, msg: _Optional[_Union[_types_pb2.Message, _Mapping]] = ..., peer_id: _Optional[str] = ...) -> None: ...
+
+class TimedWALMessage(_message.Message):
+    __slots__ = ["msg", "time"]
+    MSG_FIELD_NUMBER: _ClassVar[int]
+    TIME_FIELD_NUMBER: _ClassVar[int]
+    msg: WALMessage
+    time: _timestamp_pb2.Timestamp
+    def __init__(self, time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., msg: _Optional[_Union[WALMessage, _Mapping]] = ...) -> None: ...
+
+class TimeoutInfo(_message.Message):
+    __slots__ = ["duration", "height", "round", "step"]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    ROUND_FIELD_NUMBER: _ClassVar[int]
+    STEP_FIELD_NUMBER: _ClassVar[int]
+    duration: _duration_pb2.Duration
+    height: int
+    round: int
+    step: int
+    def __init__(self, duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., height: _Optional[int] = ..., round: _Optional[int] = ..., step: _Optional[int] = ...) -> None: ...
+
+class WALMessage(_message.Message):
+    __slots__ = ["end_height", "event_data_round_state", "msg_info", "timeout_info"]
+    END_HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    EVENT_DATA_ROUND_STATE_FIELD_NUMBER: _ClassVar[int]
+    MSG_INFO_FIELD_NUMBER: _ClassVar[int]
+    TIMEOUT_INFO_FIELD_NUMBER: _ClassVar[int]
+    end_height: EndHeight
+    event_data_round_state: _events_pb2.EventDataRoundState
+    msg_info: MsgInfo
+    timeout_info: TimeoutInfo
+    def __init__(self, event_data_round_state: _Optional[_Union[_events_pb2.EventDataRoundState, _Mapping]] = ..., msg_info: _Optional[_Union[MsgInfo, _Mapping]] = ..., timeout_info: _Optional[_Union[TimeoutInfo, _Mapping]] = ..., end_height: _Optional[_Union[EndHeight, _Mapping]] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v1/provider_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/querier_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/provider/v1/provider.proto
+# source: sentinel/vpn/v1/querier.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#sentinel/provider/v1/provider.proto\x12\x14sentinel.provider.v1\x1a\x14gogoproto/gogo.proto\"a\n\x08Provider\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08identity\x18\x03 \x01(\t\x12\x0f\n\x07website\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\tBEZ;github.com/sentinel-official/hub/x/provider/legacy/v1/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dsentinel/vpn/v1/querier.proto\x12\x0fsentinel.vpn.v1B.Z,github.com/sentinel-official/hub/x/vpn/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.provider.v1.provider_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.vpn.v1.querier_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z;github.com/sentinel-official/hub/x/provider/legacy/v1/types\250\342\036\000\310\341\036\000'
-  _PROVIDER._serialized_start=83
-  _PROVIDER._serialized_end=180
+  DESCRIPTOR._serialized_options = b'Z,github.com/sentinel-official/hub/x/vpn/types'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v1/provider_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/events_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-from gogoproto import gogo_pb2 as _gogo_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Provider(_message.Message):
-    __slots__ = ["address", "description", "identity", "name", "website"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    IDENTITY_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    WEBSITE_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    description: str
-    identity: str
-    name: str
-    website: str
-    def __init__(self, address: _Optional[str] = ..., name: _Optional[str] = ..., identity: _Optional[str] = ..., website: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
+class EventDataRoundState(_message.Message):
+    __slots__ = ["height", "round", "step"]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    ROUND_FIELD_NUMBER: _ClassVar[int]
+    STEP_FIELD_NUMBER: _ClassVar[int]
+    height: int
+    round: int
+    step: str
+    def __init__(self, height: _Optional[int] = ..., round: _Optional[int] = ..., step: _Optional[str] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/msg.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/msg.proto`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 syntax = "proto3";
-package sentinel.provider.v2;
+package sentinel.provider.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/provider/types";
 
 import "gogoproto/gogo.proto";
-import "sentinel/types/v1/status.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/provider/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 // MsgRegisterRequest defines the SDK message for registering a provider
 message MsgRegisterRequest {
   string from        = 1;
   string name        = 2;
   string identity    = 3;
   string website     = 4;
   string description = 5;
 }
 
 // MsgUpdateRequest defines the SDK message for updating a provider
 message MsgUpdateRequest {
-  string from                     = 1;
-  string name                     = 2;
-  string identity                 = 3;
-  string website                  = 4;
-  string description              = 5;
-  sentinel.types.v1.Status status = 6;
+  string from        = 1;
+  string name        = 2;
+  string identity    = 3;
+  string website     = 4;
+  string description = 5;
 }
 
 // MsgRegisterResponse defines the response of message MsgRegisterRequest
 message MsgRegisterResponse {}
 
 // MsgUpdateResponse defines the response of message MsgUpdateRequest
 message MsgUpdateResponse {}
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/msg_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/blockchain/types_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,50 @@
-from gogoproto import gogo_pb2 as _gogo_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
+from tendermint.types import block_pb2 as _block_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class MsgRegisterRequest(_message.Message):
-    __slots__ = ["description", "identity", "name", "website"]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    IDENTITY_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    WEBSITE_FIELD_NUMBER: _ClassVar[int]
-    description: str
-    identity: str
-    name: str
-    website: str
-    def __init__(self, name: _Optional[str] = ..., identity: _Optional[str] = ..., website: _Optional[str] = ..., description: _Optional[str] = ..., **kwargs) -> None: ...
+class BlockRequest(_message.Message):
+    __slots__ = ["height"]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    height: int
+    def __init__(self, height: _Optional[int] = ...) -> None: ...
 
-class MsgRegisterResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+class BlockResponse(_message.Message):
+    __slots__ = ["block"]
+    BLOCK_FIELD_NUMBER: _ClassVar[int]
+    block: _block_pb2.Block
+    def __init__(self, block: _Optional[_Union[_block_pb2.Block, _Mapping]] = ...) -> None: ...
 
-class MsgUpdateRequest(_message.Message):
-    __slots__ = ["description", "identity", "name", "status", "website"]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    IDENTITY_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    WEBSITE_FIELD_NUMBER: _ClassVar[int]
-    description: str
-    identity: str
-    name: str
-    status: _status_pb2.Status
-    website: str
-    def __init__(self, name: _Optional[str] = ..., identity: _Optional[str] = ..., website: _Optional[str] = ..., description: _Optional[str] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ..., **kwargs) -> None: ...
+class Message(_message.Message):
+    __slots__ = ["block_request", "block_response", "no_block_response", "status_request", "status_response"]
+    BLOCK_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    BLOCK_RESPONSE_FIELD_NUMBER: _ClassVar[int]
+    NO_BLOCK_RESPONSE_FIELD_NUMBER: _ClassVar[int]
+    STATUS_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    STATUS_RESPONSE_FIELD_NUMBER: _ClassVar[int]
+    block_request: BlockRequest
+    block_response: BlockResponse
+    no_block_response: NoBlockResponse
+    status_request: StatusRequest
+    status_response: StatusResponse
+    def __init__(self, block_request: _Optional[_Union[BlockRequest, _Mapping]] = ..., no_block_response: _Optional[_Union[NoBlockResponse, _Mapping]] = ..., block_response: _Optional[_Union[BlockResponse, _Mapping]] = ..., status_request: _Optional[_Union[StatusRequest, _Mapping]] = ..., status_response: _Optional[_Union[StatusResponse, _Mapping]] = ...) -> None: ...
 
-class MsgUpdateResponse(_message.Message):
+class NoBlockResponse(_message.Message):
+    __slots__ = ["height"]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    height: int
+    def __init__(self, height: _Optional[int] = ...) -> None: ...
+
+class StatusRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
+
+class StatusResponse(_message.Message):
+    __slots__ = ["base", "height"]
+    BASE_FIELD_NUMBER: _ClassVar[int]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    base: int
+    height: int
+    def __init__(self, height: _Optional[int] = ..., base: _Optional[int] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/params.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/params.proto`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 syntax = "proto3";
-package sentinel.provider.v2;
+package sentinel.provider.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/provider/types";
 
 import "gogoproto/gogo.proto";
 import "cosmos/base/v1beta1/coin.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/provider/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 message Params {
   cosmos.base.v1beta1.Coin deposit = 1 [ (gogoproto.nullable) = false ];
-  string revenue_share             = 2 [
+  string staking_share             = 2 [
     (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Dec",
     (gogoproto.nullable)   = false
   ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/provider.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/quota.proto`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 syntax = "proto3";
-package sentinel.provider.v2;
+package sentinel.subscription.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/subscription/types";
 
 import "gogoproto/gogo.proto";
-import "google/protobuf/timestamp.proto";
-import "sentinel/types/v1/status.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/provider/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message Provider {
-  string address                      = 1;
-  string name                         = 2;
-  string identity                     = 3;
-  string website                      = 4;
-  string description                  = 5;
-  sentinel.types.v1.Status status     = 6;
-  google.protobuf.Timestamp status_at = 7
-      [ (gogoproto.nullable) = false, (gogoproto.stdtime) = true ];
+message Quota {
+  string address   = 1;
+  string allocated = 2 [
+    (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
+    (gogoproto.nullable)   = false
+  ];
+  string consumed = 3 [
+    (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
+    (gogoproto.nullable)   = false
+  ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/querier.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/provider/v1/querier.proto`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 syntax = "proto3";
-package sentinel.provider.v2;
+package sentinel.provider.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/provider/types";
 
 import "cosmos/base/query/v1beta1/pagination.proto";
 import "gogoproto/gogo.proto";
 import "google/api/annotations.proto";
-import "sentinel/types/v1/status.proto";
-import "sentinel/provider/v2/params.proto";
-import "sentinel/provider/v2/provider.proto";
+import "sentinel/provider/v1/provider.proto";
+import "sentinel/provider/v1/params.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/provider/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 message QueryProvidersRequest {
   cosmos.base.query.v1beta1.PageRequest pagination = 1;
-  sentinel.types.v1.Status status                  = 2;
 }
 
 message QueryProviderRequest { string address = 1; }
 
 message QueryParamsRequest {}
 
 message QueryProvidersResponse {
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/provider/v2/querier_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/params_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,60 @@
-from cosmos.base.query.v1beta1 import pagination_pb2 as _pagination_pb2
 from gogoproto import gogo_pb2 as _gogo_pb2
-from google.api import annotations_pb2 as _annotations_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
-from sentinel.provider.v2 import params_pb2 as _params_pb2
-from sentinel.provider.v2 import provider_pb2 as _provider_pb2
+from google.protobuf import duration_pb2 as _duration_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class QueryParamsRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class QueryParamsResponse(_message.Message):
-    __slots__ = ["params"]
-    PARAMS_FIELD_NUMBER: _ClassVar[int]
-    params: _params_pb2.Params
-    def __init__(self, params: _Optional[_Union[_params_pb2.Params, _Mapping]] = ...) -> None: ...
-
-class QueryProviderRequest(_message.Message):
-    __slots__ = ["address"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    def __init__(self, address: _Optional[str] = ...) -> None: ...
-
-class QueryProviderResponse(_message.Message):
-    __slots__ = ["provider"]
-    PROVIDER_FIELD_NUMBER: _ClassVar[int]
-    provider: _provider_pb2.Provider
-    def __init__(self, provider: _Optional[_Union[_provider_pb2.Provider, _Mapping]] = ...) -> None: ...
-
-class QueryProvidersRequest(_message.Message):
-    __slots__ = ["pagination", "status"]
-    PAGINATION_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    pagination: _pagination_pb2.PageRequest
-    status: _status_pb2.Status
-    def __init__(self, pagination: _Optional[_Union[_pagination_pb2.PageRequest, _Mapping]] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ...) -> None: ...
-
-class QueryProvidersResponse(_message.Message):
-    __slots__ = ["pagination", "providers"]
-    PAGINATION_FIELD_NUMBER: _ClassVar[int]
-    PROVIDERS_FIELD_NUMBER: _ClassVar[int]
-    pagination: _pagination_pb2.PageResponse
-    providers: _containers.RepeatedCompositeFieldContainer[_provider_pb2.Provider]
-    def __init__(self, providers: _Optional[_Iterable[_Union[_provider_pb2.Provider, _Mapping]]] = ..., pagination: _Optional[_Union[_pagination_pb2.PageResponse, _Mapping]] = ...) -> None: ...
+class BlockParams(_message.Message):
+    __slots__ = ["max_bytes", "max_gas", "time_iota_ms"]
+    MAX_BYTES_FIELD_NUMBER: _ClassVar[int]
+    MAX_GAS_FIELD_NUMBER: _ClassVar[int]
+    TIME_IOTA_MS_FIELD_NUMBER: _ClassVar[int]
+    max_bytes: int
+    max_gas: int
+    time_iota_ms: int
+    def __init__(self, max_bytes: _Optional[int] = ..., max_gas: _Optional[int] = ..., time_iota_ms: _Optional[int] = ...) -> None: ...
+
+class ConsensusParams(_message.Message):
+    __slots__ = ["block", "evidence", "validator", "version"]
+    BLOCK_FIELD_NUMBER: _ClassVar[int]
+    EVIDENCE_FIELD_NUMBER: _ClassVar[int]
+    VALIDATOR_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    block: BlockParams
+    evidence: EvidenceParams
+    validator: ValidatorParams
+    version: VersionParams
+    def __init__(self, block: _Optional[_Union[BlockParams, _Mapping]] = ..., evidence: _Optional[_Union[EvidenceParams, _Mapping]] = ..., validator: _Optional[_Union[ValidatorParams, _Mapping]] = ..., version: _Optional[_Union[VersionParams, _Mapping]] = ...) -> None: ...
+
+class EvidenceParams(_message.Message):
+    __slots__ = ["max_age_duration", "max_age_num_blocks", "max_bytes"]
+    MAX_AGE_DURATION_FIELD_NUMBER: _ClassVar[int]
+    MAX_AGE_NUM_BLOCKS_FIELD_NUMBER: _ClassVar[int]
+    MAX_BYTES_FIELD_NUMBER: _ClassVar[int]
+    max_age_duration: _duration_pb2.Duration
+    max_age_num_blocks: int
+    max_bytes: int
+    def __init__(self, max_age_num_blocks: _Optional[int] = ..., max_age_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., max_bytes: _Optional[int] = ...) -> None: ...
+
+class HashedParams(_message.Message):
+    __slots__ = ["block_max_bytes", "block_max_gas"]
+    BLOCK_MAX_BYTES_FIELD_NUMBER: _ClassVar[int]
+    BLOCK_MAX_GAS_FIELD_NUMBER: _ClassVar[int]
+    block_max_bytes: int
+    block_max_gas: int
+    def __init__(self, block_max_bytes: _Optional[int] = ..., block_max_gas: _Optional[int] = ...) -> None: ...
+
+class ValidatorParams(_message.Message):
+    __slots__ = ["pub_key_types"]
+    PUB_KEY_TYPES_FIELD_NUMBER: _ClassVar[int]
+    pub_key_types: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, pub_key_types: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class VersionParams(_message.Message):
+    __slots__ = ["app_version"]
+    APP_VERSION_FIELD_NUMBER: _ClassVar[int]
+    app_version: int
+    def __init__(self, app_version: _Optional[int] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v1/session.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/genesis.proto`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 syntax = "proto3";
-package sentinel.session.v1;
+package sentinel.subscription.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/subscription/types";
 
 import "gogoproto/gogo.proto";
-import "google/protobuf/duration.proto";
-import "google/protobuf/timestamp.proto";
-import "sentinel/types/v1/bandwidth.proto";
-import "sentinel/types/v1/status.proto";
+import "sentinel/subscription/v1/params.proto";
+import "sentinel/subscription/v1/quota.proto";
+import "sentinel/subscription/v1/subscription.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/session/legacy/v1/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message Session {
-  uint64 id                         = 1;
-  uint64 subscription               = 2;
-  string node                       = 3;
-  string address                    = 4;
-  google.protobuf.Duration duration = 5
-      [ (gogoproto.stdduration) = true, (gogoproto.nullable) = false ];
-  sentinel.types.v1.Bandwidth bandwidth = 6 [ (gogoproto.nullable) = false ];
-  sentinel.types.v1.Status status       = 7;
-  google.protobuf.Timestamp status_at   = 8
-      [ (gogoproto.nullable) = false, (gogoproto.stdtime) = true ];
+message GenesisSubscription {
+  Subscription subscription = 1
+      [ (gogoproto.jsontag) = "_", (gogoproto.nullable) = false ];
+  repeated Quota quotas = 2 [ (gogoproto.nullable) = false ];
+}
+
+message GenesisState {
+  repeated GenesisSubscription subscriptions = 1
+      [ (gogoproto.jsontag) = "_,omitempty", (gogoproto.nullable) = false ];
+  Params params = 2 [ (gogoproto.nullable) = false ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v1/session_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/wal_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/session/v1/session.proto
+# source: tendermint/consensus/wal.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
+from tendermint.consensus import types_pb2 as tendermint_dot_consensus_dot_types__pb2
+from tendermint.types import events_pb2 as tendermint_dot_types_dot_events__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from sentinel.types.v1 import bandwidth_pb2 as sentinel_dot_types_dot_v1_dot_bandwidth__pb2
-from sentinel.types.v1 import status_pb2 as sentinel_dot_types_dot_v1_dot_status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!sentinel/session/v1/session.proto\x12\x13sentinel.session.v1\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a!sentinel/types/v1/bandwidth.proto\x1a\x1esentinel/types/v1/status.proto\"\x9c\x02\n\x07Session\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x14\n\x0csubscription\x18\x02 \x01(\x04\x12\x0c\n\x04node\x18\x03 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12\x35\n\x08\x64uration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\x98\xdf\x1f\x01\xc8\xde\x1f\x00\x12\x35\n\tbandwidth\x18\x06 \x01(\x0b\x32\x1c.sentinel.types.v1.BandwidthB\x04\xc8\xde\x1f\x00\x12)\n\x06status\x18\x07 \x01(\x0e\x32\x19.sentinel.types.v1.Status\x12\x37\n\tstatus_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x42\x44Z:github.com/sentinel-official/hub/x/session/legacy/v1/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1etendermint/consensus/wal.proto\x12\x14tendermint.consensus\x1a\x14gogoproto/gogo.proto\x1a tendermint/consensus/types.proto\x1a\x1dtendermint/types/events.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"X\n\x07MsgInfo\x12\x30\n\x03msg\x18\x01 \x01(\x0b\x32\x1d.tendermint.consensus.MessageB\x04\xc8\xde\x1f\x00\x12\x1b\n\x07peer_id\x18\x02 \x01(\tB\n\xe2\xde\x1f\x06PeerID\"q\n\x0bTimeoutInfo\x12\x35\n\x08\x64uration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xc8\xde\x1f\x00\x98\xdf\x1f\x01\x12\x0e\n\x06height\x18\x02 \x01(\x03\x12\r\n\x05round\x18\x03 \x01(\x05\x12\x0c\n\x04step\x18\x04 \x01(\r\"\x1b\n\tEndHeight\x12\x0e\n\x06height\x18\x01 \x01(\x03\"\x81\x02\n\nWALMessage\x12G\n\x16\x65vent_data_round_state\x18\x01 \x01(\x0b\x32%.tendermint.types.EventDataRoundStateH\x00\x12\x31\n\x08msg_info\x18\x02 \x01(\x0b\x32\x1d.tendermint.consensus.MsgInfoH\x00\x12\x39\n\x0ctimeout_info\x18\x03 \x01(\x0b\x32!.tendermint.consensus.TimeoutInfoH\x00\x12\x35\n\nend_height\x18\x04 \x01(\x0b\x32\x1f.tendermint.consensus.EndHeightH\x00\x42\x05\n\x03sum\"t\n\x0fTimedWALMessage\x12\x32\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x12-\n\x03msg\x18\x02 \x01(\x0b\x32 .tendermint.consensus.WALMessageB=Z;github.com/tendermint/tendermint/proto/tendermint/consensusb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.session.v1.session_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.consensus.wal_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z:github.com/sentinel-official/hub/x/session/legacy/v1/types\250\342\036\000\310\341\036\000'
-  _SESSION.fields_by_name['duration']._options = None
-  _SESSION.fields_by_name['duration']._serialized_options = b'\230\337\037\001\310\336\037\000'
-  _SESSION.fields_by_name['bandwidth']._options = None
-  _SESSION.fields_by_name['bandwidth']._serialized_options = b'\310\336\037\000'
-  _SESSION.fields_by_name['status_at']._options = None
-  _SESSION.fields_by_name['status_at']._serialized_options = b'\310\336\037\000\220\337\037\001'
-  _SESSION._serialized_start=213
-  _SESSION._serialized_end=497
+  DESCRIPTOR._serialized_options = b'Z;github.com/tendermint/tendermint/proto/tendermint/consensus'
+  _MSGINFO.fields_by_name['msg']._options = None
+  _MSGINFO.fields_by_name['msg']._serialized_options = b'\310\336\037\000'
+  _MSGINFO.fields_by_name['peer_id']._options = None
+  _MSGINFO.fields_by_name['peer_id']._serialized_options = b'\342\336\037\006PeerID'
+  _TIMEOUTINFO.fields_by_name['duration']._options = None
+  _TIMEOUTINFO.fields_by_name['duration']._serialized_options = b'\310\336\037\000\230\337\037\001'
+  _TIMEDWALMESSAGE.fields_by_name['time']._options = None
+  _TIMEDWALMESSAGE.fields_by_name['time']._serialized_options = b'\310\336\037\000\220\337\037\001'
+  _MSGINFO._serialized_start=208
+  _MSGINFO._serialized_end=296
+  _TIMEOUTINFO._serialized_start=298
+  _TIMEOUTINFO._serialized_end=411
+  _ENDHEIGHT._serialized_start=413
+  _ENDHEIGHT._serialized_end=440
+  _WALMESSAGE._serialized_start=443
+  _WALMESSAGE._serialized_end=700
+  _TIMEDWALMESSAGE._serialized_start=702
+  _TIMEDWALMESSAGE._serialized_end=818
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/events.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/events.proto`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 syntax = "proto3";
-package sentinel.session.v2;
+package sentinel.subscription.v1;
 
-import "cosmos/base/v1beta1/coin.proto";
 import "gogoproto/gogo.proto";
 import "sentinel/types/v1/status.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/session/types";
+option go_package = "github.com/sentinel-official/hub/x/subscription/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message EventStart {
-  uint64 id           = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
-  string node         = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
-  uint64 subscription = 3 [ (gogoproto.moretags) = "yaml:\"subscription\"" ];
-}
-
-message EventUpdate {
-  uint64 id           = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
-  string node         = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
-  uint64 subscription = 3 [ (gogoproto.moretags) = "yaml:\"subscription\"" ];
+message EventSubscribe {
+  uint64 id   = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
+  string node = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
+  uint64 plan = 3 [ (gogoproto.moretags) = "yaml:\"plan\"" ];
 }
 
 message EventSetStatus {
-  uint64 id           = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
-  string node         = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
-  uint64 subscription = 3 [ (gogoproto.moretags) = "yaml:\"subscription\"" ];
-  sentinel.types.v1.Status status = 4
+  uint64 id                       = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
+  sentinel.types.v1.Status status = 2
       [ (gogoproto.moretags) = "yaml:\"status\"" ];
 }
 
-message EventPay {
-  uint64 id           = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
-  string node         = 2 [ (gogoproto.moretags) = "yaml:\"node\"" ];
-  uint64 subscription = 3 [ (gogoproto.moretags) = "yaml:\"subscription\"" ];
-  cosmos.base.v1beta1.Coin amount = 4 [
-    (gogoproto.moretags) = "yaml:\"amount\"",
-    (gogoproto.nullable) = false
-  ];
+message EventAddQuota {
+  uint64 id      = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
+  string address = 2 [ (gogoproto.moretags) = "yaml:\"address\"" ];
+}
+
+message EventUpdateQuota {
+  uint64 id      = 1 [ (gogoproto.moretags) = "yaml:\"id\"" ];
+  string address = 2 [ (gogoproto.moretags) = "yaml:\"address\"" ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/events_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/canonical_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,51 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/session/v2/events.proto
+# source: tendermint/types/canonical.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from sentinel.types.v1 import status_pb2 as sentinel_dot_types_dot_v1_dot_status__pb2
+from tendermint.types import types_pb2 as tendermint_dot_types_dot_types__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n sentinel/session/v2/events.proto\x12\x13sentinel.session.v2\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1esentinel/types/v1/status.proto\"u\n\nEventStart\x12\x19\n\x02id\x18\x01 \x01(\x04\x42\r\xf2\xde\x1f\tyaml:\"id\"\x12\x1d\n\x04node\x18\x02 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"node\"\x12-\n\x0csubscription\x18\x03 \x01(\x04\x42\x17\xf2\xde\x1f\x13yaml:\"subscription\"\"v\n\x0b\x45ventUpdate\x12\x19\n\x02id\x18\x01 \x01(\x04\x42\r\xf2\xde\x1f\tyaml:\"id\"\x12\x1d\n\x04node\x18\x02 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"node\"\x12-\n\x0csubscription\x18\x03 \x01(\x04\x42\x17\xf2\xde\x1f\x13yaml:\"subscription\"\"\xb7\x01\n\x0e\x45ventSetStatus\x12\x19\n\x02id\x18\x01 \x01(\x04\x42\r\xf2\xde\x1f\tyaml:\"id\"\x12\x1d\n\x04node\x18\x02 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"node\"\x12-\n\x0csubscription\x18\x03 \x01(\x04\x42\x17\xf2\xde\x1f\x13yaml:\"subscription\"\x12<\n\x06status\x18\x04 \x01(\x0e\x32\x19.sentinel.types.v1.StatusB\x11\xf2\xde\x1f\ryaml:\"status\"\"\xb5\x01\n\x08\x45ventPay\x12\x19\n\x02id\x18\x01 \x01(\x04\x42\r\xf2\xde\x1f\tyaml:\"id\"\x12\x1d\n\x04node\x18\x02 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"node\"\x12-\n\x0csubscription\x18\x03 \x01(\x04\x42\x17\xf2\xde\x1f\x13yaml:\"subscription\"\x12@\n\x06\x61mount\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x15\xf2\xde\x1f\ryaml:\"amount\"\xc8\xde\x1f\x00\x42:Z0github.com/sentinel-official/hub/x/session/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tendermint/types/canonical.proto\x12\x10tendermint.types\x1a\x14gogoproto/gogo.proto\x1a\x1ctendermint/types/types.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"i\n\x10\x43\x61nonicalBlockID\x12\x0c\n\x04hash\x18\x01 \x01(\x0c\x12G\n\x0fpart_set_header\x18\x02 \x01(\x0b\x32(.tendermint.types.CanonicalPartSetHeaderB\x04\xc8\xde\x1f\x00\"5\n\x16\x43\x61nonicalPartSetHeader\x12\r\n\x05total\x18\x01 \x01(\r\x12\x0c\n\x04hash\x18\x02 \x01(\x0c\"\x9d\x02\n\x11\x43\x61nonicalProposal\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.tendermint.types.SignedMsgType\x12\x0e\n\x06height\x18\x02 \x01(\x10\x12\r\n\x05round\x18\x03 \x01(\x10\x12\x1f\n\tpol_round\x18\x04 \x01(\x03\x42\x0c\xe2\xde\x1f\x08POLRound\x12\x41\n\x08\x62lock_id\x18\x05 \x01(\x0b\x32\".tendermint.types.CanonicalBlockIDB\x0b\xe2\xde\x1f\x07\x42lockID\x12\x37\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x12\x1d\n\x08\x63hain_id\x18\x07 \x01(\tB\x0b\xe2\xde\x1f\x07\x43hainID\"\xf8\x01\n\rCanonicalVote\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.tendermint.types.SignedMsgType\x12\x0e\n\x06height\x18\x02 \x01(\x10\x12\r\n\x05round\x18\x03 \x01(\x10\x12\x41\n\x08\x62lock_id\x18\x04 \x01(\x0b\x32\".tendermint.types.CanonicalBlockIDB\x0b\xe2\xde\x1f\x07\x42lockID\x12\x37\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x12\x1d\n\x08\x63hain_id\x18\x06 \x01(\tB\x0b\xe2\xde\x1f\x07\x43hainIDB9Z7github.com/tendermint/tendermint/proto/tendermint/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.session.v2.events_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.canonical_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z0github.com/sentinel-official/hub/x/session/types\250\342\036\000\310\341\036\000'
-  _EVENTSTART.fields_by_name['id']._options = None
-  _EVENTSTART.fields_by_name['id']._serialized_options = b'\362\336\037\tyaml:\"id\"'
-  _EVENTSTART.fields_by_name['node']._options = None
-  _EVENTSTART.fields_by_name['node']._serialized_options = b'\362\336\037\013yaml:\"node\"'
-  _EVENTSTART.fields_by_name['subscription']._options = None
-  _EVENTSTART.fields_by_name['subscription']._serialized_options = b'\362\336\037\023yaml:\"subscription\"'
-  _EVENTUPDATE.fields_by_name['id']._options = None
-  _EVENTUPDATE.fields_by_name['id']._serialized_options = b'\362\336\037\tyaml:\"id\"'
-  _EVENTUPDATE.fields_by_name['node']._options = None
-  _EVENTUPDATE.fields_by_name['node']._serialized_options = b'\362\336\037\013yaml:\"node\"'
-  _EVENTUPDATE.fields_by_name['subscription']._options = None
-  _EVENTUPDATE.fields_by_name['subscription']._serialized_options = b'\362\336\037\023yaml:\"subscription\"'
-  _EVENTSETSTATUS.fields_by_name['id']._options = None
-  _EVENTSETSTATUS.fields_by_name['id']._serialized_options = b'\362\336\037\tyaml:\"id\"'
-  _EVENTSETSTATUS.fields_by_name['node']._options = None
-  _EVENTSETSTATUS.fields_by_name['node']._serialized_options = b'\362\336\037\013yaml:\"node\"'
-  _EVENTSETSTATUS.fields_by_name['subscription']._options = None
-  _EVENTSETSTATUS.fields_by_name['subscription']._serialized_options = b'\362\336\037\023yaml:\"subscription\"'
-  _EVENTSETSTATUS.fields_by_name['status']._options = None
-  _EVENTSETSTATUS.fields_by_name['status']._serialized_options = b'\362\336\037\ryaml:\"status\"'
-  _EVENTPAY.fields_by_name['id']._options = None
-  _EVENTPAY.fields_by_name['id']._serialized_options = b'\362\336\037\tyaml:\"id\"'
-  _EVENTPAY.fields_by_name['node']._options = None
-  _EVENTPAY.fields_by_name['node']._serialized_options = b'\362\336\037\013yaml:\"node\"'
-  _EVENTPAY.fields_by_name['subscription']._options = None
-  _EVENTPAY.fields_by_name['subscription']._serialized_options = b'\362\336\037\023yaml:\"subscription\"'
-  _EVENTPAY.fields_by_name['amount']._options = None
-  _EVENTPAY.fields_by_name['amount']._serialized_options = b'\362\336\037\ryaml:\"amount\"\310\336\037\000'
-  _EVENTSTART._serialized_start=143
-  _EVENTSTART._serialized_end=260
-  _EVENTUPDATE._serialized_start=262
-  _EVENTUPDATE._serialized_end=380
-  _EVENTSETSTATUS._serialized_start=383
-  _EVENTSETSTATUS._serialized_end=566
-  _EVENTPAY._serialized_start=569
-  _EVENTPAY._serialized_end=750
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types'
+  _CANONICALBLOCKID.fields_by_name['part_set_header']._options = None
+  _CANONICALBLOCKID.fields_by_name['part_set_header']._serialized_options = b'\310\336\037\000'
+  _CANONICALPROPOSAL.fields_by_name['pol_round']._options = None
+  _CANONICALPROPOSAL.fields_by_name['pol_round']._serialized_options = b'\342\336\037\010POLRound'
+  _CANONICALPROPOSAL.fields_by_name['block_id']._options = None
+  _CANONICALPROPOSAL.fields_by_name['block_id']._serialized_options = b'\342\336\037\007BlockID'
+  _CANONICALPROPOSAL.fields_by_name['timestamp']._options = None
+  _CANONICALPROPOSAL.fields_by_name['timestamp']._serialized_options = b'\310\336\037\000\220\337\037\001'
+  _CANONICALPROPOSAL.fields_by_name['chain_id']._options = None
+  _CANONICALPROPOSAL.fields_by_name['chain_id']._serialized_options = b'\342\336\037\007ChainID'
+  _CANONICALVOTE.fields_by_name['block_id']._options = None
+  _CANONICALVOTE.fields_by_name['block_id']._serialized_options = b'\342\336\037\007BlockID'
+  _CANONICALVOTE.fields_by_name['timestamp']._options = None
+  _CANONICALVOTE.fields_by_name['timestamp']._serialized_options = b'\310\336\037\000\220\337\037\001'
+  _CANONICALVOTE.fields_by_name['chain_id']._options = None
+  _CANONICALVOTE.fields_by_name['chain_id']._serialized_options = b'\342\336\037\007ChainID'
+  _CANONICALBLOCKID._serialized_start=139
+  _CANONICALBLOCKID._serialized_end=244
+  _CANONICALPARTSETHEADER._serialized_start=246
+  _CANONICALPARTSETHEADER._serialized_end=299
+  _CANONICALPROPOSAL._serialized_start=302
+  _CANONICALPROPOSAL._serialized_end=587
+  _CANONICALVOTE._serialized_start=590
+  _CANONICALVOTE._serialized_end=838
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/events_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/statesync/types_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-from cosmos.base.v1beta1 import coin_pb2 as _coin_pb2
-from gogoproto import gogo_pb2 as _gogo_pb2
-from sentinel.types.v1 import status_pb2 as _status_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class EventPay(_message.Message):
-    __slots__ = ["amount", "id", "node", "subscription"]
-    AMOUNT_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    NODE_FIELD_NUMBER: _ClassVar[int]
-    SUBSCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    amount: _coin_pb2.Coin
-    id: int
-    node: str
-    subscription: int
-    def __init__(self, id: _Optional[int] = ..., node: _Optional[str] = ..., subscription: _Optional[int] = ..., amount: _Optional[_Union[_coin_pb2.Coin, _Mapping]] = ...) -> None: ...
-
-class EventSetStatus(_message.Message):
-    __slots__ = ["id", "node", "status", "subscription"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    NODE_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    SUBSCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    node: str
-    status: _status_pb2.Status
-    subscription: int
-    def __init__(self, id: _Optional[int] = ..., node: _Optional[str] = ..., subscription: _Optional[int] = ..., status: _Optional[_Union[_status_pb2.Status, str]] = ...) -> None: ...
-
-class EventStart(_message.Message):
-    __slots__ = ["id", "node", "subscription"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    NODE_FIELD_NUMBER: _ClassVar[int]
-    SUBSCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    node: str
-    subscription: int
-    def __init__(self, id: _Optional[int] = ..., node: _Optional[str] = ..., subscription: _Optional[int] = ...) -> None: ...
-
-class EventUpdate(_message.Message):
-    __slots__ = ["id", "node", "subscription"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    NODE_FIELD_NUMBER: _ClassVar[int]
-    SUBSCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    node: str
-    subscription: int
-    def __init__(self, id: _Optional[int] = ..., node: _Optional[str] = ..., subscription: _Optional[int] = ...) -> None: ...
+class ChunkRequest(_message.Message):
+    __slots__ = ["format", "height", "index"]
+    FORMAT_FIELD_NUMBER: _ClassVar[int]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    format: int
+    height: int
+    index: int
+    def __init__(self, height: _Optional[int] = ..., format: _Optional[int] = ..., index: _Optional[int] = ...) -> None: ...
+
+class ChunkResponse(_message.Message):
+    __slots__ = ["chunk", "format", "height", "index", "missing"]
+    CHUNK_FIELD_NUMBER: _ClassVar[int]
+    FORMAT_FIELD_NUMBER: _ClassVar[int]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    MISSING_FIELD_NUMBER: _ClassVar[int]
+    chunk: bytes
+    format: int
+    height: int
+    index: int
+    missing: bool
+    def __init__(self, height: _Optional[int] = ..., format: _Optional[int] = ..., index: _Optional[int] = ..., chunk: _Optional[bytes] = ..., missing: bool = ...) -> None: ...
+
+class Message(_message.Message):
+    __slots__ = ["chunk_request", "chunk_response", "snapshots_request", "snapshots_response"]
+    CHUNK_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    CHUNK_RESPONSE_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOTS_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOTS_RESPONSE_FIELD_NUMBER: _ClassVar[int]
+    chunk_request: ChunkRequest
+    chunk_response: ChunkResponse
+    snapshots_request: SnapshotsRequest
+    snapshots_response: SnapshotsResponse
+    def __init__(self, snapshots_request: _Optional[_Union[SnapshotsRequest, _Mapping]] = ..., snapshots_response: _Optional[_Union[SnapshotsResponse, _Mapping]] = ..., chunk_request: _Optional[_Union[ChunkRequest, _Mapping]] = ..., chunk_response: _Optional[_Union[ChunkResponse, _Mapping]] = ...) -> None: ...
+
+class SnapshotsRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class SnapshotsResponse(_message.Message):
+    __slots__ = ["chunks", "format", "hash", "height", "metadata"]
+    CHUNKS_FIELD_NUMBER: _ClassVar[int]
+    FORMAT_FIELD_NUMBER: _ClassVar[int]
+    HASH_FIELD_NUMBER: _ClassVar[int]
+    HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    chunks: int
+    format: int
+    hash: bytes
+    height: int
+    metadata: bytes
+    def __init__(self, height: _Optional[int] = ..., format: _Optional[int] = ..., chunks: _Optional[int] = ..., hash: _Optional[bytes] = ..., metadata: _Optional[bytes] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/msg.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/msg.proto`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 syntax = "proto3";
-package sentinel.session.v2;
+package sentinel.session.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/session/types";
 
 import "gogoproto/gogo.proto";
-import "sentinel/session/v2/proof.proto";
+import "sentinel/session/v1/proof.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/session/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 // MsgStartRequest defines the SDK message for starting a session
 message MsgStartRequest {
-  string from    = 1;
-  uint64 id      = 2 [ (gogoproto.customname) = "ID" ];
-  string address = 3;
+  string from = 1;
+  uint64 id   = 2;
+  string node = 3;
 }
 
-// MsgUpdateDetailsRequest defines the SDK message for updating a session
-message MsgUpdateDetailsRequest {
+// MsgUpdateRequest defines the SDK message for updating a session
+message MsgUpdateRequest {
   string from     = 1;
   Proof proof     = 2 [ (gogoproto.nullable) = false ];
   bytes signature = 3;
 }
 
 // MsgEndRequest defines the SDK message for ending a session
 message MsgEndRequest {
   string from   = 1;
-  uint64 id     = 2 [ (gogoproto.customname) = "ID" ];
+  uint64 id     = 2;
   uint64 rating = 3;
 }
 
 // MsgStartResponse defines the response of message MsgStartRequest
 message MsgStartResponse {}
 
-// MsgUpdateDetailsResponse defines the response of message
-// MsgUpdateDetailsRequest
-message MsgUpdateDetailsResponse {}
+// MsgUpdateResponse defines the response of message MsgUpdateRequest
+message MsgUpdateResponse {}
 
 // MsgEndResponse defines the response of message MsgEndRequest
 message MsgEndResponse {}
 
 service MsgService {
   rpc MsgStart(MsgStartRequest) returns (MsgStartResponse);
-  rpc MsgUpdateDetails(MsgUpdateDetailsRequest)
-      returns (MsgUpdateDetailsResponse);
+  rpc MsgUpdate(MsgUpdateRequest) returns (MsgUpdateResponse);
   rpc MsgEnd(MsgEndRequest) returns (MsgEndResponse);
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/msg_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/rpc/grpc/types_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,28 @@
-from gogoproto import gogo_pb2 as _gogo_pb2
-from sentinel.session.v2 import proof_pb2 as _proof_pb2
+from tendermint.abci import types_pb2 as _types_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class MsgEndRequest(_message.Message):
-    __slots__ = ["id", "rating"]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    RATING_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    rating: int
-    def __init__(self, id: _Optional[int] = ..., rating: _Optional[int] = ..., **kwargs) -> None: ...
+class RequestBroadcastTx(_message.Message):
+    __slots__ = ["tx"]
+    TX_FIELD_NUMBER: _ClassVar[int]
+    tx: bytes
+    def __init__(self, tx: _Optional[bytes] = ...) -> None: ...
 
-class MsgEndResponse(_message.Message):
+class RequestPing(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class MsgStartRequest(_message.Message):
-    __slots__ = ["address", "id"]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    address: str
-    id: int
-    def __init__(self, id: _Optional[int] = ..., address: _Optional[str] = ..., **kwargs) -> None: ...
+class ResponseBroadcastTx(_message.Message):
+    __slots__ = ["check_tx", "deliver_tx"]
+    CHECK_TX_FIELD_NUMBER: _ClassVar[int]
+    DELIVER_TX_FIELD_NUMBER: _ClassVar[int]
+    check_tx: _types_pb2.ResponseCheckTx
+    deliver_tx: _types_pb2.ResponseDeliverTx
+    def __init__(self, check_tx: _Optional[_Union[_types_pb2.ResponseCheckTx, _Mapping]] = ..., deliver_tx: _Optional[_Union[_types_pb2.ResponseDeliverTx, _Mapping]] = ...) -> None: ...
 
-class MsgStartResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MsgUpdateDetailsRequest(_message.Message):
-    __slots__ = ["proof", "signature"]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    PROOF_FIELD_NUMBER: _ClassVar[int]
-    SIGNATURE_FIELD_NUMBER: _ClassVar[int]
-    proof: _proof_pb2.Proof
-    signature: bytes
-    def __init__(self, proof: _Optional[_Union[_proof_pb2.Proof, _Mapping]] = ..., signature: _Optional[bytes] = ..., **kwargs) -> None: ...
-
-class MsgUpdateDetailsResponse(_message.Message):
+class ResponsePing(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/params_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/genesis_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/session/v2/params.proto
+# source: sentinel/deposit/v1/genesis.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n sentinel/session/v2/params.proto\x12\x13sentinel.session.v2\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\"l\n\x06Params\x12>\n\x11inactive_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xc8\xde\x1f\x00\x98\xdf\x1f\x01\x12\"\n\x1aproof_verification_enabled\x18\x02 \x01(\x08\x42:Z0github.com/sentinel-official/hub/x/session/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!sentinel/deposit/v1/genesis.proto\x12\x13sentinel.deposit.v1B2Z0github.com/sentinel-official/hub/x/deposit/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.session.v2.params_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.deposit.v1.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z0github.com/sentinel-official/hub/x/session/types\250\342\036\000\310\341\036\000'
-  _PARAMS.fields_by_name['inactive_duration']._options = None
-  _PARAMS.fields_by_name['inactive_duration']._serialized_options = b'\310\336\037\000\230\337\037\001'
-  _PARAMS._serialized_start=111
-  _PARAMS._serialized_end=219
+  DESCRIPTOR._serialized_options = b'Z0github.com/sentinel-official/hub/x/deposit/types'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/params_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/libs/bits/types_pb2.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from gogoproto import gogo_pb2 as _gogo_pb2
-from google.protobuf import duration_pb2 as _duration_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Params(_message.Message):
-    __slots__ = ["inactive_duration", "proof_verification_enabled"]
-    INACTIVE_DURATION_FIELD_NUMBER: _ClassVar[int]
-    PROOF_VERIFICATION_ENABLED_FIELD_NUMBER: _ClassVar[int]
-    inactive_duration: _duration_pb2.Duration
-    proof_verification_enabled: bool
-    def __init__(self, inactive_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., proof_verification_enabled: bool = ...) -> None: ...
+class BitArray(_message.Message):
+    __slots__ = ["bits", "elems"]
+    BITS_FIELD_NUMBER: _ClassVar[int]
+    ELEMS_FIELD_NUMBER: _ClassVar[int]
+    bits: int
+    elems: _containers.RepeatedScalarFieldContainer[int]
+    def __init__(self, bits: _Optional[int] = ..., elems: _Optional[_Iterable[int]] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/proof.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/genesis.proto`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 syntax = "proto3";
-package sentinel.session.v2;
+package sentinel.session.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/session/types";
 
 import "gogoproto/gogo.proto";
-import "google/protobuf/duration.proto";
-import "sentinel/types/v1/bandwidth.proto";
+import "sentinel/session/v1/params.proto";
+import "sentinel/session/v1/session.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/session/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message Proof {
-  uint64 id                         = 1 [ (gogoproto.customname) = "ID" ];
-  google.protobuf.Duration duration = 2
-      [ (gogoproto.stdduration) = true, (gogoproto.nullable) = false ];
-  sentinel.types.v1.Bandwidth bandwidth = 3 [ (gogoproto.nullable) = false ];
+message GenesisState {
+  repeated Session sessions = 1
+      [ (gogoproto.jsontag) = "_,omitempty", (gogoproto.nullable) = false ];
+  Params params = 2 [ (gogoproto.nullable) = false ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/proof_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/block_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/session/v2/proof.proto
+# source: tendermint/types/block.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
-from sentinel.types.v1 import bandwidth_pb2 as sentinel_dot_types_dot_v1_dot_bandwidth__pb2
+from tendermint.types import types_pb2 as tendermint_dot_types_dot_types__pb2
+from tendermint.types import evidence_pb2 as tendermint_dot_types_dot_evidence__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fsentinel/session/v2/proof.proto\x12\x13sentinel.session.v2\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a!sentinel/types/v1/bandwidth.proto\"\x89\x01\n\x05Proof\x12\x12\n\x02id\x18\x01 \x01(\x04\x42\x06\xe2\xde\x1f\x02ID\x12\x35\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\x98\xdf\x1f\x01\xc8\xde\x1f\x00\x12\x35\n\tbandwidth\x18\x03 \x01(\x0b\x32\x1c.sentinel.types.v1.BandwidthB\x04\xc8\xde\x1f\x00\x42:Z0github.com/sentinel-official/hub/x/session/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctendermint/types/block.proto\x12\x10tendermint.types\x1a\x14gogoproto/gogo.proto\x1a\x1ctendermint/types/types.proto\x1a\x1ftendermint/types/evidence.proto\"\xca\x01\n\x05\x42lock\x12.\n\x06header\x18\x01 \x01(\x0b\x32\x18.tendermint.types.HeaderB\x04\xc8\xde\x1f\x00\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.tendermint.types.DataB\x04\xc8\xde\x1f\x00\x12\x36\n\x08\x65vidence\x18\x03 \x01(\x0b\x32\x1e.tendermint.types.EvidenceListB\x04\xc8\xde\x1f\x00\x12-\n\x0blast_commit\x18\x04 \x01(\x0b\x32\x18.tendermint.types.CommitB9Z7github.com/tendermint/tendermint/proto/tendermint/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.session.v2.proof_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.block_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z0github.com/sentinel-official/hub/x/session/types\250\342\036\000\310\341\036\000'
-  _PROOF.fields_by_name['id']._options = None
-  _PROOF.fields_by_name['id']._serialized_options = b'\342\336\037\002ID'
-  _PROOF.fields_by_name['duration']._options = None
-  _PROOF.fields_by_name['duration']._serialized_options = b'\230\337\037\001\310\336\037\000'
-  _PROOF.fields_by_name['bandwidth']._options = None
-  _PROOF.fields_by_name['bandwidth']._serialized_options = b'\310\336\037\000'
-  _PROOF._serialized_start=146
-  _PROOF._serialized_end=283
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types'
+  _BLOCK.fields_by_name['header']._options = None
+  _BLOCK.fields_by_name['header']._serialized_options = b'\310\336\037\000'
+  _BLOCK.fields_by_name['data']._options = None
+  _BLOCK.fields_by_name['data']._serialized_options = b'\310\336\037\000'
+  _BLOCK.fields_by_name['evidence']._options = None
+  _BLOCK.fields_by_name['evidence']._serialized_options = b'\310\336\037\000'
+  _BLOCK._serialized_start=136
+  _BLOCK._serialized_end=338
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/querier.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/swap/v1/querier.proto`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,46 @@
 syntax = "proto3";
-package sentinel.session.v2;
+package sentinel.swap.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/swap/types";
 
 import "cosmos/base/query/v1beta1/pagination.proto";
 import "gogoproto/gogo.proto";
 import "google/api/annotations.proto";
-import "sentinel/session/v2/session.proto";
-import "sentinel/session/v2/params.proto";
+import "sentinel/swap/v1/swap.proto";
+import "sentinel/swap/v1/params.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/session/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message QuerySessionsRequest {
+message QuerySwapsRequest {
   cosmos.base.query.v1beta1.PageRequest pagination = 1;
 }
 
-message QuerySessionsForAccountRequest {
-  string address                                   = 1;
-  cosmos.base.query.v1beta1.PageRequest pagination = 2;
-}
-
-message QuerySessionsForNodeRequest {
-  string address                                   = 1;
-  cosmos.base.query.v1beta1.PageRequest pagination = 2;
-}
-
-message QuerySessionsForSubscriptionRequest {
-  uint64 id                                        = 1;
-  cosmos.base.query.v1beta1.PageRequest pagination = 2;
-}
-
-message QuerySessionRequest { uint64 id = 1; }
+message QuerySwapRequest { bytes tx_hash = 1; }
 
 message QueryParamsRequest {}
 
-message QuerySessionsResponse {
-  repeated Session sessions = 1 [ (gogoproto.nullable) = false ];
-  cosmos.base.query.v1beta1.PageResponse pagination = 2;
-}
-
-message QuerySessionsForAccountResponse {
-  repeated Session sessions = 1 [ (gogoproto.nullable) = false ];
+message QuerySwapsResponse {
+  repeated Swap swaps = 1 [ (gogoproto.nullable) = false ];
   cosmos.base.query.v1beta1.PageResponse pagination = 2;
 }
 
-message QuerySessionsForNodeResponse {
-  repeated Session sessions = 1 [ (gogoproto.nullable) = false ];
-  cosmos.base.query.v1beta1.PageResponse pagination = 2;
-}
-
-message QuerySessionsForSubscriptionResponse {
-  repeated Session sessions = 1 [ (gogoproto.nullable) = false ];
-  cosmos.base.query.v1beta1.PageResponse pagination = 2;
-}
-
-message QuerySessionResponse {
-  Session session = 1 [ (gogoproto.nullable) = false ];
-}
+message QuerySwapResponse { Swap swap = 1 [ (gogoproto.nullable) = false ]; }
 
 message QueryParamsResponse {
   Params params = 1 [ (gogoproto.nullable) = false ];
 }
 
 service QueryService {
-  rpc QuerySessions(QuerySessionsRequest) returns (QuerySessionsResponse) {
-    option (google.api.http).get = "/sentinel/sessions";
-  }
-
-  rpc QuerySessionsForAccount(QuerySessionsForAccountRequest)
-      returns (QuerySessionsForAccountResponse) {
-    option (google.api.http).get = "/sentinel/accounts/{address}/sessions";
-  }
-
-  rpc QuerySessionsForNode(QuerySessionsForNodeRequest)
-      returns (QuerySessionsForNodeResponse) {
-    option (google.api.http).get = "/sentinel/nodes/{address}/sessions";
-  }
-
-  rpc QuerySessionsForSubscription(QuerySessionsForSubscriptionRequest)
-      returns (QuerySessionsForSubscriptionResponse) {
-    option (google.api.http).get = "/sentinel/subscriptions/{id}/sessions";
+  rpc QuerySwaps(QuerySwapsRequest) returns (QuerySwapsResponse) {
+    option (google.api.http).get = "/sentinel/swaps";
   }
 
-  rpc QuerySession(QuerySessionRequest) returns (QuerySessionResponse) {
-    option (google.api.http).get = "/sentinel/sessions/{id}";
+  rpc QuerySwap(QuerySwapRequest) returns (QuerySwapResponse) {
+    option (google.api.http).get = "/sentinel/swaps/{tx_hash}";
   }
 
   rpc QueryParams(QueryParamsRequest) returns (QueryParamsResponse) {
-    option (google.api.http).get = "/sentinel/modules/session/params";
+    option (google.api.http).get = "/sentinel/modules/swap/params";
   }
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/session.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/session/v1/proof.proto`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 syntax = "proto3";
-package sentinel.session.v2;
+package sentinel.session.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/session/types";
 
 import "gogoproto/gogo.proto";
 import "google/protobuf/duration.proto";
-import "google/protobuf/timestamp.proto";
 import "sentinel/types/v1/bandwidth.proto";
-import "sentinel/types/v1/status.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/session/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
-message Session {
-  uint64 id              = 1 [ (gogoproto.customname) = "ID" ];
-  uint64 subscription_id = 2 [ (gogoproto.customname) = "SubscriptionID" ];
-  string node_address    = 3;
-  string address         = 4;
-  google.protobuf.Duration duration = 5
+message Proof {
+  uint64 id                         = 1;
+  google.protobuf.Duration duration = 2
       [ (gogoproto.stdduration) = true, (gogoproto.nullable) = false ];
-  sentinel.types.v1.Bandwidth bandwidth = 6 [ (gogoproto.nullable) = false ];
-  sentinel.types.v1.Status status       = 7;
-  google.protobuf.Timestamp status_at   = 8
-      [ (gogoproto.nullable) = false, (gogoproto.stdtime) = true ];
+  sentinel.types.v1.Bandwidth bandwidth = 3 [ (gogoproto.nullable) = false ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/session/v2/session_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/validator_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/session/v2/session.proto
+# source: tendermint/types/validator.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from sentinel.types.v1 import bandwidth_pb2 as sentinel_dot_types_dot_v1_dot_bandwidth__pb2
-from sentinel.types.v1 import status_pb2 as sentinel_dot_types_dot_v1_dot_status__pb2
+from tendermint.crypto import keys_pb2 as tendermint_dot_crypto_dot_keys__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!sentinel/session/v2/session.proto\x12\x13sentinel.session.v2\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a!sentinel/types/v1/bandwidth.proto\x1a\x1esentinel/types/v1/status.proto\"\xc3\x02\n\x07Session\x12\x12\n\x02id\x18\x01 \x01(\x04\x42\x06\xe2\xde\x1f\x02ID\x12+\n\x0fsubscription_id\x18\x02 \x01(\x04\x42\x12\xe2\xde\x1f\x0eSubscriptionID\x12\x14\n\x0cnode_address\x18\x03 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12\x35\n\x08\x64uration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\x98\xdf\x1f\x01\xc8\xde\x1f\x00\x12\x35\n\tbandwidth\x18\x06 \x01(\x0b\x32\x1c.sentinel.types.v1.BandwidthB\x04\xc8\xde\x1f\x00\x12)\n\x06status\x18\x07 \x01(\x0e\x32\x19.sentinel.types.v1.Status\x12\x37\n\tstatus_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x42:Z0github.com/sentinel-official/hub/x/session/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tendermint/types/validator.proto\x12\x10tendermint.types\x1a\x14gogoproto/gogo.proto\x1a\x1ctendermint/crypto/keys.proto\"\x8a\x01\n\x0cValidatorSet\x12/\n\nvalidators\x18\x01 \x03(\x0b\x32\x1b.tendermint.types.Validator\x12-\n\x08proposer\x18\x02 \x01(\x0b\x32\x1b.tendermint.types.Validator\x12\x1a\n\x12total_voting_power\x18\x03 \x01(\x03\"\x82\x01\n\tValidator\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0c\x12\x33\n\x07pub_key\x18\x02 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKeyB\x04\xc8\xde\x1f\x00\x12\x14\n\x0cvoting_power\x18\x03 \x01(\x03\x12\x19\n\x11proposer_priority\x18\x04 \x01(\x03\"V\n\x0fSimpleValidator\x12-\n\x07pub_key\x18\x01 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKey\x12\x14\n\x0cvoting_power\x18\x02 \x01(\x03\x42\x39Z7github.com/tendermint/tendermint/proto/tendermint/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.session.v2.session_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.validator_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z0github.com/sentinel-official/hub/x/session/types\250\342\036\000\310\341\036\000'
-  _SESSION.fields_by_name['id']._options = None
-  _SESSION.fields_by_name['id']._serialized_options = b'\342\336\037\002ID'
-  _SESSION.fields_by_name['subscription_id']._options = None
-  _SESSION.fields_by_name['subscription_id']._serialized_options = b'\342\336\037\016SubscriptionID'
-  _SESSION.fields_by_name['duration']._options = None
-  _SESSION.fields_by_name['duration']._serialized_options = b'\230\337\037\001\310\336\037\000'
-  _SESSION.fields_by_name['bandwidth']._options = None
-  _SESSION.fields_by_name['bandwidth']._serialized_options = b'\310\336\037\000'
-  _SESSION.fields_by_name['status_at']._options = None
-  _SESSION.fields_by_name['status_at']._serialized_options = b'\310\336\037\000\220\337\037\001'
-  _SESSION._serialized_start=213
-  _SESSION._serialized_end=536
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types'
+  _VALIDATOR.fields_by_name['pub_key']._options = None
+  _VALIDATOR.fields_by_name['pub_key']._serialized_options = b'\310\336\037\000'
+  _VALIDATORSET._serialized_start=107
+  _VALIDATORSET._serialized_end=245
+  _VALIDATOR._serialized_start=248
+  _VALIDATOR._serialized_end=378
+  _SIMPLEVALIDATOR._serialized_start=380
+  _SIMPLEVALIDATOR._serialized_end=466
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v1/quota.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/types/v1/status.proto`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 syntax = "proto3";
-package sentinel.subscription.v1;
+package sentinel.types.v1;
 
-option go_package = "github.com/sentinel-official/hub/x/subscription/legacy/v1/types";
+option go_package = "github.com/sentinel-official/hub/types";
 
 import "gogoproto/gogo.proto";
 
-option (gogoproto.equal_all)           = false;
-option (gogoproto.goproto_getters_all) = false;
+option (gogoproto.goproto_getters_all)     = false;
+option (gogoproto.goproto_enum_prefix_all) = false;
 
-message Quota {
-  string address   = 1;
-  string allocated = 2 [
-    (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
-    (gogoproto.nullable)   = false
-  ];
-  string consumed = 3 [
-    (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
-    (gogoproto.nullable)   = false
-  ];
+enum Status {
+  STATUS_UNSPECIFIED = 0 [ (gogoproto.enumvalue_customname) = "Unspecified" ];
+  STATUS_ACTIVE      = 1 [ (gogoproto.enumvalue_customname) = "Active" ];
+  STATUS_INACTIVE_PENDING = 2
+      [ (gogoproto.enumvalue_customname) = "InactivePending" ];
+  STATUS_INACTIVE = 3 [ (gogoproto.enumvalue_customname) = "Inactive" ];
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v1/subscription_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/evidence_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/subscription/v1/subscription.proto
+# source: tendermint/types/evidence.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from sentinel.types.v1 import status_pb2 as sentinel_dot_types_dot_v1_dot_status__pb2
+from tendermint.types import types_pb2 as tendermint_dot_types_dot_types__pb2
+from tendermint.types import validator_pb2 as tendermint_dot_types_dot_validator__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+sentinel/subscription/v1/subscription.proto\x12\x18sentinel.subscription.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1esentinel/types/v1/status.proto\"\x8e\x03\n\x0cSubscription\x12\n\n\x02id\x18\x01 \x01(\x04\x12\r\n\x05owner\x18\x02 \x01(\t\x12\x0c\n\x04node\x18\x03 \x01(\t\x12.\n\x05price\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x30\n\x07\x64\x65posit\x18\x05 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x0c\n\x04plan\x18\x06 \x01(\x04\x12\r\n\x05\x64\x65nom\x18\x07 \x01(\t\x12\x34\n\x06\x65xpiry\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x12<\n\x04\x66ree\x18\t \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\x12)\n\x06status\x18\n \x01(\x0e\x32\x19.sentinel.types.v1.Status\x12\x37\n\tstatus_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x42IZ?github.com/sentinel-official/hub/x/subscription/legacy/v1/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ftendermint/types/evidence.proto\x12\x10tendermint.types\x1a\x14gogoproto/gogo.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1ctendermint/types/types.proto\x1a tendermint/types/validator.proto\"\xb2\x01\n\x08\x45vidence\x12J\n\x17\x64uplicate_vote_evidence\x18\x01 \x01(\x0b\x32\'.tendermint.types.DuplicateVoteEvidenceH\x00\x12S\n\x1clight_client_attack_evidence\x18\x02 \x01(\x0b\x32+.tendermint.types.LightClientAttackEvidenceH\x00\x42\x05\n\x03sum\"\xd5\x01\n\x15\x44uplicateVoteEvidence\x12&\n\x06vote_a\x18\x01 \x01(\x0b\x32\x16.tendermint.types.Vote\x12&\n\x06vote_b\x18\x02 \x01(\x0b\x32\x16.tendermint.types.Vote\x12\x1a\n\x12total_voting_power\x18\x03 \x01(\x03\x12\x17\n\x0fvalidator_power\x18\x04 \x01(\x03\x12\x37\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\"\xfb\x01\n\x19LightClientAttackEvidence\x12\x37\n\x11\x63onflicting_block\x18\x01 \x01(\x0b\x32\x1c.tendermint.types.LightBlock\x12\x15\n\rcommon_height\x18\x02 \x01(\x03\x12\x39\n\x14\x62yzantine_validators\x18\x03 \x03(\x0b\x32\x1b.tendermint.types.Validator\x12\x1a\n\x12total_voting_power\x18\x04 \x01(\x03\x12\x37\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\"B\n\x0c\x45videnceList\x12\x32\n\x08\x65vidence\x18\x01 \x03(\x0b\x32\x1a.tendermint.types.EvidenceB\x04\xc8\xde\x1f\x00\x42\x39Z7github.com/tendermint/tendermint/proto/tendermint/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.subscription.v1.subscription_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.evidence_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/sentinel-official/hub/x/subscription/legacy/v1/types\250\342\036\000\310\341\036\000'
-  _SUBSCRIPTION.fields_by_name['price']._options = None
-  _SUBSCRIPTION.fields_by_name['price']._serialized_options = b'\310\336\037\000'
-  _SUBSCRIPTION.fields_by_name['deposit']._options = None
-  _SUBSCRIPTION.fields_by_name['deposit']._serialized_options = b'\310\336\037\000'
-  _SUBSCRIPTION.fields_by_name['expiry']._options = None
-  _SUBSCRIPTION.fields_by_name['expiry']._serialized_options = b'\310\336\037\000\220\337\037\001'
-  _SUBSCRIPTION.fields_by_name['free']._options = None
-  _SUBSCRIPTION.fields_by_name['free']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Int\310\336\037\000'
-  _SUBSCRIPTION.fields_by_name['status_at']._options = None
-  _SUBSCRIPTION.fields_by_name['status_at']._serialized_options = b'\310\336\037\000\220\337\037\001'
-  _SUBSCRIPTION._serialized_start=193
-  _SUBSCRIPTION._serialized_end=591
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types'
+  _DUPLICATEVOTEEVIDENCE.fields_by_name['timestamp']._options = None
+  _DUPLICATEVOTEEVIDENCE.fields_by_name['timestamp']._serialized_options = b'\310\336\037\000\220\337\037\001'
+  _LIGHTCLIENTATTACKEVIDENCE.fields_by_name['timestamp']._options = None
+  _LIGHTCLIENTATTACKEVIDENCE.fields_by_name['timestamp']._serialized_options = b'\310\336\037\000\220\337\037\001'
+  _EVIDENCELIST.fields_by_name['evidence']._options = None
+  _EVIDENCELIST.fields_by_name['evidence']._serialized_options = b'\310\336\037\000'
+  _EVIDENCE._serialized_start=173
+  _EVIDENCE._serialized_end=351
+  _DUPLICATEVOTEEVIDENCE._serialized_start=354
+  _DUPLICATEVOTEEVIDENCE._serialized_end=567
+  _LIGHTCLIENTATTACKEVIDENCE._serialized_start=570
+  _LIGHTCLIENTATTACKEVIDENCE._serialized_end=821
+  _EVIDENCELIST._serialized_start=823
+  _EVIDENCELIST._serialized_end=889
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/msg.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/subscription/v1/msg.proto`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,80 @@
 syntax = "proto3";
-package sentinel.subscription.v2;
+package sentinel.subscription.v1;
+
+option go_package = "github.com/sentinel-official/hub/x/subscription/types";
 
 import "gogoproto/gogo.proto";
+import "cosmos/base/v1beta1/coin.proto";
 
-option go_package = "github.com/sentinel-official/hub/x/subscription/types";
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
+// MsgSubscribeToNodeRequest defines the SDK message for subscribing to a node
+message MsgSubscribeToNodeRequest {
+  string from                      = 1;
+  string address                   = 2;
+  cosmos.base.v1beta1.Coin deposit = 3 [ (gogoproto.nullable) = false ];
+}
+
+// MsgSubscribeToPlanRequest defines the SDK message for subscribing to a plan
+message MsgSubscribeToPlanRequest {
+  string from  = 1;
+  uint64 id    = 2;
+  string denom = 3;
+}
+
 // MsgCancelRequest defines the SDK message for cancelling a subscription
 message MsgCancelRequest {
   string from = 1;
   uint64 id   = 2;
 }
 
-// MsgShareRequest defines the SDK message for sharing a subscription with an
-// address
-message MsgShareRequest {
+// MsgAddQuotaRequest defines the SDK message for adding the quota to an address
+message MsgAddQuotaRequest {
   string from    = 1;
   uint64 id      = 2;
   string address = 3;
   string bytes   = 4 [
     (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
     (gogoproto.nullable)   = false
   ];
 }
 
-// MsgUpdateQuotaRequest defines the SDK message for updating the bandwidth
-// quota of an address
+// MsgUpdateQuotaRequest defines the SDK message for updating the quota of an
+// address
 message MsgUpdateQuotaRequest {
   string from    = 1;
   uint64 id      = 2;
   string address = 3;
   string bytes   = 4 [
     (gogoproto.customtype) = "github.com/cosmos/cosmos-sdk/types.Int",
     (gogoproto.nullable)   = false
   ];
 }
 
+// MsgSubscribeToNodeResponse defines the response of message
+// MsgSubscribeToNodeRequest
+message MsgSubscribeToNodeResponse {}
+
+// MsgSubscribeToPlanResponse defines the response of message
+// MsgSubscribeToPlanRequest
+message MsgSubscribeToPlanResponse {}
+
 // MsgCancelResponse defines the response of message MsgCancelRequest
 message MsgCancelResponse {}
 
-// MsgShareResponse defines the response of message MsgShareRequest
-message MsgShareResponse {}
+// MsgAddQuotaResponse defines the response of message MsgAddQuotaRequest
+message MsgAddQuotaResponse {}
 
 // MsgUpdateQuotaResponse defines the response of message MsgUpdateQuotaRequest
 message MsgUpdateQuotaResponse {}
 
 service MsgService {
+  rpc MsgSubscribeToNode(MsgSubscribeToNodeRequest)
+      returns (MsgSubscribeToNodeResponse);
+  rpc MsgSubscribeToPlan(MsgSubscribeToPlanRequest)
+      returns (MsgSubscribeToPlanResponse);
   rpc MsgCancel(MsgCancelRequest) returns (MsgCancelResponse);
-  rpc MsgShare(MsgShareRequest) returns (MsgShareResponse);
+  rpc MsgAddQuota(MsgAddQuotaRequest) returns (MsgAddQuotaResponse);
   rpc MsgUpdateQuota(MsgUpdateQuotaRequest) returns (MsgUpdateQuotaResponse);
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/subscription/v2/subscription_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/privval/types_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/subscription/v2/subscription.proto
+# source: tendermint/privval/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
+from tendermint.crypto import keys_pb2 as tendermint_dot_crypto_dot_keys__pb2
+from tendermint.types import types_pb2 as tendermint_dot_types_dot_types__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from sentinel.types.v1 import status_pb2 as sentinel_dot_types_dot_v1_dot_status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+sentinel/subscription/v2/subscription.proto\x12\x18sentinel.subscription.v2\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1esentinel/types/v1/status.proto\"\xa3\x01\n\x10\x42\x61seSubscription\x12\x12\n\x02id\x18\x01 \x01(\x04\x42\x06\xe2\xde\x1f\x02ID\x12\x17\n\x0f\x61\x63\x63ount_address\x18\x02 \x01(\t\x12)\n\x06status\x18\x03 \x01(\x0e\x32\x19.sentinel.types.v1.Status\x12\x37\n\tstatus_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\"\xab\x01\n\x10NodeSubscription\x12\x42\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32*.sentinel.subscription.v2.BaseSubscriptionB\x08\xd0\xde\x1f\x01\xc8\xde\x1f\x00\x12\x14\n\x0cnode_address\x18\x02 \x01(\t\x12\r\n\x05hours\x18\x03 \x01(\x03\x12.\n\x05price\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\x82\x01\n\x10PlanSubscription\x12\x42\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32*.sentinel.subscription.v2.BaseSubscriptionB\x08\xd0\xde\x1f\x01\xc8\xde\x1f\x00\x12\x1b\n\x07plan_id\x18\x02 \x01(\x04\x42\n\xe2\xde\x1f\x06PlanID\x12\r\n\x05\x64\x65nom\x18\x03 \x01(\t*}\n\x10SubscriptionType\x12)\n\x10TYPE_UNSPECIFIED\x10\x00\x1a\x13\x8a\x9d \x0fTypeUnspecified\x12\x1b\n\tTYPE_NODE\x10\x01\x1a\x0c\x8a\x9d \x08TypeNode\x12\x1b\n\tTYPE_PLAN\x10\x02\x1a\x0c\x8a\x9d \x08TypePlan\x1a\x04\x88\xa3\x1e\x00\x42?Z5github.com/sentinel-official/hub/x/subscription/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1etendermint/privval/types.proto\x12\x12tendermint.privval\x1a\x1ctendermint/crypto/keys.proto\x1a\x1ctendermint/types/types.proto\x1a\x14gogoproto/gogo.proto\"6\n\x11RemoteSignerError\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"!\n\rPubKeyRequest\x12\x10\n\x08\x63hain_id\x18\x01 \x01(\t\"{\n\x0ePubKeyResponse\x12\x33\n\x07pub_key\x18\x01 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKeyB\x04\xc8\xde\x1f\x00\x12\x34\n\x05\x65rror\x18\x02 \x01(\x0b\x32%.tendermint.privval.RemoteSignerError\"I\n\x0fSignVoteRequest\x12$\n\x04vote\x18\x01 \x01(\x0b\x32\x16.tendermint.types.Vote\x12\x10\n\x08\x63hain_id\x18\x02 \x01(\t\"v\n\x12SignedVoteResponse\x12*\n\x04vote\x18\x01 \x01(\x0b\x32\x16.tendermint.types.VoteB\x04\xc8\xde\x1f\x00\x12\x34\n\x05\x65rror\x18\x02 \x01(\x0b\x32%.tendermint.privval.RemoteSignerError\"U\n\x13SignProposalRequest\x12,\n\x08proposal\x18\x01 \x01(\x0b\x32\x1a.tendermint.types.Proposal\x12\x10\n\x08\x63hain_id\x18\x02 \x01(\t\"\x82\x01\n\x16SignedProposalResponse\x12\x32\n\x08proposal\x18\x01 \x01(\x0b\x32\x1a.tendermint.types.ProposalB\x04\xc8\xde\x1f\x00\x12\x34\n\x05\x65rror\x18\x02 \x01(\x0b\x32%.tendermint.privval.RemoteSignerError\"\r\n\x0bPingRequest\"\x0e\n\x0cPingResponse\"\xa6\x04\n\x07Message\x12<\n\x0fpub_key_request\x18\x01 \x01(\x0b\x32!.tendermint.privval.PubKeyRequestH\x00\x12>\n\x10pub_key_response\x18\x02 \x01(\x0b\x32\".tendermint.privval.PubKeyResponseH\x00\x12@\n\x11sign_vote_request\x18\x03 \x01(\x0b\x32#.tendermint.privval.SignVoteRequestH\x00\x12\x46\n\x14signed_vote_response\x18\x04 \x01(\x0b\x32&.tendermint.privval.SignedVoteResponseH\x00\x12H\n\x15sign_proposal_request\x18\x05 \x01(\x0b\x32\'.tendermint.privval.SignProposalRequestH\x00\x12N\n\x18signed_proposal_response\x18\x06 \x01(\x0b\x32*.tendermint.privval.SignedProposalResponseH\x00\x12\x37\n\x0cping_request\x18\x07 \x01(\x0b\x32\x1f.tendermint.privval.PingRequestH\x00\x12\x39\n\rping_response\x18\x08 \x01(\x0b\x32 .tendermint.privval.PingResponseH\x00\x42\x05\n\x03sum*\xa8\x01\n\x06\x45rrors\x12\x12\n\x0e\x45RRORS_UNKNOWN\x10\x00\x12\x1e\n\x1a\x45RRORS_UNEXPECTED_RESPONSE\x10\x01\x12\x18\n\x14\x45RRORS_NO_CONNECTION\x10\x02\x12\x1d\n\x19\x45RRORS_CONNECTION_TIMEOUT\x10\x03\x12\x17\n\x13\x45RRORS_READ_TIMEOUT\x10\x04\x12\x18\n\x14\x45RRORS_WRITE_TIMEOUT\x10\x05\x42;Z9github.com/tendermint/tendermint/proto/tendermint/privvalb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.subscription.v2.subscription_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.privval.types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/sentinel-official/hub/x/subscription/types\250\342\036\000\310\341\036\000'
-  _SUBSCRIPTIONTYPE._options = None
-  _SUBSCRIPTIONTYPE._serialized_options = b'\210\243\036\000'
-  _SUBSCRIPTIONTYPE.values_by_name["TYPE_UNSPECIFIED"]._options = None
-  _SUBSCRIPTIONTYPE.values_by_name["TYPE_UNSPECIFIED"]._serialized_options = b'\212\235 \017TypeUnspecified'
-  _SUBSCRIPTIONTYPE.values_by_name["TYPE_NODE"]._options = None
-  _SUBSCRIPTIONTYPE.values_by_name["TYPE_NODE"]._serialized_options = b'\212\235 \010TypeNode'
-  _SUBSCRIPTIONTYPE.values_by_name["TYPE_PLAN"]._options = None
-  _SUBSCRIPTIONTYPE.values_by_name["TYPE_PLAN"]._serialized_options = b'\212\235 \010TypePlan'
-  _BASESUBSCRIPTION.fields_by_name['id']._options = None
-  _BASESUBSCRIPTION.fields_by_name['id']._serialized_options = b'\342\336\037\002ID'
-  _BASESUBSCRIPTION.fields_by_name['status_at']._options = None
-  _BASESUBSCRIPTION.fields_by_name['status_at']._serialized_options = b'\310\336\037\000\220\337\037\001'
-  _NODESUBSCRIPTION.fields_by_name['base']._options = None
-  _NODESUBSCRIPTION.fields_by_name['base']._serialized_options = b'\320\336\037\001\310\336\037\000'
-  _NODESUBSCRIPTION.fields_by_name['price']._options = None
-  _NODESUBSCRIPTION.fields_by_name['price']._serialized_options = b'\310\336\037\000'
-  _PLANSUBSCRIPTION.fields_by_name['base']._options = None
-  _PLANSUBSCRIPTION.fields_by_name['base']._serialized_options = b'\320\336\037\001\310\336\037\000'
-  _PLANSUBSCRIPTION.fields_by_name['plan_id']._options = None
-  _PLANSUBSCRIPTION.fields_by_name['plan_id']._serialized_options = b'\342\336\037\006PlanID'
-  _SUBSCRIPTIONTYPE._serialized_start=665
-  _SUBSCRIPTIONTYPE._serialized_end=790
-  _BASESUBSCRIPTION._serialized_start=193
-  _BASESUBSCRIPTION._serialized_end=356
-  _NODESUBSCRIPTION._serialized_start=359
-  _NODESUBSCRIPTION._serialized_end=530
-  _PLANSUBSCRIPTION._serialized_start=533
-  _PLANSUBSCRIPTION._serialized_end=663
+  DESCRIPTOR._serialized_options = b'Z9github.com/tendermint/tendermint/proto/tendermint/privval'
+  _PUBKEYRESPONSE.fields_by_name['pub_key']._options = None
+  _PUBKEYRESPONSE.fields_by_name['pub_key']._serialized_options = b'\310\336\037\000'
+  _SIGNEDVOTERESPONSE.fields_by_name['vote']._options = None
+  _SIGNEDVOTERESPONSE.fields_by_name['vote']._serialized_options = b'\310\336\037\000'
+  _SIGNEDPROPOSALRESPONSE.fields_by_name['proposal']._options = None
+  _SIGNEDPROPOSALRESPONSE.fields_by_name['proposal']._serialized_options = b'\310\336\037\000'
+  _ERRORS._serialized_start=1352
+  _ERRORS._serialized_end=1520
+  _REMOTESIGNERERROR._serialized_start=136
+  _REMOTESIGNERERROR._serialized_end=190
+  _PUBKEYREQUEST._serialized_start=192
+  _PUBKEYREQUEST._serialized_end=225
+  _PUBKEYRESPONSE._serialized_start=227
+  _PUBKEYRESPONSE._serialized_end=350
+  _SIGNVOTEREQUEST._serialized_start=352
+  _SIGNVOTEREQUEST._serialized_end=425
+  _SIGNEDVOTERESPONSE._serialized_start=427
+  _SIGNEDVOTERESPONSE._serialized_end=545
+  _SIGNPROPOSALREQUEST._serialized_start=547
+  _SIGNPROPOSALREQUEST._serialized_end=632
+  _SIGNEDPROPOSALRESPONSE._serialized_start=635
+  _SIGNEDPROPOSALRESPONSE._serialized_end=765
+  _PINGREQUEST._serialized_start=767
+  _PINGREQUEST._serialized_end=780
+  _PINGRESPONSE._serialized_start=782
+  _PINGRESPONSE._serialized_end=796
+  _MESSAGE._serialized_start=799
+  _MESSAGE._serialized_end=1349
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/params_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/params_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sentinel/swap/v1/params.proto
+# source: sentinel/vpn/v1/params.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dsentinel/swap/v1/params.proto\x12\x10sentinel.swap.v1\x1a\x14gogoproto/gogo.proto\"F\n\x06Params\x12\x14\n\x0cswap_enabled\x18\x01 \x01(\x08\x12\x12\n\nswap_denom\x18\x02 \x01(\t\x12\x12\n\napprove_by\x18\x03 \x01(\tB7Z-github.com/sentinel-official/hub/x/swap/types\xa8\xe2\x1e\x00\xc8\xe1\x1e\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1csentinel/vpn/v1/params.proto\x12\x0fsentinel.vpn.v1B.Z,github.com/sentinel-official/hub/x/vpn/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.swap.v1.params_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.vpn.v1.params_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/sentinel-official/hub/x/swap/types\250\342\036\000\310\341\036\000'
-  _PARAMS._serialized_start=73
-  _PARAMS._serialized_end=143
+  DESCRIPTOR._serialized_options = b'Z,github.com/sentinel-official/hub/x/vpn/types'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/swap/v1/params_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/keys_pb2.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from gogoproto import gogo_pb2 as _gogo_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Params(_message.Message):
-    __slots__ = ["approve_by", "swap_denom", "swap_enabled"]
-    APPROVE_BY_FIELD_NUMBER: _ClassVar[int]
-    SWAP_DENOM_FIELD_NUMBER: _ClassVar[int]
-    SWAP_ENABLED_FIELD_NUMBER: _ClassVar[int]
-    approve_by: str
-    swap_denom: str
-    swap_enabled: bool
-    def __init__(self, swap_enabled: bool = ..., swap_denom: _Optional[str] = ..., approve_by: _Optional[str] = ...) -> None: ...
+class PublicKey(_message.Message):
+    __slots__ = ["ed25519", "secp256k1"]
+    ED25519_FIELD_NUMBER: _ClassVar[int]
+    SECP256K1_FIELD_NUMBER: _ClassVar[int]
+    ed25519: bytes
+    secp256k1: bytes
+    def __init__(self, ed25519: _Optional[bytes] = ..., secp256k1: _Optional[bytes] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/types/v1/bandwidth.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/types/v1/bandwidth.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/sentinel/vpn/v1/genesis.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/vpn/v1/genesis.proto`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 syntax = "proto3";
 package sentinel.vpn.v1;
 
 option go_package = "github.com/sentinel-official/hub/x/vpn/types";
 
 import "gogoproto/gogo.proto";
 import "sentinel/deposit/v1/deposit.proto";
-import "sentinel/node/v2/genesis.proto";
-import "sentinel/plan/v2/genesis.proto";
-import "sentinel/provider/v2/genesis.proto";
-import "sentinel/session/v2/genesis.proto";
-import "sentinel/subscription/v2/genesis.proto";
+import "sentinel/node/v1/genesis.proto";
+import "sentinel/plan/v1/genesis.proto";
+import "sentinel/provider/v1/genesis.proto";
+import "sentinel/session/v1/genesis.proto";
+import "sentinel/subscription/v1/genesis.proto";
 
 option (gogoproto.equal_all)           = false;
 option (gogoproto.goproto_getters_all) = false;
 
 message GenesisState {
   repeated sentinel.deposit.v1.Deposit deposits = 1
       [ (gogoproto.nullable) = false ];
-  sentinel.node.v2.GenesisState nodes         = 2;
-  repeated sentinel.plan.v2.GenesisPlan plans = 3
+  sentinel.node.v1.GenesisState nodes         = 2;
+  repeated sentinel.plan.v1.GenesisPlan plans = 3
       [ (gogoproto.nullable) = false ];
-  sentinel.provider.v2.GenesisState providers         = 4;
-  sentinel.session.v2.GenesisState sessions           = 5;
-  sentinel.subscription.v2.GenesisState subscriptions = 6;
+  sentinel.provider.v1.GenesisState providers         = 4;
+  sentinel.session.v1.GenesisState sessions           = 5;
+  sentinel.subscription.v1.GenesisState subscriptions = 6;
 }
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/abci/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/abci/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/abci/types_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/abci/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/abci/types_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/abci/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/blockchain/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/blockchain/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/blockchain/types_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/blockchain/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/types_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/types_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/wal.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/consensus/wal.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/consensus/wal_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/state/types_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/consensus/wal.proto
+# source: tendermint/state/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from tendermint.consensus import types_pb2 as tendermint_dot_consensus_dot_types__pb2
-from tendermint.types import events_pb2 as tendermint_dot_types_dot_events__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from tendermint.abci import types_pb2 as tendermint_dot_abci_dot_types__pb2
+from tendermint.types import types_pb2 as tendermint_dot_types_dot_types__pb2
+from tendermint.types import validator_pb2 as tendermint_dot_types_dot_validator__pb2
+from tendermint.types import params_pb2 as tendermint_dot_types_dot_params__pb2
+from tendermint.version import types_pb2 as tendermint_dot_version_dot_types__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1etendermint/consensus/wal.proto\x12\x14tendermint.consensus\x1a\x14gogoproto/gogo.proto\x1a tendermint/consensus/types.proto\x1a\x1dtendermint/types/events.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"X\n\x07MsgInfo\x12\x30\n\x03msg\x18\x01 \x01(\x0b\x32\x1d.tendermint.consensus.MessageB\x04\xc8\xde\x1f\x00\x12\x1b\n\x07peer_id\x18\x02 \x01(\tB\n\xe2\xde\x1f\x06PeerID\"q\n\x0bTimeoutInfo\x12\x35\n\x08\x64uration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xc8\xde\x1f\x00\x98\xdf\x1f\x01\x12\x0e\n\x06height\x18\x02 \x01(\x03\x12\r\n\x05round\x18\x03 \x01(\x05\x12\x0c\n\x04step\x18\x04 \x01(\r\"\x1b\n\tEndHeight\x12\x0e\n\x06height\x18\x01 \x01(\x03\"\x81\x02\n\nWALMessage\x12G\n\x16\x65vent_data_round_state\x18\x01 \x01(\x0b\x32%.tendermint.types.EventDataRoundStateH\x00\x12\x31\n\x08msg_info\x18\x02 \x01(\x0b\x32\x1d.tendermint.consensus.MsgInfoH\x00\x12\x39\n\x0ctimeout_info\x18\x03 \x01(\x0b\x32!.tendermint.consensus.TimeoutInfoH\x00\x12\x35\n\nend_height\x18\x04 \x01(\x0b\x32\x1f.tendermint.consensus.EndHeightH\x00\x42\x05\n\x03sum\"t\n\x0fTimedWALMessage\x12\x32\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x12-\n\x03msg\x18\x02 \x01(\x0b\x32 .tendermint.consensus.WALMessageB=Z;github.com/tendermint/tendermint/proto/tendermint/consensusb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctendermint/state/types.proto\x12\x10tendermint.state\x1a\x14gogoproto/gogo.proto\x1a\x1btendermint/abci/types.proto\x1a\x1ctendermint/types/types.proto\x1a tendermint/types/validator.proto\x1a\x1dtendermint/types/params.proto\x1a\x1etendermint/version/types.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb8\x01\n\rABCIResponses\x12\x37\n\x0b\x64\x65liver_txs\x18\x01 \x03(\x0b\x32\".tendermint.abci.ResponseDeliverTx\x12\x34\n\tend_block\x18\x02 \x01(\x0b\x32!.tendermint.abci.ResponseEndBlock\x12\x38\n\x0b\x62\x65gin_block\x18\x03 \x01(\x0b\x32#.tendermint.abci.ResponseBeginBlock\"d\n\x0eValidatorsInfo\x12\x35\n\rvalidator_set\x18\x01 \x01(\x0b\x32\x1e.tendermint.types.ValidatorSet\x12\x1b\n\x13last_height_changed\x18\x02 \x01(\x03\"u\n\x13\x43onsensusParamsInfo\x12\x41\n\x10\x63onsensus_params\x18\x01 \x01(\x0b\x32!.tendermint.types.ConsensusParamsB\x04\xc8\xde\x1f\x00\x12\x1b\n\x13last_height_changed\x18\x02 \x01(\x03\"S\n\x07Version\x12\x36\n\tconsensus\x18\x01 \x01(\x0b\x32\x1d.tendermint.version.ConsensusB\x04\xc8\xde\x1f\x00\x12\x10\n\x08software\x18\x02 \x01(\t\"\xfd\x04\n\x05State\x12\x30\n\x07version\x18\x01 \x01(\x0b\x32\x19.tendermint.state.VersionB\x04\xc8\xde\x1f\x00\x12\x1d\n\x08\x63hain_id\x18\x02 \x01(\tB\x0b\xe2\xde\x1f\x07\x43hainID\x12\x16\n\x0einitial_height\x18\x0e \x01(\x03\x12\x19\n\x11last_block_height\x18\x03 \x01(\x03\x12\x45\n\rlast_block_id\x18\x04 \x01(\x0b\x32\x19.tendermint.types.BlockIDB\x13\xc8\xde\x1f\x00\xe2\xde\x1f\x0bLastBlockID\x12=\n\x0flast_block_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xc8\xde\x1f\x00\x90\xdf\x1f\x01\x12\x37\n\x0fnext_validators\x18\x06 \x01(\x0b\x32\x1e.tendermint.types.ValidatorSet\x12\x32\n\nvalidators\x18\x07 \x01(\x0b\x32\x1e.tendermint.types.ValidatorSet\x12\x37\n\x0flast_validators\x18\x08 \x01(\x0b\x32\x1e.tendermint.types.ValidatorSet\x12&\n\x1elast_height_validators_changed\x18\t \x01(\x03\x12\x41\n\x10\x63onsensus_params\x18\n \x01(\x0b\x32!.tendermint.types.ConsensusParamsB\x04\xc8\xde\x1f\x00\x12,\n$last_height_consensus_params_changed\x18\x0b \x01(\x03\x12\x19\n\x11last_results_hash\x18\x0c \x01(\x0c\x12\x10\n\x08\x61pp_hash\x18\r \x01(\x0c\x42\x39Z7github.com/tendermint/tendermint/proto/tendermint/stateb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.consensus.wal_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.state.types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z;github.com/tendermint/tendermint/proto/tendermint/consensus'
-  _MSGINFO.fields_by_name['msg']._options = None
-  _MSGINFO.fields_by_name['msg']._serialized_options = b'\310\336\037\000'
-  _MSGINFO.fields_by_name['peer_id']._options = None
-  _MSGINFO.fields_by_name['peer_id']._serialized_options = b'\342\336\037\006PeerID'
-  _TIMEOUTINFO.fields_by_name['duration']._options = None
-  _TIMEOUTINFO.fields_by_name['duration']._serialized_options = b'\310\336\037\000\230\337\037\001'
-  _TIMEDWALMESSAGE.fields_by_name['time']._options = None
-  _TIMEDWALMESSAGE.fields_by_name['time']._serialized_options = b'\310\336\037\000\220\337\037\001'
-  _MSGINFO._serialized_start=208
-  _MSGINFO._serialized_end=296
-  _TIMEOUTINFO._serialized_start=298
-  _TIMEOUTINFO._serialized_end=411
-  _ENDHEIGHT._serialized_start=413
-  _ENDHEIGHT._serialized_end=440
-  _WALMESSAGE._serialized_start=443
-  _WALMESSAGE._serialized_end=700
-  _TIMEDWALMESSAGE._serialized_start=702
-  _TIMEDWALMESSAGE._serialized_end=818
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/state'
+  _CONSENSUSPARAMSINFO.fields_by_name['consensus_params']._options = None
+  _CONSENSUSPARAMSINFO.fields_by_name['consensus_params']._serialized_options = b'\310\336\037\000'
+  _VERSION.fields_by_name['consensus']._options = None
+  _VERSION.fields_by_name['consensus']._serialized_options = b'\310\336\037\000'
+  _STATE.fields_by_name['version']._options = None
+  _STATE.fields_by_name['version']._serialized_options = b'\310\336\037\000'
+  _STATE.fields_by_name['chain_id']._options = None
+  _STATE.fields_by_name['chain_id']._serialized_options = b'\342\336\037\007ChainID'
+  _STATE.fields_by_name['last_block_id']._options = None
+  _STATE.fields_by_name['last_block_id']._serialized_options = b'\310\336\037\000\342\336\037\013LastBlockID'
+  _STATE.fields_by_name['last_block_time']._options = None
+  _STATE.fields_by_name['last_block_time']._serialized_options = b'\310\336\037\000\220\337\037\001'
+  _STATE.fields_by_name['consensus_params']._options = None
+  _STATE.fields_by_name['consensus_params']._serialized_options = b'\310\336\037\000'
+  _ABCIRESPONSES._serialized_start=262
+  _ABCIRESPONSES._serialized_end=446
+  _VALIDATORSINFO._serialized_start=448
+  _VALIDATORSINFO._serialized_end=548
+  _CONSENSUSPARAMSINFO._serialized_start=550
+  _CONSENSUSPARAMSINFO._serialized_end=667
+  _VERSION._serialized_start=669
+  _VERSION._serialized_end=752
+  _STATE._serialized_start=755
+  _STATE._serialized_end=1392
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/keys_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/version/types_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/crypto/keys.proto
+# source: tendermint/version/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctendermint/crypto/keys.proto\x12\x11tendermint.crypto\x1a\x14gogoproto/gogo.proto\"D\n\tPublicKey\x12\x11\n\x07\x65\x64\x32\x35\x35\x31\x39\x18\x01 \x01(\x0cH\x00\x12\x13\n\tsecp256k1\x18\x02 \x01(\x0cH\x00:\x08\xe8\xa1\x1f\x01\xe8\xa0\x1f\x01\x42\x05\n\x03sumB:Z8github.com/tendermint/tendermint/proto/tendermint/cryptob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1etendermint/version/types.proto\x12\x12tendermint.version\x1a\x14gogoproto/gogo.proto\")\n\x03\x41pp\x12\x10\n\x08protocol\x18\x01 \x01(\x04\x12\x10\n\x08software\x18\x02 \x01(\t\"-\n\tConsensus\x12\r\n\x05\x62lock\x18\x01 \x01(\x04\x12\x0b\n\x03\x61pp\x18\x02 \x01(\x04:\x04\xe8\xa0\x1f\x01\x42;Z9github.com/tendermint/tendermint/proto/tendermint/versionb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.crypto.keys_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.version.types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z8github.com/tendermint/tendermint/proto/tendermint/crypto'
-  _PUBLICKEY._options = None
-  _PUBLICKEY._serialized_options = b'\350\241\037\001\350\240\037\001'
-  _PUBLICKEY._serialized_start=73
-  _PUBLICKEY._serialized_end=141
+  DESCRIPTOR._serialized_options = b'Z9github.com/tendermint/tendermint/proto/tendermint/version'
+  _CONSENSUS._options = None
+  _CONSENSUS._serialized_options = b'\350\240\037\001'
+  _APP._serialized_start=76
+  _APP._serialized_end=117
+  _CONSENSUS._serialized_start=119
+  _CONSENSUS._serialized_end=164
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/proof.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/crypto/proof.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/proof_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/libs/bits/types_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/crypto/proof.proto
+# source: tendermint/libs/bits/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtendermint/crypto/proof.proto\x12\x11tendermint.crypto\x1a\x14gogoproto/gogo.proto\"G\n\x05Proof\x12\r\n\x05total\x18\x01 \x01(\x03\x12\r\n\x05index\x18\x02 \x01(\x03\x12\x11\n\tleaf_hash\x18\x03 \x01(\x0c\x12\r\n\x05\x61unts\x18\x04 \x03(\x0c\"?\n\x07ValueOp\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\'\n\x05proof\x18\x02 \x01(\x0b\x32\x18.tendermint.crypto.Proof\"6\n\x08\x44ominoOp\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05input\x18\x02 \x01(\t\x12\x0e\n\x06output\x18\x03 \x01(\t\"2\n\x07ProofOp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\x0c\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"9\n\x08ProofOps\x12-\n\x03ops\x18\x01 \x03(\x0b\x32\x1a.tendermint.crypto.ProofOpB\x04\xc8\xde\x1f\x00\x42:Z8github.com/tendermint/tendermint/proto/tendermint/cryptob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tendermint/libs/bits/types.proto\x12\x14tendermint.libs.bits\"\'\n\x08\x42itArray\x12\x0c\n\x04\x62its\x18\x01 \x01(\x03\x12\r\n\x05\x65lems\x18\x02 \x03(\x04\x42=Z;github.com/tendermint/tendermint/proto/tendermint/libs/bitsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.crypto.proof_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.libs.bits.types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z8github.com/tendermint/tendermint/proto/tendermint/crypto'
-  _PROOFOPS.fields_by_name['ops']._options = None
-  _PROOFOPS.fields_by_name['ops']._serialized_options = b'\310\336\037\000'
-  _PROOF._serialized_start=74
-  _PROOF._serialized_end=145
-  _VALUEOP._serialized_start=147
-  _VALUEOP._serialized_end=210
-  _DOMINOOP._serialized_start=212
-  _DOMINOOP._serialized_end=266
-  _PROOFOP._serialized_start=268
-  _PROOFOP._serialized_end=318
-  _PROOFOPS._serialized_start=320
-  _PROOFOPS._serialized_end=377
+  DESCRIPTOR._serialized_options = b'Z;github.com/tendermint/tendermint/proto/tendermint/libs/bits'
+  _BITARRAY._serialized_start=58
+  _BITARRAY._serialized_end=97
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/crypto/proof_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/validator_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,38 @@
 from gogoproto import gogo_pb2 as _gogo_pb2
+from tendermint.crypto import keys_pb2 as _keys_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DominoOp(_message.Message):
-    __slots__ = ["input", "key", "output"]
-    INPUT_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_FIELD_NUMBER: _ClassVar[int]
-    input: str
-    key: str
-    output: str
-    def __init__(self, key: _Optional[str] = ..., input: _Optional[str] = ..., output: _Optional[str] = ...) -> None: ...
-
-class Proof(_message.Message):
-    __slots__ = ["aunts", "index", "leaf_hash", "total"]
-    AUNTS_FIELD_NUMBER: _ClassVar[int]
-    INDEX_FIELD_NUMBER: _ClassVar[int]
-    LEAF_HASH_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_FIELD_NUMBER: _ClassVar[int]
-    aunts: _containers.RepeatedScalarFieldContainer[bytes]
-    index: int
-    leaf_hash: bytes
-    total: int
-    def __init__(self, total: _Optional[int] = ..., index: _Optional[int] = ..., leaf_hash: _Optional[bytes] = ..., aunts: _Optional[_Iterable[bytes]] = ...) -> None: ...
-
-class ProofOp(_message.Message):
-    __slots__ = ["data", "key", "type"]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    data: bytes
-    key: bytes
-    type: str
-    def __init__(self, type: _Optional[str] = ..., key: _Optional[bytes] = ..., data: _Optional[bytes] = ...) -> None: ...
-
-class ProofOps(_message.Message):
-    __slots__ = ["ops"]
-    OPS_FIELD_NUMBER: _ClassVar[int]
-    ops: _containers.RepeatedCompositeFieldContainer[ProofOp]
-    def __init__(self, ops: _Optional[_Iterable[_Union[ProofOp, _Mapping]]] = ...) -> None: ...
-
-class ValueOp(_message.Message):
-    __slots__ = ["key", "proof"]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    PROOF_FIELD_NUMBER: _ClassVar[int]
-    key: bytes
-    proof: Proof
-    def __init__(self, key: _Optional[bytes] = ..., proof: _Optional[_Union[Proof, _Mapping]] = ...) -> None: ...
+class SimpleValidator(_message.Message):
+    __slots__ = ["pub_key", "voting_power"]
+    PUB_KEY_FIELD_NUMBER: _ClassVar[int]
+    VOTING_POWER_FIELD_NUMBER: _ClassVar[int]
+    pub_key: _keys_pb2.PublicKey
+    voting_power: int
+    def __init__(self, pub_key: _Optional[_Union[_keys_pb2.PublicKey, _Mapping]] = ..., voting_power: _Optional[int] = ...) -> None: ...
+
+class Validator(_message.Message):
+    __slots__ = ["address", "proposer_priority", "pub_key", "voting_power"]
+    ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    PROPOSER_PRIORITY_FIELD_NUMBER: _ClassVar[int]
+    PUB_KEY_FIELD_NUMBER: _ClassVar[int]
+    VOTING_POWER_FIELD_NUMBER: _ClassVar[int]
+    address: bytes
+    proposer_priority: int
+    pub_key: _keys_pb2.PublicKey
+    voting_power: int
+    def __init__(self, address: _Optional[bytes] = ..., pub_key: _Optional[_Union[_keys_pb2.PublicKey, _Mapping]] = ..., voting_power: _Optional[int] = ..., proposer_priority: _Optional[int] = ...) -> None: ...
+
+class ValidatorSet(_message.Message):
+    __slots__ = ["proposer", "total_voting_power", "validators"]
+    PROPOSER_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_VOTING_POWER_FIELD_NUMBER: _ClassVar[int]
+    VALIDATORS_FIELD_NUMBER: _ClassVar[int]
+    proposer: Validator
+    total_voting_power: int
+    validators: _containers.RepeatedCompositeFieldContainer[Validator]
+    def __init__(self, validators: _Optional[_Iterable[_Union[Validator, _Mapping]]] = ..., proposer: _Optional[_Union[Validator, _Mapping]] = ..., total_voting_power: _Optional[int] = ...) -> None: ...
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/libs/bits/types_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/store/types_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/libs/bits/types.proto
+# source: tendermint/store/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tendermint/libs/bits/types.proto\x12\x14tendermint.libs.bits\"\'\n\x08\x42itArray\x12\x0c\n\x04\x62its\x18\x01 \x01(\x03\x12\r\n\x05\x65lems\x18\x02 \x03(\x04\x42=Z;github.com/tendermint/tendermint/proto/tendermint/libs/bitsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctendermint/store/types.proto\x12\x10tendermint.store\"/\n\x0f\x42lockStoreState\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\x03\x12\x0e\n\x06height\x18\x02 \x01(\x03\x42\x39Z7github.com/tendermint/tendermint/proto/tendermint/storeb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.libs.bits.types_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.store.types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z;github.com/tendermint/tendermint/proto/tendermint/libs/bits'
-  _BITARRAY._serialized_start=58
-  _BITARRAY._serialized_end=97
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/store'
+  _BLOCKSTORESTATE._serialized_start=50
+  _BLOCKSTORESTATE._serialized_end=97
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/mempool/types_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/mempool/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/conn.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/conn.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/conn_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/pex_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/p2p/conn.proto
+# source: tendermint/p2p/pex.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from tendermint.p2p import types_pb2 as tendermint_dot_p2p_dot_types__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from tendermint.crypto import keys_pb2 as tendermint_dot_crypto_dot_keys__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19tendermint/p2p/conn.proto\x12\x0etendermint.p2p\x1a\x14gogoproto/gogo.proto\x1a\x1ctendermint/crypto/keys.proto\"\x0c\n\nPacketPing\"\x0c\n\nPacketPong\"R\n\tPacketMsg\x12!\n\nchannel_id\x18\x01 \x01(\x05\x42\r\xe2\xde\x1f\tChannelID\x12\x14\n\x03\x65of\x18\x02 \x01(\x08\x42\x07\xe2\xde\x1f\x03\x45OF\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"\xa6\x01\n\x06Packet\x12\x31\n\x0bpacket_ping\x18\x01 \x01(\x0b\x32\x1a.tendermint.p2p.PacketPingH\x00\x12\x31\n\x0bpacket_pong\x18\x02 \x01(\x0b\x32\x1a.tendermint.p2p.PacketPongH\x00\x12/\n\npacket_msg\x18\x03 \x01(\x0b\x32\x19.tendermint.p2p.PacketMsgH\x00\x42\x05\n\x03sum\"R\n\x0e\x41uthSigMessage\x12\x33\n\x07pub_key\x18\x01 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKeyB\x04\xc8\xde\x1f\x00\x12\x0b\n\x03sig\x18\x02 \x01(\x0c\x42\x37Z5github.com/tendermint/tendermint/proto/tendermint/p2pb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tendermint/p2p/pex.proto\x12\x0etendermint.p2p\x1a\x1atendermint/p2p/types.proto\x1a\x14gogoproto/gogo.proto\"\x0c\n\nPexRequest\";\n\x08PexAddrs\x12/\n\x05\x61\x64\x64rs\x18\x01 \x03(\x0b\x32\x1a.tendermint.p2p.NetAddressB\x04\xc8\xde\x1f\x00\"r\n\x07Message\x12\x31\n\x0bpex_request\x18\x01 \x01(\x0b\x32\x1a.tendermint.p2p.PexRequestH\x00\x12-\n\tpex_addrs\x18\x02 \x01(\x0b\x32\x18.tendermint.p2p.PexAddrsH\x00\x42\x05\n\x03sumB7Z5github.com/tendermint/tendermint/proto/tendermint/p2pb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.p2p.conn_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.p2p.pex_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z5github.com/tendermint/tendermint/proto/tendermint/p2p'
-  _PACKETMSG.fields_by_name['channel_id']._options = None
-  _PACKETMSG.fields_by_name['channel_id']._serialized_options = b'\342\336\037\tChannelID'
-  _PACKETMSG.fields_by_name['eof']._options = None
-  _PACKETMSG.fields_by_name['eof']._serialized_options = b'\342\336\037\003EOF'
-  _AUTHSIGMESSAGE.fields_by_name['pub_key']._options = None
-  _AUTHSIGMESSAGE.fields_by_name['pub_key']._serialized_options = b'\310\336\037\000'
-  _PACKETPING._serialized_start=97
-  _PACKETPING._serialized_end=109
-  _PACKETPONG._serialized_start=111
-  _PACKETPONG._serialized_end=123
-  _PACKETMSG._serialized_start=125
-  _PACKETMSG._serialized_end=207
-  _PACKET._serialized_start=210
-  _PACKET._serialized_end=376
-  _AUTHSIGMESSAGE._serialized_start=378
-  _AUTHSIGMESSAGE._serialized_end=460
+  _PEXADDRS.fields_by_name['addrs']._options = None
+  _PEXADDRS.fields_by_name['addrs']._serialized_options = b'\310\336\037\000'
+  _PEXREQUEST._serialized_start=94
+  _PEXREQUEST._serialized_end=106
+  _PEXADDRS._serialized_start=108
+  _PEXADDRS._serialized_end=167
+  _MESSAGE._serialized_start=169
+  _MESSAGE._serialized_end=283
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/pex_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/events_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/p2p/pex.proto
+# source: tendermint/types/events.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from tendermint.p2p import types_pb2 as tendermint_dot_p2p_dot_types__pb2
-from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18tendermint/p2p/pex.proto\x12\x0etendermint.p2p\x1a\x1atendermint/p2p/types.proto\x1a\x14gogoproto/gogo.proto\"\x0c\n\nPexRequest\";\n\x08PexAddrs\x12/\n\x05\x61\x64\x64rs\x18\x01 \x03(\x0b\x32\x1a.tendermint.p2p.NetAddressB\x04\xc8\xde\x1f\x00\"r\n\x07Message\x12\x31\n\x0bpex_request\x18\x01 \x01(\x0b\x32\x1a.tendermint.p2p.PexRequestH\x00\x12-\n\tpex_addrs\x18\x02 \x01(\x0b\x32\x18.tendermint.p2p.PexAddrsH\x00\x42\x05\n\x03sumB7Z5github.com/tendermint/tendermint/proto/tendermint/p2pb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtendermint/types/events.proto\x12\x10tendermint.types\"B\n\x13\x45ventDataRoundState\x12\x0e\n\x06height\x18\x01 \x01(\x03\x12\r\n\x05round\x18\x02 \x01(\x05\x12\x0c\n\x04step\x18\x03 \x01(\tB9Z7github.com/tendermint/tendermint/proto/tendermint/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.p2p.pex_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.events_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/tendermint/tendermint/proto/tendermint/p2p'
-  _PEXADDRS.fields_by_name['addrs']._options = None
-  _PEXADDRS.fields_by_name['addrs']._serialized_options = b'\310\336\037\000'
-  _PEXREQUEST._serialized_start=94
-  _PEXREQUEST._serialized_end=106
-  _PEXADDRS._serialized_start=108
-  _PEXADDRS._serialized_end=167
-  _MESSAGE._serialized_start=169
-  _MESSAGE._serialized_end=283
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types'
+  _EVENTDATAROUNDSTATE._serialized_start=51
+  _EVENTDATAROUNDSTATE._serialized_end=117
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/p2p/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/p2p/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/privval/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/privval/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/privval/types_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/privval/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/rpc/grpc/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/rpc/grpc/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/rpc/grpc/types_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/rpc/grpc/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/state/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/state/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/state/types_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/state/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/statesync/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/statesync/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/store/types_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/plan/v1/params_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/store/types.proto
+# source: sentinel/plan/v1/params.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctendermint/store/types.proto\x12\x10tendermint.store\"/\n\x0f\x42lockStoreState\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\x03\x12\x0e\n\x06height\x18\x02 \x01(\x03\x42\x39Z7github.com/tendermint/tendermint/proto/tendermint/storeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dsentinel/plan/v1/params.proto\x12\x10sentinel.plan.v1B/Z-github.com/sentinel-official/hub/x/plan/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.store.types_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.plan.v1.params_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/store'
-  _BLOCKSTORESTATE._serialized_start=50
-  _BLOCKSTORESTATE._serialized_end=97
+  DESCRIPTOR._serialized_options = b'Z-github.com/sentinel-official/hub/x/plan/types'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/block.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/block.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/block_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/canonical.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/canonical.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/events_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/sentinel/deposit/v1/params_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/types/events.proto
+# source: sentinel/deposit/v1/params.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtendermint/types/events.proto\x12\x10tendermint.types\"B\n\x13\x45ventDataRoundState\x12\x0e\n\x06height\x18\x01 \x01(\x03\x12\r\n\x05round\x18\x02 \x01(\x05\x12\x0c\n\x04step\x18\x03 \x01(\tB9Z7github.com/tendermint/tendermint/proto/tendermint/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n sentinel/deposit/v1/params.proto\x12\x13sentinel.deposit.v1B2Z0github.com/sentinel-official/hub/x/deposit/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.events_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentinel.deposit.v1.params_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types'
-  _EVENTDATAROUNDSTATE._serialized_start=51
-  _EVENTDATAROUNDSTATE._serialized_end=117
+  DESCRIPTOR._serialized_options = b'Z0github.com/sentinel-official/hub/x/deposit/types'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/evidence.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/evidence.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/params.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/params.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/types_pb2.py` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/types_pb2.pyi` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/types/validator.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/types/validator.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/src/sentinel_protobuf/tendermint/version/types.proto` & `sentinel_protobuf-0.2.1/src/sentinel_protobuf/tendermint/version/types.proto`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/README.md` & `sentinel_protobuf-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sentinel_protobuf-0.2.0/pyproject.toml` & `sentinel_protobuf-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sentinel_protobuf"
-version = "0.2.0"
+version = "0.2.1"
 description = "This package contains a compiled python version of all sentinel protobuf files with their dependencies"
 authors = [
     { name = "freQniK", email = "freQniK@mathnodes.com" },
 ]
 readme = "README.md"
 keywords = ["cosmospy", "proto", "cosmospy-protobuf", "cosmos", "sentinel-protobuf", "protobuf", "sentinel"]
 license = {text = "BSD 3-Clause License"}
```

### Comparing `sentinel_protobuf-0.2.0/PKG-INFO` & `sentinel_protobuf-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentinel_protobuf
-Version: 0.2.0
+Version: 0.2.1
 Summary: This package contains a compiled python version of all sentinel protobuf files with their dependencies
 Project-URL: Homepage, https://github.com/MathNodes/cosmospy-protobuf/
 Project-URL: Bug Tracker, https://github.com/MathNodes/cosmospy-protobuf/issues
 Author-email: freQniK <freQniK@mathnodes.com>
 License: BSD 3-Clause License
 Keywords: cosmos,cosmospy,cosmospy-protobuf,proto,protobuf,sentinel,sentinel-protobuf
 Classifier: Operating System :: OS Independent
```

