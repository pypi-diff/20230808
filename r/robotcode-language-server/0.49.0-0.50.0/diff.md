# Comparing `tmp/robotcode_language_server-0.49.0.tar.gz` & `tmp/robotcode_language_server-0.50.0.tar.gz`

## Comparing `robotcode_language_server-0.49.0.tar` & `robotcode_language_server-0.50.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    58866 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    71453 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    91023 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24170 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.49.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    58866 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    71453 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    90899 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24170 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.50.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,17 +67,15 @@
     pipe: Optional[str],
     paths: Sequence[Path],
 ) -> None:
     """Run Robot Framework Language Server."""
 
     profile: Optional[RobotBaseProfile] = None
 
-    config_files, root_folder, _ = get_config_files(
-        paths, app.config.config_files, raise_on_error=False, verbose_callback=app.verbose
-    )
+    config_files, root_folder, _ = get_config_files(paths, app.config.config_files, verbose_callback=app.verbose)
     if root_folder:
         os.chdir(root_folder)
 
     try:
         profile = (
             load_config_from_path(*config_files)
             .combine_profiles(*(app.config.profiles or []), verbose_callback=app.verbose)
```

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     CodeActionParams,
     Command,
     Range,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
 from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import HasCodeActionKinds, language_id_filter
+from robotcode.language_server.common.decorators import CODE_ACTION_KINDS_ATTR, HasCodeActionKinds, language_id_filter
 from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
@@ -45,15 +45,15 @@
     def extend_capabilities(self, capabilities: ServerCapabilities) -> None:
         if len(self.collect):
             code_action_kinds = list(
                 chain(
                     *[
                         cast(HasCodeActionKinds, e).__code_action_kinds__
                         for e in self.collect
-                        if isinstance(e, HasCodeActionKinds)
+                        if hasattr(e, CODE_ACTION_KINDS_ATTR)
                     ]
                 )
             )
 
             capabilities.code_action_provider = CodeActionOptions(
                 code_action_kinds=code_action_kinds if code_action_kinds else None,
                 resolve_provider=len(self.resolve) > 0,
```

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ErrorCodes,
     ExecuteCommandOptions,
     ExecuteCommandParams,
     LSPAny,
     ServerCapabilities,
 )
 from robotcode.jsonrpc2.protocol import JsonRPCErrorException, rpc_method
-from robotcode.language_server.common.decorators import IsCommand, get_command_name
+from robotcode.language_server.common.decorators import get_command_name, is_command
 from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 
@@ -56,15 +56,15 @@
         return command
 
     def register_all(self, instance: object) -> None:
         all_methods = [
             getattr(instance, k) for k, v in type(instance).__dict__.items() if callable(v) and not k.startswith("_")
         ]
         for method in all_methods:
-            if isinstance(method, IsCommand):
+            if is_command(method):
                 self.register(cast(_FUNC_TYPE, method))
 
     def get_command_name(self, callback: _FUNC_TYPE, name: Optional[str] = None) -> str:
         name = name or get_command_name(callback)
 
         return f"{self.PREFIX}.{name}"
```

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,21 @@
     InsertReplaceEdit,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
     TextEdit,
 )
 from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import HasAllCommitCharacters, HasTriggerCharacters, language_id_filter
+from robotcode.language_server.common.decorators import (
+    ALL_COMMIT_CHARACTERS_ATTR,
+    TRIGGER_CHARACTERS_ATTR,
+    HasAllCommitCharacters,
+    HasTriggerCharacters,
+    language_id_filter,
+)
 from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
@@ -47,25 +53,25 @@
     def extend_capabilities(self, capabilities: ServerCapabilities) -> None:
         if len(self.collect):
             trigger_chars = list(
                 chain(
                     *[
                         cast(HasTriggerCharacters, e).__trigger_characters__
                         for e in self.collect
-                        if isinstance(e, HasTriggerCharacters)
+                        if hasattr(e, TRIGGER_CHARACTERS_ATTR)
                     ]
                 )
             )
 
             commit_chars = list(
                 chain(
                     *[
                         cast(HasAllCommitCharacters, e).__all_commit_characters__
                         for e in self.collect
-                        if isinstance(e, HasAllCommitCharacters)
+                        if hasattr(e, ALL_COMMIT_CHARACTERS_ATTR)
                     ]
                 )
             )
             capabilities.completion_provider = CompletionOptions(
                 trigger_characters=trigger_chars if trigger_chars else None,
                 all_commit_characters=commit_chars if commit_chars else None,
                 resolve_provider=len(self.resolve) > 0,
```

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Range,
     ServerCapabilities,
     TextDocumentFilterType1,
     TextDocumentIdentifier,
 )
 from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.language_server.common.decorators import (
-    HasLanguageId,
+    LANGUAGE_ID_ATTR,
     language_id_filter,
 )
 from robotcode.language_server.common.has_extend_capabilities import (
     HasExtendCapabilities,
 )
 from robotcode.language_server.common.parts.protocol_part import (
     LanguageServerProtocolPart,
@@ -48,16 +48,16 @@
     ) -> Optional[List[InlineValue]]:
         ...
 
     def extend_capabilities(self, capabilities: ServerCapabilities) -> None:
         if len(self.collect):
             document_filters: DocumentSelector = []
             for e in self.collect:
