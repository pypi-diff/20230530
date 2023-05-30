# Comparing `tmp/polyglot_piranha-0.3.4.tar.gz` & `tmp/polyglot_piranha-0.3.5.tar.gz`

## Comparing `polyglot_piranha-0.3.4.tar` & `polyglot_piranha-0.3.5.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.4/Cargo.toml
--rw-r--r--   0     1001      123    35670 2023-05-26 12:53:30.000000 polyglot_piranha-0.3.4/Cargo.lock
--rw-r--r--   0     1001      123    11359 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/LICENSE
--rw-r--r--   0     1001      123     3091 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/README.md
--rw-r--r--   0     1001      123     1373 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
--rw-r--r--   0     1001      123      994 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
--rw-r--r--   0     1001      123     5517 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
--rw-r--r--   0     1001      123     5621 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
--rw-r--r--   0     1001      123    66915 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
--rw-r--r--   0     1001      123    21518 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
--rw-r--r--   0     1001      123     5106 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
--rw-r--r--   0     1001      123      377 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
--rw-r--r--   0     1001      123     3615 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
--rw-r--r--   0     1001      123     5039 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
--rw-r--r--   0     1001      123     2584 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
--rw-r--r--   0     1001      123     2605 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
--rw-r--r--   0     1001      123      550 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
--rw-r--r--   0     1001      123     2456 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
--rw-r--r--   0     1001      123    13106 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
--rw-r--r--   0     1001      123     5875 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
--rw-r--r--   0     1001      123    85120 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
--rw-r--r--   0     1001      123    55188 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
--rw-r--r--   0     1001      123    48474 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
--rw-r--r--   0     1001      123     2304 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
--rw-r--r--   0     1001      123    33367 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
--rw-r--r--   0     1001      123     6780 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
--rw-r--r--   0     1001      123     3480 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
--rw-r--r--   0     1001      123     8540 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
--rw-r--r--   0     1001      123     4153 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
--rw-r--r--   0     1001      123     4326 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
--rw-r--r--   0     1001      123     2555 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
--rw-r--r--   0     1001      123     1490 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
--rw-r--r--   0     1001      123     2091 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
--rw-r--r--   0     1001      123     2194 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
--rw-r--r--   0     1001      123     1550 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
--rw-r--r--   0     1001      123     1618 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
--rw-r--r--   0     1001      123     1573 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
--rw-r--r--   0     1001      123       75 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
--rw-r--r--   0     1001      123      109 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
--rw-r--r--   0     1001      123      175 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
--rw-r--r--   0     1001      123      103 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
--rw-r--r--   0     1001      123      154 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
--rw-r--r--   0     1001      123      155 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
--rw-r--r--   0     1001      123      160 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
--rw-r--r--   0     1001      123      122 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
--rw-r--r--   0     1001      123      229 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
--rw-r--r--   0     1001      123       97 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
--rw-r--r--   0     1001      123      202 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
--rw-r--r--   0     1001      123      213 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
--rw-r--r--   0     1001      123      216 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
--rw-r--r--   0     1001      123      361 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
--rw-r--r--   0     1001      123      525 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
--rw-r--r--   0     1001      123      526 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
--rw-r--r--   0     1001      123      488 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
--rw-r--r--   0     1001      123      489 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
--rw-r--r--   0     1001      123      526 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
--rw-r--r--   0     1001      123      704 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
--rw-r--r--   0     1001      123     1332 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
--rw-r--r--   0     1001      123      192 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
--rw-r--r--   0     1001      123      739 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
--rw-r--r--   0     1001      123      652 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
--rw-r--r--   0     1001      123     1896 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
--rw-r--r--   0     1001      123      844 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return.json
--rw-r--r--   0     1001      123     1776 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
--rw-r--r--   0     1001      123     1932 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
--rw-r--r--   0     1001      123     4525 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
--rw-r--r--   0     1001      123      251 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
--rw-r--r--   0     1001      123      246 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
--rw-r--r--   0     1001      123      142 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
--rw-r--r--   0     1001      123     1637 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
--rw-r--r--   0     1001      123     1304 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
--rw-r--r--   0     1001      123     1304 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
--rw-r--r--   0     1001      123     1107 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
--rw-r--r--   0     1001      123     2565 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/javascript/src/config_checker.js
--rw-r--r--   0     1001      123     4304 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/javascript/src/piranha.js
--rw-r--r--   0     1001      123    27988 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/javascript/src/refactor.js
--rw-r--r--   0     1001      123     1445 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/javascript/src/source_checker.js
--rw-r--r--   0     1001      123      646 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
--rw-r--r--   0     1001      123     1064 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/README.txt
--rw-r--r--   0     1001      123    26229 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
--rw-r--r--   0     1001      123        0 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
--rw-r--r--   0     1001      123      793 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/pyproject.toml
--rw-r--r--   0     1001      123     2043 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/go/edges.toml
--rw-r--r--   0     1001      123    11039 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/go/rules.toml
--rw-r--r--   0     1001      123     1466 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/go/scope_config.toml
--rwxr-xr-x   0     1001      123     2241 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/java/edges.toml
--rwxr-xr-x   0     1001      123    17674 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/java/rules.toml
--rwxr-xr-x   0     1001      123     3580 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/java/scope_config.toml
--rwxr-xr-x   0     1001      123     2251 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/kt/edges.toml
--rwxr-xr-x   0     1001      123    19368 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/kt/rules.toml
--rwxr-xr-x   0     1001      123     2142 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/kt/scope_config.toml
--rw-r--r--   0     1001      123     2316 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/swift/edges.toml
--rw-r--r--   0     1001      123    27137 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/swift/rules.toml
--rw-r--r--   0     1001      123     1684 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/swift/scope_config.toml
--rw-r--r--   0     1001      123     7391 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/lib.rs
--rw-r--r--   0     1001      123     1679 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/main.rs
--rw-r--r--   0     1001      123     3583 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/default_configs.rs
--rw-r--r--   0     1001      123     4915 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/edit.rs
--rw-r--r--   0     1001      123    10594 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/filter.rs
--rw-r--r--   0     1001      123     7097 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/language.rs
--rw-r--r--   0     1001      123    11128 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/matches.rs
--rw-r--r--   0     1001      123      924 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/mod.rs
--rw-r--r--   0     1001      123     1987 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/outgoing_edges.rs
--rw-r--r--   0     1001      123    14245 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/piranha_arguments.rs
--rw-r--r--   0     1001      123     2091 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/piranha_output.rs
--rw-r--r--   0     1001      123     7801 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/rule.rs
--rw-r--r--   0     1001      123     6286 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/rule_graph.rs
--rw-r--r--   0     1001      123     6288 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/rule_store.rs
--rw-r--r--   0     1001      123     3402 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/scopes.rs
--rw-r--r--   0     1001      123    14473 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/source_code_unit.rs
--rw-r--r--   0     1001      123     1661 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/unit_tests/piranha_arguments_test.rs
--rw-r--r--   0     1001      123     8344 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/unit_tests/rule_test.rs
--rw-r--r--   0     1001      123     6067 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/unit_tests/scopes_test.rs
--rw-r--r--   0     1001      123    11082 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/unit_tests/source_code_unit_test.rs
--rw-r--r--   0     1001      123     8260 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/mod.rs
--rw-r--r--   0     1001      123     1647 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_go.rs
--rw-r--r--   0     1001      123    12953 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_java.rs
--rw-r--r--   0     1001      123     1862 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_kt.rs
--rw-r--r--   0     1001      123     2423 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_python.rs
--rw-r--r--   0     1001      123     3532 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_swift.rs
--rw-r--r--   0     1001      123      770 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_thrift.rs
--rw-r--r--   0     1001      123     1138 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_ts.rs
--rw-r--r--   0     1001      123     1281 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_tsx.rs
--rw-r--r--   0     1001      123     5629 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/utilities/mod.rs
--rw-r--r--   0     1001      123    12743 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/utilities/tree_sitter_utilities.rs
--rw-r--r--   0     1001      123     3681 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/utilities/unit_tests/tree_sitter_utilities_test.rs
--rw-r--r--   0     1001      123     2237 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/utilities/unit_tests/utilities_test.rs
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.5/Cargo.toml
+-rw-r--r--   0     1001      123    35640 2023-05-30 17:34:13.000000 polyglot_piranha-0.3.5/Cargo.lock
+-rw-r--r--   0     1001      123    11359 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/LICENSE
+-rw-r--r--   0     1001      123     3091 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/README.md
+-rw-r--r--   0     1001      123     1373 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
+-rw-r--r--   0     1001      123      994 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
+-rw-r--r--   0     1001      123     5517 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
+-rw-r--r--   0     1001      123     5621 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
+-rw-r--r--   0     1001      123    66915 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
+-rw-r--r--   0     1001      123    21518 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
+-rw-r--r--   0     1001      123     5106 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
+-rw-r--r--   0     1001      123      377 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
+-rw-r--r--   0     1001      123     3615 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
+-rw-r--r--   0     1001      123     5039 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
+-rw-r--r--   0     1001      123     2584 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
+-rw-r--r--   0     1001      123     2605 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
+-rw-r--r--   0     1001      123      550 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
+-rw-r--r--   0     1001      123     2456 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
+-rw-r--r--   0     1001      123    13106 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
+-rw-r--r--   0     1001      123     5875 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
+-rw-r--r--   0     1001      123    85120 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
+-rw-r--r--   0     1001      123    55188 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
+-rw-r--r--   0     1001      123    48474 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
+-rw-r--r--   0     1001      123     2304 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
+-rw-r--r--   0     1001      123    33367 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
+-rw-r--r--   0     1001      123     6780 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
+-rw-r--r--   0     1001      123     3480 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
+-rw-r--r--   0     1001      123     8540 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
+-rw-r--r--   0     1001      123     4153 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
+-rw-r--r--   0     1001      123     4326 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
+-rw-r--r--   0     1001      123     2555 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
+-rw-r--r--   0     1001      123     1490 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
+-rw-r--r--   0     1001      123     2091 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
+-rw-r--r--   0     1001      123     2194 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
+-rw-r--r--   0     1001      123     1550 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
+-rw-r--r--   0     1001      123     1618 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
+-rw-r--r--   0     1001      123     1573 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
+-rw-r--r--   0     1001      123       75 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
+-rw-r--r--   0     1001      123      109 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
+-rw-r--r--   0     1001      123      175 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
+-rw-r--r--   0     1001      123      103 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
+-rw-r--r--   0     1001      123      154 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
+-rw-r--r--   0     1001      123      155 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
+-rw-r--r--   0     1001      123      160 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
+-rw-r--r--   0     1001      123      122 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
+-rw-r--r--   0     1001      123      229 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
+-rw-r--r--   0     1001      123       97 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
+-rw-r--r--   0     1001      123      202 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
+-rw-r--r--   0     1001      123      213 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
+-rw-r--r--   0     1001      123      216 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
+-rw-r--r--   0     1001      123      361 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
+-rw-r--r--   0     1001      123      525 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
+-rw-r--r--   0     1001      123      526 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
+-rw-r--r--   0     1001      123      488 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
+-rw-r--r--   0     1001      123      489 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
+-rw-r--r--   0     1001      123      526 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
+-rw-r--r--   0     1001      123      704 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
+-rw-r--r--   0     1001      123     1332 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
+-rw-r--r--   0     1001      123      192 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
+-rw-r--r--   0     1001      123      739 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
+-rw-r--r--   0     1001      123      652 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
+-rw-r--r--   0     1001      123     1896 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
+-rw-r--r--   0     1001      123      844 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return.json
+-rw-r--r--   0     1001      123     1776 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
+-rw-r--r--   0     1001      123     1932 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
+-rw-r--r--   0     1001      123     4525 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
+-rw-r--r--   0     1001      123      251 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
+-rw-r--r--   0     1001      123      246 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
+-rw-r--r--   0     1001      123      142 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
+-rw-r--r--   0     1001      123     1637 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
+-rw-r--r--   0     1001      123     1304 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
+-rw-r--r--   0     1001      123     1304 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
+-rw-r--r--   0     1001      123     1107 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
+-rw-r--r--   0     1001      123     2565 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/javascript/src/config_checker.js
+-rw-r--r--   0     1001      123     4304 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/javascript/src/piranha.js
+-rw-r--r--   0     1001      123    27988 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/javascript/src/refactor.js
+-rw-r--r--   0     1001      123     1445 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/javascript/src/source_checker.js
+-rw-r--r--   0     1001      123      646 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
+-rw-r--r--   0     1001      123     1064 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/README.txt
+-rw-r--r--   0     1001      123    26229 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
+-rw-r--r--   0     1001      123        0 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
+-rw-r--r--   0     1001      123      793 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/pyproject.toml
+-rw-r--r--   0     1001      123     2043 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/go/edges.toml
+-rw-r--r--   0     1001      123    11039 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/go/rules.toml
+-rw-r--r--   0     1001      123     1466 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/go/scope_config.toml
+-rwxr-xr-x   0     1001      123     2241 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/java/edges.toml
+-rwxr-xr-x   0     1001      123    17674 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/java/rules.toml
+-rwxr-xr-x   0     1001      123     3580 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/java/scope_config.toml
+-rwxr-xr-x   0     1001      123     2251 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/kt/edges.toml
+-rwxr-xr-x   0     1001      123    19368 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/kt/rules.toml
+-rwxr-xr-x   0     1001      123     2142 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/kt/scope_config.toml
+-rw-r--r--   0     1001      123     2316 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/swift/edges.toml
+-rw-r--r--   0     1001      123    27137 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/swift/rules.toml
+-rw-r--r--   0     1001      123     1684 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/swift/scope_config.toml
+-rw-r--r--   0     1001      123     7391 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/lib.rs
+-rw-r--r--   0     1001      123     1679 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/main.rs
+-rw-r--r--   0     1001      123     3583 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/default_configs.rs
+-rw-r--r--   0     1001      123     4915 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/edit.rs
+-rw-r--r--   0     1001      123    11028 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/filter.rs
+-rw-r--r--   0     1001      123     7097 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/language.rs
+-rw-r--r--   0     1001      123    11128 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/matches.rs
+-rw-r--r--   0     1001      123      924 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/mod.rs
+-rw-r--r--   0     1001      123     1987 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/outgoing_edges.rs
+-rw-r--r--   0     1001      123    14245 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/piranha_arguments.rs
+-rw-r--r--   0     1001      123     2091 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/piranha_output.rs
+-rw-r--r--   0     1001      123     7801 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/rule.rs
+-rw-r--r--   0     1001      123     6286 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/rule_graph.rs
+-rw-r--r--   0     1001      123     6288 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/rule_store.rs
+-rw-r--r--   0     1001      123     3402 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/scopes.rs
+-rw-r--r--   0     1001      123    14473 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/source_code_unit.rs
+-rw-r--r--   0     1001      123     1661 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/unit_tests/piranha_arguments_test.rs
+-rw-r--r--   0     1001      123     8344 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/unit_tests/rule_test.rs
+-rw-r--r--   0     1001      123     6067 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/unit_tests/scopes_test.rs
+-rw-r--r--   0     1001      123    13356 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/unit_tests/source_code_unit_test.rs
+-rw-r--r--   0     1001      123     8260 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1647 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_go.rs
+-rw-r--r--   0     1001      123    12953 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_java.rs
+-rw-r--r--   0     1001      123     1862 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_kt.rs
+-rw-r--r--   0     1001      123     2423 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_python.rs
+-rw-r--r--   0     1001      123     3532 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_swift.rs
+-rw-r--r--   0     1001      123      770 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_thrift.rs
+-rw-r--r--   0     1001      123     1138 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_ts.rs
+-rw-r--r--   0     1001      123     1281 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_tsx.rs
+-rw-r--r--   0     1001      123     5629 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/utilities/mod.rs
+-rw-r--r--   0     1001      123    12743 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/utilities/tree_sitter_utilities.rs
+-rw-r--r--   0     1001      123     3681 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/utilities/unit_tests/tree_sitter_utilities_test.rs
+-rw-r--r--   0     1001      123     2237 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/utilities/unit_tests/utilities_test.rs
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.5/PKG-INFO
```

### Comparing `polyglot_piranha-0.3.4/Cargo.toml` & `polyglot_piranha-0.3.5/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "Ameya Ketkar <ketkara@uber.com>",
   "Lazaro Clapp <lazaro@uber.com>",
   "Murali Krishna Ramanathan",
   "Uber Technologies Inc.",
 ]
 name = "piranha"
 description = "Polyglot Piranha is a library for performing structural find and replace with deep cleanup."
