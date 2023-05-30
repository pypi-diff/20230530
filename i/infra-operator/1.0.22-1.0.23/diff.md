# Comparing `tmp/infra_operator-1.0.22.tar.gz` & `tmp/infra_operator-1.0.23.tar.gz`

## Comparing `infra_operator-1.0.22.tar` & `infra_operator-1.0.23.tar`

### file list

```diff
@@ -1,36 +1,321 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/__init__.py
--rw-r--r--   0        0        0     9571 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/clients/__init__.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/clients/ghe.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/clients/mod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/create/__init__.py
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/create/aws_appmesh.py
--rwxr-xr-x   0        0        0    10656 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/create/aws_elbv2_create.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/create/aws_secretsmanager.py
--rw-r--r--   0        0        0    15214 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/create/mod.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/delete/mod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/diff/__init__.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/diff/mod.py
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/export/mod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/layout/__init__.py
--rwxr-xr-x   0        0        0     8297 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/layout/mod.py
--rwxr-xr-x   0        0        0    18727 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/operators/mod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/plugins/mod.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/plugins/wea_notify.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/preprocess/__init__.py
--rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/preprocess/mod.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/preprocess/verify.py
--rwxr-xr-x   0        0        0    19741 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/read/mod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/update/__init__.py
--rwxr-xr-x   0        0        0     2835 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/update/aws_iam_update.py
--rwxr-xr-x   0        0        0     4979 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/update/aws_sg_update.py
--rwxr-xr-x   0        0        0     1268 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/update/ghe_update.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/update/mod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/utils/__init__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/utils/dump.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 infra_operator-1.0.22/api_to_yaml/validate/mod.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 infra_operator-1.0.22/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 infra_operator-1.0.22/LICENSE
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 infra_operator-1.0.22/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 infra_operator-1.0.22/pyproject.toml
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 infra_operator-1.0.22/PKG-INFO
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 infra_operator-1.0.23/layout.yaml
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 infra_operator-1.0.23/path.txt
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 infra_operator-1.0.23/requirements.txt
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 infra_operator-1.0.23/user-data.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 infra_operator-1.0.23/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 infra_operator-1.0.23/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 infra_operator-1.0.23/.pytest_cache/README.md
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 infra_operator-1.0.23/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 infra_operator-1.0.23/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0    11186 2020-02-02 00:00:00.000000 infra_operator-1.0.23/.vscode/launch.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 infra_operator-1.0.23/.vscode/settings.json
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 infra_operator-1.0.23/api-gateway/README.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/ap-northeast-1/variables.yaml
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/ap-northeast-1/ecs_mesh/common.yml
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/ap-northeast-1/ecs_mesh/infra/infra_template/cluster.yml
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/ap-northeast-1/ecs_mesh/infra/infra_template/exec_role.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/ap-northeast-1/ecs_mesh/infra_100/infra.output.yml
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/ap-northeast-1/ecs_mesh/infra_100/infra.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/ap-northeast-1/ecs_mesh/infra_100/vg_sg_rules.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/ap-northeast-1/ecs_mesh/infra_101/infra_101.yml
+-rw-r--r--   0        0        0   219025 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/global/cloudfront/api-mapper-test/distribution.tidy.crd.template.yaml
+-rw-r--r--   0        0        0   219025 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/global/cloudfront/api-mapper-test/distribution.tidy.crd.yaml
+-rw-r--r--   0        0        0    99359 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/global/cloudfront/api-mapper-test/distribution.tidy.simplify.yaml
+-rw-r--r--   0        0        0   189792 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/global/cloudfront/api-mapper-test/distribution.tidy.yaml
+-rw-r--r--   0        0        0    12181 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/global/cloudfront/api-mapper-test/distribution.yaml
+-rw-r--r--   0        0        0   252142 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/global/cloudfront/api-mapper-test/www.binance.com.yaml
+-rw-r--r--   0        0        0   107899 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/global/cloudfront/api-mapper-test/distribution/www.binance.com.yaml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/polices/s3_ro.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/infra_template/cluster.yml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/infra_template/exec_role.yml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/infra_template/mesh.yml
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg.yml
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_ecs_sg.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_loggroup.yml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_loggroup_policy.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_mesh_vgateway.yml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_sd.yml
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_service.yml
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_target.yml
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_target_attributes.yml
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_taskdef.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/custody/dev/template/vgateway_template/vg_taskrole.yml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/variables.yaml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/appmesh/variables.yaml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/appmesh/infra-operator-tests-mesh/mesh.exported.yaml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/appmesh/infra-operator-tests-mesh/mesh.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/appmesh/infra-operator-tests-mesh/variables.yaml
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ec2/infra-operator-tests/dex_fullnode.yaml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ec2/infra-operator-tests/ebs1.yaml
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ec2/infra-operator-tests/instance.exported.yaml
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ec2/infra-operator-tests/instance.update.yaml
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ec2/infra-operator-tests/instance.yaml
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ec2/infra-operator-tests/launch-template.yaml
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ec2/infra-operator-tests/user-data.sh
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecr/repositories/routing-web.yaml
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/cluster.exported.yaml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/cluster.update.yaml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/cluster.yaml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/variables.yaml
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/alb.exported.yaml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/alb.sg.exported.yaml
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/alb.sg.update.yaml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/alb.sg.yaml
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/alb.update.yaml
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/alb.yaml
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/exec.role.exported.yaml
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/exec.role.update.yaml
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/exec.role.yaml
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/service.exported.yaml
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/service.sg.exported.yaml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/service.sg.update.yaml
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/service.sg.yaml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/service.update.yaml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/service.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/targetGroup.exported.yaml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/targetGroup.update.yaml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/targetGroup.yaml
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/task.role.exported.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/task.role.yaml
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/taskDefinition.exported.yaml
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/taskDefinition.update.yaml
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/bin-dev-infra-operator-tests-cluster/comb-1/taskDefinition.yaml
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tf-bin-dev-be-eks/cross-proxy/infra.ecr.yaml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tf-bin-dev-be-eks/cross-proxy/infra.nlb.targetGroup.yaml
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tf-bin-dev-be-eks/cross-proxy/infra.nlb.yaml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tf-bin-dev-be-eks/cross-proxy/infra.role.yaml
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tf-bin-dev-be-eks/cross-proxy/infra.sg.yaml
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tf-bin-dev-be-eks/cross-proxy/infra.sm.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/app-test-1.yaml
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/variables.yaml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/bin-dev-demo-appmesh-vg/bin-dev-demo-appmesh-vg.yaml
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/demo-appmesh/mesh.yaml
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/alb.sg.yaml
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/alb.yaml
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/cpu-scaling.sp.yaml
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/exec.role.yaml
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/gatewayroute.yaml
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/mem-scaling.sp.yaml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/mesh.yaml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/policy.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/qps-scaling.sp.yaml
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/scalableTarget.yaml
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/service.sg.yaml
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/service.yaml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/sm.yaml
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/targetGroup.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/task.role.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/taskDefinition.yaml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/virtualgateway.yaml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/virtualnode.yaml
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/virtualrouter.yaml
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/desmond-debug/virtualservice.yaml
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/alb.sg.expected.json
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/alb.sg.update.expected.json
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/alb.sg.update.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/alb.sg.yaml
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/alb.yaml
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/cpu-scaling.sp.yaml
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/exec.role.yaml
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/mem-scaling.sp.yaml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/policy.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/policy.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/qps-scaling.sp.yaml
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/scalableTarget.yaml
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/service.sg.yaml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/service.yaml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/sm.yaml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/targetGroup.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/task.role.yaml
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/infra-operator-test/taskDefinition.yaml
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/ap-northeast-1/ecs/tk-dev-ecs-cluster/office-vpn-shared/shared.sg.yaml
+-rw-r--r--   0        0        0   219025 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/global/cloudfront/api-mapper-test/distribution.tidy.crd.template.yaml
+-rw-r--r--   0        0        0   219025 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/global/cloudfront/api-mapper-test/distribution.tidy.crd.yaml
+-rw-r--r--   0        0        0    99359 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/global/cloudfront/api-mapper-test/distribution.tidy.simplify.yaml
+-rw-r--r--   0        0        0   189792 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/global/cloudfront/api-mapper-test/distribution.tidy.yaml
+-rw-r--r--   0        0        0    12181 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/global/cloudfront/api-mapper-test/distribution.yaml
+-rw-r--r--   0        0        0   252142 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/global/cloudfront/api-mapper-test/www.binance.com.yaml
+-rw-r--r--   0        0        0   107899 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/global/cloudfront/api-mapper-test/distribution/www.binance.com.yaml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/dev/polices/s3_ro.yml
+-rw-r--r--   0        0        0    99541 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/prod/global/cloudfront/binance.behaviors.yaml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/prod/global/cloudfront/Distribution/internal-survey.blsdkrgjf.io.yaml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/prod/global/cloudfront/Distribution/www.binance.com.shield.yaml
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/prod/global/cloudfront/Distribution/www.binance.com.yaml
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/prod/global/cloudfront/Distribution/www.binance.me.yaml
+-rw-r--r--   0        0        0    82525 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/qa1fdg.behaviors.yaml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/CachePolicy/CachingS3CORS.yaml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/CachePolicy/Managed-CachingOptimized.yaml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/ContinuousDeploymentPolicy/www.qa1fdg.net.2.yaml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/ContinuousDeploymentPolicy/www.qa1fdg.net.yaml
+-rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/Distribution/static.qa1fdg.net.yaml
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/Distribution/www.qa1fdg.net.staging.2.yaml
+-rw-r--r--   0        0        0   105293 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/Distribution/www.qa1fdg.net.staging.yaml
+-rw-r--r--   0        0        0   113863 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/mainsite/qa/global/cloudfront/Distribution/www.qa1fdg.net.yaml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/thailand/prod/ap-northeast-1/ec2/dispatcher/alb.sg.yaml
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/thailand/prod/ap-northeast-1/elbv2/LoadBalancer/dispatcher/alb.yaml
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/thailand/prod/ap-northeast-1/elbv2/LoadBalancer/dispatcher/nginx-alb.yaml
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/thailand/prod/ap-northeast-1/elbv2/TargetGroup/dispatcher/tg-r0.yaml
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/thailand/prod/ap-northeast-1/elbv2/TargetGroup/dispatcher/tg-r1.yaml
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 infra_operator-1.0.23/aws/thailand/prod/global/cloudfront/Distribution/www.thai-exchange.com.yaml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 infra_operator-1.0.23/docker/Dockerfile
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 infra_operator-1.0.23/docker/OWNERS
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 infra_operator-1.0.23/docker/apps.sh
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 infra_operator-1.0.23/docker/install.sh
+-rw-r--r--   0        0        0   122710 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/alb export.ipynb
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/apigateway auth.ipynb
+-rw-r--r--   0        0        0    10394 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/appmesh.ipynb
+-rw-r--r--   0        0        0   169568 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/binance-gateway-helper.ipynb
+-rw-r--r--   0        0        0   539357 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/cloudfront operators.ipynb
+-rw-r--r--   0        0        0  4588998 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/cloudfront read.ipynb
+-rw-r--r--   0        0        0   187536 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/ebs crude.ipynb
+-rw-r--r--   0        0        0   156077 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/ec2 crude.ipynb
+-rw-r--r--   0        0        0   185798 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/ecr CRUDE.ipynb
+-rw-r--r--   0        0        0   108123 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/ecs export.ipynb
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/files.ipynb
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/iam role.ipynb
+-rw-r--r--   0        0        0   175666 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/launchtemplate crude.ipynb
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/sm.ipynb
+-rw-r--r--   0        0        0   108123 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/alb export-checkpoint.ipynb
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/apigateway auth-checkpoint.ipynb
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/appmesh-checkpoint.ipynb
+-rw-r--r--   0        0        0   126633 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/binance-gateway-helper-checkpoint.ipynb
+-rw-r--r--   0        0        0    33149 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/cloudfront operators-checkpoint.ipynb
+-rw-r--r--   0        0        0  4127367 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/cloudfront read-checkpoint.ipynb
+-rw-r--r--   0        0        0   185798 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/ebs crude-checkpoint.ipynb
+-rw-r--r--   0        0        0   122710 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/ec2 crude-checkpoint.ipynb
+-rw-r--r--   0        0        0   122710 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/ecr CRUDE-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/ecs export-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/files-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/iam role-checkpoint.ipynb
+-rw-r--r--   0        0        0   156077 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/launchtemplate crude-checkpoint.ipynb
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 infra_operator-1.0.23/notebook/.ipynb_checkpoints/sm-checkpoint.ipynb
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 infra_operator-1.0.23/server/pyproject.toml
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 infra_operator-1.0.23/server/src/app.py
+-rwxr-xr-x   0        0        0     1491 2020-02-02 00:00:00.000000 infra_operator-1.0.23/server/src/upload.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 infra_operator-1.0.23/server/src/templates/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/__init__.py
+-rw-r--r--   0        0        0    13749 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/clients/__init__.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/clients/ghe.py
+-rw-r--r--   0        0        0     6724 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/clients/mod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/create/__init__.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/create/aws_appmesh.py
+-rwxr-xr-x   0        0        0     9845 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/create/aws_elbv2_create.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/create/aws_secretsmanager.py
+-rw-r--r--   0        0        0    15721 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/create/mod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/delete/__init__.py
+-rwxr-xr-x   0        0        0      914 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/delete/aws_iam_delete.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/delete/mod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/diff/__init__.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/diff/mod.py
+-rwxr-xr-x   0        0        0    10342 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/export/aws_elbv2_export.py
+-rw-r--r--   0        0        0    16274 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/export/mod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/layout/__init__.py
+-rwxr-xr-x   0        0        0     3444 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/layout/mod.py
+-rwxr-xr-x   0        0        0    23529 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/operators/mod.py
+-rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/output/mod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/plugins/mod.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/plugins/wea_notify.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/preprocess/__init__.py
+-rw-r--r--   0        0        0    13643 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/preprocess/mod.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/preprocess/verify.py
+-rwxr-xr-x   0        0        0    25203 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/read/mod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/update/__init__.py
+-rwxr-xr-x   0        0        0     2734 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/update/aws_iam_update.py
+-rwxr-xr-x   0        0        0     4923 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/update/aws_sg_update.py
+-rwxr-xr-x   0        0        0     1274 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/update/ghe_update.py
+-rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/update/mod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/utils/__init__.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/utils/config.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/utils/dump.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/utils/load.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/utils/mod.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 infra_operator-1.0.23/src/infra_operator/validate/mod.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/cloudfront_alb_nginx_v1/variables.yaml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/cloudfront_alb_nginx_v1/aws/${project}/${env}/${region}/elbv2/LoadBalancer/${name}/alb.sg.yaml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/cloudfront_alb_nginx_v1/aws/${project}/${env}/${region}/elbv2/LoadBalancer/${name}/alb.yaml
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/cloudfront_alb_nginx_v1/aws/${project}/${env}/${region}/elbv2/LoadBalancer/${name}/nginx-alb.yaml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/cloudfront_alb_nginx_v1/aws/${project}/${env}/${region}/elbv2/LoadBalancer/${name}/tg-r0.yaml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/cloudfront_alb_nginx_v1/aws/${project}/${env}/${region}/elbv2/LoadBalancer/${name}/tg-r1.yaml
+-rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/cloudfront_alb_nginx_v1/aws/${project}/${env}/global/cloudfront/Distribution/${domain}.yaml
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/ip-set/${project}_${env}_${serviceName}_global_ratelimit_whitelist_ip_set.yaml
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/ip-set/${project}_${env}_${serviceName}_ip_block_set.yaml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/ip-set/${project}_${env}_${serviceName}_mgs_lambda_ip_whitelist_set.yaml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/ip-set/ipv4_format.yaml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/ip-set/ipv6_format.yaml
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/regex-pattern-set/cookie_regex_set.yaml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/regex-pattern-set/query_regex_set.yaml
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/regex-pattern-set/referer_regex_set.yaml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/regex-pattern-set/regex-set_format.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/regex-pattern-set/shared_path_regex_set.yaml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/regex-pattern-set/ua_regex_set.yaml
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/web-acl/${project}_${env}_${service-name}_alb_v2acl.yaml
+-rw-r--r--   0        0        0    15180 2020-02-02 00:00:00.000000 infra_operator-1.0.23/templates/wafv2/web-acl/${project}_${env}_${service-name}_cf_v2acl.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/appmesh/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/appmesh/mesh/__init__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/appmesh/mesh/test_0_create.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/appmesh/mesh/test_1_export.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/appmesh/mesh/test_2_delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/instance/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/instance/test_0_create.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/instance/test_1_export.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/instance/test_2_delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/sg/__init__.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/sg/test_0_create.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/sg/test_1_export.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ec2/sg/test_2_delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/cluster/__init__.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/cluster/test_0_create.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/cluster/test_1_export.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/cluster/test_2_delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/service/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/service/test_0_create.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/service/test_1_export.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/service/test_2_delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/targetgroup/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/targetgroup/test_0_create.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/targetgroup/test_1_export.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/targetgroup/test_2_delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/taskdefinition/__init__.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/taskdefinition/test_0_create.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/taskdefinition/test_1_export.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/ecs/taskdefinition/test_2_delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/elbv2/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/elbv2/alb/test_0_create.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/elbv2/alb/test_1_export.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/elbv2/alb/test_2_delete.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/iam/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/iam/role/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/iam/role/test_0_create.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/iam/role/test_1_export.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/iam/role/test_2_delete.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/secretsmanager/secret/test_0_create.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/secretsmanager/secret/test_1_export.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/ecs_service.yml
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/task_def.yml
+-rw-r--r--   0        0        0    20998 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/vnode.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/template/ecs_service.yml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/template/infra.yml
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/template/infra_deploy.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/template/infra_init.yml
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/template/task_def.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/template/values.yml
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/template/vnode.yml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/sg.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/values.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/s230/a.json
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/s230/ecs_service.yml
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/s230/task_def.yml
+-rw-r--r--   0        0        0    20757 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/s230/values.yml
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/s230/流程.yml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/s240/ecs_service.yml
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/s240/task_def.yml
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 infra_operator-1.0.23/tests/test_data/wallet/s240/vnode.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 infra_operator-1.0.23/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 infra_operator-1.0.23/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 infra_operator-1.0.23/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 infra_operator-1.0.23/pyproject.toml
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 infra_operator-1.0.23/PKG-INFO
```

