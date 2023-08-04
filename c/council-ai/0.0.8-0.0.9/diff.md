# Comparing `tmp/council_ai-0.0.8.tar.gz` & `tmp/council_ai-0.0.9.tar.gz`

## Comparing `council_ai-0.0.8.tar` & `council_ai-0.0.9.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.8/Makefile
--rw-r--r--   0        0        0   333985 2020-02-02 00:00:00.000000 council_ai-0.0.8/council_banner.png
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.8/engine_flow.png
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 council_ai-0.0.8/env.example
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.8/requirements.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agent_tests/__init__.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agent_tests/agent_tests.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agents/__init__.py
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agents/agent.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agents/agent_chain.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agents/agent_result.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/chains/__init__.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/chains/chain.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/contexts/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/contexts/cancellation_token.py
--rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/contexts/execution_context.py
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/contexts/messages.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/basic_controller.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/controller_base.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/execution_unit.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/llm_controller.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/evaluators/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/evaluators/basic_evaluator.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/evaluators/evaluator_base.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/__init__.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/azure_llm.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/azure_llm_configuration.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/llm_base.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/llm_configuration_base.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/llm_exception.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/llm_message.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/openai_chat_completions_llm.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/openai_llm.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/openai_llm_configuration.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/mocks/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/prompt/__init__.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/prompt/prompt_builder.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/budget.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/errrors.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/if_runner.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/loop_runner_base.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/parallel.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/parallel_for.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/runner_base.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/runner_context.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/runner_executor.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/sequential.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/skill_runner_base.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/scorers/__init__.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/scorers/llm_similarity_scorer.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/scorers/scorer_base.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/scorers/scorer_exception.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/__init__.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/llm_skill.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/skill_base.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/__init__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_news_skill.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_search_skill.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/context_provider.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/google_news.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/google_search.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/schemas.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/__init__.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/env.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/option.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/parameter.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/result.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/.gitignore
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/.readthedocs.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/Makefile
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/README.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/docker-compose.yaml
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/dockerfile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/make.bat
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/requirements.txt
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/conf.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/index.rst
--rw-r--r--   0        0        0    33816 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/_static/Council_RGB_Horizontal_DarkBKG_Gradient.png
--rw-r--r--   0        0        0    35327 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/_static/Council_RGB_Horizontal_LightBKG_Gradient.png
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/_static/council.css
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/contributing/contributing.md
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/getting_started/first_example.ipynb
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/getting_started/installation.md
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/introduction/engine_flow.png
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/introduction/key_concepts.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/introduction/key_features.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/introduction/welcome.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/agents.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/chains.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/evaluators.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm.rst
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/scorers.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/utils.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/agents/agent.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/agents/agent_result.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/chains/chain.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/agent_context.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chain_context.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chain_history.rst
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chat_history.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chat_message.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chat_message_kind.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/iteration_context.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/message_collection.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/scored_chat_message.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/skill_context.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers/basic_controller.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers/controller_base.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers/execution_unit.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers/llm_controller.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/evaluators/basic_evaluator.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/evaluators/evaluator_base.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/evaluators/llm_evaluator.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/azure_llm.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/azure_llm_configuration.rst
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/llm_base.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/llm_configuration_base.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/llm_message.rst
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/llm_message_role.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/openai_llm.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/openai_llm_configuration.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/budget.rst
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/errors.rst
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/if.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/loop_runner_base.rst
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/parallel.rst
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/parallel_for.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/runner_base.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/runner_executor.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/sequential.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/skill_runner_base.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/scorers/llm_similarity_scorer.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/scorers/scorer_base.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/scorers/scorer_exception.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/google.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/llm_skill.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/skill_base.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/google/google_news_skill.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/google/google_search_skill.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/utils/option.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/utils/option_exception.rst
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/tutorials/financial.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/tutorials/research.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/tutorials/social.md
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/use_cases/langchain_llm_integration.ipynb
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/use_cases/llamaindex_integration.ipynb
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/use_cases/multi_chain_agent.ipynb
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.8/stubs/GoogleNews.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.8/LICENSE
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 council_ai-0.0.8/README.md
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 council_ai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.9/Makefile
+-rw-r--r--   0        0        0   333985 2020-02-02 00:00:00.000000 council_ai-0.0.9/council_banner.png
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 council_ai-0.0.9/env.example
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 council_ai-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/agent_tests/__init__.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/agent_tests/agent_tests.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/agents/__init__.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/agents/agent.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/agents/agent_chain.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/agents/agent_result.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/chains/__init__.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/chains/chain.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/contexts/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/contexts/cancellation_token.py
+-rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/contexts/execution_context.py
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/contexts/messages.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/controllers/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/controllers/basic_controller.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/controllers/controller_base.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/controllers/execution_unit.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/controllers/llm_controller.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/evaluators/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/evaluators/basic_evaluator.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/evaluators/evaluator_base.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/__init__.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/azure_llm.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/azure_llm_configuration.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/llm_base.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/llm_configuration_base.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/llm_exception.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/llm_message.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/openai_chat_completions_llm.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/openai_llm.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/openai_llm_configuration.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/llm/openai_token_counter.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/mocks/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/prompt/__init__.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/prompt/prompt_builder.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/__init__.py
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/budget.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/errrors.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/if_runner.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/loop_runner_base.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/parallel.py
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/parallel_for.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/runner_base.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/runner_context.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/runner_executor.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/sequential.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/skill_runner_base.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/runners/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/scorers/__init__.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/scorers/llm_similarity_scorer.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/scorers/scorer_base.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/scorers/scorer_exception.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/__init__.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/llm_skill.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/skill_base.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/google/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/google/google_news_skill.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/google/google_search_skill.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/google/google_context/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/google/google_context/context_provider.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/google/google_context/google_news.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/google/google_context/google_search.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/skills/google/google_context/schemas.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/utils/__init__.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/utils/env.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/utils/option.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/utils/parameter.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 council_ai-0.0.9/council/utils/result.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/.gitignore
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/README.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/docker-compose.yaml
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/dockerfile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/conf.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/index.rst
+-rw-r--r--   0        0        0    33816 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/_static/Council_RGB_Horizontal_DarkBKG_Gradient.png
+-rw-r--r--   0        0        0    35327 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/_static/Council_RGB_Horizontal_LightBKG_Gradient.png
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/_static/council.css
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/contributing/contributing.md
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/getting_started/first_example.ipynb
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/getting_started/installation.md
+-rw-r--r--   0        0        0   188182 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/introduction/engine_flow.png
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/introduction/key_concepts.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/introduction/key_features.md
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/introduction/welcome.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/agents.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/chains.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/controllers.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/evaluators.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm.rst
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/scorers.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/skills.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/utils.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/agents/agent.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/agents/agent_result.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/chains/chain.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/agent_context.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/chain_context.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/chain_history.rst
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/chat_history.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/chat_message.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/chat_message_kind.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/iteration_context.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/message_collection.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/scored_chat_message.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/contexts/skill_context.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/controllers/basic_controller.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/controllers/controller_base.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/controllers/execution_unit.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/controllers/llm_controller.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/evaluators/basic_evaluator.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/evaluators/evaluator_base.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/evaluators/llm_evaluator.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm/azure_llm.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm/azure_llm_configuration.rst
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm/llm_base.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm/llm_configuration_base.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm/llm_message.rst
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm/llm_message_role.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm/openai_llm.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/llm/openai_llm_configuration.rst
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/budget.rst
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/errors.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/if.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/loop_runner_base.rst
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/parallel.rst
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/parallel_for.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/runner_base.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/runner_executor.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/sequential.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/runners/skill_runner_base.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/scorers/llm_similarity_scorer.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/scorers/scorer_base.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/scorers/scorer_exception.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/skills/google.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/skills/llm_skill.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/skills/skill_base.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/skills/google/google_news_skill.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/skills/google/google_search_skill.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/utils/option.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/reference/utils/option_exception.rst
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/tutorials/financial.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/tutorials/research.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/tutorials/social.md
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/use_cases/langchain_llm_integration.ipynb
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/use_cases/llamaindex_integration.ipynb
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 council_ai-0.0.9/docs/source/use_cases/multi_chain_agent.ipynb
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.9/stubs/GoogleNews.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 council_ai-0.0.9/README.md
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 council_ai-0.0.9/PKG-INFO
```

### Comparing `council_ai-0.0.8/council_banner.png` & `council_ai-0.0.9/council_banner.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/agent_tests/agent_tests.py` & `council_ai-0.0.9/council/agent_tests/agent_tests.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/agents/agent.py` & `council_ai-0.0.9/council/agents/agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import List, Optional
 
 from council.chains import Chain
 from council.contexts import AgentContext, ChatHistory