-                if isinstance(e, HasLanguageId):
-                    for lang_id in e.__language_id__:  # type: ignore
+                if hasattr(e, LANGUAGE_ID_ATTR):
+                    for lang_id in getattr(e, LANGUAGE_ID_ATTR):
                         document_filters.append(TextDocumentFilterType1(language=lang_id))
             capabilities.inline_value_provider = InlineValueRegistrationOptions(
                 work_done_progress=True,
                 document_selector=document_filters if document_filters else None,
             )
 
     @rpc_method(name="textDocument/inlineValue", param_type=InlineValueParams)
```

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,21 @@
     SignatureHelp,
     SignatureHelpContext,
     SignatureHelpOptions,
     SignatureHelpParams,
     TextDocumentIdentifier,
 )
 from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.language_server.common.decorators import HasRetriggerCharacters, HasTriggerCharacters, language_id_filter
+from robotcode.language_server.common.decorators import (
+    RETRIGGER_CHARACTERS_ATTR,
+    TRIGGER_CHARACTERS_ATTR,
+    HasRetriggerCharacters,
+    HasTriggerCharacters,
+    language_id_filter,
+)
 from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.text_document import TextDocument
 
 from .protocol_part import LanguageServerProtocolPart
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
@@ -41,25 +47,25 @@
     def extend_capabilities(self, capabilities: ServerCapabilities) -> None:
         if len(self.collect):
             trigger_chars = list(
                 chain(
                     *[
                         cast(HasTriggerCharacters, e).__trigger_characters__
                         for e in self.collect
-                        if isinstance(e, HasTriggerCharacters)
+                        if hasattr(e, TRIGGER_CHARACTERS_ATTR)
                     ]
                 )
             )
 
             retrigger_chars = list(
                 chain(
                     *[
                         cast(HasRetriggerCharacters, e).__retrigger_characters__
                         for e in self.collect
-                        if isinstance(e, HasRetriggerCharacters)
+                        if hasattr(e, RETRIGGER_CHARACTERS_ATTR)
                     ]
                 )
             )
 
             capabilities.signature_help_provider = SignatureHelpOptions(
                 trigger_characters=trigger_chars if trigger_chars else None,
                 retrigger_characters=retrigger_chars if retrigger_chars else None,
```

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,17 +252,14 @@
             method = getattr(self, method_name)
             if callable(method):
                 yield cast(_CompleteMethod, method)
         for base in cls.__bases__:
             async for m in self._find_methods(base):
                 yield m
 
-    @language_id("robotframework")
-    @trigger_characters([" ", "*", "\t", ".", "/"])
-    # @all_commit_characters(['\n'])
     async def collect(
         self, position: Position, context: Optional[CompletionContext]
     ) -> Union[List[CompletionItem], CompletionList, None]:
         result_nodes = await get_nodes_at_position(self.model, position)
 
         result_nodes.reverse()
```

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.50.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/.gitignore` & `robotcode_language_server-0.50.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/LICENSE.txt` & `robotcode_language_server-0.50.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/README.md` & `robotcode_language_server-0.50.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.49.0/pyproject.toml` & `robotcode_language_server-0.50.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.49.0",
-  "robotcode==0.49.0",
+  "robotcode-jsonrpc2==0.50.0",
+  "robotcode==0.50.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.49.0/PKG-INFO` & `robotcode_language_server-0.50.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.49.0
+Version: 0.50.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.49.0
-Requires-Dist: robotcode==0.49.0
+Requires-Dist: robotcode-jsonrpc2==0.50.0
+Requires-Dist: robotcode==0.50.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

