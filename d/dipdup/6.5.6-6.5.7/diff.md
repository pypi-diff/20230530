# Comparing `tmp/dipdup-6.5.6.tar.gz` & `tmp/dipdup-6.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipdup-6.5.6.tar", max compression
+gzip compressed data, was "dipdup-6.5.7.tar", max compression
```

## Comparing `dipdup-6.5.6.tar` & `dipdup-6.5.7.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0     1067 2023-05-02 23:14:20.261844 dipdup-6.5.6/LICENSE
--rw-r--r--   0        0        0     3937 2023-05-02 23:14:20.261844 dipdup-6.5.6/README.md
--rw-r--r--   0        0        0     2778 2023-05-02 23:14:20.289845 dipdup-6.5.6/pyproject.toml
--rw-r--r--   0        0        0      213 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/__init__.py
--rw-r--r--   0        0        0      106 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/__main__.py
--rw-r--r--   0        0        0      585 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/baking_bad.py
--rw-r--r--   0        0        0    18507 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/cli.py
--rw-r--r--   0        0        0    22289 2023-05-02 23:14:20.289845 dipdup-6.5.6/src/dipdup/codegen.py
--rw-r--r--   0        0        0    69884 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/config.py
--rw-r--r--   0        0        0    25902 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/context.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/coinbase/__init__.py
--rw-r--r--   0        0        0     2387 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/coinbase/datasource.py
--rw-r--r--   0        0        0     1309 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/coinbase/models.py
--rw-r--r--   0        0        0     6291 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/datasource.py
--rw-r--r--   0        0        0     2420 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/factory.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/ipfs/__init__.py
--rw-r--r--   0        0        0      688 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/ipfs/datasource.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/metadata/__init__.py
--rw-r--r--   0        0        0     1773 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/metadata/datasource.py
--rw-r--r--   0        0        0      161 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/metadata/enums.py
--rw-r--r--   0        0        0     2172 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/subscription.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/tzkt/__init__.py
--rw-r--r--   0        0        0    46886 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/tzkt/datasource.py
--rw-r--r--   0        0        0     9895 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/datasources/tzkt/models.py
--rw-r--r--   0        0        0    24980 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/dipdup.py
--rw-r--r--   0        0        0     2013 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/enums.py
--rw-r--r--   0        0        0     2192 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/env.py
--rw-r--r--   0        0        0     9500 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/exceptions.py
--rw-r--r--   0        0        0     2734 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/fetcher.py
--rw-r--r--   0        0        0    25590 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/hasura.py
--rw-r--r--   0        0        0     9793 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/http.py
--rw-r--r--   0        0        0     7414 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/index.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/big_map/__init__.py
--rw-r--r--   0        0        0     3033 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/big_map/fetcher.py
--rw-r--r--   0        0        0     7103 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/big_map/index.py
--rw-r--r--   0        0        0     2131 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/big_map/matcher.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/event/__init__.py
--rw-r--r--   0        0        0     1402 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/event/fetcher.py
--rw-r--r--   0        0        0     5324 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/event/index.py
--rw-r--r--   0        0        0     3297 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/event/matcher.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/head/__init__.py
--rw-r--r--   0        0        0     2320 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/head/index.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/operation/__init__.py
--rw-r--r--   0        0        0    19397 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/operation/fetcher.py
--rw-r--r--   0        0        0    13344 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/operation/index.py
--rw-r--r--   0        0        0     7386 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/operation/matcher.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/token_transfer/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/token_transfer/fetcher.py
--rw-r--r--   0        0        0     5377 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/token_transfer/index.py
--rw-r--r--   0        0        0     1791 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/indexes/token_transfer/matcher.py
--rwxr-xr-x   0        0        0     8269 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/install.py
--rw-r--r--   0        0        0    22523 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/models.py
--rw-r--r--   0        0        0    10978 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/project.py
--rw-r--r--   0        0        0      203 2023-05-02 23:14:20.293845 dipdup-6.5.6/src/dipdup/projects/base/.dockerignore.j2
--rw-r--r--   0        0        0     2097 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/.gitignore.j2
--rw-r--r--   0        0        0      431 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/Dockerfile.j2
--rw-r--r--   0        0        0      474 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/README.md.j2
--rw-r--r--   0        0        0      489 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/dipdup.dev.yml.j2
--rw-r--r--   0        0        0      481 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/dipdup.prod.yml.j2
--rw-r--r--   0        0        0     2907 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/docker-compose.swarm.yml.j2
--rw-r--r--   0        0        0     1341 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/docker-compose.yml.j2
--rw-r--r--   0        0        0       37 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/replay.json.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0      197 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
--rw-r--r--   0        0        0      128 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/blank/dipdup.yml.j2
--rw-r--r--   0        0        0       95 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-auction.json
--rw-r--r--   0        0        0       98 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-big-maps.json
--rw-r--r--   0        0        0       83 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-dao.json
--rw-r--r--   0        0        0       83 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-dex.json
--rw-r--r--   0        0        0       95 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-domains.json
--rw-r--r--   0        0        0       92 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-events.json
--rw-r--r--   0        0        0      101 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-factories.json
--rw-r--r--   0        0        0       86 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-head.json
--rw-r--r--   0        0        0      119 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-nft-marketplace.json
--rw-r--r--   0        0        0       83 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-raw.json
--rw-r--r--   0        0        0      119 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-token-transfers.json
--rw-r--r--   0        0        0       89 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo-token.json
--rw-r--r--   0        0        0     1116 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      918 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
--rw-r--r--   0        0        0     1624 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
--rw-r--r--   0        0        0      853 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
--rw-r--r--   0        0        0     1524 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      779 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      847 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     1713 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      840 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      702 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      416 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     4878 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0     1842 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1769 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
--rw-r--r--   0        0        0      587 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
--rw-r--r--   0        0        0     1642 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
--rw-r--r--   0        0        0     1689 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
--rw-r--r--   0        0        0     1039 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
--rw-r--r--   0        0        0      960 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
--rw-r--r--   0        0        0     1868 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1795 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
--rw-r--r--   0        0        0      581 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
--rw-r--r--   0        0        0     1636 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
--rw-r--r--   0        0        0     1655 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
--rw-r--r--   0        0        0     1160 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
--rw-r--r--   0        0        0      956 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
--rw-r--r--   0        0        0      948 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      900 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      564 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
--rw-r--r--   0        0        0      536 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
--rw-r--r--   0        0        0     1475 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
--rw-r--r--   0        0        0      819 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      592 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_events/dipdup.yml.j2
--rw-r--r--   0        0        0      976 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      716 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
--rw-r--r--   0        0        0      416 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      333 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_head/dipdup.yml.j2
--rw-r--r--   0        0        0     1230 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      586 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
--rw-r--r--   0        0        0     1018 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
--rw-r--r--   0        0        0      949 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      866 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
--rw-r--r--   0        0        0     1382 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      486 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_raw/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      350 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
--rw-r--r--   0        0        0      235 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      787 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      453 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      647 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      945 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      456 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      550 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      822 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     1226 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/linters_default/Makefile.j2
--rw-r--r--   0        0        0     1032 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/linters_default/pyproject.toml.j2
--rw-r--r--   0        0        0      923 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/linters_none/Makefile.j2
--rw-r--r--   0        0        0      552 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/projects/linters_none/pyproject.toml.j2
--rw-r--r--   0        0        0     4008 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/prometheus.py
--rw-r--r--   0        0        0        0 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/py.typed
--rw-r--r--   0        0        0     4845 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/scheduler.py
--rw-r--r--   0        0        0     6041 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/sentry.py
--rw-r--r--   0        0        0      199 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/sql/dipdup_head_status.sql
--rw-r--r--   0        0        0     2111 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/sql/truncate_schema.sql
--rw-r--r--   0        0        0      227 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/templates/callback.py.j2
--rw-r--r--   0        0        0      157 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/templates/models.py.j2
--rw-r--r--   0        0        0     3029 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/transactions.py
--rw-r--r--   0        0        0     4631 2023-05-02 23:14:20.297845 dipdup-6.5.6/src/dipdup/utils/__init__.py
--rw-r--r--   0        0        0     1824 2023-05-02 23:14:20.301845 dipdup-6.5.6/src/dipdup/utils/codegen.py
--rw-r--r--   0        0        0    11813 2023-05-02 23:14:20.301845 dipdup-6.5.6/src/dipdup/utils/database.py
--rw-r--r--   0        0        0     2044 2023-05-02 23:14:20.301845 dipdup-6.5.6/src/dipdup/utils/sys.py
--rw-r--r--   0        0        0     4513 2023-05-02 23:14:20.301845 dipdup-6.5.6/src/dipdup/yaml.py
--rw-r--r--   0        0        0     5840 1970-01-01 00:00:00.000000 dipdup-6.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-30 19:26:42.640780 dipdup-6.5.7/LICENSE
+-rw-r--r--   0        0        0     3992 2023-05-30 19:26:42.640780 dipdup-6.5.7/README.md
+-rw-r--r--   0        0        0     2783 2023-05-30 19:26:42.672780 dipdup-6.5.7/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/__main__.py
+-rw-r--r--   0        0        0      585 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/baking_bad.py
+-rw-r--r--   0        0        0    19164 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/cli.py
+-rw-r--r--   0        0        0    22289 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/codegen.py
+-rw-r--r--   0        0        0    70122 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/config.py
+-rw-r--r--   0        0        0    25902 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/context.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/coinbase/__init__.py
+-rw-r--r--   0        0        0     2387 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/coinbase/datasource.py
+-rw-r--r--   0        0        0     1309 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/coinbase/models.py
+-rw-r--r--   0        0        0     6291 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/datasource.py
+-rw-r--r--   0        0        0     2420 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/factory.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/ipfs/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/ipfs/datasource.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/metadata/__init__.py
+-rw-r--r--   0        0        0     1773 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/metadata/datasource.py
+-rw-r--r--   0        0        0      161 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/metadata/enums.py
+-rw-r--r--   0        0        0     2172 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/subscription.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/tzkt/__init__.py
+-rw-r--r--   0        0        0    46886 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/tzkt/datasource.py
+-rw-r--r--   0        0        0     9895 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/datasources/tzkt/models.py
+-rw-r--r--   0        0        0    25010 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/dipdup.py
+-rw-r--r--   0        0        0     2013 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/enums.py
+-rw-r--r--   0        0        0     2192 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/env.py
+-rw-r--r--   0        0        0     9500 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/exceptions.py
+-rw-r--r--   0        0        0     2734 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/fetcher.py
+-rw-r--r--   0        0        0    25590 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/hasura.py
+-rw-r--r--   0        0        0     9884 2023-05-30 19:26:42.676780 dipdup-6.5.7/src/dipdup/http.py
+-rw-r--r--   0        0        0     7414 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/index.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/big_map/__init__.py
+-rw-r--r--   0        0        0     3033 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/big_map/fetcher.py
+-rw-r--r--   0        0        0     7103 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/big_map/index.py
+-rw-r--r--   0        0        0     2131 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/big_map/matcher.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/event/__init__.py
+-rw-r--r--   0        0        0     1402 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/event/fetcher.py
+-rw-r--r--   0        0        0     5324 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/event/index.py
+-rw-r--r--   0        0        0     3297 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/event/matcher.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/head/__init__.py
+-rw-r--r--   0        0        0     2320 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/head/index.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/operation/__init__.py
+-rw-r--r--   0        0        0    19397 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/operation/fetcher.py
+-rw-r--r--   0        0        0    13470 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/operation/index.py
+-rw-r--r--   0        0        0     8314 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/operation/matcher.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/token_transfer/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/token_transfer/fetcher.py
+-rw-r--r--   0        0        0     5377 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/token_transfer/index.py
+-rw-r--r--   0        0        0     1791 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/indexes/token_transfer/matcher.py
+-rwxr-xr-x   0        0        0     8269 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/install.py
+-rw-r--r--   0        0        0    22702 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/models.py
+-rw-r--r--   0        0        0    10978 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/project.py
+-rw-r--r--   0        0        0      203 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/.dockerignore.j2
+-rw-r--r--   0        0        0     2097 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/.gitignore.j2
+-rw-r--r--   0        0        0      431 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/Dockerfile.j2
+-rw-r--r--   0        0        0      474 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/README.md.j2
+-rw-r--r--   0        0        0      489 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/dipdup.dev.yml.j2
+-rw-r--r--   0        0        0      481 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/dipdup.prod.yml.j2
+-rw-r--r--   0        0        0     2907 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/docker-compose.swarm.yml.j2
+-rw-r--r--   0        0        0     1341 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/docker-compose.yml.j2
+-rw-r--r--   0        0        0       37 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/replay.json.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
+-rw-r--r--   0        0        0      197 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
+-rw-r--r--   0        0        0      128 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/blank/dipdup.yml.j2
+-rw-r--r--   0        0        0       95 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-auction.json
+-rw-r--r--   0        0        0       98 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-big-maps.json
+-rw-r--r--   0        0        0       83 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-dao.json
+-rw-r--r--   0        0        0       83 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-dex.json
+-rw-r--r--   0        0        0       95 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-domains.json
+-rw-r--r--   0        0        0       92 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-events.json
+-rw-r--r--   0        0        0      101 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-factories.json
+-rw-r--r--   0        0        0       86 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-head.json
+-rw-r--r--   0        0        0      119 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-nft-marketplace.json
+-rw-r--r--   0        0        0       83 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-raw.json
+-rw-r--r--   0        0        0      119 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-token-transfers.json
+-rw-r--r--   0        0        0       89 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo-token.json
+-rw-r--r--   0        0        0     1116 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_auction/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      918 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
+-rw-r--r--   0        0        0     1624 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
+-rw-r--r--   0        0        0      853 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
+-rw-r--r--   0        0        0     1524 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      779 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      847 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     1713 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      840 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      702 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_dao/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      416 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      523 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      858 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0     4878 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_dex/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0     1842 2023-05-30 19:26:42.680781 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1769 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      587 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
+-rw-r--r--   0        0        0     1642 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1689 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1039 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
+-rw-r--r--   0        0        0      960 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
+-rw-r--r--   0        0        0     1868 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1795 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      581 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
+-rw-r--r--   0        0        0     1636 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1655 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1160 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
+-rw-r--r--   0        0        0      956 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
+-rw-r--r--   0        0        0      948 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      900 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_domains/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      564 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
+-rw-r--r--   0        0        0      536 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
+-rw-r--r--   0        0        0     1475 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
+-rw-r--r--   0        0        0      819 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      592 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_events/dipdup.yml.j2
+-rw-r--r--   0        0        0      976 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_factories/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      716 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
+-rw-r--r--   0        0        0      416 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      523 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      858 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      333 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_head/dipdup.yml.j2
+-rw-r--r--   0        0        0     1230 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      586 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
+-rw-r--r--   0        0        0     1018 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
+-rw-r--r--   0        0        0      949 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      866 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
+-rw-r--r--   0        0        0     1382 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      486 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_raw/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      350 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
+-rw-r--r--   0        0        0      235 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      787 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      453 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      647 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      945 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      389 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      456 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      550 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      822 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
+-rw-r--r--   0        0        0      389 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0     1226 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/linters_default/Makefile.j2
+-rw-r--r--   0        0        0     1032 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/linters_default/pyproject.toml.j2
+-rw-r--r--   0        0        0      923 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/linters_none/Makefile.j2
+-rw-r--r--   0        0        0      552 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/projects/linters_none/pyproject.toml.j2
+-rw-r--r--   0        0        0     4008 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/prometheus.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/py.typed
+-rw-r--r--   0        0        0     4845 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/scheduler.py
+-rw-r--r--   0        0        0     6041 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/sentry.py
+-rw-r--r--   0        0        0      199 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/sql/dipdup_head_status.sql
+-rw-r--r--   0        0        0     2111 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/sql/truncate_schema.sql
+-rw-r--r--   0        0        0      227 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/templates/callback.py.j2
+-rw-r--r--   0        0        0      157 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/templates/models.py.j2
+-rw-r--r--   0        0        0     3271 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/transactions.py
+-rw-r--r--   0        0        0     4631 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/utils/__init__.py
+-rw-r--r--   0        0        0     1824 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/utils/codegen.py
+-rw-r--r--   0        0        0    11504 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/utils/database.py
+-rw-r--r--   0        0        0     2044 2023-05-30 19:26:42.684780 dipdup-6.5.7/src/dipdup/utils/sys.py
+-rw-r--r--   0        0        0     4513 2023-05-30 19:26:42.688780 dipdup-6.5.7/src/dipdup/yaml.py
+-rw-r--r--   0        0        0     5895 1970-01-01 00:00:00.000000 dipdup-6.5.7/PKG-INFO
```

### Comparing `dipdup-6.5.6/LICENSE` & `dipdup-6.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/README.md` & `dipdup-6.5.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,11 +56,12 @@
 - [@Karantezsure](https://github.com/Karantezsure)
 - [@mystdeim](https://github.com/mystdeim)
 - [@nikos-kalomoiris](https://github.com/nikos-kalomoiris)
 - [@pravind](https://github.com/pravind)
 - [@sbihel](https://github.com/sbihel)
 - [@tezosmiami](https://github.com/tezosmiami)
 - [@tomsib2001](https://github.com/tomsib2001)
+- [@TristanAllaire](https://github.com/TristanAllaire)
 - [@veqtor](https://github.com/veqtor)
 - [@xflpt](https://github.com/xflpt)
 
 If we forgot to mention you, or you want to update your record, please, open an issue or pull request.
```

### Comparing `dipdup-6.5.6/pyproject.toml` & `dipdup-6.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dipdup"
 description = "Modular framework for creating selective indexers and featureful backends for dapps"
-version = "6.5.6"
+version = "6.5.7"
 license = "MIT"
 authors = [
     "Lev Gorodetskiy <dipdup@drsr.io>",
     "Michael Zaikin <mz@baking-bad.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/dipdup-io/dipdup"
@@ -27,16 +27,16 @@
     { include = "dipdup", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 
 asyncpg = "0.27.0"
-datamodel-code-generator = "0.18.1"
-pydantic = "1.10.7"
+datamodel-code-generator = "0.19.0"
+pydantic = "1.10.8"
 tortoise-orm = "0.19.3"
 
 aiohttp = "^3.8.1"
 aiolimiter = "^1.0.0"
 anyio = "^3.3.2"
 APScheduler = "^3.8.0"
 asyncclick = "^8.0.1"
@@ -60,15 +60,15 @@
 isort = "*"
 mypy = "*"
 pytest = "*"
 pytest-aiohttp = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-xdist = "*"
-Sphinx = "*"
+Sphinx = "^7.0.0"
 sphinx-click = "*"
 sphinx-markdown-builder = "*"
 types-pytz = "*"
 types-tabulate = "*"
 
 [tool.poetry.extras]
 pytezos = ["pytezos"]
```

### Comparing `dipdup-6.5.6/src/dipdup/baking_bad.py` & `dipdup-6.5.7/src/dipdup/baking_bad.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/cli.py` & `dipdup-6.5.7/src/dipdup/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -245,15 +245,20 @@
     from dipdup.utils.database import tortoise_wrapper
 
     config: DipDupConfig = ctx.obj.config
     url = config.database.connection_string
     models = f'{config.package}.models'
 
     table: list[tuple[str, str, str | int]] = [('name', 'status', 'level')]
-    async with tortoise_wrapper(url, models):
+    async with tortoise_wrapper(
+        url=url,
+        models=models,
+        timeout=config.database.connection_timeout,
+        decimal_precision=config.advanced.decimal_precision,
+    ):
         async for index in Index.filter().order_by('name'):
             row = (index.name, index.status.value, index.level)
             table.append(row)
 
     # NOTE: Lazy import to speed up startup
     from tabulate import tabulate
 
@@ -343,14 +348,15 @@
 
     async with AsyncExitStack() as stack:
         await stack.enter_async_context(
             tortoise_wrapper(
                 url=config.database.connection_string,
                 models=config.package,
                 timeout=config.database.connection_timeout,
+                decimal_precision=config.advanced.decimal_precision,
             )
         )
         await stack.enter_async_context(hasura_gateway)
 
         await hasura_gateway.configure(force)
 
 
@@ -374,15 +380,20 @@
 
     config: DipDupConfig = ctx.obj.config
     url = config.database.connection_string
     models = f'{config.package}.models'
 
     _logger.info('Approving schema `%s`', url)
 
-    async with tortoise_wrapper(url, models):
+    async with tortoise_wrapper(
+        url=url,
+        models=models,
+        timeout=config.database.connection_timeout,
+        decimal_precision=config.advanced.decimal_precision,
+    ):
         # TODO: Non-nullable fields, remove in 7.0
         await Schema.filter(name=config.schema_name).update(
             reindex=None,
             hash='',
         )
         await Index.filter().update(
             config_hash='',
@@ -425,15 +436,20 @@
             click.echo('Not in a TTY, skipping confirmation')
         except click.Abort:
             click.echo('\nAborted')
             quit(0)
 
     _logger.info('Wiping schema `%s`', url)
 
-    async with tortoise_wrapper(url, models):
+    async with tortoise_wrapper(
+        url=url,
+        models=models,
+        timeout=config.database.connection_timeout,
+        decimal_precision=config.advanced.decimal_precision,
+    ):
         conn = get_connection()
         if isinstance(config.database, PostgresDatabaseConfig):
             await wipe_schema(
                 conn=conn,
                 schema_name=config.database.schema_name,
                 # NOTE: Don't be confused by the name of `--immune` flag, we want to drop all tables if it's set.
                 immune_tables=config.database.immune_tables if not immune else set(),
@@ -496,15 +512,20 @@
     from dipdup.utils.database import tortoise_wrapper
 
     config: DipDupConfig = ctx.obj.config
     url = config.database.connection_string
     models = f'{config.package}.models'
     package_path = env.get_package_path(config.package)
 
-    async with tortoise_wrapper(url, models):
+    async with tortoise_wrapper(
+        url=url,
+        models=models,
+        timeout=config.database.connection_timeout,
+        decimal_precision=config.advanced.decimal_precision,
+    ):
         conn = get_connection()
         output = get_schema_sql(conn, False) + '\n'
         dipdup_sql_path = Path(__file__).parent / 'sql' / 'on_reindex'
         project_sql_path = package_path / 'sql' / 'on_reindex'
 
         for sql_path in (dipdup_sql_path, project_sql_path):
             for file in iter_files(sql_path):
```

### Comparing `dipdup-6.5.6/src/dipdup/codegen.py` & `dipdup-6.5.7/src/dipdup/codegen.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/config.py` & `dipdup-6.5.7/src/dipdup/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1469,25 +1469,29 @@
     :param postpone_jobs: Do not start job scheduler until all indexes are in realtime state
     :param early_realtime: Establish realtime connection immediately after startup
     :param merge_subscriptions: Subscribe to all operations instead of exact channels
     :param metadata_interface: Expose metadata interface for TzKT
     :param skip_version_check: Do not check for new DipDup versions on startup
     :param rollback_depth: A number of levels to keep for rollback
     :param crash_reporting: Enable crash reporting
+    :param decimal_precision: Adjust decimal context precision.
+    :param alt_operation_matcher: Use different algorithm to match operations (undocumented)
     """
 
     reindex: dict[ReindexingReason, ReindexingAction] = field(default_factory=dict)
     scheduler: dict[str, Any] | None = None
     postpone_jobs: bool = False
     early_realtime: bool = False
     merge_subscriptions: bool = False
     metadata_interface: bool = False
     skip_version_check: bool = False
     rollback_depth: int = 2
     crash_reporting: bool = False
+    decimal_precision: int | None = None
+    alt_operation_matcher: bool = False
 
 
 @dataclass
 class DipDupConfig:
     """Main indexer config
 
     :param spec_version: Version of config specification, currently always `1.2`
```

### Comparing `dipdup-6.5.6/src/dipdup/context.py` & `dipdup-6.5.7/src/dipdup/context.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/coinbase/datasource.py` & `dipdup-6.5.7/src/dipdup/datasources/coinbase/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/coinbase/models.py` & `dipdup-6.5.7/src/dipdup/datasources/coinbase/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/datasource.py` & `dipdup-6.5.7/src/dipdup/datasources/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/factory.py` & `dipdup-6.5.7/src/dipdup/datasources/factory.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/ipfs/datasource.py` & `dipdup-6.5.7/src/dipdup/datasources/ipfs/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/metadata/datasource.py` & `dipdup-6.5.7/src/dipdup/datasources/metadata/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/subscription.py` & `dipdup-6.5.7/src/dipdup/datasources/subscription.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/tzkt/datasource.py` & `dipdup-6.5.7/src/dipdup/datasources/tzkt/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/datasources/tzkt/models.py` & `dipdup-6.5.7/src/dipdup/datasources/tzkt/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/dipdup.py` & `dipdup-6.5.7/src/dipdup/dipdup.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             for name, index in copy(self._indexes).items():
                 if index.state.status == IndexStatus.ONESHOT:
                     del self._indexes[name]
                     continue
 
                 tasks.append(index.process())
 
-            indexes_processed = await gather(*tasks)
+            await gather(*tasks)
 
             indexes_spawned = False
             while pending_indexes:
                 index = pending_indexes.popleft()
                 self._indexes[index._config.name] = index
                 indexes_spawned = True
 
@@ -131,17 +131,14 @@
 
                 if not start_scheduler_event.is_set():
                     start_scheduler_event.set()
             else:
                 # NOTE: Fire `on_synchronized` hook when indexes will reach realtime state again
                 on_synchronized_fired = False
 
-            if not any(indexes_processed):
-                await self._ctx._transactions.cleanup()
-
             # TODO: Replace with asyncio.Event
             await asyncio.sleep(1)
 
     async def _update_metrics(self, update_interval: float) -> None:
         while True:
             await asyncio.sleep(update_interval)
 
@@ -450,14 +447,16 @@
             else:
                 start_scheduler_event = await self._set_up_scheduler(tasks)
                 spawn_datasources_event = await self._spawn_datasources(tasks)
 
                 if not advanced_config.postpone_jobs:
                     start_scheduler_event.set()
 
+                tasks.add(create_task(self._transactions.cleanup_loop()))
+
             spawn_index_tasks = (create_task(self._ctx._spawn_index(name)) for name in self._config.indexes)
             await gather(*spawn_index_tasks)
 
             await self._set_up_index_dispatcher(
                 tasks, spawn_datasources_event, start_scheduler_event, advanced_config.early_realtime
             )
 
@@ -523,14 +522,15 @@
 
     async def _set_up_database(self, stack: AsyncExitStack) -> None:
         await stack.enter_async_context(
             tortoise_wrapper(
                 url=self._config.database.connection_string,
                 models=self._config.package,
                 timeout=self._config.database.connection_timeout,
+                decimal_precision=self._config.advanced.decimal_precision,
             )
         )
 
     async def _set_up_hooks(self, tasks: set[Task[None]], run: bool = False) -> None:
         for event_hook_config in event_hooks.values():
             self._callbacks.register_hook(event_hook_config)
```

### Comparing `dipdup-6.5.6/src/dipdup/enums.py` & `dipdup-6.5.7/src/dipdup/enums.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/env.py` & `dipdup-6.5.7/src/dipdup/env.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/exceptions.py` & `dipdup-6.5.7/src/dipdup/exceptions.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/fetcher.py` & `dipdup-6.5.7/src/dipdup/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/hasura.py` & `dipdup-6.5.7/src/dipdup/hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/http.py` & `dipdup-6.5.7/src/dipdup/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 
 from dipdup import __version__
 from dipdup.config import ResolvedHTTPConfig
 from dipdup.exceptions import FrameworkException
 from dipdup.exceptions import InvalidRequestError
 from dipdup.prometheus import Metrics
 
-safe_exceptions = (
+exceptions_to_retry = (
     aiohttp.ClientConnectionError,
     aiohttp.ClientConnectorError,
     aiohttp.ClientResponseError,
     aiohttp.ClientPayloadError,
+    # NOTE: aiohttp doesn't reraise it
+    asyncio.TimeoutError,
 )
 
 
 class HTTPGateway(AbstractAsyncContextManager[None]):
     """Base class for datasources which connect to remote HTTP endpoints"""
 
     def __init__(self, url: str, http_config: ResolvedHTTPConfig) -> None:
@@ -145,15 +147,15 @@
             try:
                 return await self._request(
                     method=method,
                     url=url,
                     weight=weight,
                     **kwargs,
                 )
-            except safe_exceptions as e:
+            except exceptions_to_retry as e:
                 if self._config.retry_count and attempt - 1 == self._config.retry_count:
                     raise e
 
                 ratelimit_sleep: float | None = None
                 if isinstance(e, aiohttp.ClientResponseError):
                     if Metrics.enabled:
                         Metrics.set_http_error(self._url, e.status)
@@ -201,15 +203,15 @@
             headers=headers,
             raise_for_status=True,
             **kwargs,
         ) as response:
             if response.status == HTTPStatus.NO_CONTENT:
                 raise InvalidRequestError('204 No Content', request_string)
             with suppress(JSONDecodeError, aiohttp.ContentTypeError):
-                return await response.json()
+                return await response.json(loads=orjson.loads)
             return await response.read()
 
     async def _replay_request(
         self,
         method: str,
         url: str,
         weight: int = 1,
```

### Comparing `dipdup-6.5.6/src/dipdup/index.py` & `dipdup-6.5.7/src/dipdup/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/big_map/fetcher.py` & `dipdup-6.5.7/src/dipdup/indexes/big_map/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/big_map/index.py` & `dipdup-6.5.7/src/dipdup/indexes/big_map/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/big_map/matcher.py` & `dipdup-6.5.7/src/dipdup/indexes/big_map/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/event/fetcher.py` & `dipdup-6.5.7/src/dipdup/indexes/event/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/event/index.py` & `dipdup-6.5.7/src/dipdup/indexes/event/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/event/matcher.py` & `dipdup-6.5.7/src/dipdup/indexes/event/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/head/index.py` & `dipdup-6.5.7/src/dipdup/indexes/head/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/operation/fetcher.py` & `dipdup-6.5.7/src/dipdup/indexes/operation/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/operation/index.py` & `dipdup-6.5.7/src/dipdup/indexes/operation/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,21 +273,22 @@
             raise FrameworkException(f'Batch level is lower than index level: {batch_level} <= {index_level}')
 
         self._logger.debug('Processing %s operation subgroups of level %s', len(operation_subgroups), batch_level)
         matched_handlers: deque[MatchedOperationsT] = deque()
         for operation_subgroup in operation_subgroups:
             if isinstance(self._config, OperationUnfilteredIndexConfig):
                 subgroup_handlers = match_operation_unfiltered_subgroup(
-                    self._config,
-                    operation_subgroup,
+                    index=self._config,
+                    operation_subgroup=operation_subgroup,
                 )
             else:
                 subgroup_handlers = match_operation_subgroup(
-                    self._config.handlers,
-                    operation_subgroup,
+                    handlers=self._config.handlers,
+                    operation_subgroup=operation_subgroup,
+                    alt=self._ctx.config.advanced.alt_operation_matcher,
                 )
 
             if subgroup_handlers:
                 self._logger.info(
                     '%s: `%s` handler matched!',
                     operation_subgroup.hash,
                     subgroup_handlers[0][1].callback,
```

### Comparing `dipdup-6.5.6/src/dipdup/indexes/operation/matcher.py` & `dipdup-6.5.7/src/dipdup/indexes/operation/matcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -139,14 +139,15 @@
 
     return matched_handlers
 
 
 def match_operation_subgroup(
     handlers: Iterable[OperationHandlerConfig],
     operation_subgroup: OperationSubgroup,
+    alt: bool = False,
 ) -> deque[MatchedOperationsT]:
     """Try to match operation subgroup with all index handlers."""
     matched_handlers: deque[MatchedOperationsT] = deque()
     operations = operation_subgroup.operations
 
     for handler_config in handlers:
         subgroup_index = 0
@@ -189,8 +190,30 @@
 
         if len(matched_operations) >= sum(0 if x.optional else 1 for x in handler_config.pattern):
             _logger.info('%s: `%s` handler matched!', operation_subgroup.hash, handler_config.callback)
 
             args = prepare_operation_handler_args(handler_config, matched_operations)
             matched_handlers.append((operation_subgroup, handler_config, args))
 
-    return matched_handlers
+    if not (alt and len(matched_handlers) in (0, 1)):
+        return matched_handlers
+
+    # NOTE: Below is a secret algorithm for very special cases
+    index_list = list(range(len(matched_handlers)))
+    id_list = []
+    for handler in matched_handlers:
+        transaction = handler[2][-1]
+        if isinstance(transaction, OperationData):
+            id_list.append(transaction.id)
+        elif isinstance(transaction, Transaction):
+            id_list.append(transaction.data.id)
+        else:
+            raise FrameworkException('Type of the first handler argument is unknown')
+
+    sorted_index_list = [x for _, x in sorted(zip(id_list, index_list))]
+    if index_list == sorted_index_list:
+        return matched_handlers
+
+    sorted_matched_handlers: deque[MatchedOperationsT] = deque()
+    for index in sorted_index_list:
+        sorted_matched_handlers.append(matched_handlers[index])
+    return sorted_matched_handlers
```

### Comparing `dipdup-6.5.6/src/dipdup/indexes/token_transfer/fetcher.py` & `dipdup-6.5.7/src/dipdup/indexes/token_transfer/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/token_transfer/index.py` & `dipdup-6.5.7/src/dipdup/indexes/token_transfer/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/indexes/token_transfer/matcher.py` & `dipdup-6.5.7/src/dipdup/indexes/token_transfer/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/install.py` & `dipdup-6.5.7/src/dipdup/install.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/models.py` & `dipdup-6.5.7/src/dipdup/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,15 +480,19 @@
         for model in self.objects:
             if update := ModelUpdate.from_model(
                 cast(Model, model),
                 ModelUpdateAction.INSERT,
             ):
                 get_pending_updates().append(update)
 
-        return await super()._execute()
+        # NOTE: A bug; raises "You should first call .save()..." otherwise
+        models: list[MODEL] = await super()._execute()
+        for model in models:
+            model._saved_in_db = True
+        return models
 
 
 class QuerySet(TortoiseQuerySet):  # type: ignore[type-arg]
     def update(self, **kwargs: Any) -> UpdateQuery:
         return UpdateQuery(
             db=self._db,
             model=self.model,
```

### Comparing `dipdup-6.5.6/src/dipdup/project.py` & `dipdup-6.5.7/src/dipdup/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,16 +282,16 @@
             name='hasura_image',
             description=(
                 'Choose Hasura version\n'
                 'Test new releases before using in production; new versions may break compatibility.'
             ),
             default=0,
             choices=(
-                'hasura/graphql-engine:v2.23.0',
-                'hasura/graphql-engine:v2.23.0',
+                'hasura/graphql-engine:v2.25.1',
+                'hasura/graphql-engine:v2.25.1',
             ),
             comments=(
                 'stable',
                 'beta',
             ),
         ),
         NotifyQuestion(
```

### Comparing `dipdup-6.5.6/src/dipdup/projects/base/.gitignore.j2` & `dipdup-6.5.7/src/dipdup/projects/base/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/base/docker-compose.swarm.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/base/docker-compose.swarm.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/base/docker-compose.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/base/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_auction/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_auction/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_big_maps/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_big_maps/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dao/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dao/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_domains/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_domains/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_events/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_events/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_factories/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_factories/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_token/dipdup.yml.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_token/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2` & `dipdup-6.5.7/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/linters_default/Makefile.j2` & `dipdup-6.5.7/src/dipdup/projects/linters_default/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/linters_default/pyproject.toml.j2` & `dipdup-6.5.7/src/dipdup/projects/linters_default/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/linters_none/Makefile.j2` & `dipdup-6.5.7/src/dipdup/projects/linters_none/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/projects/linters_none/pyproject.toml.j2` & `dipdup-6.5.7/src/dipdup/projects/linters_none/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/prometheus.py` & `dipdup-6.5.7/src/dipdup/prometheus.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/scheduler.py` & `dipdup-6.5.7/src/dipdup/scheduler.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/sentry.py` & `dipdup-6.5.7/src/dipdup/sentry.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/sql/truncate_schema.sql` & `dipdup-6.5.7/src/dipdup/sql/truncate_schema.sql`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/transactions.py` & `dipdup-6.5.7/src/dipdup/transactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import asyncio
 from collections import deque
 from contextlib import asynccontextmanager
 from typing import AsyncIterator
 from typing import Optional
 from typing import Set
 
 from tortoise.transactions import in_transaction
 
 import dipdup.models
 from dipdup.utils.database import get_connection
 from dipdup.utils.database import set_connection
 
+CLEANUP_INTERVAL = 60
+
 
 class TransactionManager:
     """Manages versioned transactions"""
 
     def __init__(
         self,
         depth: int = 2,
@@ -77,7 +80,13 @@
         """Cleanup outdated model updates"""
         most_recent_index = await dipdup.models.Index.filter().order_by('-level').first()
         if not most_recent_index:
             return
 
         last_level = most_recent_index.level - self._depth
         await dipdup.models.ModelUpdate.filter(level__lt=last_level).delete()
+
+    async def cleanup_loop(self) -> None:
+        """Cleanup outdated model updates periodically"""
+        while True:
+            await self.cleanup()
+            await asyncio.sleep(CLEANUP_INTERVAL)
```

### Comparing `dipdup-6.5.6/src/dipdup/utils/__init__.py` & `dipdup-6.5.7/src/dipdup/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/utils/codegen.py` & `dipdup-6.5.7/src/dipdup/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/utils/database.py` & `dipdup-6.5.7/src/dipdup/utils/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,36 +5,33 @@
 import logging
 from contextlib import asynccontextmanager
 from contextlib import suppress
 from pathlib import Path
 from types import ModuleType
 from typing import Any
 from typing import AsyncIterator
-from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import Optional
 from typing import Set
 from typing import Type
-from typing import Union
 
 import sqlparse  # type: ignore[import]
 from asyncpg import CannotConnectNowError  # type: ignore[import]
 from tortoise import Tortoise
 from tortoise.backends.asyncpg.client import AsyncpgDBClient
 from tortoise.backends.base.client import BaseDBAsyncClient
 from tortoise.backends.base.executor import EXECUTOR_CACHE
 from tortoise.backends.sqlite.client import SqliteClient
 from tortoise.connection import connections
 from tortoise.fields import DecimalField
 from tortoise.fields.relational import ForeignKeyFieldInstance
 from tortoise.models import Model as TortoiseModel
 from tortoise.utils import get_schema_sql
 
-from dipdup.exceptions import DatabaseEngineError
 from dipdup.exceptions import InvalidModelsError
 from dipdup.utils import iter_files
 from dipdup.utils import pascal_to_snake
 
 _logger = logging.getLogger('dipdup.database')
 _truncate_schema_path = Path(__file__).parent.parent / 'sql' / 'truncate_schema.sql'
 
@@ -47,25 +44,32 @@
 
 
 def set_connection(conn: BaseDBAsyncClient) -> None:
     connections.set(DEFAULT_CONNECTION_NAME, conn)
 
 
 @asynccontextmanager
-async def tortoise_wrapper(url: str, models: Optional[str] = None, timeout: int = 60) -> AsyncIterator[None]:
+async def tortoise_wrapper(
+    url: str,
+    models: str | None = None,
+    timeout: int = 60,
+    decimal_precision: int | None = None,
+) -> AsyncIterator[None]:
     """Initialize Tortoise with internal and project models, close connections when done"""
-    model_modules: Dict[str, Iterable[Union[str, ModuleType]]] = {
+    model_modules: dict[str, Iterable[str | ModuleType]] = {
         'int_models': ['dipdup.models'],
     }
     if models:
         if not models.endswith('.models'):
             models += '.models'
         model_modules['models'] = [models]
 
     # NOTE: Must be called before entering Tortoise context
+    decimal_precision = decimal_precision or guess_decimal_precision(models)
+    set_decimal_precision(decimal_precision)
     prepare_models(models)
 
     try:
         for attempt in range(timeout):
             try:
                 await Tortoise.init(
                     db_url=url,
@@ -144,27 +148,16 @@
 
 async def execute_sql(
     conn: BaseDBAsyncClient,
     path: Path,
     *args: Any,
     **kwargs: Any,
 ) -> None:
-    # NOTE: Fail later, directory can be empty
-    supported = True if isinstance(conn, AsyncpgDBClient) else False
-
     for file in iter_files(path, ext='.sql'):
         _logger.info('Executing script `%s`', file.name)
-
-        if not supported:
-            raise DatabaseEngineError(
-                msg=f"Can't execute SQL script `{path}`: not supported",
-                kind='sqlite',
-                required='postgres',
-            )
-
         sql = file.read()
         # NOTE: Generally it's a very bad idea to format SQL scripts with arbitrary arguments.
         # NOTE: We trust package developers here.
         sql = sql.format(*args, **kwargs)
         for statement in sqlparse.split(sql):
             # NOTE: Ignore empty statements
             with suppress(AttributeError):
@@ -172,27 +165,16 @@
 
 
 async def execute_sql_query(
     conn: BaseDBAsyncClient,
     path: Path,
     *values: Any,
 ) -> Any:
-    # NOTE: Fail later, directory can be empty
-    supported = True if isinstance(conn, AsyncpgDBClient) else False
-
     for file in iter_files(path, ext='.sql'):
         _logger.info('Executing query `%s`', file.name)
-
-        if not supported:
-            raise DatabaseEngineError(
-                msg=f"Can't execute SQL query `{path}`: not supported",
-                kind='sqlite',
-                required='postgres',
-            )
-
         sql = file.read()
         return await conn.execute_query(sql, list(values))
 
 
 async def generate_schema(
     conn: BaseDBAsyncClient,
     name: str,
@@ -255,31 +237,29 @@
     """Move table from one schema to another"""
     if isinstance(conn, SqliteClient):
         raise NotImplementedError
 
     await conn.execute_script(f'ALTER TABLE {schema}.{name} SET SCHEMA {new_schema}')
 
 
-def prepare_models(package: Optional[str]) -> None:
+def prepare_models(package: str | None) -> None:
     """Prepare TortoiseORM models to use with DipDup.
     Generate missing table names, validate models, increase decimal precision if needed.
     """
     # NOTE: Circular imports
     import dipdup.models
 
     # NOTE: Required for pytest-xdist. Models with the same name in different packages cause conflicts otherwise.
     EXECUTOR_CACHE.clear()
 
-    db_tables: Set[str] = set()
-    decimal_context = decimal.getcontext()
-    prec = decimal_context.prec
+    db_tables: set[str] = set()
 
     for app, model in iter_models(package):
         # NOTE: Enforce our class for user models
-        if app == 'models' and not issubclass(model, dipdup.models.Model):
+        if app != 'int_models' and not issubclass(model, dipdup.models.Model):
             raise InvalidModelsError(
                 'Project models must be subclassed from `dipdup.models.Model`.'
                 '\n\n'
                 'Replace `from tortoise import Model` import with `from dipdup.models import Model`.',
                 model,
             )
 
@@ -325,19 +305,33 @@
             if isinstance(field, ForeignKeyFieldInstance) and field.related_name == table_name:
                 raise InvalidModelsError(
                     'Model field names must differ from table name.',
                     model,
                     f'related_name={field.related_name}',
                 )
 
-            # NOTE: Increase decimal precision if needed
-            if isinstance(field, DecimalField):
-                prec = max(prec, field.max_digits)
-
-    # NOTE: Set new decimal precision
-    if decimal_context.prec < prec:
-        _logger.warning('Decimal context precision has been updated: %s -> %s', decimal_context.prec, prec)
-        decimal_context.prec = prec
-
-        # NOTE: DefaultContext is used for new threads
-        decimal.DefaultContext.prec = prec
-        decimal.setcontext(decimal_context)
+
+def guess_decimal_precision(package: str | None) -> int:
+    """Guess decimal precision from project models.
+
+    Doesn't work for realy big numbers.
+    """
+    prec = 0
+    for _, model in iter_models(package):
+        for field in model._meta.fields_map.values():
+            if not isinstance(field, DecimalField):
+                continue
+            prec = max(prec, field.max_digits)
+    return prec
+
+
+def set_decimal_precision(prec: int) -> None:
+    """Set decimal precision for the current and all future threads"""
+    decimal_context = decimal.getcontext()
+    if prec <= decimal_context.prec:
+        return
+
+    _logger.warning('Decimal context precision has been updated: %s -> %s', decimal_context.prec, prec)
+    decimal_context.prec = prec
+    # NOTE: DefaultContext is used for new threads
+    decimal.DefaultContext.prec = prec
+    decimal.setcontext(decimal_context)
```

### Comparing `dipdup-6.5.6/src/dipdup/utils/sys.py` & `dipdup-6.5.7/src/dipdup/utils/sys.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/src/dipdup/yaml.py` & `dipdup-6.5.7/src/dipdup/yaml.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.6/PKG-INFO` & `dipdup-6.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipdup
-Version: 6.5.6
+Version: 6.5.7
 Summary: Modular framework for creating selective indexers and featureful backends for dapps
 Home-page: https://dipdup.io/
 License: MIT
 Keywords: tezos,blockchain,sdk,michelson,indexers,tzkt,cryptocurrencies,smart-contracts
 Author: Lev Gorodetskiy
 Author-email: dipdup@drsr.io
 Requires-Python: >=3.10,<3.11
@@ -23,18 +23,18 @@
 Provides-Extra: pytezos
 Requires-Dist: APScheduler (>=3.8.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: aiolimiter (>=1.0.0,<2.0.0)
 Requires-Dist: anyio (>=3.3.2,<4.0.0)
 Requires-Dist: asyncclick (>=8.0.1,<9.0.0)
 Requires-Dist: asyncpg (==0.27.0)
-Requires-Dist: datamodel-code-generator (==0.18.1)
+Requires-Dist: datamodel-code-generator (==0.19.0)
 Requires-Dist: orjson (>=3.6.6,<4.0.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
-Requires-Dist: pydantic (==1.10.7)
+Requires-Dist: pydantic (==1.10.8)
 Requires-Dist: pyhumps (>=3.0.2,<4.0.0)
 Requires-Dist: pysignalr (==0.2.0)
 Requires-Dist: pytezos (==3.9.0) ; extra == "pytezos"
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: ruamel.yaml (>=0.17.2,<0.18.0)
 Requires-Dist: sentry-sdk (>=1.4.3,<2.0.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
@@ -101,12 +101,13 @@
 - [@Karantezsure](https://github.com/Karantezsure)
 - [@mystdeim](https://github.com/mystdeim)
 - [@nikos-kalomoiris](https://github.com/nikos-kalomoiris)
 - [@pravind](https://github.com/pravind)
 - [@sbihel](https://github.com/sbihel)
 - [@tezosmiami](https://github.com/tezosmiami)
 - [@tomsib2001](https://github.com/tomsib2001)
+- [@TristanAllaire](https://github.com/TristanAllaire)
 - [@veqtor](https://github.com/veqtor)
 - [@xflpt](https://github.com/xflpt)
 
 If we forgot to mention you, or you want to update your record, please, open an issue or pull request.
```