-from council.controllers import ControllerBase, BasicController
+from council.controllers import ControllerBase, BasicController, ExecutionUnit
 from council.evaluators import BasicEvaluator, EvaluatorBase
 from council.runners import Budget, new_runner_executor
 from council.skills import SkillBase
 from .agent_result import AgentResult
 from ..runners.budget import InfiniteBudget
 
 logger = logging.getLogger(__name__)
@@ -62,36 +62,40 @@
                 logger.info(f'message="agent iteration started" iteration="{len(context.evaluationHistory)+1}"')
                 plan = self.controller.get_plan(context=context, chains=self.chains, budget=budget)
                 logger.debug(f'message="agent controller returned {len(plan)} execution plan(s)"')
 
                 if len(plan) == 0:
                     return AgentResult()
                 for unit in plan:
-                    chain = unit.chain
-                    budget = unit.budget
-                    logger.info(f'message="chain execution started" chain="{chain.name}" execution_unit="{unit.name}"')
-                    chain_context = context.new_chain_context(unit.name)
-                    if unit.initial_state is not None:
-                        chain_context.current.append(unit.initial_state)
-                    chain.execute(chain_context, budget)
-                    logger.info(f'message="chain execution ended" chain="{chain.name}" execution_unit="{unit.name}"')
+                    budget = self._execute_unit(context, unit)
 
                 result = self.evaluator.execute(context, budget)
                 context.evaluationHistory.append(result)
 
                 result = self.controller.select_responses(context)
                 logger.debug("controller selected %d responses", len(result))
                 if len(result) > 0:
                     return AgentResult(messages=result)
 
             return AgentResult()
         finally:
             logger.info('message="agent execution ended"')
             executor.shutdown(wait=False, cancel_futures=True)
 
