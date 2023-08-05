# Comparing `tmp/ast_grep_cli-0.9.2.tar.gz` & `tmp/ast_grep_cli-0.9.3.tar.gz`

## Comparing `ast_grep_cli-0.9.2.tar` & `ast_grep_cli-0.9.3.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/Cargo.toml
--rw-r--r--   0     1001      123     2331 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/language.rs
--rw-r--r--   0     1001      123     3858 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/lib.rs
--rw-r--r--   0     1001      123    15133 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/match_tree.rs
--rw-r--r--   0     1001      123     3480 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/kind.rs
--rw-r--r--   0     1001      123     3783 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/node_match.rs
--rw-r--r--   0     1001      123    11138 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/pattern.rs
--rw-r--r--   0     1001      123      982 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/text.rs
--rw-r--r--   0     1001      123     6540 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher.rs
--rw-r--r--   0     1001      123    11359 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/meta_var.rs
--rw-r--r--   0     1001      123    15558 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/node.rs
--rw-r--r--   0     1001      123    16351 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/ops.rs
--rw-r--r--   0     1001      123     3089 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/pinned.rs
--rw-r--r--   0     1001      123    10936 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/indent.rs
--rw-r--r--   0     1001      123     6181 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/structural.rs
--rw-r--r--   0     1001      123     9380 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/template.rs
--rw-r--r--   0     1001      123     2572 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer.rs
--rw-r--r--   0     1001      123     8489 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/source.rs
--rw-r--r--   0     1001      123    16414 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/traversal.rs
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-dynamic/Cargo.toml
--rw-r--r--   0     1001      123     7940 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-dynamic/src/lib.rs
--rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/Cargo.toml
--rw-r--r--   0     1001      123     1023 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/cpp.rs
--rw-r--r--   0     1001      123      858 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/csharp.rs
--rw-r--r--   0     1001      123      815 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/css.rs
--rw-r--r--   0     1001      123     1192 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/go.rs
--rw-r--r--   0     1001      123     1013 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/json.rs
--rw-r--r--   0     1001      123     1216 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/kotlin.rs
--rw-r--r--   0     1001      123    12868 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/lib.rs
--rw-r--r--   0     1001      123      924 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/lua.rs
--rw-r--r--   0     1001      123     3198 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/parsers.rs
--rw-r--r--   0     1001      123     2043 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/python.rs
--rw-r--r--   0     1001      123     1974 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/rust.rs
--rw-r--r--   0     1001      123     1646 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/scala.rs
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-lsp/Cargo.toml
--rw-r--r--   0     1001      123    11369 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-lsp/src/lib.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/Cargo.toml
--rw-r--r--   0     1001      123     6946 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/constraints.rs
--rw-r--r--   0     1001      123     6838 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/deserialize_env.rs
--rw-r--r--   0     1001      123     4880 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/lib.rs
--rw-r--r--   0     1001      123     2765 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/maybe.rs
--rw-r--r--   0     1001      123     6514 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/referent_rule.rs
--rw-r--r--   0     1001      123    16160 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
--rw-r--r--   0     1001      123     4138 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
--rw-r--r--   0     1001      123    13151 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule.rs
--rw-r--r--   0     1001      123     6357 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule_collection.rs
--rw-r--r--   0     1001      123    11610 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule_config.rs
--rw-r--r--   0     1001      123     6716 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/transform.rs
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/crates/cli/Cargo.toml
--rw-r--r--   0     1001      123      249 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/bin/ast-grep.rs
--rw-r--r--   0     1001      123    11003 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/config.rs
--rw-r--r--   0     1001      123    10194 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/error.rs
--rw-r--r--   0     1001      123     4312 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/lang.rs
--rw-r--r--   0     1001      123     5585 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/lib.rs
--rw-r--r--   0     1001      123     1015 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/lsp.rs
--rw-r--r--   0     1001      123       94 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/main.rs
--rw-r--r--   0     1001      123    10212 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/new.rs
--rw-r--r--   0     1001      123     4861 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/cloud_print.rs
--rw-r--r--   0     1001      123    23920 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/colored_print.rs
--rw-r--r--   0     1001      123     7648 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/interactive_print.rs
--rw-r--r--   0     1001      123     9327 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/json_print.rs
--rw-r--r--   0     1001      123     3243 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/print/mod.rs
--rw-r--r--   0     1001      123     9061 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/run.rs
--rw-r--r--   0     1001      123    10914 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/scan.rs
--rw-r--r--   0     1001      123     7418 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/utils.rs
--rw-r--r--   0     1001      123    24703 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/src/verify.rs
--rw-r--r--   0     1001      123      593 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/tests/common/mod.rs
--rw-r--r--   0     1001      123      901 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/tests/run_test.rs
--rw-r--r--   0     1001      123     1364 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/tests/scan_test.rs
--rw-r--r--   0     1001      123     1027 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/tests/verify_test.rs
--rw-r--r--   0     1001      123     1236 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/pyproject.toml
--rw-r--r--   0     1001      123    60094 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/crates/cli/Cargo.lock
--rw-r--r--   0     1001      123     4951 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/README.md
--rw-r--r--   0     1001      123     1077 2023-07-22 20:26:49.000000 ast_grep_cli-0.9.2/LICENSE
--rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/Cargo.toml
+-rw-r--r--   0     1001      123     2331 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/language.rs
+-rw-r--r--   0     1001      123     3904 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/lib.rs
+-rw-r--r--   0     1001      123    15133 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/match_tree.rs
+-rw-r--r--   0     1001      123     3480 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher/kind.rs
+-rw-r--r--   0     1001      123     3783 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      123    11138 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      123      982 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher/text.rs
+-rw-r--r--   0     1001      123     6540 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher.rs
+-rw-r--r--   0     1001      123    11359 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/meta_var.rs
+-rw-r--r--   0     1001      123    16565 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/node.rs
+-rw-r--r--   0     1001      123    16351 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/ops.rs
+-rw-r--r--   0     1001      123     3089 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/pinned.rs
+-rw-r--r--   0     1001      123    10938 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/replacer/indent.rs
+-rw-r--r--   0     1001      123     6181 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/replacer/structural.rs
+-rw-r--r--   0     1001      123     9380 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/replacer/template.rs
+-rw-r--r--   0     1001      123     2572 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/replacer.rs
+-rw-r--r--   0     1001      123     8489 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/source.rs
+-rw-r--r--   0     1001      123    16414 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/traversal.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/Cargo.toml
+-rw-r--r--   0     1001      123     6946 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/constraints.rs
+-rw-r--r--   0     1001      123     6838 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/deserialize_env.rs
+-rw-r--r--   0     1001      123     4880 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/lib.rs
+-rw-r--r--   0     1001      123     2765 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/maybe.rs
+-rw-r--r--   0     1001      123     6514 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/referent_rule.rs
+-rw-r--r--   0     1001      123    16160 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
+-rw-r--r--   0     1001      123     4138 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
+-rw-r--r--   0     1001      123    13151 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/rule.rs
+-rw-r--r--   0     1001      123     6357 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/rule_collection.rs
+-rw-r--r--   0     1001      123    11610 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/rule_config.rs
+-rw-r--r--   0     1001      123     6716 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/transform.rs
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/Cargo.toml
+-rw-r--r--   0     1001      123     1023 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/cpp.rs
+-rw-r--r--   0     1001      123      858 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/csharp.rs
+-rw-r--r--   0     1001      123      815 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/css.rs
+-rw-r--r--   0     1001      123     1192 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/go.rs
+-rw-r--r--   0     1001      123     1013 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/json.rs
+-rw-r--r--   0     1001      123     1216 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/kotlin.rs
+-rw-r--r--   0     1001      123    12868 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/lib.rs
+-rw-r--r--   0     1001      123      924 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/lua.rs
+-rw-r--r--   0     1001      123     3198 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/parsers.rs
+-rw-r--r--   0     1001      123     2043 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/python.rs
+-rw-r--r--   0     1001      123     1974 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/rust.rs
+-rw-r--r--   0     1001      123     1646 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/scala.rs
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-lsp/Cargo.toml
+-rw-r--r--   0     1001      123    11369 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-lsp/src/lib.rs
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-dynamic/Cargo.toml
+-rw-r--r--   0     1001      123     7940 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/local_dependencies/ast-grep-dynamic/src/lib.rs
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.3/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      123      249 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/bin/ast-grep.rs
+-rw-r--r--   0     1001      123    10915 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/config.rs
+-rw-r--r--   0     1001      123    10194 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/error.rs
+-rw-r--r--   0     1001      123     4312 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/lang.rs
+-rw-r--r--   0     1001      123     5585 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      123     1015 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/lsp.rs
+-rw-r--r--   0     1001      123       94 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/main.rs
+-rw-r--r--   0     1001      123    10721 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/new.rs
+-rw-r--r--   0     1001      123     4839 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/print/cloud_print.rs
+-rw-r--r--   0     1001      123     8195 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/print/colored_print/test.rs
+-rw-r--r--   0     1001      123    19937 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/print/colored_print.rs
+-rw-r--r--   0     1001      123     7626 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/print/interactive_print.rs
+-rw-r--r--   0     1001      123    12839 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/print/json_print.rs
+-rw-r--r--   0     1001      123     3243 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/print/mod.rs
+-rw-r--r--   0     1001      123     9751 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/run.rs
+-rw-r--r--   0     1001      123    10914 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/scan.rs
+-rw-r--r--   0     1001      123     7418 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/utils.rs
+-rw-r--r--   0     1001      123    24703 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/src/verify.rs
+-rw-r--r--   0     1001      123      593 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/tests/common/mod.rs
+-rw-r--r--   0     1001      123      901 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/tests/run_test.rs
+-rw-r--r--   0     1001      123     1364 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/tests/scan_test.rs
+-rw-r--r--   0     1001      123     1027 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/tests/verify_test.rs
+-rw-r--r--   0     1001      123     1236 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/pyproject.toml
+-rw-r--r--   0     1001      123    60094 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/crates/cli/Cargo.lock
+-rw-r--r--   0     1001      123     4951 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/README.md
+-rw-r--r--   0     1001      123     1077 2023-07-27 17:12:42.000000 ast_grep_cli-0.9.3/LICENSE
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.9.3/PKG-INFO
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/Cargo.toml` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 edition= "2021"
 homepage= "https://ast-grep.github.io/"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.2"
+version= "0.9.3"
 
 [dependencies]
 bit-set= { version = "0.5.3" }
 regex = { version = "1.9.1" , optional = true }
 thiserror= "1.0.44"
 tree-sitter= { version = "0.9.2", package = "tree-sitter-facade-sg" }
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/language.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/lib.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 mod node;
 
 pub use language::Language;
 pub use matcher::{Matcher, NodeMatch, Pattern, PatternError};
 pub use node::Node;
 pub use source::{Doc, StrDoc};
 
+#[doc(hidden)]
+pub use node::DisplayContext;
+
 use replacer::Replacer;
 
 use node::Root;
 use source::{Edit, TSParseError};
 
 #[derive(Clone)]
 pub struct AstGrep<D: Doc> {
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/match_tree.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/kind.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/node_match.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/pattern.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher/text.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/matcher.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/meta_var.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/node.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/node.rs`

 * *Files 4% similar despite different names*