-version = "0.3.4"
+version = "0.3.5"
 edition = "2021"
 include = ["pyproject.toml", "src/"]
 exclude = ["legacy"]
 license-file = "LICENSE"
 categories = [
   "structural find-replace",
   "find-replace",
```

### Comparing `polyglot_piranha-0.3.4/Cargo.lock` & `polyglot_piranha-0.3.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "191d9573962933b4027f932c600cd252ce27a8ad5979418fe78e43c07996f27b"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.17",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
@@ -555,20 +555,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -604,17 +601,17 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -633,15 +630,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "piranha"
-version = "0.3.4"
+version = "0.3.5"
 dependencies = [
  "assert_cmd",
  "cc",
  "clap",
  "colored",
  "derive_builder",
  "env_logger",
@@ -951,15 +948,15 @@
 name = "serde_derive"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.17",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -999,17 +996,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.17"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45b6ddbb36c5b969c182aec3c4a0bce7df3fbad4b77114706a49aacc80567388"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `polyglot_piranha-0.3.4/LICENSE` & `polyglot_piranha-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/README.md` & `polyglot_piranha-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_argument.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_receive.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json` & `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java` & `polyglot_piranha-0.3.5/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak` & `polyglot_piranha-0.3.5/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect` & `polyglot_piranha-0.3.5/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/javascript/src/config_checker.js` & `polyglot_piranha-0.3.5/legacy/javascript/src/config_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/javascript/src/piranha.js` & `polyglot_piranha-0.3.5/legacy/javascript/src/piranha.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/javascript/src/refactor.js` & `polyglot_piranha-0.3.5/legacy/javascript/src/refactor.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/javascript/src/source_checker.js` & `polyglot_piranha-0.3.5/legacy/javascript/src/source_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt` & `polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/README.txt` & `polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/README.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp` & `polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/pyproject.toml` & `polyglot_piranha-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/go/edges.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/go/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/go/rules.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/go/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/go/scope_config.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/go/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/java/edges.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/java/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/java/rules.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/java/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/java/scope_config.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/java/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/kt/edges.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/kt/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/kt/rules.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/kt/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/kt/scope_config.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/kt/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/swift/edges.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/swift/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/swift/rules.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/swift/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/cleanup_rules/swift/scope_config.toml` & `polyglot_piranha-0.3.5/src/cleanup_rules/swift/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/lib.rs` & `polyglot_piranha-0.3.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/main.rs` & `polyglot_piranha-0.3.5/src/main.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/default_configs.rs` & `polyglot_piranha-0.3.5/src/models/default_configs.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/edit.rs` & `polyglot_piranha-0.3.5/src/models/edit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/filter.rs` & `polyglot_piranha-0.3.5/src/models/filter.rs`

 * *Files 3% similar despite different names*

```diff
@@ -129,17 +129,17 @@
 ///      .contains(TSQuery::new("(parameter_list)"))
 ///      .at_least(1)
 ///      .at_most(10)
 ///      .build().unwrap()
 /// ```
 ///
 macro_rules! filter {
-  (enclosing_node = $enclosing_node:expr $(, not_contains= [$($q:expr,)*])? $(, contains= $p:expr)? $(, at_least=$min:expr)? $(, at_most=$max:expr)?) => {
+  ($(enclosing_node = $enclosing_node:expr)? $(, not_contains= [$($q:expr,)*])? $(, contains= $p:expr)? $(, at_least=$min:expr)? $(, at_most=$max:expr)?) => {
     $crate::models::filter::FilterBuilder::default()
-      .enclosing_node($crate::utilities::tree_sitter_utilities::TSQuery::new($enclosing_node.to_string()))
+      $(.enclosing_node($crate::utilities::tree_sitter_utilities::TSQuery::new($enclosing_node.to_string())))?
       $(.not_contains(vec![$($crate::utilities::tree_sitter_utilities::TSQuery::new($q.to_string()),)*]))?
       $(.contains($crate::utilities::tree_sitter_utilities::TSQuery::new($p.to_string())))?
       $(.at_least($min))?
       $(.at_most($max))?
       .build().unwrap()
   };
 }
@@ -192,27 +192,40 @@
   fn _check(
     &self, filter: Filter, node: Node, rule_store: &mut RuleStore,
     substitutions: &HashMap<String, String>,
   ) -> bool {
     // This ensures that the below while loop considers the current node too when checking for filters.
     // It does not make sense to check for filter if current node is a "leaf" node.
     let mut initial_node = node;
-    if node.child_count() > 0 {
-      initial_node = node.child(0).unwrap();
-    }
 
     // No enclosing node is provided
     if filter.enclosing_node().get_query().as_str() == DEFAULT_ENCLOSING_QUERY {
       // Get the enclosing node matching the pattern specified in the filter (`filter.enclosing_node`)
-      panic!["Not implemented"]
+      self._check_current_node(filter, rule_store, substitutions, initial_node)
     } else {
+      if node.child_count() > 0 {
+        initial_node = node.child(0).unwrap();
+      }
       self._check_enclosing_node(filter, rule_store, substitutions, initial_node)
     }
   }
 
+  fn _check_current_node(
+    &self, filter: Filter, rule_store: &mut RuleStore, substitutions: &HashMap<String, String>,
+    node: Node,
+  ) -> bool {
+    if !self._filter_contains(&filter, rule_store, substitutions, &node) {
+      return false;
+    }
+    if !self._filter_not_contains(&filter, rule_store, substitutions, &node) {
+      return false;
+    }
+    true
+  }
+
   /// This function checks for the contains
   fn _check_enclosing_node(
     &self, filter: Filter, rule_store: &mut RuleStore, substitutions: &HashMap<String, String>,
     initial: Node,
   ) -> bool {
     let mut matched_enclosing_node = false;
     let mut current_node = initial;
```

### Comparing `polyglot_piranha-0.3.4/src/models/language.rs` & `polyglot_piranha-0.3.5/src/models/language.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/matches.rs` & `polyglot_piranha-0.3.5/src/models/matches.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/mod.rs` & `polyglot_piranha-0.3.5/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/outgoing_edges.rs` & `polyglot_piranha-0.3.5/src/models/outgoing_edges.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/piranha_arguments.rs` & `polyglot_piranha-0.3.5/src/models/piranha_arguments.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/piranha_output.rs` & `polyglot_piranha-0.3.5/src/models/piranha_output.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/rule.rs` & `polyglot_piranha-0.3.5/src/models/rule.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/rule_graph.rs` & `polyglot_piranha-0.3.5/src/models/rule_graph.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/rule_store.rs` & `polyglot_piranha-0.3.5/src/models/rule_store.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/scopes.rs` & `polyglot_piranha-0.3.5/src/models/scopes.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/source_code_unit.rs` & `polyglot_piranha-0.3.5/src/models/source_code_unit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/unit_tests/piranha_arguments_test.rs` & `polyglot_piranha-0.3.5/src/models/unit_tests/piranha_arguments_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/unit_tests/rule_test.rs` & `polyglot_piranha-0.3.5/src/models/unit_tests/rule_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/unit_tests/scopes_test.rs` & `polyglot_piranha-0.3.5/src/models/unit_tests/scopes_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/models/unit_tests/source_code_unit_test.rs` & `polyglot_piranha-0.3.5/src/models/unit_tests/source_code_unit_test.rs`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
  <p>Unless required by applicable law or agreed to in writing, software distributed under the
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 
-use tree_sitter::Parser;
+use tree_sitter::{Parser, Point};
 
 use crate::{
   filter,
   models::{
     default_configs::{JAVA, UNUSED_CODE_PATH},
     filter::Filter,
     language::PiranhaLanguage,
@@ -250,27 +250,27 @@
 #[test]
 fn test_satisfies_filters_at_most_0_negative() {
   let contains_0 = run_test_satisfies_filters(
     filter! {
         enclosing_node= "(method_declaration) @md",
         contains= "(
                     ((method_invocation name: (_) @name) @method)
-                    (#eq? @name equals)
+                    (#eq? @name \"equals\")
                 )",
         at_least = 0,
         at_most = 0
     },
     |result| !result,
   );
   let not_contains = run_test_satisfies_filters(
     filter! {
         enclosing_node= "(method_declaration) @md",
         not_contains= ["(
                     ((method_invocation name: (_) @name) @method)
-                    (#eq? @name equals)
+                    (#eq? @name \"equals\")
                 )",]
     },
     |result| !result,
   );
   assert_eq!(contains_0, not_contains);
 }
 
@@ -401,7 +401,91 @@
     &HashMap::from([
       ("variable_name".to_string(), "isFlagTreated".to_string()),
       ("init".to_string(), "true".to_string())
     ]),
     &mut rule_store,
   ));
 }
+
+// Tests for contains without providing an enclosing node
+fn run_test_satisfies_filters_without_enclosing(
+  filter: Filter, // Replace with the filter to test
+  assertion: fn(bool) -> bool,
+) {
+  let _rule = piranha_rule! {
+      name= "test",
+      query= "(
+            (method_declaration
+              name: (identifier) @method_name) @md
+            )",
+      filters= [filter,]
+  };
+  let rule = InstantiatedRule::new(&_rule, &HashMap::new());
+  let source_code = "class Test {
+        public void foobar(){
+            boolean isFlagTreated = true;
+            if (isFlagTreated) {
+              x = anotherFunction(isFlagTreated);
+              y = foobar();
+              y = foobar();
+              x.equals(y);
+            }
+        }
+        }";
+
+  let mut rule_store = RuleStore::default();
+  let java = get_java_tree_sitter_language();
+  let mut parser = java.parser();
+  let piranha_args = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(UNUSED_CODE_PATH.to_string())
+    .language(java)
+    .build();
+  let source_code_unit = SourceCodeUnit::new(
+    &mut parser,
+    source_code.to_string(),
+    &HashMap::new(),
+    PathBuf::new().as_path(),
+    &piranha_args,
+  );
+
+  let start = Point::new(1, 8);
+  let end = Point::new(9, 9);
+  let node = &source_code_unit
+    .root_node()
+    .descendant_for_point_range(start, end)
+    .unwrap();
+
+  assert!(assertion(source_code_unit.is_satisfied(
+    *node,
+    &rule,
+    &HashMap::from([("method_name".to_string(), "foobar".to_string()),]),
+    &mut rule_store,
+  )));
+}
+
+#[test]
+fn test_not_contains_no_enclosing_negative() {
+  run_test_satisfies_filters_without_enclosing(
+    filter! {,
+    not_contains= ["(
+                   (method_invocation
+                      name: (identifier) @inv) @md
+                   (#eq? @inv \"@method_name\")
+                      )",]},
+    |result| !result,
+  );
+}
+
+// Tests for contains with enclosing
+#[test]
+fn test_contains_no_enclosing_positive() {
+  run_test_satisfies_filters_without_enclosing(
+    filter! {,
+    contains= "(
+                   (method_invocation
+                      name: (identifier) @inv) @md
+                   (#eq? @inv \"@method_name\")
+                      )",
+    at_least =2},
+    |result| result,
+  );
+}
```

### Comparing `polyglot_piranha-0.3.4/src/tests/mod.rs` & `polyglot_piranha-0.3.5/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/tests/test_piranha_go.rs` & `polyglot_piranha-0.3.5/src/tests/test_piranha_go.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/tests/test_piranha_java.rs` & `polyglot_piranha-0.3.5/src/tests/test_piranha_java.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/tests/test_piranha_kt.rs` & `polyglot_piranha-0.3.5/src/tests/test_piranha_kt.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/tests/test_piranha_python.rs` & `polyglot_piranha-0.3.5/src/tests/test_piranha_python.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/tests/test_piranha_swift.rs` & `polyglot_piranha-0.3.5/src/tests/test_piranha_swift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/tests/test_piranha_thrift.rs` & `polyglot_piranha-0.3.5/src/tests/test_piranha_thrift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/tests/test_piranha_ts.rs` & `polyglot_piranha-0.3.5/src/tests/test_piranha_ts.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/tests/test_piranha_tsx.rs` & `polyglot_piranha-0.3.5/src/tests/test_piranha_tsx.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/utilities/mod.rs` & `polyglot_piranha-0.3.5/src/utilities/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/utilities/tree_sitter_utilities.rs` & `polyglot_piranha-0.3.5/src/utilities/tree_sitter_utilities.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/utilities/unit_tests/tree_sitter_utilities_test.rs` & `polyglot_piranha-0.3.5/src/utilities/unit_tests/tree_sitter_utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/src/utilities/unit_tests/utilities_test.rs` & `polyglot_piranha-0.3.5/src/utilities/unit_tests/utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.4/PKG-INFO` & `polyglot_piranha-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyglot_piranha
-Version: 0.3.4
+Version: 0.3.5
 License-File: LICENSE
 License-File: LICENSE
 License-File: NOTICE
 Summary: Polyglot Piranha is a library for performing structural find and replace with deep cleanup.
 Keywords: refactoring,code update,structural find-replace,structural search and replace,structural search
 Author: Uber Technologies Inc.
 Author-email: Ameya Ketkar <ketkara@uber.com>, Lazaro Clapp <lazaro@uber.com>
```