+    def _execute_unit(self, context: AgentContext, unit: ExecutionUnit) -> Budget:
+        chain = unit.chain
+        budget = unit.budget
+        logger.info(f'message="chain execution started" chain="{chain.name}" execution_unit="{unit.name}"')
+        chain_context = context.new_chain_context(unit.name)
+        if unit.initial_state is not None:
+            chain_context.current.append(unit.initial_state)
+        chain.execute(chain_context, budget)
+        logger.info(f'message="chain execution ended" chain="{chain.name}" execution_unit="{unit.name}"')
+        return budget
+
     @staticmethod
     def from_skill(skill: SkillBase, chain_description: Optional[str] = None) -> "Agent":
         """
         Helper function to create a new agent with a  :class:`.BasicController`, a
             :class:`.BasicEvaluator` and a single :class:`.SkillBase` wrapped into a :class:`.Chain`
 
         Parameters:
```

### Comparing `council_ai-0.0.8/council/agents/agent_chain.py` & `council_ai-0.0.9/council/agents/agent_chain.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/agents/agent_result.py` & `council_ai-0.0.9/council/agents/agent_result.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/chains/chain.py` & `council_ai-0.0.9/council/chains/chain.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/contexts/execution_context.py` & `council_ai-0.0.9/council/contexts/execution_context.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/contexts/messages.py` & `council_ai-0.0.9/council/contexts/messages.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/controllers/basic_controller.py` & `council_ai-0.0.9/council/controllers/basic_controller.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/controllers/controller_base.py` & `council_ai-0.0.9/council/controllers/controller_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/controllers/execution_unit.py` & `council_ai-0.0.9/council/controllers/execution_unit.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/controllers/llm_controller.py` & `council_ai-0.0.9/council/controllers/llm_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         messages = [
             LLMMessage.system_message("\n".join(task_description)),
             LLMMessage.user_message(
                 f"what are most relevant categories for: {context.chatHistory.try_last_user_message.unwrap().message}"
             ),
         ]
 
-        response = self._llm.post_chat_request(messages)[0]
+        llm_result = self._llm.post_chat_request(messages)
+        response = llm_result.first_choice
         logger.debug(f"llm response: {response}")
 
         parsed = [self.parse_line(line, chains) for line in response.splitlines()]
         filtered = [r.unwrap() for r in parsed if r.is_some() and r.unwrap()[1] > self._response_threshold]
         if (filtered is None) or (len(filtered) == 0):
             return []
```

### Comparing `council_ai-0.0.8/council/evaluators/basic_evaluator.py` & `council_ai-0.0.9/council/evaluators/basic_evaluator.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/evaluators/evaluator_base.py` & `council_ai-0.0.9/council/evaluators/evaluator_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/evaluators/llm_evaluator.py` & `council_ai-0.0.9/council/evaluators/llm_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
         """
         # Build prompt to send to the inner LLM
         responses = [skill_message.message for skill_message in skill_messages]
         prompt = self.__build_prompt(query.message, responses=responses)
 
         # Send prompt to inner LLM
         messages = [LLMMessage.system_message(prompt)]