```diff
@@ -185,46 +185,54 @@
     self.root.lang()
   }
 }
 
 // TODO: figure out how to do this
 impl<'r, L: Language> Node<'r, StrDoc<L>> {
   #[doc(hidden)]
-  pub fn display_context(&self, context_lines: usize) -> DisplayContext<'r> {
-    let bytes = self.root.doc.get_source().as_bytes();
+  pub fn display_context(&self, before: usize, after: usize) -> DisplayContext<'r> {
+    let source = self.root.doc.get_source().as_str();
+    let bytes = source.as_bytes();
     let start = self.inner.start_byte() as usize;
     let end = self.inner.end_byte() as usize;
     let (mut leading, mut trailing) = (start, end);
-    let mut lines_before = context_lines + 1;
+    let mut lines_before = before + 1;
     while leading > 0 {
       if bytes[leading - 1] == b'\n' {
         lines_before -= 1;
         if lines_before == 0 {
           break;
         }
       }
       leading -= 1;
     }
+    let mut lines_after = after + 1;
     // tree-sitter will append line ending to source so trailing can be out of bound
-    trailing = trailing.min(bytes.len() - 1);
-    let mut lines_after = context_lines + 1;
-    while trailing < bytes.len() - 1 {
-      if bytes[trailing] == b'\n' || bytes[trailing + 1] == b'\n' {
+    trailing = trailing.min(bytes.len());
+    while trailing < bytes.len() {
+      if bytes[trailing] == b'\n' {
         lines_after -= 1;
         if lines_after == 0 {
           break;
         }
       }
       trailing += 1;
     }
+    // lines_before means we matched all context, offset is `before` itself
+    let offset = if lines_before == 0 {
+      before
+    } else {
+      // otherwise, there are fewer than `before` line in src, compute the actual line
+      before + 1 - lines_before
+    };
     DisplayContext {
       matched: self.text(),
-      leading: &self.root.doc.get_source().as_str()[leading..start],
-      trailing: &self.root.doc.get_source().as_str()[end..=trailing],
-      start_line: self.inner.start_position().row() as usize + 1,
+      leading: &source[leading..start],
+      trailing: &source[end..trailing],
+      start_line: self.start_pos().0 - offset,
     }
   }
 
   pub fn root(&self) -> &Root<StrDoc<L>> {
     self.root
   }
 }
@@ -250,23 +258,22 @@
   }
 
   pub fn follows<M: Matcher<D::Lang>>(&self, m: M) -> bool {
     self.prev_all().find_map(|n| m.match_node(n)).is_some()
   }
 }
 
-#[doc(hidden)]
 pub struct DisplayContext<'r> {
   /// content for the matched node
   pub matched: Cow<'r, str>,
   /// content before the matched node
   pub leading: &'r str,
   /// content after the matched node
   pub trailing: &'r str,
-  /// start line of the matched node
+  /// zero-based start line of the context
   pub start_line: usize,
 }
 
 /// tree traversal API
 impl<'r, D: Doc> Node<'r, D> {
   #[must_use]
   pub fn parent(&self) -> Option<Self> {
@@ -512,22 +519,54 @@
     let texts: Vec<_> = children[0]
       .children()
       .map(|c| c.text().to_string())
       .collect();
     assert_eq!(texts, vec!["let", "a = 123"]);
   }
 
+  const MULTI_LINE: &str = "
+if (a) {
+  test(1)
+} else {
+  x
+}
+";
+
   #[test]
   fn test_display_context() {
+    // src, matcher, lead, trail
+    let cases = [
+      ["i()", "i()", "", ""],
+      ["i()", "i", "", "()"],
+      [MULTI_LINE, "test", "  ", "(1)"],
+    ];
     // display context should not panic
-    let s = "i()";
-    assert_eq!(s.len(), 3);
-    let root = Tsx.ast_grep(s);
-    let node = root.root();
-    assert_eq!(node.display_context(0).trailing.len(), 0);
+    for [src, matcher, lead, trail] in cases {
+      let root = Tsx.ast_grep(src);
+      let node = root.root().find(matcher).expect("should match");
+      let display = node.display_context(0, 0);
+      assert_eq!(display.leading, lead);
+      assert_eq!(display.trailing, trail);
+    }
+  }
+
+  #[test]
+  fn test_multi_line_context() {
+    let cases = [
+      ["i()", "i()", "", ""],
+      [MULTI_LINE, "test", "if (a) {\n  ", "(1)\n} else {"],
+    ];
+    // display context should not panic
+    for [src, matcher, lead, trail] in cases {
+      let root = Tsx.ast_grep(src);
+      let node = root.root().find(matcher).expect("should match");
+      let display = node.display_context(1, 1);
+      assert_eq!(display.leading, lead);
+      assert_eq!(display.trailing, trail);
+    }
   }
 
   #[test]
   fn test_replace_all_nested() {
     let root = Tsx.ast_grep("Some(Some(1))");
     let node = root.root();
     let edits = node.replace_all("Some($A)", "$A");
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/ops.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/pinned.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/indent.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/replacer/indent.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 use std::borrow::Cow;
 use std::cmp::Ordering;
 use std::ops::Range;
 
 /**
   This module is for indentation-sensitive replacement.
 
-  Ideally, structral search and replacement should all be based on AST.
-  But this means our changed AST need to be pretty-printed by structral rules,
+  Ideally, structural search and replacement should all be based on AST.
+  But this means our changed AST need to be pretty-printed by structural rules,
   which we don't have enough resource to support. An indentation solution is used.
 
   The algorithm is quite complicated, uncomprehensive, sluggish and buggy.
   But let's walk through it by example.
 
   consider this code
   ```ignore
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/structural.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer/template.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/replacer.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/source.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-core/src/traversal.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-dynamic/Cargo.toml` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-dynamic/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.2"
+version= "0.9.3"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 libloading = "0.8"
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-dynamic/src/lib.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-dynamic/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/Cargo.toml` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.2"
+version= "0.9.3"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 serde= { version = "1.0", features = ["derive"] }
 
@@ -24,15 +24,15 @@
 tree-sitter-go = { version = "0.19.1", optional = true }
 tree-sitter-html = { version = "0.19.0", optional = true }
 tree-sitter-java = { version = "0.20.0", optional = true }
 tree-sitter-javascript = { version = "0.20.0", optional = true }
 tree-sitter-json = { version = "0.19.0", optional = true }
 tree-sitter-kotlin = { version = "0.2.11", optional = true }
 tree-sitter-lua = { version = "0.0.18", optional = true }
-tree-sitter-python = { version = "0.20.2", optional = true }
+tree-sitter-python = { version = "0.20.3", optional = true }
 tree-sitter-ruby = { version = "0.20.0", optional = true }
 tree-sitter-rust = { version = "0.20.3", optional = true }
 tree-sitter-scala = { version = "0.20.1", optional = true }
 tree-sitter-swift = { version = "0.3.6", optional = true }
 tree-sitter-thrift = { version = "0.5.0", optional = true }
 tree-sitter-typescript= { version = "0.20.2", optional = true }
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/cpp.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/csharp.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/css.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/go.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/json.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/json.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/kotlin.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/lib.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/lua.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/lua.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/parsers.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/python.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/rust.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-language/src/scala.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-lsp/Cargo.toml` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-lsp/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "ast-grep-lsp"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
-version= "0.9.2"
+version= "0.9.3"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [dependencies]
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-lsp/src/lib.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-lsp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/Cargo.toml` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.9.2"
+version= "0.9.3"
 
 [features]
 default = ["regex"]
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
```

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/constraints.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/deserialize_env.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/lib.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/maybe.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/referent_rule.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/relational_rule/mod.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/relational_rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule_collection.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/rule_config.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/local_dependencies/ast-grep-config/src/transform.rs` & `ast_grep_cli-0.9.3/local_dependencies/ast-grep-config/src/transform.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/Cargo.toml` & `ast_grep_cli-0.9.3/crates/cli/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 categories = ["command-line-utilities", "development-tools", "parsing"]
 default-run = "sg"
 # use relative path because maturin does not recognize
 readme = "../../README.md"
 license-file = "../../LICENSE"
 
-version= "0.9.2"
+version= "0.9.3"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 # license.workspace = true
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 homepage= "https://ast-grep.github.io/"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/config.rs` & `ast_grep_cli-0.9.3/crates/cli/src/config.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,15 @@
   #[serde(skip_serializing_if = "Option::is_none")]
   pub test_configs: Option<Vec<TestConfig>>,
   /// util rules directories
   #[serde(skip_serializing_if = "Option::is_none")]
   pub util_dirs: Option<Vec<PathBuf>>,
   /// configuration for custom languages
   #[serde(skip_serializing_if = "Option::is_none")]
-  pub custom_languages: Option<HashMap<String, CustomLang>>, // /// overriding config for rules
-                                                             // #[serde(skip_serializing_if="Option::is_none")]
-                                                             // pub rules: Option<Vec<()>>,
+  pub custom_languages: Option<HashMap<String, CustomLang>>,
 }
 
 pub fn find_rules(config_path: Option<PathBuf>) -> Result<RuleCollection<SgLang>> {
   let config_path =
     find_config_path_with_default(config_path, None).context(EC::ReadConfiguration)?;
   let config_str = read_to_string(&config_path).context(EC::ReadConfiguration)?;
   let sg_config: AstGrepConfig = from_str(&config_str).context(EC::ParseConfiguration)?;
@@ -225,22 +223,25 @@
   Ok(TestHarness {
     test_cases,
     snapshots,
     path_map,
   })
 }
 
+/// Returns the base_directory where config is and config object.
 pub fn read_config_from_dir<P: AsRef<Path>>(path: P) -> Result<Option<(PathBuf, AstGrepConfig)>> {
-  let config_path =
+  let mut config_path =
     find_config_path_with_default(None, Some(path.as_ref())).context(EC::ReadConfiguration)?;
   if !config_path.is_file() {
     return Ok(None);
   }
   let config_str = read_to_string(&config_path).context(EC::ReadConfiguration)?;
   let sg_config = from_str(&config_str).context(EC::ParseConfiguration)?;
+  // remove sgconfig.yml from the path
+  config_path.pop(); // ./sg_config -> ./
   Ok(Some((config_path, sg_config)))
 }
 
 const CONFIG_FILE: &str = "sgconfig.yml";
 const SNAPSHOT_DIR: &str = "__snapshots__";
 
 fn find_config_path_with_default(
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/error.rs` & `ast_grep_cli-0.9.3/crates/cli/src/error.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/lang.rs` & `ast_grep_cli-0.9.3/crates/cli/src/lang.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/lib.rs` & `ast_grep_cli-0.9.3/crates/cli/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/lsp.rs` & `ast_grep_cli-0.9.3/crates/cli/src/lsp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/new.rs` & `ast_grep_cli-0.9.3/crates/cli/src/new.rs`

 * *Files 6% similar despite different names*