### Comparing `infra_operator-1.0.22/api_to_yaml/clients/ghe.py` & `infra_operator-1.0.23/src/infra_operator/clients/ghe.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         repo = self.github.get_organization(org_name).get_repo(repo_name)
         cols = list(repo.get_collaborators())
         permissions = {
             col.login: get_collaborator_permission(col)
             for col in cols if col.suspended_at is None
         }
         return {
-            "apiVersion": "repo.ghe.binance/v1alpha1",
+            "apiVersion": "repo.ghe.infra/v1alpha1",
             "metadata": {
                 "Organization": org_name,
                 "RepoName": repo_name
             },
             "kind": "Repo",
             "spec": {
                 "collaborators": permissions
```

### Comparing `infra_operator-1.0.22/api_to_yaml/create/aws_appmesh.py` & `infra_operator-1.0.23/src/infra_operator/create/aws_appmesh.py`

 * *Files identical despite different names*

### Comparing `infra_operator-1.0.22/api_to_yaml/create/aws_elbv2_create.py` & `infra_operator-1.0.23/src/infra_operator/export/aws_elbv2_export.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,18 @@
 
 import oyaml as yaml
 import json
 import boto3
 from copy import deepcopy
 from pathlib import Path
 
-from api_to_yaml.operators.mod import dict_matcher, list_to_dict_by, remove_inner_fields, to_args
+from infra_operator.operators.mod import dict_matcher, list_to_dict_by, remove_inner_fields, to_args
+from infra_operator.clients.mod import clients
 
-
-# tags_to_list = aws_base.tags_to_list
-# remove_inner_fields = aws_base.remove_inner_fields
-# with_default = aws_base.with_default
-# with_args = aws_base.with_args
-# to_args = aws_base.to_args
-# list_to_dict_by = aws_base.list_to_dict_by
-# dict_matcher = aws_base.dict_matcher
-
-client = boto3.client('elbv2')
+client = clients["elbv2"]
 
 update_ignore_arg_names = set()
 
 
 def tags_to_list(tags):
     return [{"Key": key, "Value": val} for key, val in tags.items()]
 
@@ -51,15 +43,14 @@
 def create_rules(listener_arn, rules, info):
     if len(rules) == 0:
         return
     for rule in rules:
         args = {"ListenerArn": listener_arn}
         args = with_tags(rule, args, info)
         res = client.create_rule(**args)
-        print(res)
 
 
 def create_listeners(alb_arn, listeners, info):
     if len(listeners) == 0:
         return
     for listener in listeners:
         rules = listener.pop("Rules") if "Rules" in listener else []
@@ -75,56 +66,55 @@
 def create_load_balancer(kind, content, info):
     name = info["name"]
     args = {
         "Name": name,
     }
     args = with_tags(content["metadata"], args, info)
     res = client.create_load_balancer(**args)
-    print(res)
     alb = res["LoadBalancers"][0]
     attributes_update(content, {"LoadBalancerArn": alb["LoadBalancerArn"]},
                       info)
     create_listeners(alb["LoadBalancerArn"],
                      content.get("spec", {}).get("Listeners", []), info)
 
 
 def sg_update(content, current, info):
     arn = current["LoadBalancerArn"]
-    yaml_sgs = content.get("metadata", {}).get("SecurityGroups", [])
+    yaml_sgs = content.get("SecurityGroups", [])
     yaml_sgs.sort()
     current_sgs = current.get("SecurityGroups", [])
     current_sgs.sort()
     if yaml_sgs != current_sgs:
         print("update security group")
         return client.set_security_groups(LoadBalancerArn=arn,
                                           SecurityGroups=yaml_sgs)
 
 
 def subnet_update(content, current, info):
     arn = current["LoadBalancerArn"]
-    yaml_subnets = content.get("metadata", {}).get("Subnets", [])
+    yaml_subnets = content.get("Subnets", [])
     yaml_subnets.sort()
     current_subnets = list(
         map(lambda one: one["SubnetId"], current.get("AvailabilityZones", [])))
     current_subnets.sort()
     if yaml_subnets != current_subnets:
-        subnet_mappings = content.get("metadata", {}).get("SubnetMappings")
+        subnet_mappings = content.get("SubnetMappings")
         args = {"LoadBalancerArn": arn, "Subnets": yaml_subnets}
         if subnet_mappings:
             args["SubnetMappings"] = subnet_mappings
         print("update subnet")
         return client.set_subnets(**args)
 
 
 def ip_type_update(content, current, info):
     arn = current["LoadBalancerArn"]
-    yaml_ip_type = content.get("metadata", {}).get("IpAddressType")
+    yaml_ip_type = content.get("IpAddressType")
     ip_type = current.get("IpAddressType")
     if yaml_ip_type != ip_type:
-        yaml_ip_type = content.get("metadata", {}).get("IpAddressType")
+        yaml_ip_type = content.get("IpAddressType")
         print("update ip type")
         return client.set_ip_address_type(LoadBalancerArn=arn,
                                           IpAddressType=yaml_ip_type)
 
 
 def matcher(current, target, path):
     switch = {
@@ -161,14 +151,16 @@
         del args["Priority"]
         client.modify_rule(**args)
 
 
 def listener_update(content, current, info):
     lb_arn = current["LoadBalancerArn"]
     target = to_args(content)
+    target_listeners_self = {}
+    current_listeners_self = {}
     if "Listeners" in target:
         target_listeners = deepcopy(target["Listeners"])
         target_listeners = list_to_dict_by("Port")(target_listeners)
         target_listeners_self = remove_inner_fields(["Rules"
                                                      ])(target_listeners)
     if "Listeners" in current:
         current_listeners = deepcopy(current["Listeners"])
@@ -229,23 +221,21 @@
     tag_key = 'Tags'
     lb_arn = current['LoadBalancerArn']
     current_tags = current.get('Tags', [])
     wanted_tags = with_tags(to_args(content), {}, info).get(tag_key, [])
 
     tags = [i for i in wanted_tags if i not in current_tags]
     tags_keys = [i[key] for i in tags]
-    untags_keys = [{
-        'Key': i[key]
-    } for i in current_tags
-        if i not in wanted_tags and i[key] not in tags_keys]
+    untags_keys = [i[key] for i in current_tags
+                   if i not in wanted_tags and i[key] not in tags_keys]
 
     if tags:
         client.add_tags(ResourceArns=[lb_arn], Tags=tags)
     if untags_keys:
-        client.remove_tags(ResourceArns=[lb_arn], Tags=untags_keys)
+        client.remove_tags(ResourceArns=[lb_arn], TagKeys=untags_keys)
 
 
 def update_load_balancer(kind, content, info, current):
     check_list = [
         sg_update,
         subnet_update,
         ip_type_update,
```

### Comparing `infra_operator-1.0.22/api_to_yaml/create/aws_secretsmanager.py` & `infra_operator-1.0.23/src/infra_operator/create/aws_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `infra_operator-1.0.22/api_to_yaml/create/mod.py` & `infra_operator-1.0.23/src/infra_operator/create/mod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import base64
 import json
-from api_to_yaml.clients.mod import clients
-from api_to_yaml.operators.mod import add_items_quantity, metadata_to_args, tags_to_list, to_args, transform, with_args, with_default, with_ec2_tags, with_tags
+from infra_operator.clients.mod import clients
+from infra_operator.operators.mod import add_items_quantity, metadata_to_args, tags_to_list, to_args, transform, with_args, with_default, with_ec2_tags, with_tags
 import boto3
 import sys
 import time
-import api_to_yaml.create.aws_elbv2_create as elbv2_create
-from api_to_yaml.create.aws_appmesh import AppMeshController
-import api_to_yaml.update.ghe_update as ghe_update
-import api_to_yaml.create.aws_secretsmanager as secretsmanager_client
+import infra_operator.create.aws_elbv2_create as elbv2_create
+from infra_operator.create.aws_appmesh import AppMeshController
+import infra_operator.update.ghe_update as ghe_update
+import infra_operator.create.aws_secretsmanager as secretsmanager_client
 
 # TODO: refactor this to functions
 
 
 class ECSServiceController:
     """
     ECS service
@@ -148,27 +148,28 @@
 servicediscovery = clients["servicediscovery"]
 app_scaling = clients["application-autoscaling"]
 asg = clients['asg']
 sqs = clients['sqs']
 lambda_aws = clients['lambda']
 cloudwatch = clients['cloudwatch']
 cloudfront = clients['cloudfront']
+ec2 = clients['ec2']
 
 
 def wait_target_group_with_lb(args):
-    for alb in args.get("metadata", {}).get("loadBalancers", []):
+    for alb in args.get("loadBalancers", []):
         target_group_arn = alb.get("targetGroupArn")
         if target_group_arn:
             res = elbv2.describe_target_groups(
                 TargetGroupArns=[target_group_arn])
             lb_arns = res["TargetGroups"][0]["LoadBalancerArns"]
-            print(
-                f"wait for targetgroup associate with lb: {target_group_arn}")
-            sys.stdout.flush()
             while len(lb_arns) == 0:
+                print(
+                    f"wait for targetgroup associate with lb: {target_group_arn}")
+                sys.stdout.flush()
                 time.sleep(5)  # reduce speed
                 res = elbv2.describe_target_groups(
                     TargetGroupArns=[target_group_arn])
                 lb_arns = res["TargetGroups"][0]["LoadBalancerArns"]
     return args
 
 
@@ -183,43 +184,54 @@
     if 'Policy' in args:
         args['Policy'] = json.dumps(args['Policy'])
     return args
 
 
 def create(kind, content, info):
     switch = {
+        "Instance": (ec2, "run_instances", [
+            to_args,
+            with_ec2_tags("instance", info=info),
+            with_default({"MaxCount": 1,
+                          "MinCount": 1, })
+        ], None),
+        "ECS/Cluster": (ecs, "create_cluster", [
+            to_args,
+            with_tags(capitalize=False, info=info),
+        ], None),
         "TaskDefinition": (ecs, "register_task_definition", [
             to_args,
             with_tags(capitalize=False, info=info),
-            with_default({"family": info["name"]})
+            with_default({"family": info.get("name")})
         ], None),
         "TargetGroup": (elbv2, "create_target_group", [
             to_args,
             with_tags(capitalize=True, info=info),
-            with_default({"Name": info["name"]})
+            with_default({"Name": info.get("name")})
         ], None),
         "Service": (task_set_ecs, "create_service", [
-            wait_target_group_with_lb, to_args,
+            to_args,
+            wait_target_group_with_lb,
             with_tags(capitalize=False, info=info),
             with_default({
                 "cluster": info.get("ecs_cluster"),
-                "serviceName": info["name"]
+                "serviceName": info.get("name")
             })
         ], None),
         "LoadBalancer":
         (elbv2_create, "create_load_balancer",
          [with_args({
              "kind": kind,
              "content": content,
              "info": info
          })], None),
         "SecurityGroup": (ec2, "create_security_group", [
             metadata_to_args,
             with_ec2_tags("security-group", info=info),
-            with_default({"GroupName": info["name"]}),
+            with_default({"GroupName": info.get("name")}),
         ], lambda res: [
             ("SecurityGroupRule", {
                 "IpPermissions": content.get("spec", {}).get("egress")
             }, with_default({
                 "GroupId": res["GroupId"],
                 "SG_TYPE": "egress"
             })(info)) if content.get("spec", {}).get("egress") else None,
@@ -274,17 +286,16 @@
             }),
         ], None),
         "Repo": (ghe_update, "update_repo", [], None),
         "Mesh": (appmesh, "create_mesh", [
             metadata_to_args,
             with_tags(capitalize=False, info=info),
             with_default({
-                "meshName": info["name"],
-                "spec": content.get("spec")
-            }),
+                "spec": content.get("spec"),
+            })
         ], None),
         "VirtualNode": (appmesh, "create_virtual_node", [
             metadata_to_args,
             with_tags(capitalize=False, info=info),
             with_default({
                 "spec": content.get("spec"),
             })
@@ -313,30 +324,30 @@
         "VirtualGateway": (custom_appmesh, "create_virtual_gateway", [
             metadata_to_args,
             with_tags(capitalize=False, info=info),
             with_default({
                 "spec": content.get("spec"),
             })
         ], None),
-        "VirtualGatewayRoute": (appmesh, "create_gateway_route", [
+        "GatewayRoute": (appmesh, "create_gateway_route", [
             metadata_to_args,
             with_tags(capitalize=False, info=info),
             with_default({
                 "spec": content.get("spec"),
             })
         ], None),
         "ServiceDiscoveryService": (servicediscovery, "create_service", [
             to_args,
             with_tags(capitalize=True, info=info),
-            with_default({"Name": info["name"]})
+            with_default({"Name": info.get("name")})
         ], None),
         "Secret": (secretsmanager_client, "create_secret", [
             to_args,
             with_tags(capitalize=True, info=info),
-            with_default({"Name": info["name"]}),
+            with_default({"Name": info.get("name")}),
             transform("SecretString", lambda val: val.decode(
                 "utf-8") if isinstance(val, bytes) else val),
         ], None),
         "ScalingPolicy": (app_scaling, "put_scaling_policy", [
             to_args,
         ], None),
         "ScalableTarget": (app_scaling, "register_scalable_target", [
@@ -387,14 +398,18 @@
             lambda args: {"CachePolicyConfig": args}
         ], None),
         "ContinuousDeploymentPolicy": (cloudfront, "create_continuous_deployment_policy", [
             to_args,
             add_items_quantity,
             lambda args: {"ContinuousDeploymentPolicyConfig": args}
         ], None),
+        "Volume": (ec2, "create_volume", [
+            to_args,
+            with_ec2_tags("volume", info=info),
+        ], None),
     }
     client, method, steps, hook = switch[kind]
     func = getattr(client, method)
     args = content
     for step in steps:
         args = step(args)
     res = func(**args)
```

### Comparing `infra_operator-1.0.22/api_to_yaml/delete/mod.py` & `infra_operator-1.0.23/src/infra_operator/delete/mod.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from api_to_yaml.clients.mod import clients
-from api_to_yaml.create.aws_appmesh import AppMeshController
-from api_to_yaml.create.mod import ECSServiceController
-from api_to_yaml.operators.mod import add_field, metadata_to_args, to_args, transform, with_args, with_default, with_ec2_tags, with_tags
-import api_to_yaml.create.aws_secretsmanager as secretsmanager_client
+from infra_operator.clients.mod import clients
+from infra_operator.create.aws_appmesh import AppMeshController
+from infra_operator.create.mod import ECSServiceController
+from infra_operator.delete import aws_iam_delete
+from infra_operator.operators.mod import add_field, metadata_to_args, to_args, transform, with_args, with_default, with_ec2_tags, with_tags
+import infra_operator.create.aws_secretsmanager as secretsmanager_client
+from infra_operator.read.mod import get_name
 
 ecs = clients["ecs"]
 task_set_ecs = ECSServiceController()
 elbv2 = clients["elbv2"]
 ec2 = clients["ec2"]
 iam = clients["iam"]
 appmesh = clients["appmesh"]
@@ -21,14 +23,17 @@
 cloudfront = clients['cloudfront']
 
 
 def delete(kind, content, info, current):
     metadata = content.get("metadata", {})
     spec = content.get("spec", {})
     switch = {
+        "ECS/Cluster":
+        (ecs, "delete_cluster",
+         [with_args({"cluster": get_name(content, kind, info)})]),
         "TaskDefinition":
         (ecs, "deregister_task_definition",
          [with_args({"taskDefinition": current.get("taskDefinitionArn")})]),
         "TargetGroup":
         (elbv2, "delete_target_group",
          [with_args({"TargetGroupArn": current.get("TargetGroupArn")})]),
         "Service": (task_set_ecs, "delete_service", [
@@ -39,15 +44,15 @@
             }),
         ]),
         "LoadBalancer":
         (elbv2, "delete_load_balancer",
          [with_args({"LoadBalancerArn": current.get("LoadBalancerArn")})]),
         "SecurityGroup": (ec2, "delete_security_group",
                           [with_args({"GroupId": current.get("GroupId")})]),
-        # "Role": (role_ops, "delete_role", [with_args({"current": current})]), # TODO: implement role delete
+        "Role": (aws_iam_delete, "delete_role", [with_args({"current": current})]),
         "Mesh": (appmesh, "delete_mesh",
                  [with_args({"meshName": metadata.get("meshName")})]),
         "VirtualNode": (appmesh, "delete_virtual_node", [
             with_args({
                 "meshName": metadata.get("meshName"),
                 "virtualNodeName": metadata.get("virtualNodeName")
             })
@@ -67,15 +72,15 @@
         ]),
         "VirtualGateway": (custom_appmesh, "delete_virtual_gateway", [
             with_args({
                 "meshName": metadata.get("meshName"),
                 "virtualGatewayName": metadata.get("virtualGatewayName")
             })
         ]),
-        "VirtualGatewayRoute": (appmesh, "delete_gateway_route", [
+        "GatewayRoute": (appmesh, "delete_gateway_route", [
             with_args({
                 "meshName": metadata.get("meshName"),
                 "virtualGatewayName": metadata.get("virtualGatewayName"),
                 "gatewayRouteName": metadata.get("gatewayRouteName")
             })
         ]),
         "VirtualService": (appmesh, "delete_virtual_service", [
@@ -85,94 +90,99 @@
             })
         ]),
         "ServiceDiscoveryService": (servicediscovery, "delete_service",
                                     [lambda _: {
                                         "Id": current.get("Id")
                                     }], None),
         "Secret": (secretsmanager_client, "delete_secret", [
-            lambda _: {
+            with_args({
                 "SecretId": current.get("ARN"),
                 "ForceDeleteWithoutRecovery": True,
-            }
+            })
         ]),
         "ScalingPolicy": (app_scaling, "delete_scaling_policy", [
-            lambda _: {
+            with_args({
                 "PolicyName": current.get("PolicyName"),
                 "ServiceNamespace": current.get("ServiceNamespace"),
                 "ResourceId": current.get("ResourceId"),
                 "ScalableDimension": current.get("ScalableDimension")
-            }
+            })
         ]),
         "ScalableTarget": (app_scaling, "deregister_scalable_target", [
-            lambda _: {
+            with_args({
                 "ServiceNamespace": current.get("ServiceNamespace"),
                 "ResourceId": current.get("ResourceId"),
                 "ScalableDimension": current.get("ScalableDimension")
-            }
+            })
         ]),
         "Queue": (sqs, "delete_queue", [
-            lambda _: {
+            with_args({
                 "QueueUrl": current.get("QueueUrl")
-            }
+            })
         ]),
         "LaunchTemplate": (ec2, "delete_launch_template", [
-            lambda _: {
+            with_args({
                 "LaunchTemplateName": metadata.get("LaunchTemplateName")
-            }
+            })
         ]),
         "Lambda": (lambda_aws, "delete_function", [
-            lambda _: {
+            with_args({
                 "FunctionName": metadata.get("FunctionName")
-            }
+            })
         ]),
         "AutoScalingGroup": (asg, "delete_auto_scaling_group", [
-            lambda _: {
+            with_args({
                 "AutoScalingGroupName": metadata.get("AutoScalingGroupName"),
                 "ForceDelete": True
-            }
+            })
         ]),
         "LambdaEventSource": (lambda_aws, "delete_event_source_mapping", [
-            lambda _: {
+            with_args({
                 "UUID": current.get("UUID")
-            }
+            })
         ]),
         "LifeCycleHook": (asg, "delete_lifecycle_hook", [
-            lambda _: {
+            with_args({
                 "LifecycleHookName": metadata.get("LifecycleHookName"),
                 "AutoScalingGroupName": spec.get("AutoScalingGroupName")
-            }
+            })
         ]),
         "Alarm": (cloudwatch, "delete_alarms", [
-            lambda _: {
+            with_args({
                 "AlarmNames": [metadata.get("AlarmName")]
-            }
+            })
         ]),
         "AutoScalingPolicy": (asg, "delete_policy", [
-            lambda _: {
+            with_args({
                 "PolicyName": metadata.get("PolicyName"),
                 "AutoScalingGroupName": spec.get("AutoScalingGroupName")
-            }
+            })
         ]),
         "Distribution": (cloudfront, "delete_distribution", [
-            lambda _: {
+            with_args({
                 "Id": metadata.get("Id"),
                 "IfMatch": current.get("ETag")
-            }
+            })
         ]),
         "CachePolicy": (cloudfront, "delete_cache_policy", [
-            lambda _: {
+            with_args({
                 "Id": metadata.get("Id"),
                 "IfMatch": current.get("ETag")
-            }
+            })
         ]),
         "ContinuousDeploymentPolicy": (cloudfront, "delete_continuous_deployment_policy", [
-            lambda _: {
+            with_args({
                 "Id": metadata.get("Id"),
                 "IfMatch": current.get("ETag")
-            }
+            })
+        ]),
+        "Instance": (ec2, "terminate_instances", [
+            with_args({
+                "InstanceIds": [current.get("InstanceId")],
+            })
         ]),
     }
     client, method, steps = switch[kind]
     func = getattr(client, method)
     args = content
     for step in steps:
         args = step(args)
```

### Comparing `infra_operator-1.0.22/api_to_yaml/diff/mod.py` & `infra_operator-1.0.23/src/infra_operator/diff/mod.py`

 * *Files identical despite different names*

### Comparing `infra_operator-1.0.22/api_to_yaml/export/mod.py` & `infra_operator-1.0.23/src/infra_operator/clients/mod.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,130 +1,212 @@
-import re
-from copy import deepcopy
-from api_to_yaml.operators.mod import list_to_tags, remove_field, remove_fields, remove_items_quantity, template_fields, to_crd
-from api_to_yaml.clients.mod import clients
-
-
-def export_tags(crd):
-    kind = crd["kind"].lower()
-    if kind not in set(["distribution"]):
-        return crd
-    account_id = clients["sts"].get_caller_identity()["Account"]
-    id = crd["metadata"]["Id"]
-    res = clients["cloudfront"].list_tags_for_resource(
-        Resource=f"arn:aws:cloudfront::{account_id}:{kind}/{id}")
-    tags = list_to_tags(res["Tags"]["Items"])
-    crd["metadata"]["Tags"] = tags
-    return crd
-
-
-def export(kind, current, info):
-    switch = {"Repo": [remove_fields(["metadata"])],
-              "Distribution": [remove_items_quantity,
-                               remove_fields(["ETag", "DomainName"]),
-                               lambda tidied: template_fields(
-                                   deepcopy(tidied), ["Origins", "CacheBehaviors"]),
-                               lambda content: to_crd(
-                                   content, "cloudfront.aws.binance/v1alpha1", "Distribution"),
-                               export_tags],
-              "CachePolicy": [remove_items_quantity,
-                              remove_field("ETag"),
-                              lambda content: to_crd(
-                                  content, "cloudfront.aws.binance/v1alpha1", "CachePolicy"),
-                              export_tags
-                              ],
-              "ContinuousDeploymentPolicy": [remove_items_quantity,
-                                             remove_field("ETag"),
-                                             lambda content: to_crd(
-                                                 content, "cloudfront.aws.binance/v1alpha1", "ContinuousDeploymentPolicy"),
-                                             export_tags
-                                             ],
-              "LoadBalancer": [remove_items_quantity,
-                               lambda content: to_crd(
-                                   content, "elbv2.aws.binance/v1alpha1", "LoadBalancer"),
-                               export_tags
-                               ],
-              }
-    for func in switch[kind]:
-        current = func(current)
-    return current
-
-
-def collect_cache_policy_id_(acc, content, info):
-    if type(content) == dict:
-        v = content.get("CachePolicyId")
-        if v is not None and re.match(r"^\w{8}-\w{4}-\w{4}-\w{4}-\w{12}$", v):
-            copied = deepcopy(info)
-            copied["cloudfront_type"] = "CachePolicy"
-            acc[v] = ("CachePolicy", {"metadata": {"Id": v}}, copied)
-        for k, v in content.items():
-            collect_cache_policy_id_(acc, v, info)
-    elif type(content) == list:
-        for one in content:
-            collect_cache_policy_id_(acc, one, info)
-
-
-def collect_cache_policy_id(refs, info):
-    def wrap(content):
-        collect_cache_policy_id_(refs, content, info)
-        return content
-    return wrap
-
-
-def collect_continuous_deployment_policy_id(refs, info):
-    def remove_staging(str):
-        return re.sub(r"\.staging(\.\d+)?", "", "www.qa1fdg.net.staging")
-
-    def wrap(content):
-        v = content["ContinuousDeploymentPolicyId"]
-        if re.match(r"^\w{8}-\w{4}-\w{4}-\w{4}-\w{12}$", v):
-            copied = deepcopy(info)
-            copied["cloudfront_type"] = "ContinuousDeploymentPolicy"
-            copied["refed_filename"] = remove_staging(copied["name"])
-            refs[v] = ("ContinuousDeploymentPolicy", {
-                "metadata": {"Id": v}}, copied)
-        return content
-    return wrap
-
-
-def collect_cloudfront_domain(refs, info):
-    def wrap(content):
-        domains = content["StagingDistributionDnsNames"]["Items"]
-        for i, domain in enumerate(domains):
-            if re.match(r"^\w+\.cloudfront\.net$", domain):
-                copied = deepcopy(info)
-                copied["cloudfront_type"] = "Distribution"
-                n = f".{i}" if i != 0 else ""
-                copied["refed_filename"] = f'{copied["name"]}.staging{n}'
-                copied["ref_template"] = "$file({}, DomainName)"
-                refs[domain] = ("Distribution", {
-                    "metadata": {"DomainName": domain}}, copied)
-        return content
-    return wrap
-
-
-def export_ref(kind, current, info):
-    refs = {}
-    switch = {
-        "Distribution": [collect_cache_policy_id(refs, info),
-                         collect_continuous_deployment_policy_id(refs, info),
-                         remove_items_quantity,
-                         remove_fields(["ETag", "DomainName"]),
-                         lambda tidied: template_fields(
-                             deepcopy(tidied), ["Origins", "CacheBehaviors"]),
-                         lambda content: to_crd(
-                             content, "cloudfront.aws.binance/v1alpha1", "Distribution"),
-                         export_tags],
-        "ContinuousDeploymentPolicy": [collect_cloudfront_domain(refs, info),
-                                       remove_items_quantity,
-                                       remove_field("ETag"),
-                                       lambda content: to_crd(
-                                           content, "cloudfront.aws.binance/v1alpha1", "ContinuousDeploymentPolicy"),
-                                       export_tags
-                                       ],
-    }
-    if kind in switch:
-        for func in switch[kind]:
-            current = func(current)
-        return refs, current
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import os
+import types
+import boto3
+from infra_operator.clients.ghe import GHE
+
+
+def get_account_id(self):
+    return self.get_caller_identity()["Account"]
+
+
+def find_distribution(self, Id=None, Alias=None, DomainName=None):
+    if Id is None:
+        pager = self.get_paginator("list_distributions")
+        matched = []
+        for res in pager.paginate():
+            for dist in res["DistributionList"]["Items"]:
+                if DomainName is None:
+                    if Alias in dist["Aliases"].get("Items", []):
+                        matched.append(dist)
+                else:
+                    if dist["DomainName"] == DomainName:
+                        matched.append(dist)
+        if len(matched) == 1:
+            Id = matched[0]["Id"]
+        elif len(matched) == 0:
+            return None
+        else:
+            raise Exception(
+                f"found {len(matched)} distribution with Alias: {Alias}. please specify by Id")
+    res = self.get_distribution(Id=Id)
+    res["Distribution"]["DistributionConfig"]["Id"] = Id
+    res["Distribution"]["DistributionConfig"]["ETag"] = res["ETag"]
+    res["Distribution"]["DistributionConfig"]["DomainName"] = res["Distribution"]["DomainName"]
+    return res
+
+
+def list_continuous_deployment_policies_(self):
+    res = self.list_continuous_deployment_policies()
+    marker = res["ContinuousDeploymentPolicyList"]
+    marker = None
+    while True:
+        if marker:
+            res = self.list_continuous_deployment_policies(Marker=marker)
+        else:
+            res = self.list_continuous_deployment_policies()
+        marker = res["ContinuousDeploymentPolicyList"].get("NextMarker")
+        for one in res["ContinuousDeploymentPolicyList"]["Items"]:
+            one["ContinuousDeploymentPolicy"]["ContinuousDeploymentPolicyConfig"]["Id"] = one["ContinuousDeploymentPolicy"]["Id"]
+            yield one["ContinuousDeploymentPolicy"]["ContinuousDeploymentPolicyConfig"]
+        if marker is None:
+            break
+
+
+def try_get_continuous_deployment_policy(self, Id=None, StagingDistributionDnsNames=None):
+    if Id is None:
+        for one in self.list_continuous_deployment_policies_():
+            if set(one["StagingDistributionDnsNames"]["Items"]) == set(StagingDistributionDnsNames):
+                Id = one["Id"]
+                break
+    if Id:
+        return self.get_continuous_deployment_policy(Id=Id)
+
+
+def list_cache_policies_(self):
+    marker = None
+    while True:
+        if marker:
+            res = self.list_cache_policies(Marker=marker)
+        else:
+            res = self.list_cache_policies()
+        marker = res["CachePolicyList"].get("NextMarker")
+        for one in res["CachePolicyList"]["Items"]:
+            one["CachePolicy"]["CachePolicyConfig"]["Id"] = one["CachePolicy"]["Id"]
+            yield one["CachePolicy"]["CachePolicyConfig"]
+        if marker is None:
+            break
+
+
+def find_cache_policy(self, Id=None, Name=None):
+    if Id is None:
+        cache_policies = list(self.list_cache_policies_())
+        res = [one for one in cache_policies if one["Name"] == Name]
+        if len(res) == 0:
+            return None
+        Id = res[0]["Id"]
+    result = self.get_cache_policy(Id=Id)
+    if result is None:
+        return None
+    Id = result["CachePolicy"]["Id"]
+    config = result["CachePolicy"]["CachePolicyConfig"]
+    config["Id"] = Id
+    config["ETag"] = result["ETag"]
+    return config
+
+
+cloudfront = boto3.client('cloudfront')
+cloudfront.find_distribution = types.MethodType(find_distribution, cloudfront)
+cloudfront.list_cache_policies_ = types.MethodType(
+    list_cache_policies_, cloudfront)
+cloudfront.find_cache_policy = types.MethodType(find_cache_policy, cloudfront)
+cloudfront.list_continuous_deployment_policies_ = types.MethodType(
+    list_continuous_deployment_policies_, cloudfront)
+cloudfront.try_get_continuous_deployment_policy = types.MethodType(
+    try_get_continuous_deployment_policy, cloudfront)
+
+sts = boto3.client("sts")
+sts.get_account_id = types.MethodType(get_account_id, sts)
+
+
+def find_instance(this, InstanceId, Name):
+    if InstanceId:
+        return this.describe_instances(InstanceIds=[InstanceId])
+    else:
+        return this.describe_instances(Filters=[{
+            'Name': 'tag:Name',
+            'Values': [Name]
+        }])
+
+
+def find_volume(this, VolumeId=None, Name=None):
+    if VolumeId:
+        return this.describe_volumes(VolumeIds=[VolumeId])
+    else:
+        return this.describe_volumes(Filters=[{
+            'Name': 'tag:Name',
+            'Values': [Name]
+        }])
+
+
+def find_launch_template(this, LaunchTemplateId=None, LaunchTemplateName=None):
+    if LaunchTemplateId:
+        return this.describe_launch_templates(LaunchTemplateIds=[LaunchTemplateId])
     else:
-        return {}, export(kind, current, info)
+        return this.describe_launch_templates(LaunchTemplateNames=[LaunchTemplateName])
+
+
+def update_instance(this, content, current):
+    fields = [
+        "SourceDestCheck",
+        "Attribute",
+        "BlockDeviceMappings",
+        "DisableApiTermination",
+        "EbsOptimized",
+        "EnaSupport",
+        "Groups",
+        "InstanceId",
+        "InstanceInitiatedShutdownBehavior",
+        "InstanceType",
+        "Kernel",
+        "Ramdisk",
+        "SriovNetSupport",
+        "UserData",
+        "Value",
+        "DisableApiStop",
+    ]
+    for field in fields:
+        pass
+
+
+ec2 = boto3.client("ec2")
+ec2.find_instance = types.MethodType(find_instance, ec2)
+ec2.find_volume = types.MethodType(find_volume, ec2)
+ec2.find_launch_template = types.MethodType(find_launch_template, ec2)
+
+
+def find_repository(this, registryId, repositoryName):
+    if registryId:
+        return this.describe_repositories(registryId=registryId, repositoryNames=[repositoryName])
+    else:
+        return this.describe_repositories(repositoryNames=[repositoryName])
+
+
+ecr = boto3.client('ecr')
+ecr.find_repository = types.MethodType(find_repository, ecr)
+
+clients = {
+    "ecr":
+    ecr,
+    "ecs":
+    boto3.client('ecs'),
+    "elbv2":
+    boto3.client("elbv2"),
+    "ec2": ec2,
+    "iam":
+    boto3.client("iam"),
+    "appmesh":
+    boto3.client("appmesh"),
+    "servicediscovery":
+    boto3.client("servicediscovery"),
+    "secretsmanager":
+    boto3.client("secretsmanager"),
+    "ghe":
+    GHE(base_url="https://git.toolsfdg.net/api/v3",
+        login_or_token=os.getenv('GITHUB_TOKEN')),
+    "application-autoscaling":
+        boto3.client("application-autoscaling"),
+    "sqs":
+        boto3.resource('sqs'),
+    "lambda":
+        boto3.client('lambda'),
+    "asg":
+        boto3.client('autoscaling'),
+    "cloudwatch":
+        boto3.client('cloudwatch'),
+    "cloudfront":
+        cloudfront,
+    "sts":
+        sts,
+}
```

### Comparing `infra_operator-1.0.22/api_to_yaml/operators/mod.py` & `infra_operator-1.0.23/src/infra_operator/operators/mod.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,27 +71,49 @@
         yield dict_replace(expr, '$item', item)
 
 
 def has_variable(string):
     return len(re.findall("\$\{([^\s\}]+)\}", string)) > 0
 
 
+def try_get_nested_var(var_name, variables):
+    indexes = var_name.split(".")
+    variable = None
+    cursor = variables
+    for index in indexes:
+        if index in cursor:
+            variable = cursor[index]
+            cursor = variable
+        else:
+            return None
+    return variable
+
+
+def is_expression(expr):
+    if isinstance(expr, str):
+        match = re.findall("\$\{([^\s\}]+)\}", expr)
+        return len(match) != 0
+    else:
+        return False
+
+
 def render_str(param, variables):
     match = re.findall("\$\{([^\s\}]+)\}", param)
     var_count = len(match)
     replaced_count = 0
     for var_name in match:
-        if var_name not in variables:
+        variable = try_get_nested_var(var_name, variables)
+        if variable is None:
             continue
         if len(match) == 1 and param == f"${{{var_name}}}":
             replaced_count += 1
-            param = variables[var_name]
+            param = variable
         else:
             replaced_count += 1
-            param = param.replace(f"${{{var_name}}}", variables[var_name])
+            param = param.replace(f"${{{var_name}}}", variable)
     return var_count, replaced_count, param
 
 
 def merge_dict(dicts):
     result = deepcopy(dicts[0])
     for dict in dicts:
         result.update(dict)
@@ -140,14 +162,22 @@
                 return res
             elif k == "$map":
                 map_expr = content.pop(k)
                 expr = map_expr.pop("$expr")
                 items = map_expr.pop("$items")
                 # evaluate $map first, then others.
                 return list(apply(one) for one in process_map(expr, items))
+            elif k == "$if":
+                if_expr = content.pop(k)
+                expr = if_expr.pop("$expr")
+                true_val = if_expr.pop("$true")
+                false_val = if_expr.pop("$false")
+                if is_expression(expr):
+                    raise Exception(f"$if.$expr is not expanded: {expr}")
+                return apply(true_val) if apply(expr) else apply(false_val)
             elif k == "$merge":
                 merge_expr = content.pop(k)
                 return merge_dict(list(apply(one) for one in merge_expr))
             elif k == "$lower":
                 return apply(v).lower()
             elif k == "$underscore":
                 return apply(v).replace("-", "_")
@@ -235,14 +265,35 @@
             return {k: remove_items_quantity(v) for k, v in content.items()}
     elif type(content) == list:
         return [remove_items_quantity(one) for one in content]
     else:
         return content
 
 
+def lift_field(field):
+    def wrap(content):
+        content.update(content[field])
+        del content[field]
+        return content
+    return wrap
+
+
+def remove_empty_list(content):
+    if type(content) == dict:
+        to_remove = set()
+        for key, val in content.items():
+            if val == []:
+                to_remove.add(key)
+        return {k: remove_empty_list(v) for k, v in content.items() if k not in to_remove}
+    elif type(content) == list:
+        return [remove_empty_list(one) for one in content]
+    else:
+        return content
+
+
 def split_value_field(content):
     singles = {}
     complexes = {}
     for k, v in content.items():
         if type(v) in [str, int, float, bool]:
             singles[k] = v
         else:
@@ -298,22 +349,39 @@
     singles = human_key_sort(singles)
     complexes = human_key_sort(complexes)
     result = {
         "apiVersion": api,
         "kind": kind,
         "pipelineConfig": {
             "no-apply": True,
-            "comment": "no-apply: true prevents this file being apply by api-to-yaml. auto added by api-to-yaml export. if need to apply, set to false"
+            "comment": "no-apply: true prevents this file being apply by infra-operator. auto added by infra-operator export. if need to apply, set to false"
         },
         "metadata": singles,
         "spec": complexes,
     }
     return result
 
 
+def sort_field_by(selectors, key):
+    def wrap_(obj):
+        def wrap(sels, obj):
+            if len(sels) == 0:
+                obj.sort(key=key)
+            else:
+                if sels[0] == list:
+                    body = sels[1:]
+                    for one in obj:
+                        wrap(body, one)
+                else:
+                    wrap(sels[1:], obj[sels[0]])
+        wrap(selectors, obj)
+        return obj
+    return wrap_
+
+
 def get_major_kind(count, total):
     for k, c in count.items():
         if c / total > 0.5 and total > 2:
             return json.loads(k)
 
 
 def flatten(content):
@@ -400,30 +468,115 @@
 
 def template_fields(content, fields):
     for field in fields:
         content[field] = template_field(content[field])
     return content
 
 
-def remove_keys_all(keys, content):
-    if type(content) == dict:
-        return {k: remove_keys_all(keys, v) for k, v in content.items() if k not in keys}
-    elif type(content) == list:
-        return [remove_keys_all(keys, one) for one in content]
+def remove_fields_recursive(keys):
+    def wrap(content):
+        if type(content) == dict:
+            return {k: wrap(v) for k, v in content.items() if k not in keys}
+        elif type(content) == list:
+            return [wrap(one) for one in content]
+        else:
+            return content
+    return wrap
+
+
+def rename_fields(mapping):
+    def wrap(args):
+        args = deepcopy(args)
+        pairs = mapping.items() if type(mapping) == dict else mapping
+        for field, new_name in pairs:
+            if type(field) == list:
+                rename_nested_field(field, new_name)(args)
+            else:
+                if field in args:
+                    args[new_name] = args[field]
+                    del args[field]
+        return args
+    return wrap
+
+
+def enabled_disabled_to_bool(obj, key):
+    if obj[key] == "disabled":
+        obj[key] = False
+    elif obj[key] == "enabled":
+        obj[key] = True
     else:
-        return content
+        raise Exception(f"expected disabled|enabled, got {obj[key]}")
 
 
-def remove_fields(fields):
+def list_to_args_overwrite(obj, key):
+    obj[key] = list_to_tags(obj[key])
+
+
+def map_nested_field(selectors, func):
+    def wrap_(obj):
+        def wrap(sels, obj):
+            if len(sels) == 1:
+                func(obj, sels[0])
+            else:
+                if sels[0] == list:
+                    body = sels[1:]
+                    for one in obj:
+                        wrap(body, one)
+                else:
+                    wrap(sels[1:], obj[sels[0]])
+        wrap(selectors, obj)
+        return obj
+    return wrap_
+
+
+def rename_nested_field(selectors, new_name):
+    def wrap_(obj):
+        def wrap(sels, obj):
+            if len(sels) == 1:
+                obj[new_name] = obj[sels[0]]
+                del obj[sels[0]]
+            else:
+                if sels[0] == list:
+                    body = sels[1:]
+                    for one in obj:
+                        wrap(body, one)
+                else:
+                    wrap(sels[1:], obj[sels[0]])
+        wrap(selectors, obj)
+        return obj
+    return wrap_
+
+
+def remove_nested_field(selectors):
+    def wrap_(obj):
+        def wrap(sels, obj):
+            if len(sels) == 1:
+                del obj[sels[0]]
+            else:
+                if sels[0] == list:
+                    body = sels[1:]
+                    for one in obj:
+                        wrap(body, one)
+                else:
+                    wrap(sels[1:], obj[sels[0]])
+        wrap(selectors, obj)
+        return obj
+    return wrap_
 
+
+def remove_fields(fields):
     def wrap(args):
         args = deepcopy(args)
         for field in fields:
-            if field in args:
-                del args[field]
+            if type(field) == list:
+                remove_nested_field(field)(args)
+            else:
+                if field in args:
+                    del args[field]
+
         return args
 
     return wrap
 
 
 def remove_inner_fields(fields):
 
@@ -493,16 +646,18 @@
     return content
 
 
 def metadata_to_args(content):
     return content.get("metadata", {})
 
 
-def override(a, b):
-    return a if b is None else b
+def override(*args):
+    for arg in reversed(args):
+        if arg:
+            return arg
 
 
 def identity(*arg):
     return arg
 
 
 def list_to_dict_by(key):
@@ -557,34 +712,50 @@
 
 def list_to_tags(tags, capitalize=True):
     keyName = "Key" if capitalize else "key"
     valName = "Value" if capitalize else "value"
     return {one[keyName]: one[valName] for one in tags}
 
 
+def spec_to_meta(field):
+    def wrap(crd):
+        if field in crd.get("spec", {}):
+            if "metadata" not in crd:
+                crd["metadata"] = {}
+            crd["metadata"][field] = crd["spec"][field]
+            del crd["spec"][field]
+        return crd
+    return wrap
+
+
 def with_ec2_tags(resource_type, info=None):
 
     def wrap(args):
         tags = {}
         if "Tags" in args:
             tags.update(args.pop("Tags"))
         tags.update({
             "terraform": "y",
             "prow-pipeline": "y",
             "engine": "devops-infra",
         })
-        if info and "name" in info:
+        if info and info.get("name"):
             tags["devops-infra-service"] = info.get("name")
         if info and "env" in info and "env" not in tags:
             tags["env"] = info.get("env")
-        args["TagSpecifications"] = [{
+        if "TagSpecifications" in args:
+            for tag_spec in args["TagSpecifications"]:
+                tag_spec["Tags"] = tags_to_list(tag_spec["Tags"])
+        else:
+            args["TagSpecifications"] = []
+        args["TagSpecifications"].append({
             'ResourceType':
             resource_type,  # 'client-vpn-endpoint'|'customer-gateway'|'dedicated-host'|'dhcp-options'|'egress-only-internet-gateway'|'elastic-ip'|'elastic-gpu'|'export-image-task'|'export-instance-task'|'fleet'|'fpga-image'|'host-reservation'|'image'|'import-image-task'|'import-snapshot-task'|'instance'|'instance-event-window'|'internet-gateway'|'key-pair'|'launch-template'|'local-gateway-route-table-vpc-association'|'natgateway'|'network-acl'|'network-interface'|'network-insights-analysis'|'network-insights-path'|'placement-group'|'reserved-instances'|'route-table'|'security-group'|'security-group-rule'|'snapshot'|'spot-fleet-request'|'spot-instances-request'|'subnet'|'traffic-mirror-filter'|'traffic-mirror-session'|'traffic-mirror-target'|'transit-gateway'|'transit-gateway-attachment'|'transit-gateway-connect-peer'|'transit-gateway-multicast-domain'|'transit-gateway-route-table'|'volume'|'vpc'|'vpc-peering-connection'|'vpn-connection'|'vpn-gateway'|'vpc-flow-log',
             'Tags': tags_to_list(tags, True)
-        }]
+        })
         return args
 
     return wrap
 
 
 def with_tags(capitalize=False, info=None, expect_tags_as_list=True):
 
@@ -593,15 +764,15 @@
         if key not in args:
             args[key] = {}
         args[key].update({
             "terraform": "y",
             "prow-pipeline": "y",
             "engine": "devops-infra",
         })
-        if info and "name" in info:
+        if info and info.get("name"):
             args[key]["devops-infra-service"] = info.get("name")
         if info and "env" in info and "env" not in args[key]:
             args[key]["env"] = info.get("env")
         if expect_tags_as_list:
             args[key] = tags_to_list(args[key], capitalize)
         return args
```

### Comparing `infra_operator-1.0.22/api_to_yaml/plugins/wea_notify.py` & `infra_operator-1.0.23/src/infra_operator/plugins/wea_notify.py`

 * *Files identical despite different names*

### Comparing `infra_operator-1.0.22/api_to_yaml/preprocess/mod.py` & `infra_operator-1.0.23/src/infra_operator/preprocess/mod.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from collections import defaultdict
 from copy import deepcopy
 import os
 import re
 import sys
 import oyaml as yaml
 from time import sleep
-from api_to_yaml.layout.mod import parse as parse_filename
-from api_to_yaml.operators.mod import var_replace
-from api_to_yaml.preprocess.verify import verify
-from api_to_yaml.read.mod import get_arn, get_name, get_resource
-from api_to_yaml.operators.mod import apply as apply_operators
+from infra_operator.utils import config
+from infra_operator.utils.load import load as yaml_load
+from infra_operator.layout.mod import parse as parse_filename
+from infra_operator.operators.mod import merge_dict, var_replace
+from infra_operator.preprocess.verify import verify
+from infra_operator.read.mod import get_arn, get_arn_from_resource, get_name, get_resource
+from infra_operator.operators.mod import apply as apply_operators
 
 # cache
 REF_FILE_CACHE = {}
 REF_FILE_CONTENT_CACHE = {}
 
 
 def get_variables(folder, info):
@@ -28,15 +30,22 @@
         folder = os.path.dirname(folder)
     for variable in variables:
         combined.update(variable)
     return combined
 
 
 def resolve_path(folder, ref):
-    return os.path.join(folder, ref)
+    full_path = None
+    if ref.startswith("/"):
+        full_path = os.path.join(os.getcwd(), ref[1:])
+    else:
+        full_path = os.path.join(os.getcwd(), folder, ref)
+    full_path = os.path.realpath(full_path)
+    result = full_path[len(os.getcwd())+1:]
+    return result
 
 
 def get_kind(content, info):
     kind = content.get("kind")
     # todo wafv2
     return kind
 
@@ -55,16 +64,16 @@
     kind, info, content = preprocess(content, info, folder)
     name = get_name(content, kind, info)
 
     return content, info, kind, region, name
 
 
 def resolve_arn(filename, waiting):
-    kind, info, content = preprocess_file(filename, False, True)
-    region = info["region"]
+    kind, info, content = preprocess_file(filename, {}, False, True)
+    region = info.get("region", "us-east-1")
     name = get_name(content, kind, info)
     # content, info, kind, region, name = _resolve(filename)
     arn = get_arn(content, info)
     if arn is None:
         if waiting:
             print("wait for resources: {kind}, {region}, {name}".format(
                 kind=kind, region=region, name=name))
@@ -136,14 +145,48 @@
             raise Exception(
                 f"The {key} not in {','.join(current.keys())}, please check it."
             )
         result = result.get(key)
     return result
 
 
+def parse_expression(folder, string):
+    reg = r"\$file\((.+)\)"
+    match = re.match(reg, string)
+    if match:
+        params = list(map(lambda one: one.strip(),
+                          match.groups()[0].split(",")))
+        file = resolve_path(folder, params.pop(0))
+        return {
+            "func": "FileReference",
+            "file": file,
+            "params": params
+        }
+
+
+def dot_operator(content, params, throw=True):
+    result = None
+    for param in params:
+        if param in content:
+            result = content[param]
+            content = result
+        elif throw:
+            expr = params.join(".")
+            raise Exception(f"could not find {expr} in {content}")
+    return result
+
+
+def expand_expression(expr, refed_files):
+    assert expr["func"] == "FileReference"
+    if len(expr["params"]) == 0:
+        return get_arn_from_resource(refed_files[expr["file"]])
+    else:
+        return dot_operator(refed_files[expr["file"]], expr["params"])
+
+
 def ref_file(folder, content, ref_map, waiting):
     reg = r"\$file\((.+)\)"
     def return_rendered(arn, origin): return re.sub(reg, arn, origin)
 
     if type(content) == str:
 
         match = re.match(reg, content)
@@ -153,15 +196,15 @@
             file_path = parms.pop(0)
             refed_file = resolve_path(folder, file_path)
 
             # find ref file
             if not os.path.exists(refed_file) and ".trash" in refed_file:
                 refed_file = refed_file.replace("/.trash", "")
             if not os.path.exists(refed_file):
-                refed_file = resolve_path(os.path.dirname(folder), file_path)
+                refed_file = resolve_path(folder, file_path)
                 if not os.path.exists(refed_file):
                     raise Exception(f"File not found: {refed_file}")
             # use cache
             cache_key = f'{refed_file}:{content}'
             if cache_key in REF_FILE_CACHE:
                 ref_map[refed_file] = REF_FILE_CACHE[cache_key]
                 return REF_FILE_CACHE[cache_key]
@@ -201,19 +244,14 @@
 
 
 def get_content(filepath):
     with open(filepath, 'r') as f:
         return f.read()
 
 
-def load_yaml(filepath):
-    with open(filepath, 'r') as f:
-        return yaml.safe_load(f)
-
-
 def ref_yaml_content(folder, content, ref_map):
     # load yaml obj from another file into current yaml
     reg = r"^\$yaml_content\((.+)\)$"
     if type(content) == str:
 
         match = re.match(reg, content)
         if match:
@@ -224,15 +262,15 @@
             if not os.path.exists(referred_file) and ".trash" in referred_file:
                 referred_file = referred_file.replace("/.trash", "")
             if not os.path.exists(referred_file):
                 referred_file = resolve_path(
                     os.path.dirname(folder), file_path)
                 if not os.path.exists(referred_file):
                     raise Exception(f"File not found: {referred_file}")
-            file_content = load_yaml(referred_file)
+            file_content = yaml_load(referred_file)
             return file_content
         return content
     elif type(content) == dict:
         for k, v in content.items():
             content[k] = ref_yaml_content(folder, v, ref_map)
         return content
     elif type(content) == list:
@@ -308,26 +346,40 @@
         ref_map = {}
         ref_all(filename, content, ref_map, False)
         for ref in ref_map.keys():
             references[ref].append(filename)
     return references
 
 
-def preprocess(content, info, folder, enable_ref_file=True, wait_for_ref=False):
+def resolve_ref_and_operators(folder, content,  wait_for_ref=False):
+    ref_map = {}
+    content = ref_file(folder, content, ref_map, wait_for_ref)
+    content = ref_yaml_content(folder, content, ref_map)
+    content = ref_file_content(folder, content, ref_map)
+    content = apply_operators(content)
+    return content
+
+
+def preprocess(content, info, folder, input_variables, enable_ref_file=True, wait_for_ref=False):
     kind = verify(content)
     variables = get_variables(folder, info)
+    variables = merge_dict([variables, input_variables])
     content = var_replace(content, variables)
     ref_map = {}
     if enable_ref_file:
         content = ref_file(folder, content, ref_map, wait_for_ref)
         content = ref_yaml_content(folder, content, ref_map)
         content = ref_file_content(folder, content, ref_map)
+    content = var_replace(content, variables)
     content = apply_operators(content)
     return kind, info, content
 
 
-def preprocess_file(filename, enable_ref_file=True, wait_for_ref=False):
-    info = parse_filename(filename)
+def preprocess_file(filename, input_variables, enable_ref_file=True, wait_for_ref=False):
+    if config.config.filename:
+        info = parse_filename(config.config.filename, True)
+    else:
+        info = parse_filename(filename, True)
     folder = os.path.dirname(filename)
     with open(filename) as f:
         content = yaml.safe_load(f)
-    return preprocess(content, info, folder, enable_ref_file, wait_for_ref)
+    return preprocess(content, info, folder, input_variables, enable_ref_file, wait_for_ref)
```

### Comparing `infra_operator-1.0.22/api_to_yaml/read/mod.py` & `infra_operator-1.0.23/src/infra_operator/read/mod.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import json
+import base64
 from functools import partial
-from api_to_yaml.clients.mod import clients
-from api_to_yaml.operators.mod import override, remove_inner_fields, sort_tags
+from infra_operator.clients.mod import clients
+from infra_operator.operators.mod import list_to_tags, override, remove_fields, remove_inner_fields, rename_fields, sort_tags, to_args
+
+
+def inactive_as_not_exist(res):
+    if res.get("status") == "INACTIVE":
+        return None
+    return res
 
 
 def unpack_get_response(res, multi=False):
     keys = res.keys() - set(["ResponseMetadata",
                              "failures", "IsTruncated", "tags"])
     if len(keys) != 1:
         raise Exception("unable to unpack response", res)
@@ -19,14 +26,33 @@
             return obj
         if len(obj) > 1:
             raise Exception("got multiple objects, expected one or zero", res)
         return obj[0] if len(obj) == 1 else None
     return obj
 
 
+def unpack_field(field, multi=False):
+    def wrap(res):
+        if res is None:
+            return res
+        if field in res:
+            obj = res[field]
+            if type(obj) == list:
+                if multi:
+                    return obj
+                if len(obj) > 1:
+                    raise Exception(
+                        "got multiple objects, expected one or zero", res)
+                return obj[0] if len(obj) == 1 else None
+            else:
+                return obj
+        return None
+    return wrap
+
+
 def unpack_get_queue_response(result):
     res = result.attributes
     if 'QueueArn' in res:
         res['QueueUrl'] = result.url  # add URL, that will be used in deletion
         return res
     else:
         raise Exception("unable to unpack response", res, result)
@@ -100,14 +126,28 @@
             current["ResourcePolicy"] = json.loads(rp)
     except Exception as e:
         if 'it was marked for deletion' not in str(e):
             raise e
     return current
 
 
+def get_launch_template_latest_version(current):
+    if not current:
+        return current
+    response = clients["ec2"].describe_launch_template_versions(
+        LaunchTemplateName='tf_bin_dev_nginx_test_lt',
+        MaxResults=1
+    )
+    if len(response.get("LaunchTemplateVersions", [])):
+        current["LaunchTemplateData"] = response["LaunchTemplateVersions"][0]["LaunchTemplateData"]
+        if "UserData" in current["LaunchTemplateData"]:
+            current["LaunchTemplateData"]["UserData"] = base64.b64decode(current["LaunchTemplateData"]["UserData"]).decode(encoding="utf-8")
+    return current
+
+
 def get_alb_listener_rules(listener):
     res = clients["elbv2"].describe_rules(ListenerArn=listener["ListenerArn"])
     rules = unpack_get_response(res, True)
     tidied_rules = []
     for rule in rules:
         if rule["Priority"] == "default":
             continue
@@ -170,16 +210,16 @@
     response = clients["ec2"].describe_security_group_rules(Filters=[{
         "Name":
         "group-id",
         "Values": [GroupId]
     }],
         MaxResults=1000)
     rules = unpack_get_response(response, True)
-    rules.sort(key=lambda rule: (rule["IsEgress"], rule["IpProtocol"],
-               rule.get("FromPort"), rule.get("ToPort"), rule.get("CidrIpv4")))
+    rules.sort(key=lambda rule: (rule.get("IsEgress", False), rule.get("IpProtocol", "-1"),
+               rule.get("FromPort", 0), rule.get("ToPort", 65535), rule.get("CidrIpv4", "")))
     current["Rules"] = rules
     return current
 
 
 def sort_ip_ranges(ip_permission):
     ip_permission["IpRanges"].sort(key=lambda one: one["CidrIp"])
     return ip_permission
@@ -205,14 +245,52 @@
         return None
     for svc in current.get("Services", []):
         if svc.get("Name") == name:
             return svc
     return None
 
 
+def get_instance_ebs_volume(current):
+    if current is None:
+        return None
+    for one in current["BlockDeviceMappings"]:
+        VolumeId = one["Ebs"]["VolumeId"]
+        DeleteOnTermination = one["Ebs"]["DeleteOnTermination"]
+        volume = unpack_get_response(
+            clients["ec2"].find_volume(VolumeId=VolumeId))
+        clean = remove_fields(
+            ["State", "CreateTime", "Attachments", "AvailabilityZone", "MultiAttachEnabled"])(volume)
+        clean = rename_fields({"Size": "VolumeSize"})(clean)
+        if clean["VolumeType"] == "gp2":
+            del clean["Iops"]
+        if clean["SnapshotId"] == "":
+            del clean["SnapshotId"]
+        clean["DeleteOnTermination"] = DeleteOnTermination
+        if len(clean.get("Tags", [])) > 0:
+            tags = clean.pop("Tags")
+            if "TagSpecifications" not in current:
+                current["TagSpecifications"] = []
+            if len(list(filter(lambda one: one["ResourceType"] == "volume", current["TagSpecifications"]))) == 0:
+                current["TagSpecifications"].append({
+                    "ResourceType": "volume",
+                    "Tags": list_to_tags(tags)
+                })
+        one["Ebs"] = clean
+    return current
+
+
+def get_repo_lifecycle_policy(current):
+    registryId = current["registryId"]
+    repositoryName = current["repositoryName"]
+    res = clients["ecr"].get_lifecycle_policy(
+        registryId=registryId, repositoryName=repositoryName)
+    current["lifecycle-policy"] = json.loads(res["lifecyclePolicyText"])
+    return current
+
+
 def get_role_policies(current):
     RoleName = current["RoleName"]
     PolicyNames = [
         one
         for res in clients["iam"].get_paginator("list_role_policies").paginate(
             RoleName=RoleName) for one in unpack_get_response(res, True)
     ]
@@ -277,82 +355,125 @@
         current["routes"].append({
             "name": desc["gatewayRouteName"],
             **desc["spec"]
         })
     return current
 
 
+def find_secret(results, name):
+    filtered = list(filter(lambda obj: obj.get('Name') == name, results))
+    if len(filtered) > 1:
+        raise Exception(
+            "impossible error, find more than one secrets", filtered)
+    if len(filtered) == 0:
+        return
+    return filtered[0]
+
+
 def get_name(content, kind, info):
     if content is None:
         content = {}
     switch = {
+        "Instance": to_args(content).get("Tags", {}).get("Name"),
+        "Repository": override(to_args(content).get("repositoryName")),
+        "ECS/Cluster":
+        override(info.get("name"),
+                 to_args(content).get("clusterName"),
+                 content.get("clusterName")),
         "TaskDefinition":
         override(info.get("name"),
-                 content.get("metadata", {}).get("family")),
+                 to_args(content).get("family"),
+                 content.get("family")),
         "TargetGroup":
         override(info.get("name"),
-                 content.get("metadata", {}).get("Name")),
+                 to_args(content).get("Name"),
+                 content.get("Name")),
         "Service":
         override(info.get("name"),
-                 content.get("metadata", {}).get("serviceName")),
+                 to_args(content).get("serviceName"),
+                 content.get("serviceName")),
         "LoadBalancer":
         override(info.get("name"),
-                 content.get("metadata", {}).get("Name")),
+                 to_args(content).get("Name"),
+                 content.get("Name")),
         "SecurityGroup":
         override(info.get("name"),
-                 content.get("metadata", {}).get("GroupName")),
+                 to_args(content).get("GroupName"),
+                 content.get("GroupName")),
         "Role":
         override(info.get("name"),
-                 content.get("metadata", {}).get("RoleName")),
+                 to_args(content).get("RoleName"),
+                 content.get("RoleName")),
         "Repo":
         override(info.get("name"),
-                 content.get("metadata", {}).get("RepoName")),
+                 to_args(content).get("RepoName"),
+                 content.get("RepoName")),
         "Org":
         override(info.get("organization"),
-                 content.get("metadata", {}).get("Organization")),
+                 to_args(content).get("Organization"),
+                 content.get("Organization")),
         "Mesh":
