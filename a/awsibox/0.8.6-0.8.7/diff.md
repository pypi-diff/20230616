# Comparing `tmp/awsibox-0.8.6.tar.gz` & `tmp/awsibox-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsibox-0.8.6.tar", last modified: Fri Jun 16 09:27:16 2023, max compression
+gzip compressed data, was "awsibox-0.8.7.tar", last modified: Fri Jun 16 09:29:31 2023, max compression
```

## Comparing `awsibox-0.8.6.tar` & `awsibox-0.8.7.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.295170 awsibox-0.8.6/
--rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.6/.gitignore
--rw-r--r--   0 mello     (1000) mello     (1000)      257 2023-06-16 08:09:06.000000 awsibox-0.8.6/MANIFEST.in
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-16 09:27:16.295170 awsibox-0.8.6/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.6/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.191169 awsibox-0.8.6/awsibox/
--rw-r--r--   0 mello     (1000) mello     (1000)    19452 2023-06-15 12:57:11.000000 awsibox-0.8.6/awsibox/RP.py
--rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-06-16 09:26:49.000000 awsibox-0.8.6/awsibox/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.6/awsibox/args.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.191169 awsibox-0.8.6/awsibox/aws/
--rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/aws/CloudFormationResourceSpecification.json
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.175168 awsibox-0.8.6/awsibox/cfg/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.183169 awsibox-0.8.6/awsibox/cfg/ibox/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.223169 awsibox-0.8.6/awsibox/cfg/ibox/com/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.227169 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/capacity.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1252 2023-06-16 09:13:11.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.227169 awsibox-0.8.6/awsibox/cfg/ibox/com/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.227169 awsibox-0.8.6/awsibox/cfg/ibox/com/cloudformation/
--rw-r--r--   0 mello     (1000) mello     (1000)      658 2023-06-06 14:25:53.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.227169 awsibox-0.8.6/awsibox/cfg/ibox/com/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     1521 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1656 2023-06-14 15:23:58.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/cloudfront/for-services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      121 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/cloudfront/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.227169 awsibox-0.8.6/awsibox/cfg/ibox/com/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1810 2023-06-16 09:12:56.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/common.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.231169 awsibox-0.8.6/awsibox/cfg/ibox/com/dynamodb/
--rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.231169 awsibox-0.8.6/awsibox/cfg/ibox/com/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ec2/securitygroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.235169 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1414 2023-06-14 16:05:45.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3140 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6894 2023-06-14 16:14:09.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      899 2023-06-14 16:05:02.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.235169 awsibox-0.8.6/awsibox/cfg/ibox/com/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.235169 awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.239169 awsibox-0.8.6/awsibox/cfg/ibox/com/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-05-01 13:36:02.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/events/ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/events/ecs-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-05-01 13:33:03.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/events/ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/events/spot_advisor.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.239169 awsibox-0.8.6/awsibox/cfg/ibox/com/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.239169 awsibox-0.8.6/awsibox/cfg/ibox/com/kms/
--rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.243169 awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/layers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/py-packager.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.243169 awsibox-0.8.6/awsibox/cfg/ibox/com/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.243169 awsibox-0.8.6/awsibox/cfg/ibox/com/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/s3/bucket-log.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.243169 awsibox-0.8.6/awsibox/cfg/ibox/com/servicediscovery/
--rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.247170 awsibox-0.8.6/awsibox/cfg/ibox/com/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.247170 awsibox-0.8.6/awsibox/cfg/ibox/com/ssm/
--rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.183169 awsibox-0.8.6/awsibox/cfg/ibox/res/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.247170 awsibox-0.8.6/awsibox/cfg/ibox/res/apigateway/
--rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/apigateway/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/apigateway/deployments.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/apigateway/domain-names.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.247170 awsibox-0.8.6/awsibox/cfg/ibox/res/application-autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2965 2023-06-14 15:41:11.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.251170 awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-06-14 15:45:22.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5137 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.251170 awsibox-0.8.6/awsibox/cfg/ibox/res/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.251170 awsibox-0.8.6/awsibox/cfg/ibox/res/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     4829 2023-06-14 15:51:31.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      243 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/cloudfront/policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.255170 awsibox-0.8.6/awsibox/cfg/ibox/res/cloudwatch/
--rw-r--r--   0 mello     (1000) mello     (1000)     7727 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1041 2023-06-14 15:57:15.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.255170 awsibox-0.8.6/awsibox/cfg/ibox/res/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1081 2023-06-14 16:01:55.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.255170 awsibox-0.8.6/awsibox/cfg/ibox/res/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)      160 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/ec2/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.255170 awsibox-0.8.6/awsibox/cfg/ibox/res/ecr/
--rw-r--r--   0 mello     (1000) mello     (1000)      136 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/ecr/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/ecr/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.255170 awsibox-0.8.6/awsibox/cfg/ibox/res/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     9924 2023-06-14 16:06:44.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/ecs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/ecs/services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1021 2023-06-06 14:25:53.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.259170 awsibox-0.8.6/awsibox/cfg/ibox/res/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/efs/filesystems.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      561 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/efs/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.259170 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticache/
--rw-r--r--   0 mello     (1000) mello     (1000)     5327 2023-05-31 09:04:53.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.259170 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     4187 2023-06-14 16:14:27.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4552 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2962 2023-06-06 14:25:53.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.259170 awsibox-0.8.6/awsibox/cfg/ibox/res/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/events/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.263170 awsibox-0.8.6/awsibox/cfg/ibox/res/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     2364 2023-06-14 16:17:13.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/iam/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/iam/instance-profiles.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/iam/policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.263170 awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/functions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2591 2023-06-14 16:23:01.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/versions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.267170 awsibox-0.8.6/awsibox/cfg/ibox/res/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     8105 2023-05-10 15:52:15.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/rds/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.267170 awsibox-0.8.6/awsibox/cfg/ibox/res/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/route53/hostedzones.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/route53/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     7638 2023-06-14 15:16:13.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/route53/recordsets.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.267170 awsibox-0.8.6/awsibox/cfg/ibox/res/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)     2808 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/s3/bucket-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     8088 2023-06-15 07:52:15.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/s3/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.267170 awsibox-0.8.6/awsibox/cfg/ibox/res/scheduler/
--rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.267170 awsibox-0.8.6/awsibox/cfg/ibox/res/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      449 2023-06-14 16:29:21.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/sns/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/sns/subscriptions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.271170 awsibox-0.8.6/awsibox/cfg/ibox/res/sqs/
--rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/sqs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/res/sqs/queue-policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.183169 awsibox-0.8.6/awsibox/cfg/ibox/stacks/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.271170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/agw/
--rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/agw/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/agw/infra-info.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.271170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/cch/
--rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/cch/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.271170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/clf/
--rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/clf/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.271170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     4594 2023-05-11 09:07:31.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3294 2023-06-15 07:55:39.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/ec2/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.271170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-15 07:56:29.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2378 2023-06-14 16:05:52.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/ecs/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-15 07:55:51.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.275170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/lbd/
--rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.275170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      209 2023-06-14 15:24:08.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/rds/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.279170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/
--rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-06-15 07:57:04.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-event-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      559 2023-06-16 09:17:19.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      910 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2152 2023-06-16 09:17:10.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/vpc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.279170 awsibox-0.8.6/awsibox/cfg/ibox/stacks/tsk/
--rw-r--r--   0 mello     (1000) mello     (1000)     2459 2023-06-14 16:36:55.000000 awsibox-0.8.6/awsibox/cfg/ibox/stacks/tsk/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    16806 2023-06-16 09:12:22.000000 awsibox-0.8.6/awsibox/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1685 2023-04-17 10:03:18.000000 awsibox-0.8.6/awsibox/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.6/awsibox/discover.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2421 2023-06-16 08:07:40.000000 awsibox-0.8.6/awsibox/generate.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.287170 awsibox-0.8.6/awsibox/lambdas/
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.6/awsibox/lambdas/ASGSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.6/awsibox/lambdas/AtEdgeAddHeaders.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.6/awsibox/lambdas/CCRFargateSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.6/awsibox/lambdas/CCRLightHouse.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.6/awsibox/lambdas/CCRStackReplicator.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.6/awsibox/lambdas/CloudWatchAlarmStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.6/awsibox/lambdas/CloudWatchRepeatedNotify.code
--rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.6/awsibox/lambdas/EC2StartStopTagged.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.6/awsibox/lambdas/ECSClusterAutoscale.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.6/awsibox/lambdas/ECSDrainInstance.code
--rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.6/awsibox/lambdas/ECSDrainTasks.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.6/awsibox/lambdas/ECSEventTaskStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.6/awsibox/lambdas/ECSEventsSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.6/awsibox/lambdas/ECSRaiseASGAlarm.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.6/awsibox/lambdas/ECSRunTask.code
--rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.6/awsibox/lambdas/ECSUpdateDesiredCount.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.6/awsibox/lambdas/ElasticSearchSnapShot.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5370 2023-06-07 12:49:30.000000 awsibox-0.8.6/awsibox/lambdas/InfraInfo.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.6/awsibox/lambdas/ManageService.code
--rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.6/awsibox/lambdas/PaidApi.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.6/awsibox/lambdas/PyPackager.code
--rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.6/awsibox/lambdas/Python37SSM.layer
--rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.6/awsibox/lambdas/R53RecordInstanceId.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.6/awsibox/lambdas/ServiceDiscovery.code
--rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.6/awsibox/lambdas/ServiceUnavailable.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.6/awsibox/lambdas/StacksOps.code
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.291170 awsibox-0.8.6/awsibox/mod/
--rw-r--r--   0 mello     (1000) mello     (1000)     3962 2023-06-16 08:24:34.000000 awsibox-0.8.6/awsibox/mod/autoscaling.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3746 2023-06-16 09:25:14.000000 awsibox-0.8.6/awsibox/mod/cloudformation.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2169 2023-06-16 08:27:11.000000 awsibox-0.8.6/awsibox/mod/cloudfront.py
--rw-r--r--   0 mello     (1000) mello     (1000)    13198 2023-06-16 08:28:25.000000 awsibox-0.8.6/awsibox/mod/ec2.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2353 2023-06-16 08:28:54.000000 awsibox-0.8.6/awsibox/mod/ecr.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2829 2023-06-16 08:29:28.000000 awsibox-0.8.6/awsibox/mod/efs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5205 2023-06-16 08:30:20.000000 awsibox-0.8.6/awsibox/mod/elasticloadbalancing.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3320 2023-06-16 08:30:51.000000 awsibox-0.8.6/awsibox/mod/iam.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2945 2023-06-16 08:14:41.000000 awsibox-0.8.6/awsibox/mod/joker.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5849 2023-06-16 08:32:12.000000 awsibox-0.8.6/awsibox/mod/rds.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2674 2023-06-16 08:32:47.000000 awsibox-0.8.6/awsibox/mod/s3.py
--rw-r--r--   0 mello     (1000) mello     (1000)     7926 2023-06-16 08:33:12.000000 awsibox-0.8.6/awsibox/mod/waf.py
--rw-r--r--   0 mello     (1000) mello     (1000)    46030 2023-06-09 13:02:41.000000 awsibox-0.8.6/awsibox/shared.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.291170 awsibox-0.8.6/awsibox/user-data/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.295170 awsibox-0.8.6/awsibox/user-data/SCRIPTS/
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.6/awsibox/user-data/SCRIPTS/ELBCHECK.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.6/awsibox/user-data/SCRIPTS/END.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.6/awsibox/user-data/SCRIPTS/INIT.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.6/awsibox/user-data/SCRIPTS/PACKAGE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.6/awsibox/user-data/SCRIPTS/SERVICE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.6/awsibox/user-data/SCRIPTS/SETUP.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.6/awsibox/user-data/ecs-cluster.sh
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.175168 awsibox-0.8.6/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.175168 awsibox-0.8.6/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.187169 awsibox-0.8.6/build/lib/awsibox.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-16 09:27:15.000000 awsibox-0.8.6/build/lib/awsibox.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)     8805 2023-06-16 09:27:15.000000 awsibox-0.8.6/build/lib/awsibox.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-06-16 09:27:15.000000 awsibox-0.8.6/build/lib/awsibox.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-06-16 09:27:15.000000 awsibox-0.8.6/build/lib/awsibox.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-06-16 09:27:15.000000 awsibox-0.8.6/build/lib/awsibox.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:27:16.295170 awsibox-0.8.6/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)     3350 2023-06-15 12:57:11.000000 awsibox-0.8.6/scripts/ibox_generate_templates.py
--rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-06-16 09:27:16.295170 awsibox-0.8.6/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      536 2023-06-16 08:09:19.000000 awsibox-0.8.6/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.393291 awsibox-0.8.7/
+-rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.7/.gitignore
+-rw-r--r--   0 mello     (1000) mello     (1000)      257 2023-06-16 08:09:06.000000 awsibox-0.8.7/MANIFEST.in
+-rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-16 09:29:31.393291 awsibox-0.8.7/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.7/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.277289 awsibox-0.8.7/awsibox/
+-rw-r--r--   0 mello     (1000) mello     (1000)    19452 2023-06-15 12:57:11.000000 awsibox-0.8.7/awsibox/RP.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-06-16 09:28:20.000000 awsibox-0.8.7/awsibox/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.7/awsibox/args.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.281289 awsibox-0.8.7/awsibox/aws/
+-rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/aws/CloudFormationResourceSpecification.json
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.265289 awsibox-0.8.7/awsibox/cfg/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.273289 awsibox-0.8.7/awsibox/cfg/ibox/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.313290 awsibox-0.8.7/awsibox/cfg/ibox/com/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.317290 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/capacity.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1252 2023-06-16 09:13:11.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudformation/
+-rw-r--r--   0 mello     (1000) mello     (1000)      658 2023-06-06 14:25:53.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1521 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1656 2023-06-14 15:23:58.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/for-services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      121 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1810 2023-06-16 09:12:56.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/common.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/dynamodb/
+-rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.325290 awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/securitygroup.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.329290 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1414 2023-06-14 16:05:45.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3140 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6894 2023-06-14 16:14:09.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      899 2023-06-14 16:05:02.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.329290 awsibox-0.8.7/awsibox/cfg/ibox/com/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.329290 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.333290 awsibox-0.8.7/awsibox/cfg/ibox/com/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-05-01 13:36:02.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-05-01 13:33:03.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/spot_advisor.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.333290 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.337290 awsibox-0.8.7/awsibox/cfg/ibox/com/kms/
+-rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.337290 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/layers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/py-packager.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/s3/bucket-log.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/servicediscovery/
+-rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.273289 awsibox-0.8.7/awsibox/cfg/ibox/res/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/
+-rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/deployments.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/domain-names.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.345291 awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2965 2023-06-14 15:41:11.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.345291 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-06-14 15:45:22.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5137 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.345291 awsibox-0.8.7/awsibox/cfg/ibox/res/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4829 2023-06-14 15:51:31.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      243 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/
+-rw-r--r--   0 mello     (1000) mello     (1000)     7727 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1041 2023-06-14 15:57:15.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1081 2023-06-14 16:01:55.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      160 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ec2/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/ecr/
+-rw-r--r--   0 mello     (1000) mello     (1000)      136 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecr/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecr/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.353291 awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     9924 2023-06-14 16:06:44.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1021 2023-06-06 14:25:53.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.353291 awsibox-0.8.7/awsibox/cfg/ibox/res/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/efs/filesystems.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      561 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/efs/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.353291 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticache/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5327 2023-05-31 09:04:53.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.357291 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4187 2023-06-14 16:14:27.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4552 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2962 2023-06-06 14:25:53.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.357291 awsibox-0.8.7/awsibox/cfg/ibox/res/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/events/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.357291 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2364 2023-06-14 16:17:13.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/instance-profiles.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.357291 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/functions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2591 2023-06-14 16:23:01.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/versions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     8105 2023-05-10 15:52:15.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/rds/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/route53/hostedzones.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/route53/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     7638 2023-06-14 15:16:13.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/route53/recordsets.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2808 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/s3/bucket-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     8088 2023-06-15 07:52:15.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/s3/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/scheduler/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      449 2023-06-14 16:29:21.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/sns/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/sns/subscriptions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/res/sqs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/sqs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/sqs/queue-policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.273289 awsibox-0.8.7/awsibox/cfg/ibox/stacks/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/infra-info.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/cch/
+-rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/cch/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/clf/
+-rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/clf/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4594 2023-05-11 09:07:31.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3294 2023-06-15 07:55:39.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.369291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-15 07:56:29.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2378 2023-06-14 16:05:52.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-15 07:55:51.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.369291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/lbd/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.369291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      209 2023-06-14 15:24:08.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/rds/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.373291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/
+-rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-06-15 07:57:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-event-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      559 2023-06-16 09:17:19.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      910 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2152 2023-06-16 09:17:10.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/vpc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.373291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/tsk/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2459 2023-06-14 16:36:55.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/tsk/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    16806 2023-06-16 09:12:22.000000 awsibox-0.8.7/awsibox/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1685 2023-04-17 10:03:18.000000 awsibox-0.8.7/awsibox/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/discover.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2407 2023-06-16 09:27:54.000000 awsibox-0.8.7/awsibox/generate.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.385291 awsibox-0.8.7/awsibox/lambdas/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/ASGSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/AtEdgeAddHeaders.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.7/awsibox/lambdas/CCRFargateSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.7/awsibox/lambdas/CCRLightHouse.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.7/awsibox/lambdas/CCRStackReplicator.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.7/awsibox/lambdas/CloudWatchAlarmStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.7/awsibox/lambdas/CloudWatchRepeatedNotify.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/EC2StartStopTagged.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.7/awsibox/lambdas/ECSClusterAutoscale.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.7/awsibox/lambdas/ECSDrainInstance.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.7/awsibox/lambdas/ECSDrainTasks.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.7/awsibox/lambdas/ECSEventTaskStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.7/awsibox/lambdas/ECSEventsSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.7/awsibox/lambdas/ECSRaiseASGAlarm.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.7/awsibox/lambdas/ECSRunTask.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/ECSUpdateDesiredCount.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/ElasticSearchSnapShot.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5370 2023-06-07 12:49:30.000000 awsibox-0.8.7/awsibox/lambdas/InfraInfo.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.7/awsibox/lambdas/ManageService.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/PaidApi.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.7/awsibox/lambdas/PyPackager.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/Python37SSM.layer
+-rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.7/awsibox/lambdas/R53RecordInstanceId.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.7/awsibox/lambdas/ServiceDiscovery.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.7/awsibox/lambdas/ServiceUnavailable.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.7/awsibox/lambdas/StacksOps.code
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.389291 awsibox-0.8.7/awsibox/mod/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3962 2023-06-16 08:24:34.000000 awsibox-0.8.7/awsibox/mod/autoscaling.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3746 2023-06-16 09:25:14.000000 awsibox-0.8.7/awsibox/mod/cloudformation.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2169 2023-06-16 08:27:11.000000 awsibox-0.8.7/awsibox/mod/cloudfront.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    13198 2023-06-16 08:28:25.000000 awsibox-0.8.7/awsibox/mod/ec2.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2353 2023-06-16 08:28:54.000000 awsibox-0.8.7/awsibox/mod/ecr.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2829 2023-06-16 08:29:28.000000 awsibox-0.8.7/awsibox/mod/efs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5205 2023-06-16 08:30:20.000000 awsibox-0.8.7/awsibox/mod/elasticloadbalancing.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3320 2023-06-16 08:30:51.000000 awsibox-0.8.7/awsibox/mod/iam.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2945 2023-06-16 08:14:41.000000 awsibox-0.8.7/awsibox/mod/joker.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5849 2023-06-16 08:32:12.000000 awsibox-0.8.7/awsibox/mod/rds.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2674 2023-06-16 08:32:47.000000 awsibox-0.8.7/awsibox/mod/s3.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     7926 2023-06-16 08:33:12.000000 awsibox-0.8.7/awsibox/mod/waf.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    46030 2023-06-09 13:02:41.000000 awsibox-0.8.7/awsibox/shared.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.389291 awsibox-0.8.7/awsibox/user-data/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.393291 awsibox-0.8.7/awsibox/user-data/SCRIPTS/
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/ELBCHECK.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/END.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/INIT.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/PACKAGE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/SERVICE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/SETUP.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.7/awsibox/user-data/ecs-cluster.sh
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.265289 awsibox-0.8.7/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.265289 awsibox-0.8.7/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.277289 awsibox-0.8.7/build/lib/awsibox.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)     8805 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.393291 awsibox-0.8.7/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     3350 2023-06-15 12:57:11.000000 awsibox-0.8.7/scripts/ibox_generate_templates.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-06-16 09:29:31.393291 awsibox-0.8.7/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      536 2023-06-16 08:09:19.000000 awsibox-0.8.7/setup.py
```

### Comparing `awsibox-0.8.6/.gitignore` & `awsibox-0.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/PKG-INFO` & `awsibox-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.6
+Version: 0.8.7
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBox
         AwsIBox - **AWS** **I**nfrastructure in a **Box**
