# Comparing `tmp/iambic_core-0.7.6.tar.gz` & `tmp/iambic_core-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.7.6.tar", max compression
+gzip compressed data, was "iambic_core-0.8.1.tar", max compression
```

## Comparing `iambic_core-0.7.6.tar` & `iambic_core-0.8.1.tar`

### file list

```diff
@@ -1,158 +1,163 @@
--rw-r--r--   0        0        0    11356 2023-05-15 14:23:53.922064 iambic_core-0.7.6/LICENSE.md
--rw-r--r--   0        0        0    10551 2023-05-15 14:23:53.922064 iambic_core-0.7.6/README.md
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/__init__.py
--rw-r--r--   0        0        0    20099 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/templates.py
--rw-r--r--   0        0        0     3312 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/utils.py
--rw-r--r--   0        0        0    77079 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/logger.py
--rw-r--r--   0        0        0    24862 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5516 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/parser.py
--rw-r--r--   0        0        0    48014 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/template_generation.py
--rw-r--r--   0        0        0    28445 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/lambda/app.py
--rw-r--r--   0        0        0    14239 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/main.py
--rw-r--r--   0        0        0      664 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/__init__.py
--rw-r--r--   0        0        0     2799 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1753 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     2149 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     2268 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     2483 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    16350 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    33385 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    18144 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13616 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15896 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    18077 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10649 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21757 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24395 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    21076 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22579 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4534 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31619 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35514 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    28498 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1291 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     3009 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10183 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13766 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8515 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8648 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      908 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5247 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1359 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9282 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11393 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2685 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1290 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9492 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13610 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      864 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      173 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     2243 2023-05-15 14:23:53.962067 iambic_core-0.7.6/pyproject.toml
--rw-r--r--   0        0        0    12917 1970-01-01 00:00:00.000000 iambic_core-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-30 20:48:04.299115 iambic_core-0.8.1/LICENSE.md
+-rw-r--r--   0        0        0    15630 2023-05-30 20:48:04.299115 iambic_core-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20099 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/templates.py
+-rw-r--r--   0        0        0     3312 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/utils.py
+-rw-r--r--   0        0        0    77625 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/logger.py
+-rw-r--r--   0        0        0    24977 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5516 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/parser.py
+-rw-r--r--   0        0        0    48021 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    31220 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/lambda/app.py
+-rw-r--r--   0        0        0    14289 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2799 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2728 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2268 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2712 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     2102 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    17407 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0     1721 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    39352 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    18144 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13681 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15896 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    18077 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10706 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21757 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24521 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    21076 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22644 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     5650 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31619 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35636 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    30301 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/exceptions.py
+-rw-r--r--   0        0        0    18860 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/models.py
+-rw-r--r--   0        0        0    11040 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py
+-rw-r--r--   0        0        0    19286 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py
+-rw-r--r--   0        0        0     1291 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     3009 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10209 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    14003 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8515 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8798 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      908 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14801 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5237 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1359 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9327 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11442 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2685 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1290 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9587 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13610 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      864 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      994 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      173 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     2312 2023-05-30 20:48:04.347116 iambic_core-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    18129 1970-01-01 00:00:00.000000 iambic_core-0.8.1/PKG-INFO
```

### Comparing `iambic_core-0.7.6/LICENSE.md` & `iambic_core-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/config/dynamic_config.py` & `iambic_core-0.8.1/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/config/utils.py` & `iambic_core-0.8.1/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/config/wizard.py` & `iambic_core-0.8.1/iambic/config/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from iambic.plugins.v0_1_0.aws.iam.role.models import (
     AWS_IAM_ROLE_TEMPLATE_TYPE,
     AwsIamRoleTemplate,
 )
 from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
 from iambic.plugins.v0_1_0.aws.models import (
     ARN_RE,
+    IAMBIC_CHANGE_DETECTION_SUFFIX,
     IAMBIC_HUB_ROLE_NAME,
     IAMBIC_SPOKE_ROLE_NAME,
     AWSAccount,
     AWSIdentityCenter,
     AWSOrganization,
     BaseAWSOrgRule,
     Partition,
@@ -912,17 +913,15 @@
         else:
             created_successfully = asyncio.run(
                 create_spoke_role_stack(
                     cf_client=cf_client,
                     hub_account_id=account_id,
                     role_arn=role_arn,
                     read_only=read_only,
-                    hub_role_stack_name=hub_role_name,
                     hub_role_name=hub_role_name,
-                    spoke_role_stack_name=spoke_role_name,
                     spoke_role_name=spoke_role_name,
                     tags=tags,
                 )
             )
             if not created_successfully:
                 log.error(
                     "Failed to create the required IAMbic role. Account not added."
@@ -989,26 +988,26 @@
                 "No editable accounts found.\n"
                 "TIP: An AWS account cannot be edited if it attached to an Organization in the config."
             )
             return
         else:
             account = self.config.aws.accounts[0]
 
-        choices = ["Go back", "Update IAMbic control", "Update Region"]
+        choices = ["Go back", "Update region"]
         if not account.org_id:
             choices.append("Update name")
 
         while True:
             action = questionary.select(
                 "What would you like to do?",
                 choices=choices,
             ).unsafe_ask()
             if action == "Go back":
                 return
-            elif action == "Update name":
+            elif action == "Update region":
                 account.default_region = set_aws_region(
                     "What region should IAMbic use?", account.default_region
                 )
             elif action == "Update name":
                 account.account_name = questionary.text(
                     "What is the name of the AWS Account?",
                     default=account.account_name,
@@ -1831,48 +1830,59 @@
             default="",
             validate=validate_aws_cf_input_tags,
         ).ask()
         tags = aws_cf_parse_key_value_string(unparse_tags)
         return hub_role_name, spoke_role_name, tags
 
     def configuration_wizard_change_detection_setup(self, aws_org: AWSOrganization):
+        self.setup_aws_configuration()
         click.echo(
             "\nTo setup change detection for iambic it requires creating CloudFormation stacks "
             "and a CloudFormation stack set.\n"
             "To review the templates used or deploy them manually, the IdentityRule templates used can be found here:\n"
             "https://github.com/noqdev/iambic/tree/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates\n"
             "If you have already manually deployed the templates, answer yes to proceed.\n"
             "IAMbic will validate that your stacks have been deployed successfully and will not attempt to replace them."
         )
+        unparse_tags = questionary.text(
+            "Add Tags (leave blank or `team=ops_team, cost_center=engineering`): ",
+            default="",
+            validate=validate_aws_cf_input_tags,
+        ).ask()
+        tags = aws_cf_parse_key_value_string(unparse_tags)
         if not questionary.confirm("Proceed?").unsafe_ask():
             return
 
         session, _ = self.get_boto3_session_for_account(aws_org.org_account_id)
+        # cloudtrail is not cross-region, so we need to use us-east-1
         cf_client = session.client(
-            "cloudformation", region_name=self.aws_default_region
+            "cloudformation", region_name="us-east-1"  # self.aws_default_region
         )
         org_client = session.client(
             "organizations", region_name=self.aws_default_region
         )
 
         successfully_created = asyncio.run(
             create_iambic_eventbridge_stacks(
                 cf_client,
                 org_client,
                 aws_org.org_id,
                 aws_org.org_account_id,
                 self.cf_role_arn,
+                tags=tags,
             )
         )
         if not successfully_created:
             return
 
         role_name = IAMBIC_SPOKE_ROLE_NAME
         hub_account_id = self.hub_account_id
-        sqs_arn = f"arn:aws:sqs:{self.aws_default_region}:{hub_account_id}:IAMbicChangeDetectionQueue"
+        # cloudtrail is not cross-region, so we need to use us-east-1
+        # sqs_arn = f"arn:aws:sqs:{self.aws_default_region}:{hub_account_id}:IAMbicChangeDetectionQueue{IAMBIC_CHANGE_DETECTION_SUFFIX}"
+        sqs_arn = f"arn:aws:sqs:us-east-1:{hub_account_id}:IAMbicChangeDetectionQueue{IAMBIC_CHANGE_DETECTION_SUFFIX}"
 
         if not self.existing_role_template_map:
             log.info("Loading AWS role templates...")
             self.existing_role_template_map = asyncio.run(
                 get_existing_template_map(self.repo_dir, AWS_IAM_ROLE_TEMPLATE_TYPE)
             )
```

### Comparing `iambic_core-0.7.6/iambic/core/aio_utils/__init__.py` & `iambic_core-0.8.1/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/core/exceptions.py` & `iambic_core-0.8.1/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/core/git.py` & `iambic_core-0.8.1/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/core/iambic_enum.py` & `iambic_core-0.8.1/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/core/iambic_plugin.py` & `iambic_core-0.8.1/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/core/logger.py` & `iambic_core-0.8.1/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/core/models.py` & `iambic_core-0.8.1/iambic/core/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 class IambicPydanticBaseModel(PydanticBaseModel):
     metadata_iambic_fields = Field(
         set(), description="metadata for iambic", exclude=True, hidden_from_schema=True
     )
     metadata_commented_dict: dict = Field(
-        {}, description="yaml inline comments", hidden_from_schema=True
+        {}, description="yaml comments", hidden_from_schema=True
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         ancestors = inspect.getmro(type(self))
         for ancestor in ancestors:
@@ -306,14 +306,16 @@
 
 class ProposedChangeType(Enum):
     CREATE = "Create"
     UPDATE = "Update"
     DELETE = "Delete"
     ATTACH = "Attach"
     DETACH = "Detach"
+    # This is used for states that we don't know how to handle. e.g. Exceptions during apply time
+    UNKNOWN = "Unknown"
 
 
 class ProposedChange(PydanticBaseModel):
     change_type: ProposedChangeType
     account: Optional[
         str
     ]  # Used for Org related changes like permission set account assignments
```

### Comparing `iambic_core-0.7.6/iambic/core/noq_json.py` & `iambic_core-0.8.1/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/core/parser.py` & `iambic_core-0.8.1/iambic/core/parser.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/core/template_generation.py` & `iambic_core-0.8.1/iambic/core/template_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1066,15 +1066,15 @@
             elif new_value is None:
                 # cloud is represented by None, local is a BaseModel.
                 # this will only work if the local BaseModel does not carry
                 # any local metadata that needs to survive outside of cloud.
                 setattr(merged_model, key, new_value)
             else:
                 raise TypeError(
-                    f"Type of {type(new_value)} is not supported. {IAMBIC_ERR_MSG}"
+                    f"Type of {type(new_value)}({key}) is not supported. {IAMBIC_ERR_MSG}"
                 )
         elif key not in iambic_fields:
             setattr(merged_model, key, new_value)
     return merged_model
 
 
 def delete_orphaned_templates(
```

### Comparing `iambic_core-0.7.6/iambic/core/utils.py` & `iambic_core-0.8.1/iambic/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -330,47 +330,107 @@
             d[k] = sort_dict(d[k], prioritize)
         if isinstance(d[k], list) and len(d[k]) >= 1 and isinstance(d[k][0], dict):
             for i in range(len(d[k])):
                 d[k][i] = sort_dict(d[k][i], prioritize)
     return d
 
 
+def flatten_comment_data(data):
+    if type(data) == list:
+        return "".join([comment_token.value for comment_token in data])
+    elif data:
+        return data.value
+    else:
+        return data
+
+
 def transform_comments(yaml_dict):
+    from ruamel.yaml import CommentedMap
+
     comment_dict = {}
     yaml_dict["metadata_commented_dict"] = comment_dict
+    if yaml_dict.ca.comment:
+        comment_dict["__file_header__"] = yaml_dict.ca.comment[
+            1
+        ]  # this is intentional, index 1 is the header, index 0 is the footer...
+        # process multiline comments from array structure
+        if comment_dict["__file_header__"]:
+            comment_dict["__file_header__"] = "".join(
+                [
+                    comment_token.value
+                    for comment_token in comment_dict["__file_header__"]
+                ]
+            )
     for key, comment in yaml_dict.ca.items.items():
-        # flatten comment for now since we do not have
-        # a lot of experience with more complex comment token
-        flatten_comment = None
-        if comment[2]:
-            flatten_comment = comment[2].value
-        elif comment[3] and type(comment[3]) == list:
-            flatten_comment = " ".join([token.value.strip() for token in comment[3]])
-        comment_dict[key] = flatten_comment
+        # comment is a array of [pre_key, post_key, pre_value, post_value]
+        # convert comment into only primitive types because
+        # pydantic will require custom serializer
+        comments = [flatten_comment_data(element) for element in comment]
+        comment_dict[key] = comments
         value = yaml_dict[key]
         if isinstance(value, list) and len(value) > 0 and isinstance(value[0], dict):
             yaml_dict[key] = [transform_comments(n) for n in value]
         elif isinstance(value, dict):
             yaml_dict[key] = transform_comments(value)
+    for key, value in yaml_dict.items():
+        if isinstance(value, list) and len(value) > 0 and isinstance(value[0], dict):
+            yaml_dict[key] = [transform_comments(n) for n in value]
+        elif isinstance(value, CommentedMap):
+            yaml_dict[key] = transform_comments(value)
     return yaml_dict
 
 
 def create_commented_map(_dict: dict):
     from ruamel.yaml import CommentedMap
 
     commented_map = CommentedMap()
     index = 0
     comment_key_to_comment = _dict.pop("metadata_commented_dict", {})
     for key, value in _dict.items():
         if isinstance(value, list) and len(value) > 0 and isinstance(value[0], dict):
             value = [create_commented_map(n) for n in value]
         elif isinstance(value, dict):
             value = create_commented_map(value)
-        commented_map.insert(index, key, value, comment_key_to_comment.get(key, None))
+        commented_map.insert(index, key, value, None)
+        maybe_comment = comment_key_to_comment.get(key, None)
+        if maybe_comment:
+            if maybe_comment[0]:
+                # post_key comment
+                commented_map.yaml_set_comment_before_after_key(
+                    key=key,
+                    after=maybe_comment[0],
+                )
+            if maybe_comment[1]:
+                # pre_key comment
+                commented_map.yaml_set_comment_before_after_key(
+                    key=key,
+                    before=maybe_comment[1],
+                )
+            if maybe_comment[2]:
+                # post value comment
+                commented_map.yaml_add_eol_comment(key=key, comment=maybe_comment[2])
+                if maybe_comment[2][0] == "\n":
+                    # patch silly raumel behavior: when comment is `\n  # line 1`,
+                    # current implementation adds another `# ` before the \n
+                    commented_map.ca._items[key][2]._value = maybe_comment[
+                        2
+                    ]  # brittle to raumel implementation
+            if maybe_comment[3]:
+                # pre value comment
+                pre_value_comment = maybe_comment[3]
+                if pre_value_comment[0] == "#":
+                    # patch silly raumel behavior: it can add additional # character
+                    pre_value_comment = pre_value_comment[1:]
+                    pre_value_comment = pre_value_comment.strip()
+                commented_map.yaml_set_comment_before_after_key(
+                    key=key, after=pre_value_comment
+                )
         index = index + 1
+    if comment_key_to_comment.get("__file_header__", None):
+        commented_map.yaml_set_start_comment(comment_key_to_comment["__file_header__"])
     return commented_map
 
 
 typ = "rt"
 yaml = NoqYaml(typ=typ)
 yaml.preserve_quotes = True
 yaml.indent(mapping=2, sequence=4, offset=2)
@@ -398,14 +458,17 @@
         import-only. Default is True.
 
     Returns:
     - A Boolean indicating whether the resource should be evaluated on the provider.
     """
     from iambic.core.models import AccessModelMixin
 
+    if getattr(resource, "organization_account_needed", None):
+        return getattr(provider_details, "organization_account", False)
+
     no_op_values = [IambicManaged.DISABLED]
     if exclude_import_only:
         no_op_values.append(IambicManaged.IMPORT_ONLY)
 
     if (
         provider_details.iambic_managed in no_op_values
         or getattr(resource, "iambic_managed", None) in no_op_values
```

### Comparing `iambic_core-0.7.6/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.8.1/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.8.1/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.8.1/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/github/templates/iambic-import.yml` & `iambic_core-0.8.1/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/github/utils.py` & `iambic_core-0.8.1/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/lambda/app.py` & `iambic_core-0.8.1/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/main.py` & `iambic_core-0.8.1/iambic/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 @cli.command()
 @click.option(
     "--repo-dir",
     "-d",
     "repo_dir",
     required=False,
     type=click.Path(exists=True),
+    default=os.getenv("IAMBIC_REPO_DIR"),
     help="The repo directory containing the templates. Example: ~/iambic-templates",
 )
 def detect(repo_dir: str):
     run_detect(repo_dir)
 
 
 def run_detect(repo_dir: str):
@@ -394,15 +395,15 @@
     required=False,
     type=click.Path(exists=True),
     default=os.getenv("IAMBIC_REPO_DIR"),
     help="The repo directory containing the templates. Example: ~/iambic-templates",
 )
 def import_(repo_dir: str):
     config_path = asyncio.run(resolve_config_template_path(repo_dir))
-    config = asyncio.run(load_config(config_path))
+    config: Config = asyncio.run(load_config(config_path))
     check_and_update_resource_limit(config)
     exe_message = ExecutionMessage(
         execution_id=str(uuid.uuid4()), command=Command.IMPORT
     )
     asyncio.run(config.run_import(exe_message, repo_dir))
```

### Comparing `iambic_core-0.7.6/iambic/output/__init__.py` & `iambic_core-0.8.1/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/output/filters.py` & `iambic_core-0.8.1/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/output/models.py` & `iambic_core-0.8.1/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.8.1/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.8.1/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.8.1/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/output/text.py` & `iambic_core-0.8.1/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/README.md` & `iambic_core-0.8.1/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files 14% similar despite different names*

```diff
@@ -2,47 +2,52 @@
 Description: >-
   Setup IAMbic EventBridge Bus and Queue.
   This template creates an EventBridge Bus w/ Policy, an EventBridge Rule, and an SQS Queue.
 Parameters:
   OrgID:
     Type: String
     Description: AWS Organization ID.
+  Suffix:
+    Type: String
+    Description: Suffix to append to the name of the EventBridge Bus and SQS Queue.
+    Default: ""
 Resources:
   IAMbicEventBus:
     Type: 'AWS::Events::EventBus'
     Properties:
-      Name: 'IAMbicChangeDetectionEventBus'
+      Name: !Sub 'IAMbicChangeDetectionEventBus${Suffix}'
   IAMbicEventBusPolicy:
     Type: 'AWS::Events::EventBusPolicy'
     Properties:
-      StatementId: 'IAMbicEventBusPolicy'
+      StatementId: !Sub 'IAMbicEventBusPolicy${Suffix}'
       EventBusName: !Ref IAMbicEventBus
       Statement:
         Effect: "Allow"
         Principal: "*"
         Action: 'events:PutEvents'
         Resource: !GetAtt IAMbicEventBus.Arn
         Condition:
           StringEquals:
             aws:PrincipalOrgID: !Ref OrgID
     DependsOn:
       - IAMbicEventBus
   IAMbicEventRule:
     Type: 'AWS::Events::Rule'
     Properties:
-      Name: IAMbicChangeDetectionRule
+      Name: !Sub 'IAMbicChangeDetectionRule${Suffix}'
       Description: 'Captures changes when an Identity is created/Updated/deleted.'
       EventBusName: !Ref IAMbicEventBus
       EventPattern:
         detail-type:
           - AWS API Call via CloudTrail
         detail:
           eventSource:
             - iam.amazonaws.com
             - sso.amazonaws.com
+            - organizations.amazonaws.com
           eventName:
             - prefix: Create
             - prefix: Update
             - prefix: Attach
             - prefix: Detach
             - prefix: Add
             - prefix: Delete
@@ -56,15 +61,15 @@
           Id: IAMbicChangeDetectionQueue
     DependsOn:
       - IAMbicEventBus
       - IAMbicChangeDetectionQueue
   IAMbicChangeDetectionQueue:
     Type: 'AWS::SQS::Queue'
     Properties:
-      QueueName: IAMbicChangeDetectionQueue
+      QueueName: !Sub 'IAMbicChangeDetectionQueue${Suffix}'
       MessageRetentionPeriod: 604800
   IAMbicChangeDetectionQueueSQSPolicy:
     Type: AWS::SQS::QueuePolicy
     Properties:
       Queues:
         - !Ref IAMbicChangeDetectionQueue
       PolicyDocument:
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 AWSTemplateFormatVersion: 2010-09-09
 Description: >-
   Setup IAMbic Event forwarding.
   This template creates the rule responsible for forwarding Events in the default bus to the org wide IAMbicEventBus.
 Parameters:
   TargetEventBusArn:
     Type: String
+  Suffix:
+    Type: String
+    Description: Suffix to append to the name of the role, rule, and other resources
+    Default: ""
 Resources:
   IAMbicEventForwardingRole:
     Type: 'AWS::IAM::Role'
     Properties:
-      RoleName: 'IAMbicEventForwardingRole'
+      RoleName: !Sub 'IAMbicEventForwardingRole${Suffix}'
       AssumeRolePolicyDocument:
         Version: '2012-10-17'
         Statement:
           - Effect: Allow
             Principal:
               Service: events.amazonaws.com
             Action:
@@ -27,24 +31,25 @@
                 Action:
                   - 'events:PutEvents'
                 Resource:
                   - !Ref TargetEventBusArn
   IAMbicEventForwardingRule:
     Type: 'AWS::Events::Rule'
     Properties:
-      Name: IAMbicEventForwardingRule
+      Name: !Sub 'IAMbicEventForwardingRule${Suffix}'
       Description: 'Captures IAM and SSO events and forwards the events to the IAMbicEventBus for processing.'
       EventBusName: default
       EventPattern:
         detail-type:
           - AWS API Call via CloudTrail
         detail:
           eventSource:
             - iam.amazonaws.com
             - sso.amazonaws.com
+            - organizations.amazonaws.com
           eventName:
             - prefix: Create
             - prefix: Update
             - prefix: Attach
             - prefix: Detach
             - prefix: Add
             - prefix: Delete
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import asyncio
 import os
 from datetime import datetime, timedelta
-from typing import Union
+from typing import Any, Optional, Union
 
 from iambic.core.logger import log
 from iambic.plugins.v0_1_0.aws.models import (
+    IAMBIC_CHANGE_DETECTION_SUFFIX,
     IAMBIC_HUB_ROLE_NAME,
     IAMBIC_SPOKE_ROLE_NAME,
     get_hub_role_arn,
 )
 from iambic.plugins.v0_1_0.aws.utils import boto_crud_call, legacy_paginated_search
 
 TEMPLATE_DIR = f"{str(os.path.dirname(__file__))}/templates"
@@ -233,89 +234,124 @@
                     failed_instances=failed_instances,
                 )
 
             return not bool(failed_instances)
 
 
 async def create_change_detection_stacks(
-    cf_client, org_id: str, org_account_id: str, role_arn: str = None
+    cf_client,
+    org_id: str,
+    org_account_id: str,
+    role_arn: str = None,
+    tags: Optional[dict] = None,
 ) -> bool:
     region = cf_client.meta.region_name
-    additional_kwargs = {"RoleARN": role_arn} if role_arn else {}
+    additional_kwargs: dict[str, Any] = {"RoleARN": role_arn} if role_arn else {}
+
+    if tags:
+        additional_kwargs["Tags"] = tags
+
     stack_created = await create_stack(
         cf_client,
-        stack_name="IAMbicCentralChangeRule",
+        stack_name=f"IAMbicCentralChangeRule{IAMBIC_CHANGE_DETECTION_SUFFIX}",
         template_body=get_central_rule_template_body(),
-        parameters=[{"ParameterKey": "OrgID", "ParameterValue": org_id}],
+        parameters=[
+            {"ParameterKey": "OrgID", "ParameterValue": org_id},
+            {
+                "ParameterKey": "Suffix",
+                "ParameterValue": IAMBIC_CHANGE_DETECTION_SUFFIX,
+            },
+        ],
         **additional_kwargs,
     )
     if stack_created:
         stack_created = await create_stack(
             cf_client,
-            stack_name="IAMbicForwardEventRule",
+            stack_name=f"IAMbicForwardEventRule{IAMBIC_CHANGE_DETECTION_SUFFIX}",
             template_body=get_rule_forwarding_template_body(),
             parameters=[
                 {
                     "ParameterKey": "TargetEventBusArn",
-                    "ParameterValue": f"arn:aws:events:{region}:{org_account_id}:event-bus/IAMbicChangeDetectionEventBus",
-                }
+                    "ParameterValue": f"arn:aws:events:{region}:{org_account_id}:event-bus/IAMbicChangeDetectionEventBus{IAMBIC_CHANGE_DETECTION_SUFFIX}",
+                },
+                {
+                    "ParameterKey": "Suffix",
+                    "ParameterValue": IAMBIC_CHANGE_DETECTION_SUFFIX,
+                },
             ],
             Capabilities=["CAPABILITY_NAMED_IAM"],
             **additional_kwargs,
         )
 
     return stack_created
 
 
 async def create_change_detection_stack_sets(
-    cf_client, org_client, org_account_id: str
+    cf_client,
+    org_client,
+    org_account_id: str,
+    tags: Optional[dict] = None,
 ) -> bool:
     region = cf_client.meta.region_name
     org_roots = await legacy_paginated_search(
         org_client.list_roots, response_key="Roots"
     )
+    kwargs = {}
+    if tags:
+        kwargs["Tags"] = tags
 
     return await create_stack_set(
         cf_client,
-        stack_set_name="IAMbicForwardEventRule",
+        stack_set_name=f"IAMbicForwardEventRule{IAMBIC_CHANGE_DETECTION_SUFFIX}",
         template_body=get_rule_forwarding_template_body(),
         parameters=[
             {
                 "ParameterKey": "TargetEventBusArn",
-                "ParameterValue": f"arn:aws:events:{region}:{org_account_id}:event-bus/IAMbicChangeDetectionEventBus",
-            }
+                "ParameterValue": f"arn:aws:events:{region}:{org_account_id}:event-bus/IAMbicChangeDetection{IAMBIC_CHANGE_DETECTION_SUFFIX}EventBus",
+            },
+            {
+                "ParameterKey": "Suffix",
+                "ParameterValue": IAMBIC_CHANGE_DETECTION_SUFFIX,
+            },
         ],
         deployment_targets={
             "OrganizationalUnitIds": [root["Id"] for root in org_roots],
             "AccountFilterType": "NONE",
         },
         deployment_regions=[region],
         operation_preferences={
-            "MaxConcurrentCount": 1,
-            "FailureToleranceCount": 1,
+            "RegionConcurrencyType": "PARALLEL",
+            "MaxConcurrentCount": 100,
+            "FailureToleranceCount": 100,
         },
         Capabilities=["CAPABILITY_NAMED_IAM"],
+        **kwargs,
     )
 
 
 async def create_iambic_eventbridge_stacks(
-    cf_client, org_client, org_id: str, account_id: str, role_arn: str = None
+    cf_client,
+    org_client,
+    org_id: str,
+    account_id: str,
+    role_arn: str = None,
+    tags=None,
 ) -> bool:
     region = cf_client.meta.region_name
     successfully_created = await create_change_detection_stacks(
-        cf_client, org_id, account_id, role_arn
+        cf_client, org_id, account_id, role_arn, tags
     )
     if successfully_created:
         log.info(
             f"WARNING: Do not exit; creating stack instances.\n"
             f"You can check the progress here:\n"
-            f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacksets/IAMbicForwardEventRule/stacks\n"
+            f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacksets/IAMbicForwardEventRule{IAMBIC_CHANGE_DETECTION_SUFFIX}/stacks\n"
         )
         return await create_change_detection_stack_sets(
-            cf_client, org_client, account_id
+            cf_client, org_client, account_id, tags
         )
 
     return successfully_created
 
 
 async def create_spoke_role_stack_set(
     cf_client,
@@ -360,16 +396,16 @@
         deployment_targets={
             "OrganizationalUnitIds": [root["Id"] for root in org_roots],
             "AccountFilterType": "NONE",
         },
         deployment_regions=[region],
         operation_preferences={
             "RegionConcurrencyType": "PARALLEL",
-            "MaxConcurrentCount": 10,
-            "FailureToleranceCount": 10,
+            "MaxConcurrentCount": 100,
+            "FailureToleranceCount": 100,
         },
         Capabilities=["CAPABILITY_NAMED_IAM"],
         **kwargs,
     )
 
 
 async def create_spoke_role_stack(
@@ -442,14 +478,15 @@
             cf_client,
             hub_account_id,
             role_arn,
             read_only=read_only,
             stack_name=spoke_role_name,
             hub_role_name=hub_role_name,
             spoke_role_name=spoke_role_name,
+            tags=tags,
         )
 
     return stack_created
 
 
 async def create_iambic_role_stacks(
     cf_client,
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import base64
 import json
 import uuid
 from itertools import chain
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Coroutine, Union
 
 import boto3
 
 from iambic.config.dynamic_config import ExtendsConfig, ExtendsConfigKey
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
@@ -23,14 +23,15 @@
 from iambic.core.template_generation import get_existing_template_map
 from iambic.core.utils import async_batch_processor, gather_templates, yaml
 from iambic.plugins.v0_1_0.aws.event_bridge.models import (
     GroupMessageDetails,
     ManagedPolicyMessageDetails,
     PermissionSetMessageDetails,
     RoleMessageDetails,
+    SCPMessageDetails,
     UserMessageDetails,
 )
 from iambic.plugins.v0_1_0.aws.iam.group.models import AWS_IAM_GROUP_TEMPLATE_TYPE
 from iambic.plugins.v0_1_0.aws.iam.group.template_generation import (
     collect_aws_groups,
     generate_aws_group_templates,
 )
@@ -55,14 +56,23 @@
     collect_aws_permission_sets,
     generate_aws_permission_set_templates,
 )
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.utils import (
     generate_permission_set_map,
 )
 from iambic.plugins.v0_1_0.aws.models import AWSAccount
+from iambic.plugins.v0_1_0.aws.organizations.scp.models import AWS_SCP_POLICY_TEMPLATE
+from iambic.plugins.v0_1_0.aws.organizations.scp.template_generation import (
+    collect_aws_scp_policies,
+    generate_aws_scp_policy_templates,
+    get_organizations_account_map,
+)
+from iambic.plugins.v0_1_0.aws.organizations.scp.utils import (
+    service_control_policy_is_enabled,
+)
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
 
 
 async def load(config: AWSConfig) -> AWSConfig:
     config_account_idx_map = {
@@ -74,25 +84,34 @@
                 "You have a `hub_role_arn` defined on an `aws.account` specified in your IAMbic configuration that will be ignored. "
                 "IAMbic will prefer the `hub_role_arn` specified under your AWS Organization. To remove this message, "
                 "please remove the `hub_role_arn` specified in an `AWS Account`."
             )
         orgs_accounts = await asyncio.gather(
             *[org.get_accounts() for org in config.organizations]
         )
-        for org_accounts in orgs_accounts:
+        for org_accounts, org in zip(orgs_accounts, config.organizations):
             for account in org_accounts:
                 if (
                     account_elem := config_account_idx_map.get(account.account_id)
                 ) is not None:
                     config.accounts[
                         account_elem
                     ].hub_session_info = account.hub_session_info
                     config.accounts[
                         account_elem
                     ].identity_center_details = account.identity_center_details
+
+                    # if the account is an organization account, set the organization details
+                    if org.org_account_id == account.account_id:
+                        await config.accounts[
+                            account_elem
+                        ].set_account_organization_details(
+                            organization=org,
+                            config=config,
+                        )
                 else:
                     log.warning(
                         "Account not found in config. Account will be ignored.",
                         account_id=account.account_id,
                         account_name=account.account_name,
                     )
     elif config.accounts:
@@ -370,15 +389,15 @@
 async def import_aws_resources(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     base_output_dir: str,
     messages: list = None,
     remote_worker=None,
 ):
-    tasks = []
+    tasks: list[Coroutine] = []
 
     if not exe_message.metadata or exe_message.metadata["service"] == "identity_center":
         identity_center_template_map = None
         if not remote_worker or exe_message.metadata:
             identity_center_template_map = await get_existing_template_map(
                 repo_dir=base_output_dir,
                 template_type="AWS::IdentityCenter.*",
@@ -392,14 +411,18 @@
                 base_output_dir,
                 messages,
                 remote_worker,
                 identity_center_template_map,
             )
         )
 
+    tasks += await import_organization_resources(
+        exe_message, config, base_output_dir, messages, remote_worker
+    )  # type: ignore
+
     if not exe_message.metadata or exe_message.metadata["service"] == "iam":
         iam_template_map = None
 
         if not remote_worker or exe_message.metadata:
             iam_template_map = await get_existing_template_map(
                 repo_dir=base_output_dir,
                 template_type="AWS::IAM.*",
@@ -410,16 +433,16 @@
             import_service_resources(
                 exe_message,
                 config,
                 base_output_dir,
                 "iam",
                 [
                     collect_aws_roles,
-                    collect_aws_groups,
                     collect_aws_users,
+                    collect_aws_groups,
                     collect_aws_managed_policies,
                 ],
                 [
                     generate_aws_role_templates,
                     generate_aws_user_templates,
                     generate_aws_group_templates,
                     generate_aws_managed_policy_templates,
@@ -429,26 +452,75 @@
                 iam_template_map,
             )
         )
 
     await asyncio.gather(*tasks)
 
 
+async def import_organization_resources(
+    exe_message: ExecutionMessage,
+    config: AWSConfig,
+    base_output_dir: str,
+    messages: list = None,
+    remote_worker=None,
+) -> list[Coroutine]:
+    tasks = []
+    if not config.organizations:
+        return tasks
+    exe_messages = await config.get_command_by_organization_account(exe_message)
+    scp_template_map = await get_existing_template_map(
+        repo_dir=base_output_dir,
+        template_type=AWS_SCP_POLICY_TEMPLATE,
+        nested=True,
+    )
+
+    for exe_msg in exe_messages:
+        aws_account_map: dict[str, AWSAccount] = await get_organizations_account_map(
+            exe_msg, config
+        )
+        aws_account = aws_account_map[exe_msg.provider_id]  # type: ignore
+        org_client = await aws_account.get_boto3_client("organizations")
+
+        if not (await service_control_policy_is_enabled(org_client)):
+            pass
+
+        # this is also configured at aws config load method
+        await aws_account.set_account_organization_details(
+            await config.get_organization_from_account(exe_msg.provider_id), config
+        )
+        tasks.append(
+            import_service_resources(
+                exe_msg,
+                config,
+                base_output_dir,
+                "scp",
+                [collect_aws_scp_policies],
+                [generate_aws_scp_policy_templates],
+                messages,
+                remote_worker,
+                scp_template_map,
+            )
+        )
+
+    return tasks
+
+
 async def detect_changes(  # noqa: C901
     config: AWSConfig, repo_dir: str
 ) -> Union[str, None]:
     if not config.sqs_cloudtrail_changes_queues:
         log.debug("No cloudtrail changes queue arn found. Returning")
         return
 
     role_messages = []
     user_messages = []
     group_messages = []
     managed_policy_messages = []
     permission_set_messages = []
+    scp_messages = []
     commit_message = "Out of band changes detected.\nSummary:\n"
 
     for queue_arn in config.sqs_cloudtrail_changes_queues:
         queue_name = queue_arn.split(":")[-1]
         region_name = queue_arn.split(":")[3]
         session = await config.get_boto_session_from_arn(queue_arn, region_name)
         identity = session.client("sts").get_caller_identity()
@@ -506,14 +578,15 @@
                         decoded_message.get("userIdentity", {})
                         .get("principalId")
                         .split(":")[-1]
                     )
                     if actor != identity_arn:
                         account_id = decoded_message.get("recipientAccountId")
                         request_params = decoded_message["requestParameters"]
+                        response_elements = decoded_message["responseElements"]
                         event = decoded_message["eventName"]
                         resource_id = None
                         resource_type = None
                         if role_name := request_params.get("roleName"):
                             resource_id = role_name
                             resource_type = "Role"
                             role_messages.append(
@@ -571,14 +644,42 @@
                             permission_set_messages.append(
                                 PermissionSetMessageDetails(
                                     account_id=account_id,
                                     instance_arn=request_params.get("instanceArn"),
                                     permission_set_arn=permission_set_arn,
                                 )
                             )
+                        elif scp_policy_id := SCPMessageDetails.get_policy_id(
+                            request_params,
+                            response_elements,
+                        ):
+                            resource_id = scp_policy_id
+                            resource_type = "SCPPolicy"
+                            scp_messages.append(
+                                SCPMessageDetails(
+                                    account_id=account_id,
+                                    policy_id=scp_policy_id,
+                                    delete=bool(event == "DeletePolicy"),
+                                    event=event,
+                                )
+                            )
+                        elif SCPMessageDetails.tag_event(
+                            event,
+                            decoded_message["eventSource"],
+                        ):
+                            resource_id = request_params.get("resourceId")
+                            resource_type = "SCPPolicy"
+                            scp_messages.append(
+                                SCPMessageDetails(
+                                    account_id=account_id,
+                                    policy_id=resource_id,
+                                    delete=False,
+                                    event=event,
+                                )
+                            )
 
                         if resource_id:
                             commit_message = (
                                 f"{commit_message}User {session_name} performed action {event} "
                                 f"on {resource_type}({resource_id}) on account {account_id}.\n"
                             )
                 except Exception as err:
@@ -594,29 +695,43 @@
 
     exe_message = ExecutionMessage(
         execution_id=str(uuid.uuid4()), command=Command.IMPORT, provider_type="aws"
     )
     collect_tasks = []
     iam_template_map = None
     identity_center_template_map = None
+    scp_template_map = None
 
-    if role_messages or user_messages or group_messages or managed_policy_messages:
+    if (
+        role_messages
+        or user_messages
+        or group_messages
+        or managed_policy_messages
+        or scp_messages
+    ):
         iam_template_map = await get_existing_template_map(
             repo_dir=repo_dir,
             template_type="AWS::IAM.*",
             nested=True,
         )
 
     if permission_set_messages:
         identity_center_template_map = await get_existing_template_map(
             repo_dir=repo_dir,
             template_type="AWS::IdentityCenter.*",
             nested=True,
         )
 
+    if scp_messages:
+        scp_template_map = await get_existing_template_map(
+            repo_dir=repo_dir,
+            template_type=AWS_SCP_POLICY_TEMPLATE,
+            nested=True,
+        )
+
     if role_messages:
         collect_tasks.append(
             collect_aws_roles(exe_message, config, iam_template_map, role_messages)
         )
     if user_messages:
         collect_tasks.append(
             collect_aws_users(exe_message, config, iam_template_map, user_messages)
@@ -636,14 +751,30 @@
             collect_aws_permission_sets(
                 exe_message,
                 config,
                 identity_center_template_map,
                 permission_set_messages,
             )
         )
+    if scp_messages:
+        exe_messages = await config.get_command_by_organization_account(exe_message)
+
+        # for each execution message (by organization), collect the SCP policies.
+        for message in exe_messages:
+            if current_messages := [
+                m for m in scp_messages if m.account_id == message.provider_id
+            ]:
+                collect_tasks.append(
+                    collect_aws_scp_policies(
+                        message,
+                        config,
+                        scp_template_map,
+                        current_messages,
+                    )
+                )
 
     if collect_tasks:
         await asyncio.gather(*collect_tasks)
 
         tasks = []
         if role_messages:
             tasks.append(
@@ -679,14 +810,31 @@
                     exe_message,
                     config,
                     repo_dir,
                     identity_center_template_map,
                     permission_set_messages,
                 )
             )
+        if scp_messages:
+            exe_messages = await config.get_command_by_organization_account(exe_message)
+
+            # for each execution message (by organization), collect the SCP policies.
+            for message in exe_messages:
+                if current_messages := [
+                    m for m in scp_messages if m.account_id == message.provider_id
+                ]:
+                    tasks.append(
+                        generate_aws_scp_policy_templates(
+                            message,
+                            config,
+                            repo_dir,
+                            scp_template_map,
+                            current_messages,
+                        )
+                    )
         await asyncio.gather(*tasks)
 
         return commit_message
 
 
 async def decode_aws_secret(config: AWSConfig, extend: ExtendsConfig) -> dict:
     if extend.key.value != ExtendsConfigKey.AWS_SECRETS_MANAGER.value:
@@ -751,14 +899,20 @@
     remote_worker=None,
 ) -> bool:
     run_import = False
     accounts_to_apply = []
     for org_accounts in orgs_accounts:
         for account in org_accounts:
             if config_account_idx_map.get(account.account_id) is None:
+                account.variables.extend(
+                    [
+                        Variable(key="account_id", value=account.account_id),
+                        Variable(key="account_name", value=account.account_name),
+                    ]
+                )
                 config.accounts.append(account)
                 log.warning(
                     "New AWS account discovered. Adding account to config.",
                     account_id=account.account_id,
                     account_name=account.account_name,
                 )
                 if account.iambic_managed not in [
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,15 @@
         if existing_policy_doc:
             policy_drift = await aio_wrapper(
                 DeepDiff,
                 existing_policy_doc,
                 policy_document,
                 ignore_order=True,
                 report_repetition=True,
+                exclude_regex_paths=["metadata_commented_dict"],
             )
 
             # DeepDiff will return type changes as actual type functions and not strings,
             # and this will cause json serialization to fail later on when we process
             # the proposed changes. We force type changes to strings here.
             policy_drift = json.loads(policy_drift.to_json())
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,15 @@
         existing_policy_document = json.loads(existing_policy_document)
     policy_drift = await aio_wrapper(
         DeepDiff,
         existing_policy_document,
         template_policy_document,
         ignore_order=True,
         report_repetition=True,
+        exclude_regex_paths=["metadata_commented_dict"],
     )
     # DeepDiff will return type changes as actual type functions and not strings,
     # and this will cause json serialization to fail later on when we process
     # the proposed changes. We force type changes to strings here.
 
     if policy_drift:
         policy_drift = json.loads(policy_drift.to_json())
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,15 @@
 
         policy_drift = await aio_wrapper(
             DeepDiff,
             existing_policy_document,
             template_policy_document,
             report_repetition=True,
             ignore_order=True,
+            exclude_regex_paths=["metadata_commented_dict"],
         )
 
         # DeepDiff will return type changes as actual type functions and not strings,
         # and this will cause json serialization to fail later on when we process
         # the proposed changes. We force type changes to strings here.
         policy_drift = json.loads(policy_drift.to_json())
 
@@ -561,14 +562,15 @@
         if existing_policy_doc:
             policy_drift = await aio_wrapper(
                 DeepDiff,
                 existing_policy_doc,
                 policy_document,
                 ignore_order=True,
                 report_repetition=True,
+                exclude_regex_paths=["metadata_commented_dict"],
             )
 
             # DeepDiff will return type changes as actual type functions and not strings,
             # and this will cause json serialization to fail later on when we process
             # the proposed changes. We force type changes to strings here.
             policy_drift = json.loads(policy_drift.to_json())
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,15 @@
         if existing_policy_doc:
             policy_drift = await aio_wrapper(
                 DeepDiff,
                 existing_policy_doc,
                 policy_document,
                 ignore_order=True,
                 report_repetition=True,
+                exclude_regex_paths=["metadata_commented_dict"],
             )
 
             # DeepDiff will return type changes as actual type functions and not strings,
             # and this will cause json serialization to fail later on when we process
             # the proposed changes. We force type changes to strings here.
             policy_drift = json.loads(policy_drift.to_json())
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 from typing import Optional
 
 from pydantic import BaseModel, Field, validator
 
 from iambic.core.iambic_plugin import ProviderPlugin
+from iambic.core.models import ExecutionMessage
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
 from iambic.plugins.v0_1_0.aws.handlers import (
     apply,
     aws_account_update_and_discovery,
     decode_aws_secret,
     detect_changes,
     import_aws_resources,
@@ -19,14 +20,15 @@
 from iambic.plugins.v0_1_0.aws.iam.policy.models import AwsIamManagedPolicyTemplate
 from iambic.plugins.v0_1_0.aws.iam.role.models import AwsIamRoleTemplate
 from iambic.plugins.v0_1_0.aws.iam.user.models import AwsIamUserTemplate
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.models import (
     AwsIdentityCenterPermissionSetTemplate,
 )
 from iambic.plugins.v0_1_0.aws.models import AWSAccount, AWSOrganization
+from iambic.plugins.v0_1_0.aws.organizations.scp.models import AwsScpPolicyTemplate
 
 
 class AWSConfig(BaseModel):
     organizations: list[AWSOrganization] = Field(
         [], description="A list of AWS Organizations to be managed by iambic"
     )
     accounts: list[AWSAccount] = Field(
@@ -101,14 +103,41 @@
     async def get_boto_session_from_arn(self, arn: str, region_name: str = None):
         region_name = region_name or arn.split(":")[3]
         account_id = arn.split(":")[4]
         aws_account_map = {account.account_id: account for account in self.accounts}
         aws_account = aws_account_map[account_id]
         return await aws_account.get_boto3_session(region_name)
 
+    async def get_organization_accounts(self) -> list[AWSAccount]:
+        org_accounts = []
+        # each organization has an account, retrieve it
+        for org in self.organizations:
+            org_accounts += filter(
+                lambda acc: acc.account_id == org.org_account_id, self.accounts
+            )
+
+        return org_accounts
+
+    async def get_organization_from_account(self, account_id) -> AWSOrganization:
+        """Get the organization that owns the account"""
+        return list(
+            filter(lambda org: account_id == org.org_account_id, self.organizations)
+        )[0]
+
+    async def get_command_by_organization_account(
+        self, command: ExecutionMessage
+    ) -> list[ExecutionMessage]:
+        commands = []
+        for org in self.organizations:
+            command_cp = command.copy()
+            command_cp.provider_id = org.org_account_id
+            commands.append(command_cp)
+
+        return commands
+
 
 IAMBIC_PLUGIN = ProviderPlugin(
     config_name="aws",
     version=PLUGIN_VERSION,
     provider_config=AWSConfig,
     async_apply_callable=apply,
     async_import_callable=import_aws_resources,
@@ -118,9 +147,10 @@
     async_discover_upstream_config_changes_callable=aws_account_update_and_discovery,
     templates=[
         AwsIdentityCenterPermissionSetTemplate,
         AwsIamGroupTemplate,
         AwsIamRoleTemplate,
         AwsIamUserTemplate,
         AwsIamManagedPolicyTemplate,
+        AwsScpPolicyTemplate,
     ],
 )
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,14 +604,15 @@
 
         policy_drift = await aio_wrapper(
             DeepDiff,
             existing_inline_policy,
             template_inline_policy,
             report_repetition=True,
             ignore_order=True,
+            exclude_regex_paths=["metadata_commented_dict"],
         )
 
     if template_inline_policy and (not existing_inline_policy or bool(policy_drift)):
         log_str = "Changes to the InlinePolicyDocument discovered."
         if policy_drift:
             response.append(
                 ProposedChange(
@@ -686,14 +687,15 @@
     if existing_permission_boundary:
         policy_drift = await aio_wrapper(
             DeepDiff,
             existing_permission_boundary,
             template_permission_boundary,
             report_repetition=True,
             ignore_order=True,
+            exclude_regex_paths=["metadata_commented_dict"],
         )
 
     if template_permission_boundary and (
         not existing_permission_boundary or bool(policy_drift)
     ):
         log_str = "Changes to the PermissionsBoundary discovered."
         if policy_drift:
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from iambic.core.logger import log
 from iambic.core.models import (
     AccessModelMixin,
     AccountChangeDetails,
     BaseModel,
     BaseTemplate,
     ExpiryModel,
+    ProposedChange,
+    ProposedChangeType,
     ProviderChild,
     TemplateChangeDetails,
     Variable,
 )
 from iambic.core.utils import (
     NoqSemaphore,
     evaluate_on_provider,
@@ -43,30 +45,36 @@
 yaml = YAML()
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
 
 ARN_RE = r"(^arn:([^:]*):([^:]*):([^:]*):(|\*|[\d]{12}|cloudfront|aws|{{var.account_id}}):(.+)$)|^\*$"
 
-IAMBIC_HUB_ROLE_NAME = "IambicHubRole"
-IAMBIC_SPOKE_ROLE_NAME = "IambicSpokeRole"
+IAMBIC_HUB_ROLE_NAME = os.getenv("IAMBIC_HUB_ROLE_NAME", "IambicHubRole")
+IAMBIC_SPOKE_ROLE_NAME = os.getenv("IAMBIC_SPOKE_ROLE_NAME", "IambicSpokeRole")
+IAMBIC_CHANGE_DETECTION_SUFFIX = os.getenv("IAMBIC_CHANGE_DETECTION_SUFFIX", "")
 
 
 def get_hub_role_arn(account_id: str, role_name=None) -> str:
     if not role_name:
         role_name = IAMBIC_HUB_ROLE_NAME
     return f"arn:aws:iam::{account_id}:role/{role_name}"
 
 
 def get_spoke_role_arn(account_id: str, role_name=None) -> str:
     if not role_name:
         role_name = IAMBIC_SPOKE_ROLE_NAME
     return f"arn:aws:iam::{account_id}:role/{role_name}"
 
 
+class StatementEffect(str, Enum):
+    ALLOW = "Allow"
+    DENY = "Deny"
+
+
 @yaml_object(yaml)
 class Partition(Enum):
     AWS = "aws"
     AWS_GOV = "aws-us-gov"
     AWS_CHINA = "aws-cn"
 
     @classmethod
@@ -279,29 +287,36 @@
         description="A unique identifier designating the identity of the organization",
     )
     account_name: str
     partition: Optional[Partition] = Field(
         Partition.AWS,
         description="The AWS partition the account is in. Options are aws, aws-us-gov, and aws-cn",
     )
-    variables: Optional[List[Variable]] = Field(
+    variables: list[Variable] = Field(
         [],
         description="A list of variables to be used when creating templates",
     )
     hub_session_info: Optional[dict] = None
     identity_center_details: Optional[Union[IdentityCenterDetails, None]] = None
     spoke_role_arn: str = Field(
         None,
         description="(Auto-populated) The role arn to assume into when making calls to the account",
     )
     assume_role_arn: Optional[str] = Field(
         None,
         description="The role arn to assume into when making calls to the account",
         exclude=True,
     )
+    organization: Optional[AWSOrganization] = Field(
+        None, description="The AWS Organization this account belongs to"
+    )
+    aws_config: Optional[AWSConfig] = Field(
+        None,
+        description="when an account is an organization account, it needs the AWS Config settings",
+    )
 
     class Config:
         fields = {"hub_session_info": {"exclude": True}}
         extra = Extra.forbid
 
     async def get_boto3_session(self, region_name: str = None):
         region_name = region_name or self.region_name
@@ -441,14 +456,25 @@
                         user["UserId"]: user for user in user_or_group["Users"]
                     }
                 else:
                     self.identity_center_details.group_map = {
                         group["GroupId"]: group for group in user_or_group["Groups"]
                     }
 
+    async def set_account_organization_details(
+        self,
+        organization: AWSOrganization,
+        config: AWSConfig,
+    ):
+        """Set the account's organization details
+        when the account is the organization account
+        """
+        self.organization = organization
+        self.aws_config = config
+
     def dict(
         self,
         *,
         include: Optional[
             Union["AbstractSetIntStr", "MappingIntStrAny"]  # noqa
         ] = None,
         exclude: Optional[
@@ -460,14 +486,17 @@
         exclude_defaults: bool = False,
         exclude_none: bool = True,
     ) -> "DictStrAny":  # noqa
         required_exclude = {
             "boto3_session_map",
             "hub_session_info",
             "identity_center_details",
+            "organization_account",
+            "organization",
+            "aws_config",
         }
         if exclude:
             exclude.update(required_exclude)
         else:
             exclude = required_exclude
 
         resp = super(AWSAccount, self).dict(
@@ -475,14 +504,25 @@
             exclude=exclude,
             by_alias=by_alias,
             skip_defaults=skip_defaults,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
+
+        if "variables" in resp:
+            resp["variables"] = [
+                i
+                for i in resp.get("variables", [])
+                if i.get("key") not in ["account_id", "account_name"]
+            ]
+
+            if resp["variables"] == []:
+                resp.pop("variables")
+
         return sort_dict(
             resp,
             [
                 "account_id",
                 "account_name",
                 "org_id",
                 "identity_center",
@@ -501,14 +541,19 @@
     @property
     def all_identifiers(self) -> set[str]:
         if self.account_name:
             return {self.account_id, self.account_name.lower()}
         else:
             return set(self.account_id)
 
+    @property
+    def organization_account(self) -> bool:
+        """if current account is an organization account"""
+        return bool(self.organization and self.aws_config)
+
     def __str__(self):
         return f"{self.account_name} - ({self.account_id})"
 
 
 class BaseAWSOrgRule(BaseModel):
     iambic_managed: IambicManaged = Field(
         IambicManaged.UNDEFINED,
@@ -765,21 +810,26 @@
         relevant_accounts_str = [str(account) for account in relevant_accounts]
         log.info(log_str, accounts=relevant_accounts_str, **log_params)
 
         account_changes: list[AccountChangeDetails] = await asyncio.gather(
             *tasks, return_exceptions=True
         )
         proposed_changes: list[AccountChangeDetails] = []
-        exceptions_seen = set()
+        exceptions_seen = list()
 
         for account_change in account_changes:
             if isinstance(account_change, AccountChangeDetails):
                 proposed_changes.append(account_change)
             else:
-                exceptions_seen.add(str(account_change))
+                exceptions_seen.append(
+                    ProposedChange(
+                        change_type=ProposedChangeType.UNKNOWN,
+                        exceptions_seen=[str(account_change)],
+                    )  # type: ignore
+                )
 
         if exceptions_seen:
             exceptions_seen = list(exceptions_seen)
             proposed_change_accounts = set(
                 change.account for change in proposed_changes
             )
             for aws_account in relevant_accounts:
@@ -787,39 +837,41 @@
                     continue
                 proposed_changes.append(
                     AccountChangeDetails(
                         account=str(aws_account),
                         resource_id=self.resource_id,
                         resource_type=self.resource_type,
                         exceptions_seen=exceptions_seen,
-                    )
+                    )  # type: ignore
                 )
 
         template_changes.extend_changes(proposed_changes)
 
         if template_changes.exceptions_seen:
             if self.deleted:
                 cmd_verb = "removing"
             elif ctx.execute:
                 cmd_verb = "applying"
             else:
                 cmd_verb = "detecting"
             log_str = f"Error encountered when {cmd_verb} resource changes."
-        elif account_changes and ctx.execute:
-            if self.deleted:
-                self.delete()
-                log_str = "Successfully removed resource."
-            else:
-                log_str = "Successfully applied resource changes."
-        elif account_changes:
-            log_str = "Successfully detected required resource changes."
+            log.error(log_str, accounts=relevant_accounts_str, **log_params)
         else:
-            log_str = "No changes detected for resource."
+            if account_changes and ctx.execute:
+                if self.deleted:
+                    self.delete()
+                    log_str = "Successfully removed resource."
+                else:
+                    log_str = "Successfully applied resource changes."
+            elif account_changes:
+                log_str = "Successfully detected required resource changes."
+            else:
+                log_str = "No changes detected for resource."
 
-        log.info(log_str, accounts=relevant_accounts_str, **log_params)
+            log.info(log_str, accounts=relevant_accounts_str, **log_params)
         return template_changes
 
     @property
     def resource_id(self):
         return self.properties.resource_id
 
     @property
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,17 @@
     results = {key: [] for key in response_keys}
 
     while True:
         response = await boto_crud_call(search_fnc, **search_kwargs)
         for response_key in response_keys:
             results[response_key].extend(response.get(response_key, []))
 
-        if not response["IsTruncated"] or (max_results and len(results) >= max_results):
+        if not response.get("IsTruncated") or (
+            max_results and len(results) >= max_results
+        ):
             return results if retain_key else results[response_key]
         else:
             search_kwargs["Marker"] = response["Marker"]
 
 
 def get_identity_arn(caller_identity: dict) -> str:
     arn = caller_identity.get("Arn")
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import typing
 from enum import Enum
 from itertools import chain
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiohttp import ClientResponseError
-from pydantic import Field
+from pydantic import Extra, Field
 
 from iambic.core.context import ctx
 from iambic.core.logger import log
 from iambic.core.models import (
     AccountChangeDetails,
     BaseModel,
     ExpiryModel,
@@ -31,15 +31,18 @@
 
 class MemberDataType(Enum):
     USER = "user"
     GROUP = "group"
 
 
 class Member(BaseModel, ExpiryModel):
-    id: Optional[str] = None
+    id: Optional[str] = Field(
+        None,
+        description="Unique ID for the member. This value is imported by IAMbic, and doesn't need to be manually set.",
+    )
     name: str
     data_type: MemberDataType
     """TODO: validate name
 
     https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-sspr-policy#userprincipalname-policies-that-apply-to-all-user-accounts
 
     The total length must not exceed 113 characters
@@ -90,15 +93,15 @@
     mail_nickname: Optional[str] = Field(
         None,
         description="Mail nickname of the group",
         regex=r"^[!#$%&'*+-./0-9=?A-Z^_`a-z{|}~]{1,64}$",
     )
     group_id: Optional[str] = Field(
         None,
-        description="Unique Group ID for the group. Usually it's {idp-name}-{name}",
+        description="Unique Group ID for the group. This value is imported by IAMbic, and doesn't need to be manually set.",
     )
     description: Optional[str] = Field("", description="Description of the group")
     group_types: Optional[list[str]] = Field(
         [], description="Specifies the group type and its membership."
     )
     mail: Optional[str] = Field(description="Email address of the group")
     mail_enabled: Optional[bool] = False
@@ -192,14 +195,17 @@
     extra: Any = Field(None, description=("Extra attributes to store"), exclude=True)
 
     def __init__(self, **data):
         if "mail_nickname" not in data:
             data["mail_nickname"] = data.get("name")
         super().__init__(**data)
 
+    class Config:
+        extra = Extra.ignore
+
     @property
     def resource_type(self) -> str:
         return "azure_ad:group"
 
     @property
     def resource_id(self) -> str:
         return self.mail or self.name
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import typing
 from enum import Enum
 from itertools import chain
 from typing import Optional
 
 from aiohttp import ClientResponseError
-from pydantic import Field
+from pydantic import Extra, Field
 
 from iambic.core.context import ctx
 from iambic.core.logger import log
 from iambic.core.models import (
     AccountChangeDetails,
     BaseModel,
     ExpiryModel,
@@ -31,15 +31,18 @@
 class UserStatus(Enum):
     active = "active"
     provisioned = "provisioned"
     deprovisioned = "deprovisioned"
 
 
 class UserTemplateProperties(BaseModel, ExpiryModel):
-    user_id: Optional[str] = Field("", description="Unique identifier for the user")
+    user_id: Optional[str] = Field(
+        "",
+        description="Unique identifier for the user. This value is imported by IAMbic, and doesn't need to be manually set.",
+    )
     username: str
     display_name: str
     mail_nickname: Optional[str]
     given_name: Optional[str]
     employee_id: Optional[str]
     domain: Optional[str]
     fullname: Optional[str]
@@ -69,14 +72,17 @@
     surname: Optional[str] = Field(
         None, description="Surname of the user", exclude=True
     )
     user_principal_name: Optional[str] = Field(
         None, description="User principal name of the user", exclude=True
     )
 
+    class Config:
+        extra = Extra.ignore
+
     @property
     def resource_type(self) -> str:
         return "azure_ad:user"
 
     @property
     def resource_id(self) -> str:
         return self.username
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,9 +430,16 @@
                         .execute,
                         http=http,
                     )
                 )
 
         log.info(log_str, users=[user.email for user in users_to_add], **log_params)
     if tasks:
-        await asyncio.gather(*tasks)
+        res = await asyncio.gather(*tasks, return_exceptions=True)
+        for r in res:
+            if not isinstance(r, Exception):
+                continue
+            if isinstance(r, HttpError) and r.reason in ["Member already exists."]:
+                continue
+            raise r
+
     return response
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     private_key: SecretStr
     client_email: str
     client_id: str
     auth_uri: str
     token_uri: str
     auth_provider_x509_cert_url: str
     client_x509_cert_url: str
-    variables: Optional[list[Variable]] = Field(
+    variables: list[Variable] = Field(
         [],
         description="A list of variables to be used when creating templates",
     )
     iambic_managed: Optional[IambicManaged] = Field(
         IambicManaged.UNDEFINED,
         description="Controls the directionality of iambic changes",
     )
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 OKTA_APP_TEMPLATE_TYPE = "NOQ::Okta::App"
 
 
 class AppProperties(ExpiryModel, BaseModel):
     name: str = Field(..., description="Name of the app")
     status: Optional[Status] = Field(None, description="Status of the app")
     id: Optional[str] = Field(
-        None, description="Unique App ID for the app. Usually it's {idp-name}-{name}"
+        None,
+        description="Unique ID for the app. This value is imported by IAMbic, and doesn't need to be manually set.",
     )
     file_path: str = Field(
         "",
         description="Path to the template file",
         exclude=True,
         hidden_from_schema=True,
     )
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,16 @@
     background_check_status: Optional[bool]
     extra: Any = Field(None, description=("Extra attributes to store"))
 
 
 class GroupProperties(ExpiryModel, BaseModel):
     name: str = Field(..., description="Name of the group")
     group_id: str = Field(
-        "", description="Unique Group ID for the group. Usually it's {idp-name}-{name}"
+        "",
+        description="Unique Group ID for the group. This value is imported by IAMbic, and doesn't need to be manually set.",
     )
     file_path: str = Field(
         "", description="File path of the group", exclude=True, hidden_from_schema=True
     )
     description: Optional[str] = Field("", description="Description of the group")
     extra: Any = Field(None, description=("Extra attributes to store"))
     members: List[UserSimple] = Field([], description="Users in the group")
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,18 @@
 class Assignment(BaseModel):
     role: str
     resource_set: str
 
 
 class UserProperties(BaseModel):
     username: str = Field(..., description="Username of the user")
-    user_id: str = Field("", description="Unique User ID for the user")
+    user_id: str = Field(
+        "",
+        description="Unique User ID for the user. This value is imported by IAMbic, and doesn't need to be manually set.",
+    )
     status: UserStatus = Field(UserStatus.active, description="Status of the user")
     profile: dict[str, Any]
     extra: Optional[dict[str, Any]] = Field(
         None, description=("Extra attributes to store for the user")
     )
 
     @classmethod
```

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/request_handler/expire_resources.py` & `iambic_core-0.8.1/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/request_handler/git_apply.py` & `iambic_core-0.8.1/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/request_handler/git_plan.py` & `iambic_core-0.8.1/iambic/request_handler/git_plan.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 
     :param config_path:
     :param repo_dir:
     :return:
     """
     ctx_eval_only_original_value = ctx.eval_only
     ctx.eval_only = True
+    changes = []
     try:
         changes = await apply_git_changes(config_path, repo_dir)
     finally:
         ctx.eval_only = ctx_eval_only_original_value
         return changes
```

### Comparing `iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.6/pyproject.toml` & `iambic_core-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.7.6"
+version = "0.8.1"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
 
@@ -66,14 +66,17 @@
 types-mock = "^5.0.0.5"
 rich = "^13.3.2"
 dictdiffer = "^0.9.0"
 msal = "^1.21.0"
 aiohttp = "^3.8.4"
 pyopenssl = "^23.0.0"
 stringcase = "^1.2.0"
+tomlkit = "^0.11.8"
+typing-extensions = "^4.6.1"
+tenacity = "^8.2.2"
 
 [tool.poetry.scripts]
 iambic = "iambic.main:cli"
 
 [tool.poetry.group.dev.dependencies]
 types-cachetools = "^5.3.0.4"
 types-pyyaml = "^6.0.12.8"
```

### Comparing `iambic_core-0.7.6/PKG-INFO` & `iambic_core-0.8.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.7.6
+Version: 0.8.1
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -45,22 +45,30 @@
 Requires-Dist: pytest-xdist (>=3.2.1,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: slack-bolt (>=1.16.4,<2.0.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Requires-Dist: types-dateparser (>=1.1.4.5,<2.0.0.0)
 Requires-Dist: types-mock (>=5.0.0.5,<6.0.0.0)
+Requires-Dist: typing-extensions (>=4.6.1,<5.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
 
+[![noqdev - iambic](https://img.shields.io/static/v1?label=noqdev&message=iambic&color=blue&logo=github)](https://github.com/noqdev/iambic "Go to GitHub repo")
 [![Supported Versions](https://img.shields.io/pypi/pyversions/iambic-core.svg)](https://pypi.org/project/iambic-core)
 [![codecov.io](https://codecov.io/github/noqdev/iambic/coverage.svg?branch=main)](https://codecov.io/github/noqdev/iambic?branch=main)
+[![stars - iambic](https://img.shields.io/github/stars/noqdev/iambic?style=social)](https://github.com/noqdev/iambic)
+[![forks - iambic](https://img.shields.io/github/forks/noqdev/iambic?style=social)](https://github.com/noqdev/iambic)
+
+[![slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)](https://communityinviter.com/apps/noqcommunity/noq)
 
 # IAMbic: Cloud IAM as Code
 
 "IAMbic: the Terraform of Cloud IAM"
 
 Easily manage and streamline cloud Identity and Access Management (IAM) with IAMbic, a multi-cloud IAM control plane. Discover more at [https://docs.iambic.org](https://docs.iambic.org).
 
@@ -73,24 +81,32 @@
 - **[Dynamic AWS Permissions](https://docs.iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
 - **[Drift Prevention](https://docs.iambic.org/how_to_guides/prevent-drift)**: Protect the IAM resources you want to be exclusively managed via IAMbic. What is in Git becomes the absolute source of truth.
 - **[GitOps-driven Cloud IAM (IAMOps)](https://docs.iambic.org/reference/iamops_philosophy)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
 - **Centralized Management**: IAMbic keeps Git updated with the latest, complete state of your cloud environment, maintaining a single source of truth for auditing and compliance across multiple cloud providers in Git.
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
+Check out [IAMbic IAMOps Philosophy](/reference/iamops_philosophy) and an [example IAMbic templates repository](https://github.com/noqdev/iambic-templates-examples) to see a real-life example of IAMbic.
+
 ## 📣 Let's chat
+
 Do you want to connect with our contributors?
 
 Just click the button below and follow the instructions.
 
 [![slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)](https://communityinviter.com/apps/noqcommunity/noq)
 
 ## Getting Started
 
-Dive into IAMbic with our [quick-start guide](http://docs.iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
+Dive into IAMbic with our [quick-start guide](http://docs.iambic.org/getting_started/) and explore powerful
+[template examples](https://github.com/noqdev/iambic-templates-examples/) for AWS Multi-Account Roles,
+Identity Center (SSO) Permission Sets, Service Control Policies, Dynamic Permissions,
+Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments.
+
+We are rapidly expanding support for existing resources and cloud providers, so check back often!
 
 ## Installing IAMbic and Supported Versions
 
 IAMbic is available on PyPI:
 
 ```console
 python -m pip install iambic-core
@@ -100,17 +116,18 @@
 
 ### Template Examples
 
 Here are some examples showcasing IAMbic's capabilities:
 
 #### AWS Multi-Account Cloudwatch Role
 
-Create a Cloudwatch role with static permissions across three accounts, dynamically generating role names based on the account the role is deployed to. This template would
-result in the creation of three roles: "dev_cloudwatch",
-"staging_cloudwatch", and "prod_cloudwatch" on the respective AWS accounts. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
+Create a Cloudwatch role with static permissions across three accounts, dynamically generating role names based on the account the role is deployed to. This template would result in the creation of three roles: "dev_cloudwatch",
+"staging_cloudwatch", and "prod_cloudwatch" on the respective AWS accounts.
+
+See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws), the AWS IAM Role section of our [Example Templates repository](https://github.com/noqdev/iambic-templates-examples/blob/main/resources/aws/iam/role/all_accounts/account_name_iambic_test_role.yaml), and our [blog post on multi-account roles](https://www.noq.dev/blog/aws-permission-bouncers-letting-loose-in-dev-keeping-it-tight-in-prod) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
 identifier: '{{var.account_name}}_cloudwatch'
 included_accounts:
     - dev
     - staging
@@ -201,14 +218,53 @@
                     s3:ResourceTag/sensitive: 'true'
   role_name: '{{var.account_name}}_backend_developer'
   tags:
     - key: owner
       value: devops
 ```
 
+### AWS Identity Center (SSO) Permission Sets
+
+Create an AWS Identity Center (SSO) permission set with varying permissions based on the AWS account. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws), the AWS IC/SSO Permission Set section of our [Example Templates repository](https://github.com/noqdev/iambic-templates-examples/blob/main/resources/aws/identity_center/permission_set/design.yaml), and our blog post on [Tailoring AWS Identity Center (SSO) Permissions Per Account with IAMbic](https://www.noq.dev/blog/tailor-aws-identity-center-sso-permissions-per-account-with-iambic) for more information.
+
+```yaml
+template_type: NOQ::AWS::IdentityCenter::PermissionSet
+access_rules:
+  - expires_at: 2028-05-19T14:17 UTC
+    groups:
+      - engineering
+identifier: design
+properties:
+  name: design
+  customer_managed_policy_references:
+    - name: base_deny
+  inline_policy:
+    statement:
+      - action:
+          - ec2:list*
+        effect: Deny
+        resource:
+          - '*'
+      - action:
+          - ec2:list*
+        effect: Deny
+        expires_at: 2033-05-19T14:17 UTC
+        resource:
+          - '*'
+  managed_policies:
+    - arn: arn:aws:iam::aws:policy/AWSHealthFullAccess
+  permissions_boundary:
+    customer_managed_policy_reference:
+      name: base_permission_boundary
+  session_duration: PT4H
+  tags:
+    - key: owner
+      value: design@example.com
+```
+
 ### Okta Application Assignments
 
 Manage Okta application assignments, including expiration dates for specific users. See the [Getting Started guide for Okta](https://docs.iambic.org/getting_started/okta) for more information.
 
 ```yaml
 template_type: NOQ::Okta::App
 idp_name: development
@@ -218,14 +274,69 @@
     - user: username@example.com
     - user: username2@example.com
     - user: username3@example.com
       expires_at: 2023-09-01T00:00 UTC
   status: ACTIVE
 ```
 
+### AWS Service Control Policies
+
+Managing access to AWS services can be a tricky business. That's where Service Control Policies (SCPs) come in. SCPs allow you to define what services and actions are accessible within your AWS accounts. With IAMbic, you can import your existing SCPs, create new ones that restrict access to specific AWS services, and prevent any drift from occurring to ensure that you're protecting sensitive information the way you intend.
+
+For instance, let's say you want to limit access to certain AWS regions. You can create an SCP that denies access to all regions except those you specify. This can be particularly useful if you're looking to maintain tighter control over your data residency and compliance.
+
+Here's an example of how you can set this up:
+
+```yaml
+template_type: NOQ::AWS::Organizations::SCP
+account_id: '123456789012'
+iambic_managed: enforced
+identifier: RestrictRegions
+org_id: o-123456
+properties:
+  policy_document:
+    statement:
+      - condition:
+          StringNotEquals:
+            aws:RequestedRegion:
+              - us-east-1
+              - us-west-2
+        effect: Deny
+        not_action:
+          - a4b:*
+          - budgets:*
+          - ce:*
+          - chime:*
+          - cloudfront:*
+          - cur:*
+          - globalaccelerator:*
+          - health:*
+          - iam:*
+          - importexport:*
+          - mobileanalytics:*
+          - organizations:*
+          - route53:*
+          - route53domains:*
+          - shield:*
+          - support:*
+          - trustedadvisor:*
+          - waf:*
+          - wellarchitected:*
+        resource:
+          - '*'
+  policy_name: RestrictRegions
+  targets:
+    roots:
+      - r-123
+```
+
+In this example, the SCP named `RestrictRegions` denies access to all AWS regions except `us-east-1` and `us-west-2`. It also excludes certain global services from the restriction.
+
+For more information on how to get started with AWS and SCPs, check out our [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) and the [AWS SCP Section of our Example Templates repository](https://github.com/noqdev/iambic-templates-examples/blob/main/resources/aws/organizations/scp/iambic_test_org_account/restrict_regions.yaml). You can also learn more about tailoring AWS Identity Center (SSO) permissions per account with IAMbic in our [blog post](https://noq-0.webflow.io/blog/scps-protecting-your-aws-environment-and-your-job).
+
 ### Okta Group Assignments
 
 Easily manage Okta group assignments with expiration dates for members. See the [Getting Started guide for Okta](https://docs.iambic.org/getting_started/okta) for more information.
 
 ```yaml
 template_type: NOQ::Okta::Group
 idp_name: main
```