-        override(info.get("name"),
-                 content.get("metadata", {}).get("meshName")),
+        override(info.get("mesh"),
+                 to_args(content).get("meshName"),
+                 content.get("meshName")),
         "VirtualNode":
         override(info.get("name"),
-                 content.get("metadata", {}).get("virtualNodeName")),
+                 to_args(content).get("virtualNodeName"),
+                 content.get("virtualNodeName")),
         "VirtualRouter":
         override(info.get("name"),
-                 content.get("metadata", {}).get("virtualRouterName")),
+                 to_args(content).get("virtualRouterName"),
+                 content.get("virtualRouterName")),
         "Route":
         override(info.get("name"),
-                 content.get("metadata", {}).get("routeName")),
+                 to_args(content).get("routeName"),
+                 content.get("routeName")),
         "VirtualGateway":
         override(info.get("name"),
-                 content.get("metadata", {}).get("virtualGatewayName")),
-        "VirtualGatewayRoute":
+                 to_args(content).get("virtualGatewayName"),
+                 content.get("virtualGatewayName")),
+        "GatewayRoute":
         override(info.get("name"),
-                 content.get("metadata", {}).get("gatewayRouteName")),
+                 to_args(content).get("gatewayRouteName"),
+                 content.get("gatewayRouteName")),
         "VirtualService":
         override(info.get("name"),
-                 content.get("metadata", {}).get("virtualServiceName")),
+                 to_args(content).get("virtualServiceName"),
+                 content.get("virtualServiceName")),
         "ServiceDiscoveryService":
         override(info.get("name"),
-                 content.get("metadata", {}).get("Name")),
+                 to_args(content).get("Name"),
+                 content.get("Name")),
         "Secret":
         override(info.get("name"),
-                 content.get("metadata", {}).get("Name")),
+                 to_args(content).get("Name"),
+                 content.get("Name")),
         "ScalingPolicy":
         override(info.get("name"),
-                 content.get("metadata", {}).get("PolicyName")),
+                 to_args(content).get("PolicyName"),
+                 content.get("PolicyName")),
         "Distribution": info.get("name"),