```

### Comparing `awsibox-0.8.6/awsibox/RP.py` & `awsibox-0.8.7/awsibox/RP.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/args.py` & `awsibox-0.8.7/awsibox/args.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/aws/CloudFormationResourceSpecification.json` & `awsibox-0.8.7/awsibox/aws/CloudFormationResourceSpecification.json`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/capacity.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/capacity.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/cloudfront/for-services.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/for-services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/common.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/common.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ec2/bottlerocket.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/bottlerocket.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/capacityprovider.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/capacityprovider.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/fargate-spot.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/ecs/task.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/task.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/events/cluster-autoscale.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/events/cluster-autoscale.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/events/ec2.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/events/ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/events/ecs-spot.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/events/ecs.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/events/spot_advisor.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/events/spot_advisor.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/iam/managed-policies.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/iam/policy-update_stack.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-update_stack.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/iam/roles.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/py-packager.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/py-packager.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/lambda/service-unavailable.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/service-unavailable.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/s3/bucket-log.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/s3/bucket-log.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/apigateway/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/cloudfront/policies.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/cloudwatch/alarms.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/alarms.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/ecr/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/ecr/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/ecs/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/ecs/services.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/efs/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/efs/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/elasticache/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticache/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/events/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/events/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/iam/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/iam/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/iam/managed-policies.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/iam/policies.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/iam/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/iam/roles.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/functions.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/functions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/permissions.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/permissions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/lambda/versions.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/versions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/rds/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/rds/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/route53/hostedzones.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/route53/hostedzones.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/route53/recordsets.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/route53/recordsets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/s3/bucket-policies.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/s3/bucket-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/s3/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/s3/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/scheduler/ibox_base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/scheduler/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/sns/subscriptions.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/sns/subscriptions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/res/sqs/queue-policies.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/res/sqs/queue-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/agw/i_type.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/agw/infra-info.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/infra-info.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/ec2/i_type.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/ecs/buildkite.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/buildkite.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/ecs/i_type.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-base.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-extra-01.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-extra-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/res/vpc.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/vpc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg/ibox/stacks/tsk/i_type.yml` & `awsibox-0.8.7/awsibox/cfg/ibox/stacks/tsk/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/cfg.py` & `awsibox-0.8.7/awsibox/cfg.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/common.py` & `awsibox-0.8.7/awsibox/common.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/discover.py` & `awsibox-0.8.7/awsibox/discover.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/generate.py` & `awsibox-0.8.7/awsibox/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     cloudfront,
     ec2,
     ecr,
     efs,
     iam,
     joker,
     elasticloadbalancing,
-    mappings,
     rds,
     s3,
     waf,
 )
 
 
 def execute_method(RP_cmm):
```