```diff
@@ -61,19 +61,18 @@
       )
       .prompt()?;
       Ok(entity)
     }
   }
 
   fn choose_language(&self) -> Result<SgLang> {
-    if self.yes {
-      self
-        .lang
-        .map(Ok)
-        .unwrap_or_else(|| Err(anyhow::anyhow!(EC::InsufficientCLIArgument("lang"))))
+    if let Some(lang) = self.lang {
+      Ok(lang)
+    } else if self.yes {
+      Err(anyhow::anyhow!(EC::InsufficientCLIArgument("lang")))
     } else {
       Ok(inquire::Select::new("Choose rule's language", SgLang::all_langs()).prompt()?)
     }
   }
 
   fn ask_name(&self, entity: &'static str) -> Result<String> {
     if let Some(name) = &self.name {
@@ -115,20 +114,20 @@
   if let Some(entity) = arg.entity.take() {
     run_create_entity(entity, arg)
   } else {
     ask_entity_type(arg)
   }
 }
 
+// base_dir, config
 type FoundConfig = (PathBuf, AstGrepConfig);
 
 fn run_create_entity(entity: Entity, arg: NewArg) -> Result<()> {
   // check if we are under a project dir
-  if let Some(mut found) = read_config_from_dir(&arg.base_dir)? {
-    found.0.pop(); // remove sgconfig.yml from the path
+  if let Some(found) = read_config_from_dir(&arg.base_dir)? {
     return do_create_entity(entity, found, arg);
   }
   // check if we creating a project
   if entity == Entity::Project {
     create_new_project(arg)
   } else {
     // if not, return error
@@ -144,18 +143,18 @@
     Entity::Util => create_new_util(found, arg),
     Entity::Project => Err(anyhow::anyhow!(EC::ProjectAlreadyExist)),
   }
 }
 
 fn ask_entity_type(arg: NewArg) -> Result<()> {
   // 1. check if we are under a sgconfig.yml
-  if let Some(sg_config) = read_config_from_dir(&arg.base_dir)? {
+  if let Some(found) = read_config_from_dir(&arg.base_dir)? {
     // 2. ask users what to create if yes
     let entity = arg.ask_entity_type()?;
-    do_create_entity(entity, sg_config, arg)
+    do_create_entity(entity, found, arg)
   } else {
     // 3. ask users to provide project info if no sgconfig found
     print!("No sgconfig.yml found. ");
     create_new_project(arg)
   }
 }
 
@@ -188,26 +187,25 @@
   Ok(())
 }
 
 fn default_rule(id: &str, lang: SgLang) -> String {
   format!(
     r#"id: {id}
 message: Add your rule message here....
-severity: error # error, warning, hint, info
+severity: error # error, warning, info, hint
 language: {lang}
 rule:
   pattern: Your Rule Pattern here...
 # utils: Extract repeated rule as local utility here.
 # note: Add detailed explanation for the rule."#
   )
 }
 
 fn create_new_rule(found: FoundConfig, arg: NewArg) -> Result<()> {
-  let base_dir = found.0;
-  let sg_config = found.1;
+  let (base_dir, sg_config) = found;
   let name = arg.ask_name("rule")?;
   let rule_dir = if sg_config.rule_dirs.len() > 1 {
     let dirs = sg_config.rule_dirs.iter().map(|p| p.display()).collect();
     let display =
       inquire::Select::new("Which rule dir do you want to save your rule?", dirs).prompt()?;
     base_dir.join(display.to_string())
   } else {
@@ -275,16 +273,15 @@
 rule:
   pattern: Your Rule Pattern here...
 # utils: Extract repeated rule as local utility here."#
   )
 }
 
 fn create_new_util(found: FoundConfig, arg: NewArg) -> Result<()> {
-  let base_dir = found.0;
-  let sg_config = found.1;
+  let (base_dir, sg_config) = found;
   let Some(utils) = sg_config.util_dirs else {
     return Err(anyhow::anyhow!(EC::NoUtilDirConfigured));
   };
   if utils.is_empty() {
     return Err(anyhow::anyhow!(EC::NoUtilDirConfigured));
   }
   let util_dir = if utils.len() > 1 {
@@ -335,16 +332,38 @@
       base_dir: temp.to_path_buf(),
     };
     run_create_new(arg).unwrap();
     assert!(temp.join("rules/test-rule.yml").exists());
     Ok(())
   }
 
+  fn create_util(temp: &Path) -> Result<()> {
+    let arg = NewArg {
+      entity: Some(Entity::Util),
+      name: Some("test-utils".into()),
+      lang: Some(SupportLang::Rust.into()),
+      yes: true,
+      base_dir: temp.to_path_buf(),
+    };
+    run_create_new(arg).unwrap();
+    assert!(temp.join("utils/test-utils.yml").exists());
+    Ok(())
+  }
+
   #[test]
   fn test_create_new() -> Result<()> {
     let dir = TempDir::new("sgtest")?;
     create_project(dir.path())?;
     create_rule(dir.path())?;
     drop(dir); // drop at the end since temp dir clean up is done in Drop
     Ok(())
   }
+
+  #[test]
+  fn test_create_util() -> Result<()> {
+    let dir = TempDir::new("sgtest")?;
+    create_project(dir.path())?;
+    create_util(dir.path())?;
+    drop(dir); // drop at the end since temp dir clean up is done in Drop
+    Ok(())
+  }
 }
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/print/cloud_print.rs` & `ast_grep_cli-0.9.3/crates/cli/src/print/cloud_print.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use super::{Diff, Printer};
 use crate::lang::SgLang;
 use ast_grep_config::{RuleConfig, Severity};
 use clap::ValueEnum;
 
 use anyhow::Result;
 use ast_grep_core::{NodeMatch as SgNodeMatch, StrDoc};
-pub use codespan_reporting::{files::SimpleFile, term::ColorArg};
+use codespan_reporting::files::SimpleFile;
 use std::io::{Stdout, Write};
 use std::sync::Mutex;
 
 type NodeMatch<'a, L> = SgNodeMatch<'a, StrDoc<L>>;
 
 use std::borrow::Cow;
 use std::path::{Path, PathBuf};
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/print/colored_print.rs` & `ast_grep_cli-0.9.3/crates/cli/src/print/colored_print.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 use super::{Diff, Printer};
 use crate::lang::SgLang;
 use ast_grep_config::{RuleConfig, Severity};
+use ast_grep_core::DisplayContext;
 
 use ansi_term::{Color, Style};
 use anyhow::Result;
 use clap::ValueEnum;
 use codespan_reporting::diagnostic::{self, Diagnostic, Label};
+use codespan_reporting::files::SimpleFile;
 use codespan_reporting::term::termcolor::{ColorChoice, StandardStream, WriteColor};
 use codespan_reporting::term::{self, DisplayStyle};
-pub use codespan_reporting::{files::SimpleFile, term::ColorArg};
 use similar::{ChangeTag, DiffOp, TextDiff};
 
 use std::borrow::Cow;
 use std::fmt::Display;
 use std::io::Write;
 use std::path::Path;
 use std::sync::Mutex;
 
+mod test;
+
 use ast_grep_core::{NodeMatch as SgNodeMatch, StrDoc};
 type NodeMatch<'a, L> = SgNodeMatch<'a, StrDoc<L>>;
 
 // add this macro because neither trait_alias nor type_alias_impl is supported.
 macro_rules! Matches {
   ($lt: lifetime) => { impl Iterator<Item = NodeMatch<$lt, SgLang>> };
 }
@@ -60,14 +63,15 @@
 }
 
 pub struct ColoredPrinter<W: WriteColor> {
   writer: Mutex<W>,
   config: term::Config,
   styles: PrintStyles,
   heading: Heading,
+  context: (u16, u16),
 }
 impl ColoredPrinter<StandardStream> {
   pub fn stdout<C: Into<ColorChoice>>(color: C) -> Self {
     let color = color.into();
     ColoredPrinter::new(StandardStream::stdout(color)).color(color)
   }
 }
@@ -75,14 +79,15 @@
 impl<W: WriteColor> ColoredPrinter<W> {
   pub fn new(writer: W) -> Self {
     Self {
       writer: Mutex::new(writer),
       styles: PrintStyles::from(ColorChoice::Auto),
       config: term::Config::default(),
       heading: Heading::Auto,
+      context: (0, 0),
     }
   }
 
   pub fn color<C: Into<ColorChoice>>(mut self, color: C) -> Self {
     let color = color.into();
     self.styles = PrintStyles::from(color);
     self
@@ -98,14 +103,23 @@
     self
   }
 
   pub fn heading(mut self, heading: Heading) -> Self {
     self.heading = heading;
     self
   }
+
+  pub fn context(mut self, context: (u16, u16)) -> Self {
+    self.context = context;
+    self
+  }
+
+  fn context_span(&self) -> usize {
+    (self.context.0 + self.context.1) as usize
+  }
 }
 
 impl<W: WriteColor> Printer for ColoredPrinter<W> {
   fn print_rule<'a>(
     &self,
     matches: Matches!('a),
     file: SimpleFile<Cow<str>, &String>,
@@ -136,19 +150,18 @@
         .with_labels(labels);
       term::emit(&mut *writer, config, &file, &diagnostic)?;
     }
     Ok(())
   }
 
   fn print_matches<'a>(&self, matches: Matches!('a), path: &Path) -> Result<()> {
-    let writer = &mut *self.writer.lock().expect("should success");
     if self.heading.should_print() {
-      print_matches_with_heading(matches, path, &self.styles, writer)
+      print_matches_with_heading(matches, path, self)
     } else {
-      print_matches_with_prefix(matches, path, &self.styles, writer)
+      print_matches_with_prefix(matches, path, self)
     }
   }
 
   fn print_diffs<'a>(&self, diffs: Diffs!('a), path: &Path) -> Result<()> {
     let writer = &mut *self.writer.lock().expect("should success");
     print_diffs(diffs, path, &self.styles, writer)
   }
@@ -214,49 +227,51 @@
 // merging overlapping/adjacent matches
 // adjacent matches: matches that starts or ends on the same line
 struct MatchMerger<'a> {
   last_start_line: usize,
   last_end_line: usize,
   last_trailing: &'a str,
   last_end_offset: usize,
+  context: (u16, u16),
 }
 
 impl<'a> MatchMerger<'a> {
-  fn new(nm: &NodeMatch<'a, SgLang>) -> Self {
-    let display = nm.display_context(0);
-    let last_start_line = display.start_line;
-    let last_end_line = nm.end_pos().0;
+  fn new(nm: &NodeMatch<'a, SgLang>, (before, after): (u16, u16)) -> Self {
+    let display = nm.display_context(before as usize, after as usize);
+    let last_start_line = display.start_line + 1;
+    let last_end_line = nm.end_pos().0 + 1;
     let last_trailing = display.trailing;
     let last_end_offset = nm.range().end;
     Self {
       last_start_line,
       last_end_line,
       last_end_offset,
       last_trailing,
+      context: (before, after),
     }
   }
 
   // merge non-overlapping matches but start/end on the same line
   fn merge_adjacent(&mut self, nm: &NodeMatch<'a, SgLang>) -> Option<usize> {
-    let start_line = nm.start_pos().0;
-    let display = nm.display_context(0);
-    if start_line == self.last_end_line {
+    let display = self.display(nm);
+    let start_line = display.start_line;
+    if start_line <= self.last_end_line + self.context.1 as usize {
       let last_end_offset = self.last_end_offset;
       self.last_end_offset = nm.range().end;
       self.last_trailing = display.trailing;
       Some(last_end_offset)
     } else {
       None
     }
   }
 
   fn conclude_match(&mut self, nm: &NodeMatch<'a, SgLang>) {
-    let display = nm.display_context(0);
-    self.last_start_line = display.start_line;
-    self.last_end_line = nm.end_pos().0;
+    let display = self.display(nm);
+    self.last_start_line = display.start_line + 1;
+    self.last_end_line = nm.end_pos().0 + 1;
     self.last_trailing = display.trailing;
     self.last_end_offset = nm.range().end;
   }
 
   #[inline]
   fn check_overlapping(&self, nm: &NodeMatch<'a, SgLang>) -> bool {
     let range = nm.range();
@@ -267,52 +282,61 @@
       // guaranteed by pre-order
       debug_assert!(range.end <= self.last_end_offset);
       true
     } else {
       false
     }
   }
+
+  fn display(&self, nm: &NodeMatch<'a, SgLang>) -> DisplayContext<'a> {
+    let (before, after) = self.context;
+    nm.display_context(before as usize, after as usize)
+  }
 }
 
-fn print_matches_with_heading<'a, W: Write>(
+fn print_matches_with_heading<'a, W: WriteColor>(
   mut matches: Matches!('a),
   path: &Path,
-  styles: &PrintStyles,
-  writer: &mut W,
+  printer: &ColoredPrinter<W>,
 ) -> Result<()> {
+  let styles = &printer.styles;
+  let writer = &mut *printer.writer.lock().expect("cannot get printer lock");
   print_prelude(path, styles, writer)?;
   let Some(first_match) = matches.next() else {
     return Ok(())
   };
   let source = first_match.root().get_text();
-  let display = first_match.display_context(0);
 
-  let mut merger = MatchMerger::new(&first_match);
+  let mut merger = MatchMerger::new(&first_match, printer.context);
+
+  let display = merger.display(&first_match);
   let mut ret = display.leading.to_string();
   styles.push_matched_to_ret(&mut ret, &display.matched)?;
 
   for nm in matches {
     if merger.check_overlapping(&nm) {
       continue;
     }
-    let display = nm.display_context(0);
+    let display = merger.display(&nm);
     // merge adjacent matches
     if let Some(last_end_offset) = merger.merge_adjacent(&nm) {
       ret.push_str(&source[last_end_offset..nm.range().start]);
       styles.push_matched_to_ret(&mut ret, &display.matched)?;
       continue;
     }
     ret.push_str(merger.last_trailing);
     let lines = ret.lines().count();
     let mut num = merger.last_start_line;
     let width = (lines + num).to_string().chars().count();
     write!(writer, "{num:>width$}│")?; // initial line num
     print_highlight(ret.lines(), width, &mut num, writer)?;
     writeln!(writer)?; // end match new line
-                       //
+    if printer.context_span() >= 1 {
+      writeln!(writer, "{:╴>width$}┤", "")?; // make separation
+    }
     merger.conclude_match(&nm);
     ret = display.leading.to_string();
     styles.push_matched_to_ret(&mut ret, &display.matched)?;
   }
   ret.push_str(merger.last_trailing);
   let lines = ret.lines().count();
   let mut num = merger.last_start_line;
@@ -323,44 +347,48 @@
   writeln!(writer)?; // end
   Ok(())
 }
 
 fn print_matches_with_prefix<'a, W: WriteColor>(
   mut matches: Matches!('a),
   path: &Path,
-  styles: &PrintStyles,
-  writer: &mut W,
+  printer: &ColoredPrinter<W>,
 ) -> Result<()> {
+  let styles = &printer.styles;
+  let writer = &mut *printer.writer.lock().expect("cannot get printer lock");
   let path = path.display();
   let Some(first_match) = matches.next() else {
     return Ok(())
   };
   let source = first_match.root().get_text();
-  let display = first_match.display_context(0);
 
-  let mut merger = MatchMerger::new(&first_match);
+  let mut merger = MatchMerger::new(&first_match, printer.context);
+  let display = merger.display(&first_match);
   let mut ret = display.leading.to_string();
   styles.push_matched_to_ret(&mut ret, &display.matched)?;
   for nm in matches {
     if merger.check_overlapping(&nm) {
       continue;
     }
+    let display = merger.display(&nm);
     // merge adjacent matches
     if let Some(last_end_offset) = merger.merge_adjacent(&nm) {
       ret.push_str(&source[last_end_offset..nm.range().start]);
       styles.push_matched_to_ret(&mut ret, &display.matched)?;
       continue;
     }
     ret.push_str(merger.last_trailing);
     for (n, line) in ret.lines().enumerate() {
       let num = merger.last_start_line + n;
       writeln!(writer, "{path}:{num}:{line}")?;
     }
+    if printer.context_span() >= 1 {
+      writeln!(writer, "--")?; // make separation
+    }
     merger.conclude_match(&nm);
-    let display = nm.display_context(0);
     ret = display.leading.to_string();
     styles.push_matched_to_ret(&mut ret, &display.matched)?;
   }
   ret.push_str(merger.last_trailing);
   for (n, line) in ret.lines().enumerate() {
     let num = merger.last_start_line + n;
     writeln!(writer, "{path}:{num}:{line}")?;
@@ -635,168 +663,7 @@
           // console API may be available.
           Ok(k) => k != "dumb" && k != "cygwin",
         }
       }
     }
   }
 }
-
-#[cfg(test)]
-mod test {
-  use super::*;
-  use ast_grep_config::{from_yaml_string, GlobalRules};
-  use ast_grep_core::replacer::Fixer;
-  use ast_grep_language::{Language, SupportLang};
-  use codespan_reporting::term::termcolor::Buffer;
-
-  fn make_test_printer() -> ColoredPrinter<Buffer> {
-    ColoredPrinter::new(Buffer::no_color()).color(ColorChoice::Never)
-  }
-  fn get_text(printer: &ColoredPrinter<Buffer>) -> String {
-    let buffer = printer.writer.lock().expect("should work");
-    let bytes = buffer.as_slice();
-    std::str::from_utf8(bytes)
-      .expect("buffer should be valid utf8")
-      .to_owned()
-  }
-
-  #[test]
-  fn test_emtpy_printer() {
-    let printer = make_test_printer();
-    assert_eq!(get_text(&printer), "");
-  }
-
-  // source, pattern, debug note
-  type Case<'a> = (&'a str, &'a str, &'a str);
-
-  const MATCHES_CASES: &[Case] = &[
-    ("let a = 123", "a", "Simple match"),
-    ("Some(1), Some(2), Some(3)", "Some", "Same line match"),
-    (
-      "Some(1), Some(2)\nSome(3), Some(4)",
-      "Some",
-      "Multiple line match",
-    ),
-    (
-      "import a from 'b';import a from 'b';",
-      "import a from 'b';",
-      "immediate following but not overlapping",
-    ),
-    ("Some(Some(123))", "Some($A)", "overlapping"),
-  ];
-  #[test]
-  fn test_print_matches() {
-    for &(source, pattern, note) in MATCHES_CASES {
-      // heading is required for CI
-      let printer = make_test_printer().heading(Heading::Always);
-      let grep = SgLang::from(SupportLang::Tsx).ast_grep(source);
-      let matches = grep.root().find_all(pattern);
-      printer.print_matches(matches, "test.tsx".as_ref()).unwrap();
-      let expected: String = source
-        .lines()
-        .enumerate()
-        .map(|(i, l)| format!("{}│{l}\n", i + 1))
-        .collect();
-      // append heading to expected
-      let output = format!("test.tsx\n{expected}\n");
-      assert_eq!(get_text(&printer), output, "{note}");
-    }
-  }
-
-  #[test]
-  fn test_print_matches_without_heading() {
-    for &(source, pattern, note) in MATCHES_CASES {
-      let printer = make_test_printer().heading(Heading::Never);
-      let grep = SgLang::from(SupportLang::Tsx).ast_grep(source);
-      let matches = grep.root().find_all(pattern);
-      printer.print_matches(matches, "test.tsx".as_ref()).unwrap();
-      // append heading to expected
-      let output: String = source
-        .lines()
-        .enumerate()
-        .map(|(i, e)| format!("test.tsx:{}:{e}\n", i + 1))
-        .collect();
-      assert_eq!(get_text(&printer), output, "{note}");
-    }
-  }
-
-  #[test]
-  fn test_print_rules() {
-    let globals = GlobalRules::default();
-    for &(source, pattern, note) in MATCHES_CASES {
-      let printer = make_test_printer()
-        .heading(Heading::Never)
-        .style(ReportStyle::Short);
-      let grep = SgLang::from(SupportLang::TypeScript).ast_grep(source);
-      let matches = grep.root().find_all(pattern);
-      let source = source.to_string();
-      let file = SimpleFile::new(Cow::Borrowed("test.tsx"), &source);
-      let rule = from_yaml_string(
-        &format!(
-          r"
-id: test-id
-message: test rule
-severity: info
-language: TypeScript
-rule:
-  pattern: {pattern}"
-        ),
-        &globals,
-      )
-      .expect("should parse")
-      .pop()
-      .unwrap();
-      printer.print_rule(matches, file, &rule).expect("test only");
-      let text = get_text(&printer);
-      assert!(text.contains("test.tsx"), "{note}");
-      assert!(text.contains("note[test-id]"), "{note}");
-      assert!(text.contains("test rule"), "{note}");
-    }
-  }
-
-  // source, pattern, rewrite, debug note
-  type DiffCase<'a> = (&'a str, &'a str, &'a str, &'a str);
-
-  const DIFF_CASES: &[DiffCase] = &[
-    ("let a = 123", "a", "b", "Simple match"),
-    (
-      "Some(1), Some(2), Some(3)",
-      "Some",
-      "Any",
-      "Same line match",
-    ),
-    (
-      "Some(1), Some(2)\nSome(3), Some(4)",
-      "Some",
-      "Any",
-      "Multiple line match",
-    ),
-    (
-      "import a from 'b';import a from 'b';",
-      "import a from 'b';",
-      "",
-      "immediate following but not overlapping",
-    ),
-    (
-      "\n\ntest",
-      "test",
-      "rest",
-      // https://github.com/ast-grep/ast-grep/issues/517
-      "leading empty space",
-    ),
-  ];
-
-  #[test]
-  fn test_print_diffs() {
-    for &(source, pattern, rewrite, note) in DIFF_CASES {
-      // heading is required for CI
-      let printer = make_test_printer().heading(Heading::Always);
-      let lang = SgLang::from(SupportLang::Tsx);
-      let fixer = Fixer::try_new(rewrite, &lang).expect("should work");
-      let grep = lang.ast_grep(source);
-      let matches = grep.root().find_all(pattern);
-      let diffs = matches.map(|n| Diff::generate(n, &pattern, &fixer));
-      printer.print_diffs(diffs, "test.tsx".as_ref()).unwrap();
-      assert!(get_text(&printer).contains(rewrite), "{note}");
-    }
-  }
-}
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/print/interactive_print.rs` & `ast_grep_cli-0.9.3/crates/cli/src/print/interactive_print.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use crate::error::ErrorContext as EC;
 use crate::lang::SgLang;
 use crate::utils;
 
 use anyhow::{Context, Result};
 use ast_grep_config::RuleConfig;
 use ast_grep_core::{NodeMatch as SgNodeMatch, StrDoc};
-pub use codespan_reporting::{files::SimpleFile, term::ColorArg};
+use codespan_reporting::files::SimpleFile;
 
 use std::sync::atomic::{AtomicBool, Ordering};
 
 type NodeMatch<'a, L> = SgNodeMatch<'a, StrDoc<L>>;
 
 use std::borrow::Cow;
 use std::path::{Path, PathBuf};
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/print/json_print.rs` & `ast_grep_cli-0.9.3/crates/cli/src/run.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,359 +1,339 @@
-use crate::lang::SgLang;
-use ast_grep_config::{RuleConfig, Severity};
-use ast_grep_core::{meta_var::MetaVariable, Node as SgNode, NodeMatch as SgNodeMatch, StrDoc};
-
-type NodeMatch<'a, L> = SgNodeMatch<'a, StrDoc<L>>;
-type Node<'a, L> = SgNode<'a, StrDoc<L>>;
+use std::path::{Path, PathBuf};
 
-use std::collections::HashMap;
+use anyhow::{Context, Result};
+use ast_grep_core::replacer::Fixer;
+use ast_grep_core::traversal::Visitor;
+use ast_grep_core::{Matcher, Pattern as SgPattern, StrDoc};
+use ast_grep_language::Language;
+use clap::Parser;
+use ignore::WalkParallel;
 
-use super::{Diff, Printer};
-use anyhow::Result;
-pub use codespan_reporting::{files::SimpleFile, term::ColorArg};
-use serde::{Deserialize, Serialize};
-
-use std::borrow::Cow;
-use std::io::{Stdout, Write};
-use std::path::Path;
-use std::sync::atomic::{AtomicBool, Ordering};
-use std::sync::Mutex;
-
-// add this macro because neither trait_alias nor type_alias_impl is supported.
-macro_rules! Matches {
-  ($lt: lifetime) => { impl Iterator<Item = NodeMatch<$lt, SgLang>> };
-}
-macro_rules! Diffs {
-  ($lt: lifetime) => { impl Iterator<Item = Diff<$lt>> };
-}
-
-#[derive(Serialize, Deserialize)]
-#[serde(rename_all = "camelCase")]
-struct Position {
-  line: usize,
-  column: usize,
-}
-
-#[derive(Serialize, Deserialize)]
-#[serde(rename_all = "camelCase")]
-struct Range {
-  /// inclusive start, exclusive end
-  byte_offset: std::ops::Range<usize>,
-  start: Position,
-  end: Position,
-}
-
-#[derive(Serialize, Deserialize)]
-#[serde(rename_all = "camelCase")]
-struct LabelJSON<'a> {
-  text: &'a str,
-  range: Range,
-}
-
-#[derive(Serialize, Deserialize)]
-#[serde(rename_all = "camelCase")]
-struct MatchNode<'a> {
-  text: Cow<'a, str>,
-  range: Range,
-}
-
-#[derive(Serialize, Deserialize)]
-#[serde(rename_all = "camelCase")]
-struct MatchJSON<'a> {
-  text: Cow<'a, str>,
-  range: Range,
-  file: Cow<'a, str>,
-  #[serde(skip_serializing_if = "Option::is_none")]
-  replacement: Option<Cow<'a, str>>,
-  language: SgLang,
-  #[serde(skip_serializing_if = "Option::is_none")]
-  meta_variables: Option<MetaVariables<'a>>,
-}
-
-#[derive(Serialize, Deserialize)]
-#[serde(rename_all = "camelCase")]
-struct MetaVariables<'a> {
-  single: HashMap<String, MatchNode<'a>>,
-  multi: HashMap<String, Vec<MatchNode<'a>>>,
-  transformed: HashMap<String, String>,
-}
-fn from_env<'a>(nm: &NodeMatch<'a, SgLang>) -> Option<MetaVariables<'a>> {
-  let env = nm.get_env();
-  let mut vars = env.get_matched_variables().peekable();
-  vars.peek()?;
-  let mut single = HashMap::new();
-  let mut multi = HashMap::new();
-  let mut transformed = HashMap::new();
-  for var in vars {
-    use MetaVariable as MV;
-    match var {
-      MV::Named(n, _) => {
-        if let Some(node) = env.get_match(&n) {
-          single.insert(
-            n,
-            MatchNode {
-              text: node.text(),
-              range: get_range(node),
-            },
-          );
-        } else if let Some(bytes) = env.get_transformed(&n) {
-          transformed.insert(n, String::from_utf8_lossy(bytes).into_owned());
-        }
-      }
-      MV::NamedEllipsis(n) => {
-        let nodes = env.get_multiple_matches(&n);
-        multi.insert(
-          n,
-          nodes
-            .into_iter()
-            .map(|node| MatchNode {
-              text: node.text(),
-              range: get_range(&node),
-            })
-            .collect(),
-        );
-      }
-      _ => continue,
-    }
-  }
-  Some(MetaVariables {
-    single,
-    multi,
-    transformed,
-  })
-}
-
-fn get_range(n: &Node<'_, SgLang>) -> Range {
-  let start_pos = n.start_pos();
-  let end_pos = n.end_pos();
-  Range {
-    byte_offset: n.range(),
-    start: Position {
-      line: start_pos.0,
-      column: start_pos.1,
-    },
-    end: Position {
-      line: end_pos.0,
-      column: end_pos.1,
-    },
+use crate::config::{register_custom_language, IgnoreFile, NoIgnore};
+use crate::error::ErrorContext as EC;
+use crate::lang::SgLang;
+use crate::print::{
+  ColorArg, ColoredPrinter, Diff, Heading, InteractivePrinter, JSONPrinter, Printer,
+};
+use crate::utils::{filter_file_pattern, is_from_stdin, MatchUnit};
+use crate::utils::{run_std_in, StdInWorker};
+use crate::utils::{run_worker, Items, Worker};
+
+type Pattern<L> = SgPattern<StrDoc<L>>;
+
+// NOTE: have to register custom lang before clap read arg
+// RunArg has a field of SgLang
+pub fn register_custom_language_if_is_run(args: &[String]) {
+  if !args.is_empty() || args[1].starts_with('-') || args[1] == "run" {
+    register_custom_language(None);
   }
 }
 
-impl<'a> MatchJSON<'a> {
-  fn new(nm: NodeMatch<'a, SgLang>, path: &'a str) -> Self {
-    MatchJSON {
-      file: Cow::Borrowed(path),
-      text: nm.text(),
-      language: *nm.lang(),
-      replacement: None,
-      range: get_range(&nm),
-      meta_variables: from_env(&nm),
-    }
-  }
-}
-fn get_labels<'a>(nm: &NodeMatch<'a, SgLang>) -> Option<Vec<MatchNode<'a>>> {
-  let env = nm.get_env();
-  let labels = env.get_labels("secondary")?;
-  Some(
-    labels
-      .iter()
-      .map(|l| MatchNode {
-        text: l.text(),
-        range: get_range(l),
-      })
-      .collect(),
+fn lang_help() -> String {
+  format!(
+    "The language of the pattern. Supported languages are:\n{:?}",
+    SgLang::all_langs()
   )
 }
 
-#[derive(Serialize, Deserialize)]
-#[serde(rename_all = "camelCase")]
-struct RuleMatchJSON<'a> {
-  #[serde(flatten)]
-  matched: MatchJSON<'a>,
-  rule_id: &'a str,
-  severity: Severity,
-  message: String,
-  #[serde(skip_serializing_if = "Option::is_none")]
-  labels: Option<Vec<MatchNode<'a>>>,
-}
-impl<'a> RuleMatchJSON<'a> {
-  fn new(nm: NodeMatch<'a, SgLang>, path: &'a str, rule: &'a RuleConfig<SgLang>) -> Self {
-    let message = rule.get_message(&nm);
-    let labels = get_labels(&nm);
-    let matched = MatchJSON::new(nm, path);
-    Self {
-      matched,
-      rule_id: &rule.id,
-      severity: rule.severity.clone(),
-      message,
-      labels,
+const LANG_HELP_LONG: &str = "The language of the pattern. For full language list, visit https://ast-grep.github.io/reference/languages.html";
+
+#[derive(Parser)]
+pub struct RunArg {
+  // search pattern related options
+  /// AST pattern to match.
+  #[clap(short, long)]
+  pattern: String,
+
+  /// String to replace the matched AST node.
+  #[clap(short, long)]
+  rewrite: Option<String>,
+
+  /// Print query pattern's tree-sitter AST. Requires lang be set explicitly.
+  #[clap(long, requires = "lang")]
+  debug_query: bool,
+
+  /// The language of the pattern query.
+  #[clap(short, long, help(lang_help()), long_help=LANG_HELP_LONG)]
+  lang: Option<SgLang>,
+
+  // output related options
+  /// Start interactive edit session. Code rewrite only happens inside a session.
+  #[clap(short, long)]
+  interactive: bool,
+
+  /// Output matches in structured JSON text useful for tools like jq.
+  /// Conflicts with interactive.
+  #[clap(long, conflicts_with = "interactive")]
+  json: bool,
+
+  /// Print the file name as heading before all matches of that file.
+  /// File path will be printed before each match as prefix if heading is disabled.
+  /// This is the default mode when printing to a terminal.
+  #[clap(long, default_value = "auto")]
+  heading: Heading,
+
+  /// Controls output color.
+  #[clap(long, default_value = "auto")]
+  color: ColorArg,
+
+  // input related options
+  /// The paths to search. You can provide multiple paths separated by spaces.
+  #[clap(value_parser, default_value = ".")]
+  paths: Vec<PathBuf>,
+
+  /// Apply all rewrite without confirmation if true.
+  #[clap(short = 'U', long, requires = "rewrite")]
+  update_all: bool,
+
+  /// Do not respect hidden file system or ignore files (.gitignore, .ignore, etc.).
+  /// You can suppress multiple ignore files by passing `no-ignore` multiple times.
+  #[clap(long, action = clap::ArgAction::Append)]
+  no_ignore: Vec<IgnoreFile>,
+
+  /// Enable search code from StdIn.
+  ///
+  /// Use this if you need to take code stream from standard input.
+  /// If the environment variable `AST_GREP_NO_STDIN` exist, ast-grep will disable StdIn mode.
+  #[clap(long)]
+  stdin: bool,
+
+  // context related options
+  /// Show NUM lines after each match.
+  #[clap(
+    short = 'A',
+    long,
+    default_value = "0",
+    conflicts_with = "context",
+    value_name = "NUM"
+  )]
+  after: u16,
+  /// Show NUM lines before each match.
+  #[clap(
+    short = 'B',
+    long,
+    default_value = "0",
+    conflicts_with = "context",
+    value_name = "NUM"
+  )]
+  before: u16,
+  /// Show NUM lines around each match.
+  #[clap(short = 'C', long, default_value = "0", value_name = "NUM")]
+  context: u16,
+}
+
+// Every run will include Search or Replace
+// Search or Replace by arguments `pattern` and `rewrite` passed from CLI
+pub fn run_with_pattern(arg: RunArg) -> Result<()> {
+  if arg.json {
+    return run_pattern_with_printer(arg, JSONPrinter::stdout());
+  }
+  let context = if arg.context != 0 {
+    (arg.context, arg.context)
+  } else {
+    (arg.before, arg.after)
+  };
+  let printer = ColoredPrinter::stdout(arg.color)
+    .heading(arg.heading)
+    .context(context);
+  let interactive = arg.interactive || arg.update_all;
+  if interactive {
+    let from_stdin = arg.stdin && is_from_stdin();
+    let printer = InteractivePrinter::new(printer, arg.update_all, from_stdin)?;
+    run_pattern_with_printer(arg, printer)
+  } else {
+    run_pattern_with_printer(arg, printer)
+  }
+}
+
+fn run_pattern_with_printer(arg: RunArg, printer: impl Printer + Sync) -> Result<()> {
+  if arg.stdin && is_from_stdin() {
+    run_std_in(RunWithSpecificLang::new(arg, printer)?)
+  } else if arg.lang.is_some() {
+    run_worker(RunWithSpecificLang::new(arg, printer)?)
+  } else {
+    run_worker(RunWithInferredLang { arg, printer })
+  }
+}
+
+struct RunWithInferredLang<Printer> {
+  arg: RunArg,
+  printer: Printer,
+}
+
+impl<P: Printer + Sync> Worker for RunWithInferredLang<P> {
+  type Item = (MatchUnit<Pattern<SgLang>>, SgLang);
+  fn build_walk(&self) -> WalkParallel {
+    let arg = &self.arg;
+    let threads = num_cpus::get().min(12);
+    NoIgnore::disregard(&arg.no_ignore)
+      .walk(&arg.paths)
+      .threads(threads)
+      .build_parallel()
+  }
+
+  fn produce_item(&self, path: &Path) -> Option<Self::Item> {
+    let lang = SgLang::from_path(path)?;
+    let matcher = Pattern::try_new(&self.arg.pattern, lang).ok()?;
+    let match_unit = filter_file_pattern(path, lang, matcher)?;
+    Some((match_unit, lang))
+  }
+
+  fn consume_items(&self, items: Items<Self::Item>) -> Result<()> {
+    let rewrite = &self.arg.rewrite;
+    let printer = &self.printer;
+    printer.before_print()?;
+    for (match_unit, lang) in items {
+      let rewrite = rewrite
+        .as_ref()
+        .map(|s| Fixer::try_new(s, &lang))
+        .transpose();
+      match rewrite {
+        Ok(r) => match_one_file(printer, &match_unit, &r)?,
+        Err(e) => {
+          match_one_file(printer, &match_unit, &None)?;
+          eprintln!("⚠️  Rewriting was skipped because pattern fails to parse. Error detail:");
+          eprintln!("╰▻ {e}");
+        }
+      }
     }
+    printer.after_print()?;
+    Ok(())
   }
 }
 
-pub struct JSONPrinter<W: Write> {
-  output: Mutex<W>,
-  // indicate if any matches happened
-  matched: AtomicBool,
-}
-impl JSONPrinter<Stdout> {
-  pub fn stdout() -> Self {
-    Self::new(std::io::stdout())
+struct RunWithSpecificLang<Printer> {
+  arg: RunArg,
+  printer: Printer,
+  pattern: Pattern<SgLang>,
+}
+
+impl<Printer> RunWithSpecificLang<Printer> {
+  fn new(arg: RunArg, printer: Printer) -> Result<Self> {
+    let pattern = &arg.pattern;
+    let lang = arg.lang.ok_or(anyhow::anyhow!(EC::LanguageNotSpecified))?;
+    let pattern = Pattern::try_new(pattern, lang).context(EC::ParsePattern)?;
+    Ok(Self {
+      arg,
+      printer,
+      pattern,
+    })
   }
 }
 
-impl<W: Write> JSONPrinter<W> {
-  pub fn new(output: W) -> Self {
-    // no match happened yet
-    Self {
-      output: Mutex::new(output),
-      matched: AtomicBool::new(false),
-    }
-  }
-
-  fn print_docs<S: Serialize>(&self, docs: impl Iterator<Item = S>) -> Result<()> {
-    let mut docs = docs.peekable();
-    if docs.peek().is_none() {
-      return Ok(());
-    }
-    let mut lock = self.output.lock().expect("should work");
-    let matched = self.matched.swap(true, Ordering::AcqRel);
-    if !matched {
-      writeln!(&mut lock)?;
-      let doc = docs.next().expect("must not be empty");
-      serde_json::to_writer_pretty(&mut *lock, &doc)?;
-    }
-    for doc in docs {
-      writeln!(&mut lock, ",")?;
-      serde_json::to_writer_pretty(&mut *lock, &doc)?;
+impl<P: Printer + Sync> Worker for RunWithSpecificLang<P> {
+  type Item = MatchUnit<Pattern<SgLang>>;
+  fn build_walk(&self) -> WalkParallel {
+    let arg = &self.arg;
+    let threads = num_cpus::get().min(12);
+    let lang = arg.lang.expect("must present");
+    NoIgnore::disregard(&arg.no_ignore)
+      .walk(&arg.paths)
+      .threads(threads)
+      .types(lang.file_types())
+      .build_parallel()
+  }
+  fn produce_item(&self, path: &Path) -> Option<Self::Item> {
+    let arg = &self.arg;
+    let pattern = self.pattern.clone();
+    let lang = arg.lang.expect("must present");
+    filter_file_pattern(path, lang, pattern)
+  }
+  fn consume_items(&self, items: Items<Self::Item>) -> Result<()> {
+    let printer = &self.printer;
+    printer.before_print()?;
+    let arg = &self.arg;
+    let lang = arg.lang.expect("must present");
+    if arg.debug_query {
+      println!("Pattern TreeSitter {:?}", self.pattern);
+    }
+    let rewrite = if let Some(s) = &arg.rewrite {
+      Some(Fixer::try_new(s, &lang).context(EC::ParsePattern)?)
+    } else {
+      None
+    };
+    for match_unit in items {
+      match_one_file(printer, &match_unit, &rewrite)?;
     }
+    printer.after_print()?;
     Ok(())
   }
 }
 
-impl<W: Write> Printer for JSONPrinter<W> {
-  fn print_rule<'a>(
-    &self,
-    matches: Matches!('a),
-    file: SimpleFile<Cow<str>, &String>,
-    rule: &RuleConfig<SgLang>,
-  ) -> Result<()> {
-    let path = file.name();
-    let jsons = matches.map(|nm| RuleMatchJSON::new(nm, path, rule));
-    self.print_docs(jsons)
-  }
-
-  fn print_matches<'a>(&self, matches: Matches!('a), path: &Path) -> Result<()> {
-    let path = path.to_string_lossy();
-    let jsons = matches.map(|nm| MatchJSON::new(nm, &path));
-    self.print_docs(jsons)
-  }
-
-  fn print_diffs<'a>(&self, diffs: Diffs!('a), path: &Path) -> Result<()> {
-    let path = path.to_string_lossy();
-    let jsons = diffs.map(|diff| {
-      let mut v = MatchJSON::new(diff.node_match, &path);
-      v.replacement = Some(diff.replacement);
-      v
-    });
-    self.print_docs(jsons)
-  }
-  fn print_rule_diffs<'a>(
-    &self,
-    diffs: Diffs!('a),
-    path: &Path,
-    rule: &RuleConfig<SgLang>,
-  ) -> Result<()> {
-    let path = path.to_string_lossy();
-    let jsons = diffs.map(|diff| {
-      let mut v = RuleMatchJSON::new(diff.node_match, &path, rule);
-      v.matched.replacement = Some(diff.replacement);
-      v
-    });
-    self.print_docs(jsons)
-  }
-
-  fn before_print(&self) -> Result<()> {
-    let mut lock = self.output.lock().expect("should work");
-    write!(&mut lock, "[")?;
-    Ok(())
+impl<P: Printer + Sync> StdInWorker for RunWithSpecificLang<P> {
+  fn parse_stdin(&self, src: String) -> Option<Self::Item> {
+    let lang = self.arg.lang.expect("must present");
+    let grep = lang.ast_grep(src);
+    let has_match = grep.root().find(&self.pattern).is_some();
+    has_match.then(|| MatchUnit {
+      path: PathBuf::from("STDIN"),
+      matcher: self.pattern.clone(),
+      grep,
+    })
   }
+}
 
-  fn after_print(&self) -> Result<()> {
-    let mut lock = self.output.lock().expect("should work");
-    let matched = self.matched.load(Ordering::Acquire);
-    if matched {
-      writeln!(&mut lock)?;
-    }
-    writeln!(&mut lock, "]")?;
-    Ok(())
+fn match_one_file(
+  printer: &impl Printer,
+  match_unit: &MatchUnit<impl Matcher<SgLang>>,
+  rewrite: &Option<Fixer<String>>,
+) -> Result<()> {
+  let MatchUnit {
+    path,
+    grep,
+    matcher,
+  } = match_unit;
+
+  let matches = Visitor::new(matcher).reentrant(false).visit(grep.root());
+  if let Some(rewrite) = rewrite {
+    let diffs = matches.map(|m| Diff::generate(m, matcher, rewrite));
+    printer.print_diffs(diffs, path)
+  } else {
+    printer.print_matches(matches, path)
   }
 }
 
 #[cfg(test)]
 mod test {
   use super::*;
-  use ast_grep_language::{Language, SupportLang};
+  use ast_grep_language::SupportLang;
 
-  struct Test(String);
-  impl Write for Test {
-    fn write(&mut self, buf: &[u8]) -> std::io::Result<usize> {
-      let s = std::str::from_utf8(buf).expect("should ok");
-      self.0.push_str(s);
-      Ok(buf.len())
-    }
-    fn flush(&mut self) -> std::io::Result<()> {
-      Ok(())
+  fn default_run_arg() -> RunArg {
+    RunArg {
+      pattern: String::new(),
+      rewrite: None,
+      color: ColorArg::Never,
+      no_ignore: vec![],
+      stdin: false,
+      interactive: false,
+      lang: None,
+      json: false,
+      heading: Heading::Never,
+      debug_query: false,
+      update_all: false,
+      paths: vec![PathBuf::from(".")],
+      before: 0,
+      after: 0,
+      context: 0,
     }
   }
-  fn make_test_printer() -> JSONPrinter<Test> {
-    JSONPrinter::new(Test(String::new()))
-  }
-  fn get_text(printer: &JSONPrinter<Test>) -> String {
-    let lock = printer.output.lock().unwrap();
-    lock.0.to_string()
-  }
 
   #[test]
-  fn test_emtpy_printer() {
-    let printer = make_test_printer();
-    printer.before_print().unwrap();
-    printer
-      .print_matches(std::iter::empty(), "test.tsx".as_ref())
-      .unwrap();
-    printer.after_print().unwrap();
-    assert_eq!(get_text(&printer), "[]\n");
-  }
-
-  // source, pattern, debug note
-  type Case<'a> = (&'a str, &'a str, &'a str);
-
-  const MATCHES_CASES: &[Case] = &[
-    ("let a = 123", "a", "Simple match"),
-    ("Some(1), Some(2), Some(3)", "Some", "Same line match"),
-    (
-      "Some(1), Some(2)\nSome(3), Some(4)",
-      "Some",
-      "Multiple line match",
-    ),
-    (
-      "import a from 'b';import a from 'b';",
-      "import a from 'b';",
-      "immediate following but not overlapping",
-    ),
-  ];
+  fn test_run_with_pattern() {
+    let arg = RunArg {
+      pattern: "console.log".to_string(),
+      ..default_run_arg()
+    };
+    assert!(run_with_pattern(arg).is_ok())
+  }
+
   #[test]
-  fn test_invariant() {
-    for &(source, pattern, note) in MATCHES_CASES {
-      // heading is required for CI
-      let printer = make_test_printer();
-      let grep = SgLang::from(SupportLang::Tsx).ast_grep(source);
-      let matches = grep.root().find_all(pattern);
-      printer.before_print().unwrap();
-      printer.print_matches(matches, "test.tsx".as_ref()).unwrap();
-      printer.after_print().unwrap();
-      let json_str = get_text(&printer);
-      let json: Vec<MatchJSON> = serde_json::from_str(&json_str).unwrap();
-      assert_eq!(json[0].text, pattern, "{note}");
-    }
+  fn test_run_with_specific_lang() {
+    let arg = RunArg {
+      pattern: "Some(result)".to_string(),
+      lang: Some(SupportLang::Rust.into()),
+      stdin: true,
+      ..default_run_arg()
+    };
+    assert!(run_with_pattern(arg).is_ok())
   }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/print/mod.rs` & `ast_grep_cli-0.9.3/crates/cli/src/print/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/run.rs` & `ast_grep_cli-0.9.3/crates/cli/src/scan.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,303 +1,364 @@
+use std::collections::HashMap;
 use std::path::{Path, PathBuf};
 
 use anyhow::{Context, Result};
-use ast_grep_core::replacer::Fixer;
-use ast_grep_core::traversal::Visitor;
-use ast_grep_core::{Matcher, Pattern as SgPattern, StrDoc};
-use ast_grep_language::Language;
-use clap::Parser;
+use ast_grep_config::{RuleCollection, RuleConfig, Severity};
+use ast_grep_core::{Matcher, NodeMatch, StrDoc};
+use clap::Args;
 use ignore::WalkParallel;
 
-use crate::config::{register_custom_language, IgnoreFile, NoIgnore};
+use crate::config::{find_rules, read_rule_file, register_custom_language, IgnoreFile, NoIgnore};
 use crate::error::ErrorContext as EC;
 use crate::lang::SgLang;
 use crate::print::{
-  ColorArg, ColoredPrinter, Diff, Heading, InteractivePrinter, JSONPrinter, Printer,
+  CloudPrinter, ColorArg, ColoredPrinter, Diff, InteractivePrinter, JSONPrinter, Platform, Printer,
+  ReportStyle, SimpleFile,
 };
-use crate::utils::{filter_file_pattern, is_from_stdin, MatchUnit};
-use crate::utils::{run_std_in, StdInWorker};
+use crate::utils::filter_file_interactive;
+use crate::utils::{is_from_stdin, run_std_in, StdInWorker};
 use crate::utils::{run_worker, Items, Worker};
 
-type Pattern<L> = SgPattern<StrDoc<L>>;
+type AstGrep = ast_grep_core::AstGrep<StrDoc<SgLang>>;
 
-// NOTE: have to register custom lang before clap read arg
-// RunArg has a field of SgLang
-pub fn register_custom_language_if_is_run(args: &[String]) {
-  if !args.is_empty() || args[1].starts_with('-') || args[1] == "run" {
-    register_custom_language(None);
-  }
-}
-
-fn lang_help() -> String {
-  format!(
-    "The language of the pattern. Supported languages are:\n{:?}",
-    SgLang::all_langs()
-  )
-}
-
-const LANG_HELP_LONG: &str = "The language of the pattern. For full language list, visit https://ast-grep.github.io/reference/languages.html";
-
-#[derive(Parser)]
-pub struct RunArg {
-  /// AST pattern to match.
+#[derive(Args)]
+pub struct ScanArg {
+  /// Path to ast-grep root config, default is sgconfig.yml.
   #[clap(short, long)]
-  pattern: String,
+  config: Option<PathBuf>,
 
-  /// String to replace the matched AST node.
-  #[clap(short, long)]
-  rewrite: Option<String>,
-
-  /// Print query pattern's tree-sitter AST. Requires lang be set explicitly.
-  #[clap(long, requires = "lang")]
-  debug_query: bool,
-
-  /// The language of the pattern query.
-  #[clap(short, long, help(lang_help()), long_help=LANG_HELP_LONG)]
-  lang: Option<SgLang>,
+  /// Scan the codebase with one specified rule, without project config setup.
+  #[clap(short, long, conflicts_with = "config")]
+  rule: Option<PathBuf>,
 
   /// Start interactive edit session. Code rewrite only happens inside a session.
-  #[clap(short, long)]
+  #[clap(short, long, conflicts_with = "json", conflicts_with = "format")]
   interactive: bool,
 
-  /// The paths to search. You can provide multiple paths separated by spaces.
-  #[clap(value_parser, default_value = ".")]
-  paths: Vec<PathBuf>,
+  /// Controls output color.
+  #[clap(long, default_value = "auto")]
+  color: ColorArg,
 
-  /// Apply all rewrite without confirmation if true.
-  #[clap(short = 'U', long, requires = "rewrite")]
-  update_all: bool,
+  #[clap(short, long, conflicts_with = "json")]
+  format: Option<Platform>,
 
-  /// Output matches in structured JSON text useful for tools like jq.
-  /// Conflicts with interactive.
-  #[clap(long, conflicts_with = "interactive")]
+  #[clap(long, default_value = "rich")]
+  report_style: ReportStyle,
+
+  /// Output matches in structured JSON text. This is useful for tools like jq.
+  /// Conflicts with color and report-style.
+  #[clap(long, conflicts_with = "color", conflicts_with = "report_style")]
   json: bool,
 
-  /// Print the file name as heading before all matches of that file.
-  /// File path will be printed before each match as prefix if heading is disabled.
-  /// This is the default mode when printing to a terminal.
-  #[clap(long, default_value = "auto")]
-  heading: Heading,
+  /// Apply all rewrite without confirmation if true.
+  #[clap(short = 'U', long)]
+  update_all: bool,
 
-  /// Controls output color.
-  #[clap(long, default_value = "auto")]
-  color: ColorArg,
+  /// The paths to search. You can provide multiple paths separated by spaces.
+  #[clap(value_parser, default_value = ".")]
+  paths: Vec<PathBuf>,
 
-  /// Do not respect hidden file system or ignore files (.gitignore, .ignore, etc.).
-  /// You can suppress multiple ignore files by passing `no-ignore` multiple times.
+  /// Do not respect ignore files. You can suppress multiple ignore files by passing `no-ignore` multiple times.
   #[clap(long, action = clap::ArgAction::Append)]
   no_ignore: Vec<IgnoreFile>,
 
   /// Enable search code from StdIn.
   ///
   /// Use this if you need to take code stream from standard input.
   /// If the environment variable `AST_GREP_NO_STDIN` exist, ast-grep will disable StdIn mode.
   #[clap(long)]
   stdin: bool,
 }
 
-// Every run will include Search or Replace
-// Search or Replace by arguments `pattern` and `rewrite` passed from CLI
-pub fn run_with_pattern(arg: RunArg) -> Result<()> {
+pub fn run_with_config(arg: ScanArg) -> Result<()> {
+  register_custom_language(arg.config.clone());
   if arg.json {
-    return run_pattern_with_printer(arg, JSONPrinter::stdout());
+    let printer = JSONPrinter::stdout();
+    return run_scan(arg, printer);
+  }
+  if let Some(_format) = &arg.format {
+    let printer = CloudPrinter::stdout();
+    return run_scan(arg, printer);
   }
-  let printer = ColoredPrinter::stdout(arg.color).heading(arg.heading);
+  let printer = ColoredPrinter::stdout(arg.color).style(arg.report_style);
   let interactive = arg.interactive || arg.update_all;
   if interactive {
     let from_stdin = arg.stdin && is_from_stdin();
     let printer = InteractivePrinter::new(printer, arg.update_all, from_stdin)?;
-    run_pattern_with_printer(arg, printer)
+    run_scan(arg, printer)
   } else {
-    run_pattern_with_printer(arg, printer)
+    run_scan(arg, printer)
   }
 }
 
-fn run_pattern_with_printer(arg: RunArg, printer: impl Printer + Sync) -> Result<()> {
+fn run_scan<P: Printer + Sync>(arg: ScanArg, printer: P) -> Result<()> {
   if arg.stdin && is_from_stdin() {
-    run_std_in(RunWithSpecificLang::new(arg, printer)?)
-  } else if arg.lang.is_some() {
-    run_worker(RunWithSpecificLang::new(arg, printer)?)
+    let worker = ScanWithRule::try_new(arg, printer)?;
+    run_std_in(worker)
   } else {
-    run_worker(RunWithInferredLang { arg, printer })
+    let worker = ScanWithConfig::try_new(arg, printer)?;
+    run_worker(worker)
   }
 }
 
-struct RunWithInferredLang<Printer> {
-  arg: RunArg,
+struct ScanWithConfig<Printer> {
+  arg: ScanArg,
   printer: Printer,
+  configs: RuleCollection<SgLang>,
+}
+impl<P: Printer> ScanWithConfig<P> {
+  fn try_new(mut arg: ScanArg, printer: P) -> Result<Self> {
+    let configs = if let Some(path) = &arg.rule {
+      let rules = read_rule_file(path, None)?;
+      RuleCollection::try_new(rules).context(EC::GlobPattern)?
+    } else {
+      find_rules(arg.config.take())?
+    };
+    Ok(Self {
+      arg,
+      printer,
+      configs,
+    })
+  }
 }
 
-impl<P: Printer + Sync> Worker for RunWithInferredLang<P> {
-  type Item = (MatchUnit<Pattern<SgLang>>, SgLang);
+impl<P: Printer + Sync> Worker for ScanWithConfig<P> {
+  type Item = (PathBuf, AstGrep);
   fn build_walk(&self) -> WalkParallel {
     let arg = &self.arg;
     let threads = num_cpus::get().min(12);
     NoIgnore::disregard(&arg.no_ignore)
       .walk(&arg.paths)
       .threads(threads)
       .build_parallel()
   }
-
   fn produce_item(&self, path: &Path) -> Option<Self::Item> {
-    let lang = SgLang::from_path(path)?;
-    let matcher = Pattern::try_new(&self.arg.pattern, lang).ok()?;
-    let match_unit = filter_file_pattern(path, lang, matcher)?;
-    Some((match_unit, lang))
+    let rules = self.configs.for_path(path);
+    if rules.is_empty() {
+      return None;
+    }
+    let lang = rules[0].language;
+    let combined = CombinedScan::new(rules);
+    let unit = filter_file_interactive(path, lang, ast_grep_core::matcher::MatchAll)?;
+    if combined.find(&unit.grep) {
+      return Some((unit.path, unit.grep));
+    }
+    None
   }
-
   fn consume_items(&self, items: Items<Self::Item>) -> Result<()> {
-    let rewrite = &self.arg.rewrite;
-    let printer = &self.printer;
-    printer.before_print()?;
-    for (match_unit, lang) in items {
-      let rewrite = rewrite
-        .as_ref()
-        .map(|s| Fixer::try_new(s, &lang))
-        .transpose();
-      match rewrite {
-        Ok(r) => match_one_file(printer, &match_unit, &r)?,
-        Err(e) => {
-          match_one_file(printer, &match_unit, &None)?;
-          eprintln!("⚠️  Rewriting was skipped because pattern fails to parse. Error detail:");
-          eprintln!("╰▻ {e}");
+    self.printer.before_print()?;
+    let mut has_error = 0;
+    for (path, grep) in items {
+      let file_content = grep.root().text().to_string();
+      let path = &path;
+      let rules = self.configs.for_path(path);
+      let combined = CombinedScan::new(rules);
+      let matched = combined.scan(&grep);
+      for (idx, matches) in matched {
+        let rule = &combined.rules[idx];
+        if matches!(rule.severity, Severity::Error) {
+          has_error += 1;
         }
+        match_rule_on_file(path, matches, rule, &file_content, &self.printer)?;
       }
     }
-    printer.after_print()?;
-    Ok(())
+    self.printer.after_print()?;
+    if has_error > 0 {
+      Err(anyhow::anyhow!(EC::DiagnosticError(has_error)))
+    } else {
+      Ok(())
+    }
   }
 }
 
-struct RunWithSpecificLang<Printer> {
-  arg: RunArg,
+struct ScanWithRule<Printer> {
   printer: Printer,
-  pattern: Pattern<SgLang>,
+  rule: RuleConfig<SgLang>,
 }
-
-impl<Printer> RunWithSpecificLang<Printer> {
-  fn new(arg: RunArg, printer: Printer) -> Result<Self> {
-    let pattern = &arg.pattern;
-    let lang = arg.lang.ok_or(anyhow::anyhow!(EC::LanguageNotSpecified))?;
-    let pattern = Pattern::try_new(pattern, lang).context(EC::ParsePattern)?;
-    Ok(Self {
-      arg,
-      printer,
-      pattern,
-    })
+impl<P: Printer> ScanWithRule<P> {
+  fn try_new(arg: ScanArg, printer: P) -> Result<Self> {
+    let rule = if let Some(path) = &arg.rule {
+      read_rule_file(path, None)?.pop().unwrap()
+    } else {
+      return Err(anyhow::anyhow!(EC::RuleNotSpecified));
+    };
+    Ok(Self { printer, rule })
   }
 }
 
-impl<P: Printer + Sync> Worker for RunWithSpecificLang<P> {
-  type Item = MatchUnit<Pattern<SgLang>>;
+impl<P: Printer + Sync> Worker for ScanWithRule<P> {
+  type Item = (PathBuf, AstGrep);
   fn build_walk(&self) -> WalkParallel {
-    let arg = &self.arg;
-    let threads = num_cpus::get().min(12);
-    let lang = arg.lang.expect("must present");
-    NoIgnore::disregard(&arg.no_ignore)
-      .walk(&arg.paths)
-      .threads(threads)
-      .types(lang.file_types())
-      .build_parallel()
+    unreachable!()
   }
-  fn produce_item(&self, path: &Path) -> Option<Self::Item> {
-    let arg = &self.arg;
-    let pattern = self.pattern.clone();
-    let lang = arg.lang.expect("must present");
-    filter_file_pattern(path, lang, pattern)
+  fn produce_item(&self, _p: &Path) -> Option<Self::Item> {
+    unreachable!()
   }
   fn consume_items(&self, items: Items<Self::Item>) -> Result<()> {
-    let printer = &self.printer;
-    printer.before_print()?;
-    let arg = &self.arg;
-    let lang = arg.lang.expect("must present");
-    if arg.debug_query {
-      println!("Pattern TreeSitter {:?}", self.pattern);
+    self.printer.before_print()?;
+    let mut has_error = 0;
+    for (path, grep) in items {
+      let file_content = grep.root().text().to_string();
+      let rule = &self.rule;
+      let matches = grep.root().find_all(&rule.matcher).collect();
+      if matches!(rule.severity, Severity::Error) {
+        has_error += 1;
+      }
+      match_rule_on_file(&path, matches, rule, &file_content, &self.printer)?;
     }
-    let rewrite = if let Some(s) = &arg.rewrite {
-      Some(Fixer::try_new(s, &lang).context(EC::ParsePattern)?)
+    self.printer.after_print()?;
+    if has_error > 0 {
+      Err(anyhow::anyhow!(EC::DiagnosticError(has_error)))
     } else {
-      None
-    };
-    for match_unit in items {
-      match_one_file(printer, &match_unit, &rewrite)?;
+      Ok(())
     }
-    printer.after_print()?;
-    Ok(())
   }
 }
 
-impl<P: Printer + Sync> StdInWorker for RunWithSpecificLang<P> {
+impl<P: Printer + Sync> StdInWorker for ScanWithRule<P> {
   fn parse_stdin(&self, src: String) -> Option<Self::Item> {
-    let lang = self.arg.lang.expect("must present");
+    use ast_grep_core::Language;
+    let lang = self.rule.language;
     let grep = lang.ast_grep(src);
-    let has_match = grep.root().find(&self.pattern).is_some();
-    has_match.then(|| MatchUnit {
-      path: PathBuf::from("STDIN"),
-      matcher: self.pattern.clone(),
-      grep,
-    })
+    let has_match = grep.root().find(&self.rule.matcher).is_some();
+    has_match.then(|| (PathBuf::from("STDIN"), grep))
   }
 }
 
-fn match_one_file(
-  printer: &impl Printer,
-  match_unit: &MatchUnit<impl Matcher<SgLang>>,
-  rewrite: &Option<Fixer<String>>,
+fn match_rule_on_file(
+  path: &Path,
+  matches: Vec<NodeMatch<StrDoc<SgLang>>>,
+  rule: &RuleConfig<SgLang>,
+  file_content: &String,
+  reporter: &impl Printer,
 ) -> Result<()> {
-  let MatchUnit {
-    path,
-    grep,
-    matcher,
-  } = match_unit;
-
-  let matches = Visitor::new(matcher).reentrant(false).visit(grep.root());
-  if let Some(rewrite) = rewrite {
-    let diffs = matches.map(|m| Diff::generate(m, matcher, rewrite));
-    printer.print_diffs(diffs, path)
+  let matches = matches.into_iter();
+  let file = SimpleFile::new(path.to_string_lossy(), file_content);
+  if let Some(fixer) = &rule.fixer {
+    let diffs = matches.map(|m| Diff::generate(m, &rule.matcher, fixer));
+    reporter.print_rule_diffs(diffs, path, rule)?;
   } else {
-    printer.print_matches(matches, path)
+    reporter.print_rule(matches, file, rule)?;
+  }
+  Ok(())
+}
+
+struct CombinedScan<'r> {
+  rules: Vec<&'r RuleConfig<SgLang>>,
+  kind_rule_mapping: Vec<Vec<usize>>,
+}
+
+impl<'r> CombinedScan<'r> {
+  fn new(rules: Vec<&'r RuleConfig<SgLang>>) -> Self {
+    let mut mapping = Vec::new();
+    for (idx, rule) in rules.iter().enumerate() {
+      for kind in &rule
+        .matcher
+        .potential_kinds()
+        .unwrap_or_else(|| panic!("rule `{}` must have kind", &rule.id))
+      {
+        // NOTE: common languages usually have about several hundred kinds
+        // from 200+ ~ 500+, it is okay to waste about 500 * 24 Byte vec size = 12kB
+        // see https://github.com/Wilfred/difftastic/tree/master/vendored_parsers
+        while mapping.len() <= kind {
+          mapping.push(vec![]);
+        }
+        mapping[kind].push(idx);
+      }
+    }
+    Self {
+      rules,
+      kind_rule_mapping: mapping,
+    }
+  }
+
+  fn find(&self, root: &AstGrep) -> bool {
+    for node in root.root().dfs() {
+      let kind = node.kind_id() as usize;
+      let Some(rule_idx) = self.kind_rule_mapping.get(kind) else {
+        continue;
+      };
+      for &idx in rule_idx {
+        let rule = &self.rules[idx];
+        if rule.matcher.match_node(node.clone()).is_some() {
+          return true;
+        }
+      }
+    }
+    false
+  }
+  fn scan<'a>(&self, root: &'a AstGrep) -> HashMap<usize, Vec<NodeMatch<'a, StrDoc<SgLang>>>> {
+    let mut results = HashMap::new();
+    for node in root.root().dfs() {
+      let kind = node.kind_id() as usize;
+      let Some(rule_idx) = self.kind_rule_mapping.get(kind) else {
+        continue;
+      };
+      for &idx in rule_idx {
+        let rule = &self.rules[idx];
+        let Some(ret) = rule.matcher.match_node(node.clone()) else {
+          continue;
+        };
+        let matches = results.entry(idx).or_insert_with(Vec::new);
+        matches.push(ret);
+      }
+    }
+    results
   }
 }
 
 #[cfg(test)]
 mod test {
   use super::*;
-  use ast_grep_language::SupportLang;
-  #[test]
-  fn test_run_with_pattern() {
-    let arg = RunArg {
-      pattern: "console.log".to_string(),
-      rewrite: None,
-      color: ColorArg::Never,
-      no_ignore: vec![],
-      stdin: false,
-      interactive: false,
-      lang: None,
-      json: false,
-      heading: Heading::Never,
-      debug_query: false,
-      update_all: false,
-      paths: vec![PathBuf::from(".")],
-    };
-    assert!(run_with_pattern(arg).is_ok())
+  use std::fs::File;
+  use std::io::Write;
+  use tempdir::TempDir;
+
+  const RULE: &str = r#"
+id: test
+message: Add your rule message here....
+severity: error # error, warning, hint, info
+language: Rust
+rule:
+  pattern: Some(123)
+"#;
+
+  pub fn create_test_files<'a>(
+    names_and_contents: impl IntoIterator<Item = (&'a str, &'a str)>,
+  ) -> TempDir {
+    let dir = TempDir::new("sgtest").unwrap();
+    for (name, contents) in names_and_contents {
+      let path = dir.path().join(name);
+      let mut file = File::create(path.clone()).unwrap();
+      file.write_all(contents.as_bytes()).unwrap();
+      file.sync_all().unwrap();
+    }
+    dir
   }
 
   #[test]
-  fn test_run_with_specific_lang() {
-    let arg = RunArg {
-      pattern: "Some(result)".to_string(),
-      rewrite: None,
+  fn test_run_with_config() {
+    let dir = create_test_files([("sgconfig.yml", "ruleDirs: [rules]")]);
+    std::fs::create_dir_all(dir.path().join("rules")).unwrap();
+    let mut file = File::create(dir.path().join("rules/test.yml")).unwrap();
+    file.write_all(RULE.as_bytes()).unwrap();
+    let mut file = File::create(dir.path().join("test.rs")).unwrap();
+    file
+      .write_all("fn test() { Some(123) }".as_bytes())
+      .unwrap();
+    file.sync_all().unwrap();
+    let arg = ScanArg {
+      config: Some(dir.path().join("sgconfig.yml")),
+      rule: None,
+      report_style: ReportStyle::Rich,
       color: ColorArg::Never,
       no_ignore: vec![],
       interactive: false,
-      lang: Some(SupportLang::Rust.into()),
       json: false,
-      heading: Heading::Never,
-      debug_query: false,
       update_all: false,
-      stdin: true,
       paths: vec![PathBuf::from(".")],
+      stdin: false,
+      format: None,
     };
-    assert!(run_with_pattern(arg).is_ok())
+    assert!(run_with_config(arg).is_ok());
   }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/utils.rs` & `ast_grep_cli-0.9.3/crates/cli/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/src/verify.rs` & `ast_grep_cli-0.9.3/crates/cli/src/verify.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/tests/common/mod.rs` & `ast_grep_cli-0.9.3/crates/cli/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/tests/run_test.rs` & `ast_grep_cli-0.9.3/crates/cli/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/tests/scan_test.rs` & `ast_grep_cli-0.9.3/crates/cli/tests/scan_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/crates/cli/tests/verify_test.rs` & `ast_grep_cli-0.9.3/crates/cli/tests/verify_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/pyproject.toml` & `ast_grep_cli-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-cli"
-version = "0.9.2"
+version = "0.9.3"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_cli-0.9.2/crates/cli/Cargo.lock` & `ast_grep_cli-0.9.3/crates/cli/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -122,15 +122,15 @@
  "similar",
  "tempdir",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "serde",
@@ -138,38 +138,38 @@
  "tempdir",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading 0.8.0",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "ast-grep-core",
  "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-c",
  "tree-sitter-cpp",
@@ -189,27 +189,27 @@
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "dashmap",
  "serde",
  "serde_json",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -270,15 +270,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "benches"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -1895,17 +1895,17 @@
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-python"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dda114f58048f5059dcf158aff691dffb8e113e6d2b50d94263fd68711975287"
+checksum = "f47ebd9cac632764b2f4389b08517bf2ef895431dd163eb562e3d2062cc23a14"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-ruby"
```

### Comparing `ast_grep_cli-0.9.2/README.md` & `ast_grep_cli-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/LICENSE` & `ast_grep_cli-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.9.2/PKG-INFO` & `ast_grep_cli-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-grep-cli
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.9.2 Classifier: Development
+Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.9.3 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Rust Classifier: Topic :: Security Classifier: Topic :: Software Development
 :: Quality Assurance Classifier: Topic :: Software Development Classifier:
 Topic :: Text Processing License-File: LICENSE License-File: LICENSE Summary:
 Structural Search and Rewrite code at large scale using precise AST pattern.
```