-        "CachePolicy": override(info.get("name"), content.get("metadata", {}).get("Name")),
+        "CachePolicy": override(info.get("name"), to_args(content).get("Name")),
+        "Volume": to_args(content).get("Tags", {}).get("Name"),
     }
     if kind in switch:
         return switch[kind]
     return info.get("name")
 
 
 def get_resource(content, kind, info):
     switch = {
+        "Instance": ("ec2", "find_instance", {
+            "InstanceId": to_args(content).get("InstanceId"),
+            "Name": get_name(content, kind, info)
+        }, [unpack_get_response, unpack_field("Instances"), get_instance_ebs_volume]),
+        "ECS/Cluster": ("ecs", "describe_clusters", {
+            "clusters": [get_name(content, kind, info)],
+            "include": ["ATTACHMENTS", "CONFIGURATIONS", "SETTINGS", "TAGS"]
+        }, [unpack_get_response, inactive_as_not_exist]),
         "TaskDefinition": ("ecs", "describe_task_definition", {
             "taskDefinition": get_name(content, kind, info)
         }, [unpack_get_response]),
         "TargetGroup": ("elbv2", "describe_target_groups", {
             "Names": [get_name(content, kind, info)]
         }, [unpack_get_response]),
         "Service": ("ecs", "describe_services", {
@@ -384,74 +505,74 @@
         "VirtualNode": ("appmesh", "describe_virtual_node", {
             "virtualNodeName": get_name(content, kind, info),
             "meshName": content.get("metadata", {}).get("meshName")
         }, [unpack_get_response]),
         "VirtualRouter": ("appmesh", "describe_virtual_router", {
             "virtualRouterName":
             get_name(content, kind, info),
-            "meshName":
-            content.get("metadata", {}).get("meshName")
+            "meshName": content.get("metadata", {}).get("meshName")
         }, [unpack_get_response, get_router_routes]),
         "Route": ("appmesh", "describe_route", {
             "routeName":
             get_name(content, kind, info),
-            "meshName":
-            content.get("metadata", {}).get("meshName"),
-            "virtualRouterName":
-            content.get("metadata", {}).get("virtualRouterName")
+            "meshName": content.get("metadata", {}).get("meshName"),
+            "virtualRouterName": content.get("metadata", {}).get("virtualRouterName")
         }, [unpack_get_response]),
         "VirtualGateway": ("appmesh", "describe_virtual_gateway", {
             "virtualGatewayName":
             get_name(content, kind, info),
-            "meshName":
-            content.get("metadata", {}).get("meshName")
+            "meshName": content.get("metadata", {}).get("meshName")
         }, [unpack_get_response, get_gateway_routes]),
-        "VirtualGatewayRoute": ("appmesh", "describe_gateway_route", {
+        "VirtualGateways": ("appmesh", "list_virtual_gateways", {
+            "meshName": content.get("metadata", {}).get("meshName")
+        }, [lambda res: unpack_get_response(res, True), lambda res: list(map(get_gateway_routes, res))]),
+        "GatewayRoute": ("appmesh", "describe_gateway_route", {
             "gatewayRouteName":
             get_name(content, kind, info),
-            "meshName":
-            content.get("metadata", {}).get("meshName"),
-            "virtualGatewayName":
-            content.get("metadata", {}).get("virtualGatewayName")
+            "meshName": content.get("metadata", {}).get("meshName"),
+            "virtualGatewayName": content.get("metadata", {}).get("virtualGatewayName")
         }, [unpack_get_response]),
         "VirtualService": ("appmesh", "describe_virtual_service", {
             "virtualServiceName":
             get_name(content, kind, info),
-            "meshName":
-            content.get("metadata", {}).get("meshName")
+            "meshName": content.get("metadata", {}).get("meshName")
         }, [unpack_get_response]),
         "ServiceDiscoveryService": ("servicediscovery", "list_services", {
             "Filters": [{
                 "Name":
                 "NAMESPACE_ID",
                 "Values": [content.get("metadata", {}).get("NamespaceId")]
             }]
         }, [partial(get_sd_service, get_name(content, kind, info))]),
         "Secret": ("secretsmanager", "list_secrets", {
             "Filters": [{
                 "Key": "name",
                 "Values": [get_name(content, kind, info)]
             }]
-        }, [unpack_get_response, get_secret_resource_policy]),
+        }, [
+            lambda res: unpack_get_response(res, True),
+            lambda res: find_secret(res, get_name(content, kind, info)),
+            get_secret_resource_policy]),
         "ScalingPolicy": ("app_scaling", "describe_scaling_policies", {
             "PolicyNames": [get_name(content, kind, info)],
             "ServiceNamespace": content.get("metadata", {}).get("ServiceNamespace"),
             "ResourceId": content.get("metadata", {}).get("ResourceId", ""),
         }, [unpack_get_response]),
         "ScalableTarget": ("app_scaling", "describe_scalable_targets", {
             "ServiceNamespace": content.get("metadata", {}).get("ServiceNamespace"),
             "ResourceIds": [content.get("metadata", {}).get("ResourceId", "")],
             "ScalableDimension": content.get("metadata", {}).get("ScalableDimension", ""),
         }, [unpack_get_response]),
         "Queue": ("sqs", "get_queue_by_name", {
             "QueueName": content.get("metadata", {}).get("QueueName")
         }, [unpack_get_queue_response]),
-        "LaunchTemplate": ("ec2", "describe_launch_templates", {
-            "LaunchTemplateNames": [content.get("metadata", {}).get("LaunchTemplateName")]
-        }, [unpack_get_response]),
+        "LaunchTemplate": ("ec2", "find_launch_template", {
+            "LaunchTemplateId": content.get("metadata", {}).get("LaunchTemplateId"),
+            "LaunchTemplateName": content.get("metadata", {}).get("LaunchTemplateName"),
+        }, [unpack_get_response, get_launch_template_latest_version]),
         "Lambda": ("lambda", "get_function", {
             "FunctionName": content.get("metadata", {}).get("FunctionName")
         }, [unpack_get_lambda_response]),
         "AutoScalingGroup": ("asg", "describe_auto_scaling_groups", {
             "AutoScalingGroupNames": [content.get("metadata", {}).get("AutoScalingGroupName")]
         }, [unpack_get_response]),
         "LambdaEventSource": ("lambda", "list_event_source_mappings", {
@@ -477,14 +598,22 @@
             "Id": content.get("metadata", {}).get("Id"),
             "Name": content.get("metadata", {}).get("Name"),
         }, [check_name(get_name(content, kind, info), kind)]),
         "ContinuousDeploymentPolicy": ("cloudfront", "try_get_continuous_deployment_policy", {
             "Id": content.get("metadata", {}).get("Id"),
             "StagingDistributionDnsNames": content.get("spec", {}).get("StagingDistributionDnsNames"),
         }, [unpack_get_continuous_deployment_policy_response]),
+        "Repository": ("ecr", "find_repository", {
+            "registryId": to_args(content).get("registryId"),
+            "repositoryName": get_name(content, kind, info),
+        }, [unpack_get_response, get_repo_lifecycle_policy]),
+        "Volume": ("ec2", "find_volume", {
+            "VolumeId": to_args(content).get("VolumeId"),
+            "Name": get_name(content, kind, info),
+        }, [unpack_get_response]),
     }
     api, method, kwargs, processes = switch[kind]
     client = clients[api]
     func = getattr(client, method)
     try:
         res = func(**kwargs)
     except Exception as ex:
```

### Comparing `infra_operator-1.0.22/api_to_yaml/update/aws_iam_update.py` & `infra_operator-1.0.23/src/infra_operator/update/aws_iam_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import json
 import boto3
 
-from api_to_yaml.operators.mod import dict_matcher, list_to_dict_by
+from infra_operator.operators.mod import dict_matcher, list_to_dict_by
 
 client = boto3.client('iam')
 
 
 def trust_relationship_update(content, current):
     RoleName = current["RoleName"]
-    content = content.get("metadata", {}).get("AssumeRolePolicyDocument")
+    content = content.get("AssumeRolePolicyDocument")
     current = current.get("AssumeRolePolicyDocument")
     if content != current:
         client.update_assume_role_policy(
             RoleName=RoleName,
             PolicyDocument=json.dumps(content)
         )
 
 
 def meta_update(content, current):
     RoleName = current["RoleName"]
-    content = content.get("metadata")
     if current.get("Description") != content.get("Description") or current.get("MaxSessionDuration") != content.get("MaxSessionDuration"):
         client.update_role(RoleName=RoleName, Description=content.get(
             "Description", current["Description"]), MaxSessionDuration=content.get("MaxSessionDuration", current["MaxSessionDuration"]))
 
 
 def inline_policy_update(content, current):
     RoleName = current["RoleName"]
     target_policies = {k: v["PolicyDocument"] for k, v in list_to_dict_by(
-        "PolicyName")(content.get("spec", {}).get("inline-policies", [])).items()}
+        "PolicyName")(content.get("inline-policies", [])).items()}
     current_policies = {k: v["PolicyDocument"] for k, v in list_to_dict_by(
-        "PolicyName")(current.get("inline-policy", [])).items()}
+        "PolicyName")(current.get("inline-policies", [])).items()}
     to_delete, to_create, to_update, unchanged = dict_matcher(
         target_policies, current_policies)
     for key in to_create + to_update:
         client.put_role_policy(
             RoleName=RoleName,
             PolicyName=key,
             PolicyDocument=json.dumps(target_policies[key])
@@ -48,17 +47,17 @@
             PolicyName=key
         )
 
 
 def managed_policy_update(content, current):
     RoleName = current["RoleName"]
     target_policies = {v["PolicyArn"]: True for k, v in list_to_dict_by(
-        "PolicyArn")(content.get("spec", {}).get("managed-policies", [])).items()}
+        "PolicyArn")(content.get("managed-policies", [])).items()}
     current_policies = {v["PolicyArn"]: True for k, v in list_to_dict_by(
-        "PolicyArn")(current.get("spec", {}).get("managed-policies", [])).items()}
+        "PolicyArn")(current.get("managed-policies", [])).items()}
     to_delete, to_create, to_update, unchanged = dict_matcher(
         target_policies, current_policies)
     for key in to_create + to_update:
         client.attach_role_policy(
             RoleName=RoleName,
             PolicyArn=key
         )