### Comparing `awsibox-0.8.6/awsibox/lambdas/ASGSpot.code` & `awsibox-0.8.7/awsibox/lambdas/ASGSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/AtEdgeAddHeaders.code` & `awsibox-0.8.7/awsibox/lambdas/AtEdgeAddHeaders.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/CCRFargateSpot.code` & `awsibox-0.8.7/awsibox/lambdas/CCRFargateSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/CCRLightHouse.code` & `awsibox-0.8.7/awsibox/lambdas/CCRLightHouse.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/CCRStackReplicator.code` & `awsibox-0.8.7/awsibox/lambdas/CCRStackReplicator.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/CloudWatchAlarmStateChange.code` & `awsibox-0.8.7/awsibox/lambdas/CloudWatchAlarmStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/CloudWatchRepeatedNotify.code` & `awsibox-0.8.7/awsibox/lambdas/CloudWatchRepeatedNotify.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/EC2StartStopTagged.code` & `awsibox-0.8.7/awsibox/lambdas/EC2StartStopTagged.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ECSClusterAutoscale.code` & `awsibox-0.8.7/awsibox/lambdas/ECSClusterAutoscale.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ECSDrainInstance.code` & `awsibox-0.8.7/awsibox/lambdas/ECSDrainInstance.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ECSDrainTasks.code` & `awsibox-0.8.7/awsibox/lambdas/ECSDrainTasks.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ECSEventTaskStateChange.code` & `awsibox-0.8.7/awsibox/lambdas/ECSEventTaskStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ECSEventsSpot.code` & `awsibox-0.8.7/awsibox/lambdas/ECSEventsSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ECSRaiseASGAlarm.code` & `awsibox-0.8.7/awsibox/lambdas/ECSRaiseASGAlarm.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ECSRunTask.code` & `awsibox-0.8.7/awsibox/lambdas/ECSRunTask.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ECSUpdateDesiredCount.code` & `awsibox-0.8.7/awsibox/lambdas/ECSUpdateDesiredCount.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ElasticSearchSnapShot.code` & `awsibox-0.8.7/awsibox/lambdas/ElasticSearchSnapShot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/InfraInfo.code` & `awsibox-0.8.7/awsibox/lambdas/InfraInfo.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ManageService.code` & `awsibox-0.8.7/awsibox/lambdas/ManageService.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/PaidApi.code` & `awsibox-0.8.7/awsibox/lambdas/PaidApi.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/PyPackager.code` & `awsibox-0.8.7/awsibox/lambdas/PyPackager.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/Python37SSM.layer` & `awsibox-0.8.7/awsibox/lambdas/Python37SSM.layer`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/R53RecordInstanceId.code` & `awsibox-0.8.7/awsibox/lambdas/R53RecordInstanceId.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ServiceDiscovery.code` & `awsibox-0.8.7/awsibox/lambdas/ServiceDiscovery.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/ServiceUnavailable.code` & `awsibox-0.8.7/awsibox/lambdas/ServiceUnavailable.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/lambdas/StacksOps.code` & `awsibox-0.8.7/awsibox/lambdas/StacksOps.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/autoscaling.py` & `awsibox-0.8.7/awsibox/mod/autoscaling.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/cloudformation.py` & `awsibox-0.8.7/awsibox/mod/cloudformation.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/cloudfront.py` & `awsibox-0.8.7/awsibox/mod/cloudfront.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/ec2.py` & `awsibox-0.8.7/awsibox/mod/ec2.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/ecr.py` & `awsibox-0.8.7/awsibox/mod/ecr.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/efs.py` & `awsibox-0.8.7/awsibox/mod/efs.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/elasticloadbalancing.py` & `awsibox-0.8.7/awsibox/mod/elasticloadbalancing.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/iam.py` & `awsibox-0.8.7/awsibox/mod/iam.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/joker.py` & `awsibox-0.8.7/awsibox/mod/joker.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/rds.py` & `awsibox-0.8.7/awsibox/mod/rds.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/s3.py` & `awsibox-0.8.7/awsibox/mod/s3.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/mod/waf.py` & `awsibox-0.8.7/awsibox/mod/waf.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/shared.py` & `awsibox-0.8.7/awsibox/shared.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/user-data/SCRIPTS/ELBCHECK.sh` & `awsibox-0.8.7/awsibox/user-data/SCRIPTS/ELBCHECK.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/user-data/SCRIPTS/END.sh` & `awsibox-0.8.7/awsibox/user-data/SCRIPTS/END.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/user-data/SCRIPTS/INIT.sh` & `awsibox-0.8.7/awsibox/user-data/SCRIPTS/INIT.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/user-data/SCRIPTS/PACKAGE.sh` & `awsibox-0.8.7/awsibox/user-data/SCRIPTS/PACKAGE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/user-data/SCRIPTS/SERVICE.sh` & `awsibox-0.8.7/awsibox/user-data/SCRIPTS/SERVICE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/user-data/SCRIPTS/SETUP.sh` & `awsibox-0.8.7/awsibox/user-data/SCRIPTS/SETUP.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/awsibox/user-data/ecs-cluster.sh` & `awsibox-0.8.7/awsibox/user-data/ecs-cluster.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/build/lib/awsibox.egg-info/PKG-INFO` & `awsibox-0.8.7/build/lib/awsibox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.6
+Version: 0.8.7
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBox
         AwsIBox - **AWS** **I**nfrastructure in a **Box**
```

### Comparing `awsibox-0.8.6/build/lib/awsibox.egg-info/SOURCES.txt` & `awsibox-0.8.7/build/lib/awsibox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/scripts/ibox_generate_templates.py` & `awsibox-0.8.7/scripts/ibox_generate_templates.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/setup.cfg` & `awsibox-0.8.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.6/setup.py` & `awsibox-0.8.7/setup.py`

 * *Files identical despite different names*