-        llm_response = self.llm.post_chat_request(messages=messages)[0]
+        result = self.llm.post_chat_request(messages=messages)
+        llm_response = result.first_choice
 
         # Parse LLM response with the score for each message we want to score
         scores = [self.__parse_eval(line) for line in llm_response.split("\n")]
 
         agent_messages = []
         for skill_message, score in filter(lambda tuple: tuple[1].is_some(), zip(skill_messages, scores)):
             agent_message = ScoredChatMessage(
```

### Comparing `council_ai-0.0.8/council/llm/azure_llm.py` & `council_ai-0.0.9/council/llm/azure_llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,13 +30,13 @@
     """
     Represents an OpenAI language model hosted on Azure.
     """
 
     config: AzureLLMConfiguration
 
     def __init__(self, config: AzureLLMConfiguration):
-        super().__init__(config, AzureOpenAIChatCompletionsModelProvider(config).post_request)
+        super().__init__(config, AzureOpenAIChatCompletionsModelProvider(config).post_request, None)
 
     @staticmethod
     def from_env() -> "AzureLLM":
         config: AzureLLMConfiguration = AzureLLMConfiguration.from_env()
         return AzureLLM(config)
```

### Comparing `council_ai-0.0.8/council/llm/azure_llm_configuration.py` & `council_ai-0.0.9/council/llm/azure_llm_configuration.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/llm/llm_configuration_base.py` & `council_ai-0.0.9/council/llm/llm_configuration_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/llm/llm_message.py` & `council_ai-0.0.9/council/llm/llm_message.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import abc
 from enum import Enum
 from typing import Optional, List, Iterable
 
 from council.contexts import ChatMessage, ChatMessageKind
 
 
 class LLMMessageRole(str, Enum):
@@ -33,58 +34,70 @@
         role (LLMMessageRole): the role/persona the message is coming from. Could be either user, system or assistant
         content (str): the message content
     """
 
     _role: LLMMessageRole
     _content: str
 
-    def __init__(self, role: LLMMessageRole, content: str):
+    def __init__(self, role: LLMMessageRole, content: str, name: Optional[str] = None):
         """Initialize a new instance"""
         self._role = role
         self._content = content
+        self._name = name
 
     @staticmethod
-    def system_message(content: str) -> "LLMMessage":
+    def system_message(content: str, name: Optional[str] = None) -> "LLMMessage":
         """
         Create a new system message
 
         Parameters:
             content (str): the message content
+            name (str): name of the author of this message
         """
-        return LLMMessage(role=LLMMessageRole.System, content=content)
+        return LLMMessage(role=LLMMessageRole.System, content=content, name=name)
 
     @staticmethod
-    def user_message(content: str) -> "LLMMessage":
+    def user_message(content: str, name: Optional[str] = None) -> "LLMMessage":
         """
         Create a new user message
 
         Parameters:
             content (str): the message content
+            name (str): name of the author of this message
         """
-        return LLMMessage(role=LLMMessageRole.User, content=content)
+        return LLMMessage(role=LLMMessageRole.User, content=content, name=name)
 
     @staticmethod
-    def assistant_message(content: str) -> "LLMMessage":
+    def assistant_message(content: str, name: Optional[str] = None) -> "LLMMessage":
         """
         Create a new assistant message
 
         Parameters:
             content (str): the message content
+            name (str): name of the author of this message
         """
-        return LLMMessage(role=LLMMessageRole.Assistant, content=content)
+        return LLMMessage(role=LLMMessageRole.Assistant, content=content, name=name)
 
     def dict(self) -> dict[str, str]:
-        return {"role": self._role.value, "content": self._content}
+        result = {"role": self._role.value, "content": self._content}
+        if self._name is not None:
+            result["name"] = self._name
+        return result
 
     @property
     def content(self) -> str:
         """Retrieve the content of this instance"""
         return self._content
 
     @property
+    def name(self) -> Optional[str]:
+        """Retrieve the name authoring the content of this instance"""
+        return self._name
+
+    @property
     def role(self) -> LLMMessageRole:
         """Retrieve the role of this instance"""
         return self._role
 
     def is_of_role(self, role: LLMMessageRole) -> bool:
         """Check the role of this instance"""
         return self._role == role
@@ -98,7 +111,26 @@
             return LLMMessage.assistant_message(chat_message.message)
         return None
 
     @staticmethod
     def from_chat_messages(messages: Iterable[ChatMessage]) -> List["LLMMessage"]:
         m = map(LLMMessage.from_chat_message, messages)
         return [msg for msg in m if msg is not None]
+
+
+class LLMessageTokenCounterBase(abc.ABC):
+    @abc.abstractmethod
+    def count_messages_token(self, messages: List[LLMMessage]) -> int:
+        """
+        Counts the total number of tokens in a list of LLM messages, including assistant tokens.
+
+        Args:
+            messages (List[LLMMessage]): A list of LLMMessage objects representing the messages.
+
+        Returns:
+            int: The total number of tokens, including assistant tokens.
+
+        Raises:
+            LLMTokenLimitException: If a token limit is set (0 < limit < result) and the token count exceeds the limit.
+
+        """
+        pass
```

### Comparing `council_ai-0.0.8/council/llm/openai_chat_completions_llm.py` & `council_ai-0.0.9/council/llm/openai_chat_completions_llm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 import httpx
 
-from typing import List, Any, Protocol, Sequence
+from typing import List, Any, Protocol, Sequence, Optional
 
 from . import LLMConfigurationBase
-from .llm_message import LLMMessage
+from .llm_message import LLMMessage, LLMessageTokenCounterBase
 from .llm_exception import LLMException
-from .llm_base import LLMBase
+from .llm_base import LLMBase, LLMResult
+from ..runners import Consumption
 
 logger = logging.getLogger(__name__)
 
 
 class Provider(Protocol):
     def __call__(self, payload: dict[str, Any]) -> httpx.Response:
         ...
@@ -66,14 +67,18 @@
         self._completion = completion_tokens
         self._prompt = prompt_tokens
         self._total = total_tokens
 
     def __str__(self) -> str:
         return f'prompt_tokens="{self._prompt}" total_tokens="{self._total}" completion_tokens="{self._completion}"'
 
+    @property
+    def total_tokens(self) -> int:
+        return self._total
+
     @staticmethod
     def from_dict(obj: Any) -> "Usage":
         _completion_tokens = int(obj.get("completion_tokens"))
         _prompt_tokens = int(obj.get("prompt_tokens"))
         _total_tokens = int(obj.get("total_tokens"))
         return Usage(_completion_tokens, _prompt_tokens, _total_tokens)
 
@@ -124,26 +129,30 @@
 class OpenAIChatCompletionsModel(LLMBase):
     """
     Represents an OpenAI language model hosted on Azure.
     """
 
     config: LLMConfigurationBase
 
-    def __init__(self, config: LLMConfigurationBase, provider: Provider):
+    def __init__(
+        self, config: LLMConfigurationBase, provider: Provider, token_counter: Optional[LLMessageTokenCounterBase]
+    ):
+        super().__init__(token_counter)
         self.config = config
         self._provider = provider
 
-    def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> List[str]:
+    def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> LLMResult:
         payload = self.config.build_default_payload()
         payload["messages"] = [message.dict() for message in messages]
         for key, value in kwargs.items():
             payload[key] = value
 
         r = self._post_request(payload)
-        return [c.message.content for c in r.choices]
+        consumption = Consumption(r.usage.total_tokens, "token", r.model)
+        return LLMResult(choices=[c.message.content for c in r.choices], consumptions=[consumption])
 
     def _post_request(self, payload) -> OpenAIChatCompletionsResult:
         logger.debug(f'message="Sending chat GPT completions request" payload="{payload}"')
         response = self._provider.__call__(payload)
         if response.status_code != httpx.codes.OK:
             raise LLMException(f"Wrong status code: {response.status_code}. Reason: {response.text}")
```

### Comparing `council_ai-0.0.8/council/llm/openai_llm.py` & `council_ai-0.0.9/council/llm/openai_llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import httpx
 
 from typing import Any, Optional
 
-from . import OpenAIChatCompletionsModel
+from . import OpenAIChatCompletionsModel, OpenAITokenCounter
 from .openai_llm_configuration import OpenAILLMConfiguration
 
 
 class OpenAIChatCompletionsModelProvider:
     """
     Represents an OpenAI language model hosted on Azure.
     """
@@ -29,13 +29,17 @@
     """
     Represents an OpenAI large language model hosted on OpenAI.
     """
 
     config: OpenAILLMConfiguration
 
     def __init__(self, config: OpenAILLMConfiguration):
-        super().__init__(config, OpenAIChatCompletionsModelProvider(config).post_request)
+        super().__init__(
+            config,
+            OpenAIChatCompletionsModelProvider(config).post_request,
+            token_counter=OpenAITokenCounter.from_model(config.model.unwrap_or("")),
+        )
 
     @staticmethod
     def from_env(model: Optional[str] = None) -> "OpenAILLM":
         config: OpenAILLMConfiguration = OpenAILLMConfiguration.from_env(model=model)
         return OpenAILLM(config)
```

### Comparing `council_ai-0.0.8/council/llm/openai_llm_configuration.py` & `council_ai-0.0.9/council/llm/openai_llm_configuration.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/mocks/__init__.py` & `council_ai-0.0.9/council/mocks/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 import time
 import random
 from typing import List, Any, Callable, Optional, Protocol
 
 from council.agents import Agent, AgentResult
 from council.contexts import AgentContext, ScoredChatMessage, SkillContext, ChatMessage
-from council.llm import LLMBase, LLMMessage
+from council.llm import LLMBase, LLMMessage, LLMessageTokenCounterBase, LLMTokenLimitException, LLMResult
 from council.runners import Budget
 from council.scorers import ScorerBase
 from council.skills import SkillBase
 
 
 class LLMMessagesToStr(Protocol):
     def __call__(self, messages: List[LLMMessage]) -> List[str]:
         ...
 
 
 def llm_message_content_to_str(messages: List[LLMMessage]) -> List[str]:
     return [msg.content for msg in messages]
 
 
+class MockTokenCounter(LLMessageTokenCounterBase):
+    def __init__(self, limit: int = -1):
+        self._limit = limit
+
+    def count_messages_token(self, messages: List[LLMMessage]) -> int:
+        result = 0
+        for msg in messages:
+            result += len(msg.content)
+
+        if 0 < self._limit < result:
+            raise LLMTokenLimitException(token_count=result, limit=self._limit, model="mock")
+        return result
+
+
 class MockSkill(SkillBase):
     def __init__(self, name: str = "mock", action: Optional[Callable[[SkillContext, Budget], ChatMessage]] = None):
         super().__init__(name)
         self._action = action if action is not None else self.empty_message
 
     def execute(self, context: SkillContext, budget: Budget) -> ChatMessage:
         return self._action(context, budget)
@@ -31,21 +45,22 @@
         return self.build_success_message("")
 
     def set_action_custom_message(self, message: str) -> None:
         self._action = lambda context, budget: self.build_success_message(message)
 
 
 class MockLLM(LLMBase):
-    def __init__(self, action: Optional[LLMMessagesToStr] = None):
+    def __init__(self, action: Optional[LLMMessagesToStr] = None, token_limit: int = -1):
+        super().__init__(token_counter=MockTokenCounter(token_limit))
         self._action = action
 
-    def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> List[str]:
+    def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> LLMResult:
         if self._action is not None:
-            return self._action(messages)
-        return [f"{self.__class__.__name__}"]
+            return LLMResult(choices=self._action(messages))
+        return LLMResult(choices=[f"{self.__class__.__name__}"])
 
     @staticmethod
     def from_responses(responses: List[str]) -> "MockLLM":
         return MockLLM(action=(lambda x: responses))
 
     @staticmethod
     def from_response(response: str) -> "MockLLM":
```

### Comparing `council_ai-0.0.8/council/prompt/prompt_builder.py` & `council_ai-0.0.9/council/prompt/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/runners/__init__.py` & `council_ai-0.0.9/council/runners/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .errrors import RunnerError, RunnerTimeoutError, RunnerSkillError, RunnerPredicateError, RunnerGeneratorError
 from .runner_context import RunnerContext
-from .budget import Budget
+from .budget import Consumption, ConsumptionEvent, Budget
 from .types import RunnerPredicate, RunnerGenerator
 from .runner_executor import RunnerExecutor, new_runner_executor
 from .runner_base import RunnerBase
 from .skill_runner_base import SkillRunnerBase
 from .sequential import Sequential
 from .parallel import Parallel
 from .if_runner import If
```

### Comparing `council_ai-0.0.8/council/runners/errrors.py` & `council_ai-0.0.9/council/runners/errrors.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/runners/if_runner.py` & `council_ai-0.0.9/council/runners/if_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,10 @@
         executor: RunnerExecutor,
     ) -> None:
         try:
             result = self.predicate(context.make_chain_context(), context.budget.remaining())
         except Exception as e:
             context.append(ChatMessage.skill("IfRunner", f"predicate raised exception: {e}", is_error=True))
             raise RunnerPredicateError from e
+
         if result:
             self.runner.run(context, executor)
```

### Comparing `council_ai-0.0.8/council/runners/parallel.py` & `council_ai-0.0.9/council/runners/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,12 @@
     ) -> None:
         contexts = [(runner, context.fork()) for runner in self.runners]
 
         # Seems like it is a bad idea using lambda as the function in submit,
         # which results into inconsistent invocation (wrong arguments)
         fs = [executor.submit(runner.run, inner, executor) for (runner, inner) in contexts]
         try:
-            dones, not_dones = futures.wait(fs, context.budget.remaining().duration, futures.FIRST_EXCEPTION)
+            dones, not_dones = futures.wait(fs, context.budget.remaining_duration, futures.FIRST_EXCEPTION)
             self.rethrow_if_exception(dones)
         finally:
             context.merge([context for (_, context) in contexts])
             [f.cancel() for f in fs]
```

### Comparing `council_ai-0.0.8/council/runners/parallel_for.py` & `council_ai-0.0.9/council/runners/parallel_for.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         all_fs = []
         try:
             for batch in batched(self._generate(chain_context, context.budget.remaining()), self._parallelism):
                 inner = [context.fork() for _ in batch]
                 inner_contexts.extend(inner)
                 fs = [executor.submit(self._run_skill, inner, iteration) for (inner, iteration) in zip(inner, batch)]
                 all_fs.extend(fs)
-                dones, not_dones = futures.wait(fs, context.budget.remaining().duration, futures.FIRST_EXCEPTION)
+                dones, not_dones = futures.wait(fs, context.budget.remaining_duration, futures.FIRST_EXCEPTION)
                 self.rethrow_if_exception(dones)
         finally:
             [f.cancel() for f in all_fs]
             context.merge(inner_contexts)
 
     def _run_skill(self, context: RunnerContext, iteration: IterationContext):
         index = iteration.index
```

### Comparing `council_ai-0.0.8/council/runners/runner_base.py` & `council_ai-0.0.9/council/runners/runner_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/runners/runner_context.py` & `council_ai-0.0.9/council/runners/runner_context.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/runners/sequential.py` & `council_ai-0.0.9/council/runners/sequential.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/runners/skill_runner_base.py` & `council_ai-0.0.9/council/runners/skill_runner_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def run_skill(self, context: RunnerContext, executor: RunnerExecutor) -> None:
         """
         Run the skill in a different thread, and await for completion
         """
         future = executor.submit(self.run_in_current_thread, context, IterationContext.empty())
         try:
-            future.result(timeout=context.budget.remaining().duration)
+            future.result(timeout=context.budget.remaining_duration)
         finally:
             future.cancel()
 
     def run_in_current_thread(self, context: RunnerContext, iteration_context: Option[IterationContext]) -> None:
         """
         Run the skill in the current thread
         """
```

### Comparing `council_ai-0.0.8/council/scorers/llm_similarity_scorer.py` & `council_ai-0.0.9/council/scorers/llm_similarity_scorer.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     def to_dict(self) -> Dict[str, Any]:
         result = super().to_dict()
         result["expected"] = self._expected
         return result
 
     def _score(self, message: ChatMessage) -> float:
         messages = self._build_messages(message)
-        choices = self._llm.post_chat_request(messages)
-        if len(choices) < 1:
+        result = self._llm.post_chat_request(messages)
+        if len(result.choices) < 1:
             return self._parse_response("")
-        return self._parse_response(choices[0])
+        return self._parse_response(result.first_choice)
 
     def _build_messages(self, message: ChatMessage) -> List[LLMMessage]:
         prompt = [
             "You are an assistant specialized in evaluating the similarity between two messages.",
             "# Instructions",
             "# compare the {expected} message and the {actual} message",
             "# given a similarity score out of 100%",
```

### Comparing `council_ai-0.0.8/council/scorers/scorer_base.py` & `council_ai-0.0.9/council/scorers/scorer_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/skills/llm_skill.py` & `council_ai-0.0.9/council/skills/llm_skill.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import List, Protocol
 
 from council.contexts import SkillContext, ChatMessage
 from council.llm import LLMBase, LLMMessage
 from council.prompt import PromptBuilder
 from council.runners import Budget
+from council.runners.budget import Consumption
 from council.skills import SkillBase
 
 
 class ReturnMessages(Protocol):
     def __call__(self, context: SkillContext) -> List[LLMMessage]:
         ...
 
@@ -69,17 +70,22 @@
         """
 
         super().__init__(name=name)
         self._llm = llm
         self._context_messages = context_messages
         self._builder = PromptBuilder(system_prompt)
 
-    def execute(self, context: SkillContext, _budget: Budget) -> ChatMessage:
+    def execute(self, context: SkillContext, budget: Budget) -> ChatMessage:
         """Execute `LLMSkill`."""
 
         history_messages = self._context_messages(context)
         system_prompt = LLMMessage.system_message(self._builder.apply(context))
         messages = [system_prompt, *history_messages]
         llm_response = self._llm.post_chat_request(messages=messages)
-        if len(llm_response) < 1:
+        if len(llm_response.choices) < 1:
             return self.build_error_message(message="no response")
-        return self.build_success_message(message=llm_response[0], data=llm_response)
+
+        budget.add_consumption(consumption=Consumption(1, "call", "LLMSkill"), source=self.name)
+        for c in llm_response.consumptions:
+            budget.add_consumption(consumption=c, source=self.name)
+
+        return self.build_success_message(message=llm_response.first_choice, data=llm_response)
```

### Comparing `council_ai-0.0.8/council/skills/skill_base.py` & `council_ai-0.0.9/council/skills/skill_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/skills/google/google_news_skill.py` & `council_ai-0.0.9/council/skills/google/google_news_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/skills/google/google_search_skill.py` & `council_ai-0.0.9/council/skills/google/google_search_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/skills/google/google_context/context_provider.py` & `council_ai-0.0.9/council/skills/google/google_context/context_provider.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/skills/google/google_context/google_news.py` & `council_ai-0.0.9/council/skills/google/google_context/google_news.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/skills/google/google_context/google_search.py` & `council_ai-0.0.9/council/skills/google/google_context/google_search.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/skills/google/google_context/schemas.py` & `council_ai-0.0.9/council/skills/google/google_context/schemas.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/utils/env.py` & `council_ai-0.0.9/council/utils/env.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/utils/option.py` & `council_ai-0.0.9/council/utils/option.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/utils/parameter.py` & `council_ai-0.0.9/council/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/council/utils/result.py` & `council_ai-0.0.9/council/utils/result.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/.readthedocs.yaml` & `council_ai-0.0.9/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/Makefile` & `council_ai-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/make.bat` & `council_ai-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/conf.py` & `council_ai-0.0.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 ]
 # fmt: off
 # so that black does not mess with it
 html_theme_options = {
     "footer_icons": [
         {
             "name": "Discord",
-            "url": "https://discord.gg/uhusYQcP",
+            "url": "https://discord.gg/DWNCftGQZ3",
             "html": "",
             "class": "fa-brands fa-solid fa-discord",
         },
         {
             "name": "Github",
             "url": "https://github.com/chain-ml/council",
             "html": "",
```

### Comparing `council_ai-0.0.8/docs/source/index.rst` & `council_ai-0.0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/_static/Council_RGB_Horizontal_DarkBKG_Gradient.png` & `council_ai-0.0.9/docs/source/_static/Council_RGB_Horizontal_DarkBKG_Gradient.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/_static/Council_RGB_Horizontal_LightBKG_Gradient.png` & `council_ai-0.0.9/docs/source/_static/Council_RGB_Horizontal_LightBKG_Gradient.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/getting_started/first_example.ipynb` & `council_ai-0.0.9/docs/source/getting_started/first_example.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'cells'": '{delete: [17]}'}*

```diff
@@ -181,23 +181,14 @@
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "result = agent.execute_from_user_message(\"hello world?!\")\n",
                 "print(result.best_message.message)\n"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "collapsed": false
-            },
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `council_ai-0.0.8/docs/source/getting_started/installation.md` & `council_ai-0.0.9/docs/source/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/introduction/key_concepts.md` & `council_ai-0.0.9/docs/source/introduction/key_concepts.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/introduction/key_features.md` & `council_ai-0.0.9/docs/source/introduction/key_features.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/introduction/welcome.md` & `council_ai-0.0.9/docs/source/introduction/welcome.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Welcome
 
 
-Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
+[Council](https://github.com/chain-ml/council/) is an open-source framework for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
 
 Council extends the LLM tool ecosystem by enabling advanced control and scalable oversight for AI agents. Users can create sophisticated agents with predictable behavior by leveraging Council's powerful approach to control flow using Controllers, Filters, Evaluators and Budgets for agents. This allows the automated routing between agents, comparing, evaluating and selecting the best results for a (sub-)task. 
 
 The framework provides connectivity to a wide variety of Large Language Models (LLMs) natively and by integrating with popular libraries such as LangChain and LlamaIndex.
 
 Council aims to facilitate packaging and seamlessly deploying Agents at scale on multiple deployment platforms while enabling enterprise-grade monitoring and advanced quality control in a future release (contributions are welcome).
 
 # Community
 
-Join our Discord community to connect with the core development team and users <a href="https://discord.gg/uhusYQcP">here</a>.
+Join our Discord community to connect with the core development team and users <a href="https://discord.gg/DWNCftGQZ3">here</a>.
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-# Welcome Council is an open-source framework for the rapid development and
-robust deployment of customized generative AI applications using teams of
-`agents` - built in Python and (soon) Rust. Council extends the LLM tool
-ecosystem by enabling advanced control and scalable oversight for AI agents.
-Users can create sophisticated agents with predictable behavior by leveraging
-Council's powerful approach to control flow using Controllers, Filters,
-Evaluators and Budgets for agents. This allows the automated routing between
-agents, comparing, evaluating and selecting the best results for a (sub-)task.
-The framework provides connectivity to a wide variety of Large Language Models
-(LLMs) natively and by integrating with popular libraries such as LangChain and
-LlamaIndex. Council aims to facilitate packaging and seamlessly deploying
-Agents at scale on multiple deployment platforms while enabling enterprise-
-grade monitoring and advanced quality control in a future release
-(contributions are welcome). # Community Join our Discord community to connect
-with the core development team and users here.
+# Welcome [Council](https://github.com/chain-ml/council/) is an open-source
+framework for the rapid development and robust deployment of customized
+generative AI applications using teams of `agents` - built in Python and (soon)
+Rust. Council extends the LLM tool ecosystem by enabling advanced control and
+scalable oversight for AI agents. Users can create sophisticated agents with
+predictable behavior by leveraging Council's powerful approach to control flow
+using Controllers, Filters, Evaluators and Budgets for agents. This allows the
+automated routing between agents, comparing, evaluating and selecting the best
+results for a (sub-)task. The framework provides connectivity to a wide variety
+of Large Language Models (LLMs) natively and by integrating with popular
+libraries such as LangChain and LlamaIndex. Council aims to facilitate
+packaging and seamlessly deploying Agents at scale on multiple deployment
+platforms while enabling enterprise-grade monitoring and advanced quality
+control in a future release (contributions are welcome). # Community Join our
+Discord community to connect with the core development team and users here.
```

### Comparing `council_ai-0.0.8/docs/source/reference/runners.rst` & `council_ai-0.0.9/docs/source/reference/runners.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,15 @@
     council.runners.RunnerGeneratorError
     council.runners.RunnerPredicateError
     council.runners.RunnerSkillError
     council.runners.RunnerTimeoutError
     :full:
     :namespace: council.runners
 
+Classes
+-------
+
 .. toctree::
     :maxdepth: 1
     :glob:
 
     runners/*
```

### Comparing `council_ai-0.0.8/docs/source/reference/runners/parallel_for.rst` & `council_ai-0.0.9/docs/source/reference/runners/parallel_for.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/tutorials/social.md` & `council_ai-0.0.9/docs/source/tutorials/social.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/use_cases/langchain_llm_integration.ipynb` & `council_ai-0.0.9/docs/source/use_cases/langchain_llm_integration.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/use_cases/llamaindex_integration.ipynb` & `council_ai-0.0.9/docs/source/use_cases/llamaindex_integration.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/docs/source/use_cases/multi_chain_agent.ipynb` & `council_ai-0.0.9/docs/source/use_cases/multi_chain_agent.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/stubs/GoogleNews.pyi` & `council_ai-0.0.9/stubs/GoogleNews.pyi`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/LICENSE` & `council_ai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.8/README.md` & `council_ai-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Note: Some of the features listed above are work-in-progress and due in a future release (refer to Roadmap section below).
 
 # Key Concepts
 
 Key components of the framework are shown in below image and further introduced in this section.
 
-![engine flow](engine_flow.png "engine")
+![engine flow](docs/source/introduction/engine_flow.png "engine")
 
 ## Agent
 Agents encapsulate the end-to-end application logic from prompt input to final response across Controller, Evaluation and registered Chains of Skills. Agents itself can be recursively nested within other Agents in the form of AgentChains.
 
 ## Controller
 Controllers determine user intent given a prompt and prompt history and route the prompt to one or multiple of registered Chains before leveraging one or multiple Evaluators to score returned results and determine further course of action (including the ability to determine whether a revision is needed in which case Chains might be prompted again). Controllers will control whether one or multiple Chains are called, whether calls happen in series or in parallel. They will also be responsible for the distribution of compute budget to Chains and handling Chains that are not able to return results within the allocated compute budget. A State Management component will allow Controllers to save and retrieve state across user sessions. Controllers can be implemented in Python or (soon) Rust (to meet the needs of performance-critical applications).
 
@@ -145,30 +145,31 @@
 
 A detailed documentation of Council can be found at <a href="https://council.dev">council.dev</a>.
 
 # Roadmap
 
 We have big plans and an ambitious roadmap for the framework with incremental releases scheduled every two weeks. 
 
-Major milestones the core team is working towards are shown in below table. The roadmap is subject to frequent changes as community needs emerge. Breaking changes to our APIs are still to be expected.
+Major milestones the core team is working towards are shown below. The roadmap is subject to frequent changes as community needs emerge. Breaking changes to our APIs are still to be expected.
 
-
-| Feature  | Details | Status / ETA |
-| ------------- | ------------- | ------------- |
-| ~~Framework Core~~  | Key features and interfaces | ✅ |
-| Deployment Platform Integration  | Package, deploy and operate agents at scale in production via integration with popular deployment platforms | Q3 2023 |
-| Ecosystem Integration | Integrate with tools and frameworks in the broader LLM ecosystem | Q3 2023  |
-| Application Templates  | Provide reusable templates for LLM-enabled applications that allow fast creation of Agents addressing common use cases | Q3 2023 |
-| Quality & Evaluation Framework  | Automated and human-supervised test suites (via tool integration), enable management of reusable test cases | Q4 2023 |
+**Q3 2023**
+- [x] **Framework Core**: Key features and interfaces
+- [ ] **Conversational Automation**: Expand upon framework core with advanced filtering, evaluation and budgeting for agents
+- [ ] **Ecosystem Integration**: Integrate with tools and frameworks in the broader LLM ecosystem
+
+**Q4 2023**
+- [ ] **Application Templates**: Provide reusable templates for LLM-enabled applications that allow fast creation of Agents addressing common use cases
+- [ ] **Deployment Platform Integration**: Package, deploy and operate agents at scale in production via integration with popular deployment platforms
+- [ ] **Quality & Evaluation Framework**: Automated and human-supervised test suites (via tool integration), enable management of reusable test cases 
 
 # Support
 
-Please submit a Github issue should you need any help or reach out to the team via Discord.
+Please submit a Github issue should you need any help or reach out to the team via <a href="https://discord.gg/DWNCftGQZ3">Discord</a>.
 
 # Contributors
 
 Council is a project under active development. We welcome all contributions, pull requests, feature requests or reported issues.
 
 # Community
 
-Join our Discord community to connect with the core development team and users <a href="https://discord.gg/uhusYQcP">here</a>.
+Join our Discord community to connect with the core development team and users <a href="https://discord.gg/DWNCftGQZ3">here</a>.
```

### Comparing `council_ai-0.0.8/pyproject.toml` & `council_ai-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "council-ai"
-version = "0.0.8"
+version = "0.0.9"
 description = "Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = []
 license = "Apache-2.0"
 
 dynamic = ["dependencies"]
```

### Comparing `council_ai-0.0.8/PKG-INFO` & `council_ai-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: council-ai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications
 Project-URL: Source, https://github.com/chain-ml/council
 Project-URL: Documentation, https://council.dev
 License-Expression: Apache-2.0
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: google-api-python-client-stubs
@@ -12,14 +12,15 @@
 Requires-Dist: googlenews==1.6.8
 Requires-Dist: httpx==0.24.1
 Requires-Dist: jinja2~=3.1.2
 Requires-Dist: more-itertools~=9.1.0
 Requires-Dist: progressbar==2.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: requests~=2.31.0
+Requires-Dist: tiktoken==0.4.0
 Description-Content-Type: text/markdown
 
 ![Council](council_banner.png "council")
 
 <h1><p align="center">Council: AI Agent Platform with Control Flow and Scalable Oversight</p></h1>
 
 # Welcome
@@ -42,15 +43,15 @@
 
 Note: Some of the features listed above are work-in-progress and due in a future release (refer to Roadmap section below).
 
 # Key Concepts
 
 Key components of the framework are shown in below image and further introduced in this section.
 
-![engine flow](engine_flow.png "engine")
+![engine flow](docs/source/introduction/engine_flow.png "engine")
 
 ## Agent
 Agents encapsulate the end-to-end application logic from prompt input to final response across Controller, Evaluation and registered Chains of Skills. Agents itself can be recursively nested within other Agents in the form of AgentChains.
 
 ## Controller
 Controllers determine user intent given a prompt and prompt history and route the prompt to one or multiple of registered Chains before leveraging one or multiple Evaluators to score returned results and determine further course of action (including the ability to determine whether a revision is needed in which case Chains might be prompted again). Controllers will control whether one or multiple Chains are called, whether calls happen in series or in parallel. They will also be responsible for the distribution of compute budget to Chains and handling Chains that are not able to return results within the allocated compute budget. A State Management component will allow Controllers to save and retrieve state across user sessions. Controllers can be implemented in Python or (soon) Rust (to meet the needs of performance-critical applications).
 
@@ -165,30 +166,31 @@
 
 A detailed documentation of Council can be found at <a href="https://council.dev">council.dev</a>.
 
 # Roadmap
 
 We have big plans and an ambitious roadmap for the framework with incremental releases scheduled every two weeks. 
 
-Major milestones the core team is working towards are shown in below table. The roadmap is subject to frequent changes as community needs emerge. Breaking changes to our APIs are still to be expected.
+Major milestones the core team is working towards are shown below. The roadmap is subject to frequent changes as community needs emerge. Breaking changes to our APIs are still to be expected.
 
-
-| Feature  | Details | Status / ETA |
-| ------------- | ------------- | ------------- |
-| ~~Framework Core~~  | Key features and interfaces | ✅ |
-| Deployment Platform Integration  | Package, deploy and operate agents at scale in production via integration with popular deployment platforms | Q3 2023 |
-| Ecosystem Integration | Integrate with tools and frameworks in the broader LLM ecosystem | Q3 2023  |
-| Application Templates  | Provide reusable templates for LLM-enabled applications that allow fast creation of Agents addressing common use cases | Q3 2023 |
-| Quality & Evaluation Framework  | Automated and human-supervised test suites (via tool integration), enable management of reusable test cases | Q4 2023 |
+**Q3 2023**
+- [x] **Framework Core**: Key features and interfaces
+- [ ] **Conversational Automation**: Expand upon framework core with advanced filtering, evaluation and budgeting for agents
+- [ ] **Ecosystem Integration**: Integrate with tools and frameworks in the broader LLM ecosystem
+
+**Q4 2023**
+- [ ] **Application Templates**: Provide reusable templates for LLM-enabled applications that allow fast creation of Agents addressing common use cases
+- [ ] **Deployment Platform Integration**: Package, deploy and operate agents at scale in production via integration with popular deployment platforms
+- [ ] **Quality & Evaluation Framework**: Automated and human-supervised test suites (via tool integration), enable management of reusable test cases 
 
 # Support
 
-Please submit a Github issue should you need any help or reach out to the team via Discord.
+Please submit a Github issue should you need any help or reach out to the team via <a href="https://discord.gg/DWNCftGQZ3">Discord</a>.
 
 # Contributors
 
 Council is a project under active development. We welcome all contributions, pull requests, feature requests or reported issues.
 
 # Community
 
-Join our Discord community to connect with the core development team and users <a href="https://discord.gg/uhusYQcP">here</a>.
+Join our Discord community to connect with the core development team and users <a href="https://discord.gg/DWNCftGQZ3">here</a>.
```