```

### Comparing `infra_operator-1.0.22/api_to_yaml/update/aws_sg_update.py` & `infra_operator-1.0.23/src/infra_operator/update/aws_sg_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import boto3
 
-from api_to_yaml.operators.mod import dict_matcher, list_to_dict_by, remove_inner_fields, to_args, with_ec2_tags, with_tags
-from api_to_yaml.layout.mod import parse as filename_parse
+from infra_operator.operators.mod import dict_matcher, list_to_dict_by, with_ec2_tags, with_tags
 
 
 client = boto3.client('ec2')
 
 
 def get_key(one):
     if "CidrIpv4" in one:
@@ -59,25 +58,25 @@
                 if key in rule:
                     if key in ignoreFields:
                         for one in rule[key]:
                             if ignoreFields[key] in one:
                                 one.pop(ignoreFields[key])
                     target_rule_dict.update(
                         list_to_dict_by(
-                            lambda obj: (key, rule.get("IpProtocol"), rule.get("FromPort"), rule.get("ToPort"), obj.get(subKeys[key])))(rule[key]))
+                            lambda obj: (key, rule.get("IpProtocol","-1"), rule.get("FromPort", 0), rule.get("ToPort", 65535), obj.get(subKeys[key])))(rule[key]))
         for rule in current:
             for key in Keys:
                 if key in rule:
                     if key in ignoreFields:
                         for one in rule[key]:
                             if ignoreFields[key] in one:
                                 one.pop(ignoreFields[key])
                     current_rule_dict.update(
                         list_to_dict_by(
-                            lambda obj: (key, rule.get("IpProtocol"), rule.get("FromPort"), rule.get("ToPort"), obj.get(subKeys[key])))(rule[key]))
+                            lambda obj: (key, rule.get("IpProtocol","-1"), rule.get("FromPort", 0), rule.get("ToPort", 65535), obj.get(subKeys[key])))(rule[key]))
         to_delete, to_create, to_update, unchanged = dict_matcher(
             target_rule_dict, current_rule_dict)
         for compound_key in to_create:
             key, IpProtocol, FromPort, ToPort, val = compound_key
             inner_obj = target_rule_dict[compound_key]
             func = getattr(client, f"authorize_security_group_{sg_type}")
             args = {"GroupId": group_id,
```

### Comparing `infra_operator-1.0.22/api_to_yaml/update/ghe_update.py` & `infra_operator-1.0.23/src/infra_operator/update/ghe_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-from api_to_yaml.layout.mod import parse as filename_parse
+from infra_operator.layout.mod import parse as filename_parse
 import os
 from github import Github
 
-from api_to_yaml.operators.mod import dict_matcher
+from infra_operator.operators.mod import dict_matcher
 
 github = Github(base_url="https://git.toolsfdg.net/api/v3",
                 login_or_token=os.getenv('GITHUB_TOKEN'), retry=3)
 
 
 def collaborator_update(content, current):
     repo = github.get_organization(current["metadata"]["Organization"]).get_repo(
```

### Comparing `infra_operator-1.0.22/api_to_yaml/update/mod.py` & `infra_operator-1.0.23/src/infra_operator/update/mod.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from copy import deepcopy
 import oyaml as yaml
-from api_to_yaml.clients.mod import clients
-from api_to_yaml.create.aws_appmesh import AppMeshController
-from api_to_yaml.create.mod import ECSServiceController
-from api_to_yaml.operators.mod import add_field, add_items_quantity, drop_tags, list_to_tags, metadata_to_args, override, remove_fields, tags_to_list, to_args, transform, with_args, with_default, with_tags
-import api_to_yaml.create.aws_elbv2_create as elbv2_create
-import api_to_yaml.update.aws_iam_update as iam_update
-import api_to_yaml.update.ghe_update as ghe_update
-import api_to_yaml.create.aws_secretsmanager as secretsmanager_client
-import api_to_yaml.update.aws_sg_update as sg_update
+from infra_operator.clients.mod import clients
+from infra_operator.create.aws_appmesh import AppMeshController
+from infra_operator.create.mod import ECSServiceController
+from infra_operator.operators.mod import add_field, add_items_quantity, drop_tags, list_to_tags, metadata_to_args, override, remove_fields, rename_fields, tags_to_list, to_args, transform, with_args, with_default, with_tags
+import infra_operator.create.aws_elbv2_create as elbv2_create
+import infra_operator.update.aws_iam_update as iam_update
+import infra_operator.update.ghe_update as ghe_update
+import infra_operator.create.aws_secretsmanager as secretsmanager_client
+import infra_operator.update.aws_sg_update as sg_update
 
 ecs = clients["ecs"]
 task_set_ecs = ECSServiceController()
 elbv2 = clients["elbv2"]
 ec2 = clients["ec2"]
 iam = clients["iam"]
 appmesh = clients["appmesh"]
@@ -61,20 +61,25 @@
             cloudfront.untag_resource(
                 Resource=arn, TagKeys={"Items": untags})
     return wrap
 
 
 def update(kind, content, info, current, line):
     switch = {
+        "ECS/Cluster": (ecs, "update_cluster", [
+            to_args,
+            rename_fields({"clusterName": "cluster"}),
+            remove_fields(["tags"])
+        ], []),
         "TaskDefinition": (ecs, "register_task_definition", [
             to_args,
             with_tags(capitalize=False, info=info),
             with_default({
                 "family":
-                override(info["name"],
+                override(info.get("name"),
                          content.get("metadata", {}).get("family"))
             })
         ], []),
         "TargetGroup": (elbv2, "modify_target_group", [
             to_args,
             with_tags(capitalize=True, info=info),
             with_default({"TargetGroupArn": current.get("TargetGroupArn")}),
@@ -83,27 +88,27 @@
         ], []),
         "Service": (task_set_ecs, "update_service", [
             to_args,
             with_default({
                 "cluster":
                 info.get("ecs_cluster"),
                 "service":
-                override(info["name"],
+                override(info.get("name"),
                          content.get("metadata", {}).get("serviceName"))
             })
         ], [
             lambda res: update_service_tags(
                 res['service']['serviceArn'],
                 with_tags(capitalize=False, info=info)
                 (to_args(content)).get("tags", []))
         ]),
         "LoadBalancer": (elbv2_create, "update_load_balancer", [
             with_args({
                 "kind": kind,
-                "content": content,
+                "content": to_args(content),
                 "info": info,
                 "current": current
             }),
             elbv2_create.alb_canary_config_hook(line)
         ], []),
         "SecurityGroup": (sg_update, "update_security_group", [
             lambda _: {
@@ -118,15 +123,15 @@
                 "tags":
                 current.get("metadata", {}).get("tags", {})
             }
         ], []),
         "Role": (iam_update, "update_role", [
             with_args({
                 "kind": kind,
-                "content": content,
+                "content": to_args(content),
                 "info": info,
                 "current": current
             })
         ], []),
         "Repo": (ghe_update, "update_repo", [
             with_args({
                 "kind": kind,
@@ -164,15 +169,15 @@
         "VirtualGateway": (custom_appmesh, "update_virtual_gateway", [
             metadata_to_args,
             remove_fields(["tags"]),
             with_default({
                 "spec": content.get("spec"),
             })
         ], []),
-        "VirtualGatewayRoute": (appmesh, "update_gateway_route", [
+        "GatewayRoute": (appmesh, "update_gateway_route", [
             metadata_to_args,
             remove_fields(["tags"]),
             with_default({
                 "spec": content.get("spec"),
             })
         ], []),
         "VirtualService": (appmesh, "update_virtual_service", [
@@ -232,16 +237,16 @@
             lambda args: {
                 "Id": args.pop("Id"),
                 "IfMatch": args.pop("ETag"),
                 "DistributionConfig": args
             }
         ], [
             cloudfront_update_tags(
-                f'arn:aws:cloudfront::{sts.get_account_id()}:distribution/{content["metadata"]["Id"]}',
-                content["metadata"].get("Tags", [])
+                f'arn:aws:cloudfront::{sts.get_account_id()}:distribution/{content.get("metadata", {}).get("Id")}',
+                content.get("metadata", {}).get("Tags", [])
             )
         ]),
         "CachePolicy": (cloudfront, "update_cache_policy", [
             to_args,
             add_field("ETag", current.get("ETag")),
             add_items_quantity,
             lambda args: {
```

### Comparing `infra_operator-1.0.22/api_to_yaml/validate/mod.py` & `infra_operator-1.0.23/src/infra_operator/validate/mod.py`

 * *Files identical despite different names*

### Comparing `infra_operator-1.0.22/LICENSE` & `infra_operator-1.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `infra_operator-1.0.22/pyproject.toml` & `infra_operator-1.0.23/server/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [project]
-name = "infra-operator"
-version = "1.0.22"
+name = "infra-operator-server"
+version = "1.0.23"
 authors = [
   { name="Desmond", email="desmond.cao@binance.com" },
 ]
-description = "Turn apis into declarative yaml files"
+description = "Provide api for turning apis into declarative yaml files"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-  'oyaml==1.0',
-  'boto3==1.26.65',
-  'PyGithub==1.57',
+  'infra-operator==1.0.22',
+  'Flask==2.2.3'
 ]
 
 [project.urls]
-"Homepage" = "https://git.toolsfdg.net/devops/api-mapper"
-"Bug Tracker" = "https://git.toolsfdg.net/devops/api-mapper/issues"
+"Homepage" = "https://git.toolsfdg.net/devops/infra-operator"
+"Bug Tracker" = "https://git.toolsfdg.net/devops/infra-operator/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
-  "api_to_yaml/**/*.py"
+  "src/**/*.py"
 ]
```

