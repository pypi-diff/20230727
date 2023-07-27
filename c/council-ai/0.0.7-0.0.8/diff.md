# Comparing `tmp/council_ai-0.0.7.tar.gz` & `tmp/council_ai-0.0.8.tar.gz`

## Comparing `council_ai-0.0.7.tar` & `council_ai-0.0.8.tar`

### file list

```diff
@@ -1,157 +1,163 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.7/Makefile
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.7/engine_flow.png
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 council_ai-0.0.7/env.example
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.7/requirements.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agent_tests/__init__.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agent_tests/agent_tests.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agents/__init__.py
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agents/agent.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agents/agent_chain.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/agents/agent_result.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/chains/__init__.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/chains/chain.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/contexts/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/contexts/cancellation_token.py
--rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/contexts/execution_context.py
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/contexts/messages.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/basic_controller.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/controller_base.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/execution_unit.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/controllers/llm_controller.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/evaluators/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/evaluators/basic_evaluator.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/evaluators/evaluator_base.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/__init__.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/azure_llm.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/azure_llm_configuration.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/llm_base.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/llm_configuration_base.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/llm_exception.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/llm_message.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/openai_chat_completions_llm.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/openai_llm.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/llm/openai_llm_configuration.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/mocks/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/prompt/__init__.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/prompt/prompt_builder.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/budget.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/errrors.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/if_runner.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/loop_runner_base.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/parallel.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/parallel_for.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/runner_base.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/runner_context.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/runner_executor.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/sequential.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/skill_runner_base.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/runners/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/scorers/__init__.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/scorers/llm_similarity_scorer.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/scorers/scorer_base.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/scorers/scorer_exception.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/__init__.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/llm_skill.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/skill_base.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/__init__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_news_skill.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_search_skill.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/context_provider.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/google_news.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/google_search.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/skills/google/google_context/schemas.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/__init__.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/env.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/option.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/parameter.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 council_ai-0.0.7/council/utils/result.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/.gitignore
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/.readthedocs.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/Makefile
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/README.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/docker-compose.yaml
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/dockerfile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/make.bat
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/requirements.txt
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/conf.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/index.rst
--rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/_static/00_chainml_logo.png
--rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/_static/02_chainml_logo_black.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/contributing/contributing.md
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/getting_started/first_example.ipynb
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/getting_started/installation.md
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/introduction/engine_flow.png
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/introduction/key_concepts.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/introduction/key_features.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/introduction/welcome.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/agents.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/chains.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/evaluators.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm.rst
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/scorers.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/utils.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/agents/agent.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/agents/agent_result.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/chains/chain.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/agent_context.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chain_context.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chain_history.rst
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chat_history.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chat_message.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/chat_message_kind.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/iteration_context.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/message_collection.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/scored_chat_message.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/contexts/skill_context.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers/basic_controller.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers/controller_base.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers/execution_unit.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/controllers/llm_controller.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/evaluators/basic_evaluator.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/evaluators/evaluator_base.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/evaluators/llm_evaluator.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/azure_llm.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/azure_llm_configuration.rst
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/llm_base.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/llm_configuration_base.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/llm_message.rst
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/llm_message_role.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/openai_llm.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/llm/openai_llm_configuration.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/budget.rst
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/errors.rst
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/if.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/loop_runner_base.rst
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/parallel.rst
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/parallel_for.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/runner_base.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/runner_executor.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/sequential.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/runners/skill_runner_base.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/scorers/llm_similarity_scorer.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/scorers/scorer_base.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/scorers/scorer_exception.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/google.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/llm_skill.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/skill_base.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/google/google_news_skill.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/skills/google/google_search_skill.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/utils/option.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/reference/utils/option_exception.rst
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/use_cases/langchain_llm_integration.ipynb
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 council_ai-0.0.7/docs/source/use_cases/multi_chain_agent.ipynb
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.7/stubs/GoogleNews.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.7/LICENSE
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 council_ai-0.0.7/README.md
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 council_ai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.8/Makefile
+-rw-r--r--   0        0        0   333985 2020-02-02 00:00:00.000000 council_ai-0.0.8/council_banner.png
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.8/engine_flow.png
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 council_ai-0.0.8/env.example
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.8/requirements.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agent_tests/__init__.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agent_tests/agent_tests.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agents/__init__.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agents/agent.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agents/agent_chain.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/agents/agent_result.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/chains/__init__.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/chains/chain.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/contexts/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/contexts/cancellation_token.py
+-rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/contexts/execution_context.py
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/contexts/messages.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/basic_controller.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/controller_base.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/execution_unit.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/controllers/llm_controller.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/evaluators/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/evaluators/basic_evaluator.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/evaluators/evaluator_base.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/__init__.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/azure_llm.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/azure_llm_configuration.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/llm_base.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/llm_configuration_base.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/llm_exception.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/llm_message.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/openai_chat_completions_llm.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/openai_llm.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/llm/openai_llm_configuration.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/mocks/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/prompt/__init__.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/prompt/prompt_builder.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/budget.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/errrors.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/if_runner.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/loop_runner_base.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/parallel.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/parallel_for.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/runner_base.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/runner_context.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/runner_executor.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/sequential.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/skill_runner_base.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/runners/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/scorers/__init__.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/scorers/llm_similarity_scorer.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/scorers/scorer_base.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/scorers/scorer_exception.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/__init__.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/llm_skill.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/skill_base.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_news_skill.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_search_skill.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/context_provider.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/google_news.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/google_search.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/skills/google/google_context/schemas.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/__init__.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/env.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/option.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/parameter.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 council_ai-0.0.8/council/utils/result.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/.gitignore
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/Makefile
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/README.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/docker-compose.yaml
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/dockerfile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/make.bat
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/requirements.txt
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/conf.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/index.rst
+-rw-r--r--   0        0        0    33816 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/_static/Council_RGB_Horizontal_DarkBKG_Gradient.png
+-rw-r--r--   0        0        0    35327 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/_static/Council_RGB_Horizontal_LightBKG_Gradient.png
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/_static/council.css
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/contributing/contributing.md
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/getting_started/first_example.ipynb
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/getting_started/installation.md
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/introduction/engine_flow.png
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/introduction/key_concepts.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/introduction/key_features.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/introduction/welcome.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/agents.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/chains.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/evaluators.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm.rst
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/scorers.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/utils.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/agents/agent.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/agents/agent_result.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/chains/chain.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/agent_context.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chain_context.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chain_history.rst
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chat_history.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chat_message.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/chat_message_kind.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/iteration_context.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/message_collection.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/scored_chat_message.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/contexts/skill_context.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers/basic_controller.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers/controller_base.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers/execution_unit.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/controllers/llm_controller.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/evaluators/basic_evaluator.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/evaluators/evaluator_base.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/evaluators/llm_evaluator.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/azure_llm.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/azure_llm_configuration.rst
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/llm_base.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/llm_configuration_base.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/llm_message.rst
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/llm_message_role.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/openai_llm.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/llm/openai_llm_configuration.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/budget.rst
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/errors.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/if.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/loop_runner_base.rst
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/parallel.rst
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/parallel_for.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/runner_base.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/runner_executor.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/sequential.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/runners/skill_runner_base.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/scorers/llm_similarity_scorer.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/scorers/scorer_base.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/scorers/scorer_exception.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/google.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/llm_skill.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/skill_base.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/google/google_news_skill.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/skills/google/google_search_skill.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/utils/option.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/reference/utils/option_exception.rst
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/tutorials/financial.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/tutorials/research.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/tutorials/social.md
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/use_cases/langchain_llm_integration.ipynb
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/use_cases/llamaindex_integration.ipynb
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 council_ai-0.0.8/docs/source/use_cases/multi_chain_agent.ipynb
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.8/stubs/GoogleNews.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.8/LICENSE
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 council_ai-0.0.8/README.md
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 council_ai-0.0.8/PKG-INFO
```

### Comparing `council_ai-0.0.7/engine_flow.png` & `council_ai-0.0.8/engine_flow.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/agent_tests/agent_tests.py` & `council_ai-0.0.8/council/agent_tests/agent_tests.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/agents/agent.py` & `council_ai-0.0.8/council/agents/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,20 +97,35 @@
         Parameters:
              skill(SkillBase): a skill
              chain_description(str): Optional, chain description
         Returns:
             Agent: a new instance
         """
         chain = Chain(name="BasicChain", description=chain_description or "basic chain", runners=[skill])
+        return Agent.from_chain(chain)
+
+    @staticmethod
+    def from_chain(chain: Chain) -> "Agent":
+        """
+        Helper function to create a new agent with a  :class:`.BasicController`, a
+            :class:`.BasicEvaluator` and a single :class:`.SkillBase` wrapped into a :class:`.Chain`
+
+        Parameters:
+             chain(Chain): a chain
+        Returns:
+            Agent: a new instance
+        """
         return Agent(controller=BasicController(), chains=[chain], evaluator=BasicEvaluator())
 
-    def execute_from_user_message(self, message: str) -> AgentResult:
+    def execute_from_user_message(self, message: str, budget: Optional[Budget] = None) -> AgentResult:
         """
         Helper function that executes an agent with a simple user message.
 
         Parameters:
             message(str): the user message
+            budget (Budget): the budget for the agent execution
         Returns:
              AgentResult:
         """
+        execution_budget = budget or InfiniteBudget()
         context = AgentContext(ChatHistory.from_user_message(message))
-        return self.execute(context, budget=InfiniteBudget())
+        return self.execute(context, budget=execution_budget)
```

### Comparing `council_ai-0.0.7/council/agents/agent_chain.py` & `council_ai-0.0.8/council/agents/agent_chain.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/agents/agent_result.py` & `council_ai-0.0.8/council/agents/agent_result.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/chains/chain.py` & `council_ai-0.0.8/council/chains/chain.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/contexts/execution_context.py` & `council_ai-0.0.8/council/contexts/execution_context.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/contexts/messages.py` & `council_ai-0.0.8/council/contexts/messages.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/controllers/basic_controller.py` & `council_ai-0.0.8/council/controllers/basic_controller.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/controllers/controller_base.py` & `council_ai-0.0.8/council/controllers/controller_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/controllers/execution_unit.py` & `council_ai-0.0.8/council/controllers/execution_unit.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/controllers/llm_controller.py` & `council_ai-0.0.8/council/controllers/llm_controller.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/evaluators/basic_evaluator.py` & `council_ai-0.0.8/council/evaluators/basic_evaluator.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/evaluators/evaluator_base.py` & `council_ai-0.0.8/council/evaluators/evaluator_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/evaluators/llm_evaluator.py` & `council_ai-0.0.8/council/evaluators/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/llm/azure_llm.py` & `council_ai-0.0.8/council/llm/azure_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/llm/llm_base.py` & `council_ai-0.0.8/council/llm/llm_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/llm/llm_configuration_base.py` & `council_ai-0.0.8/council/llm/llm_configuration_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,30 +49,29 @@
     temperature: Parameter[float]
     max_tokens: Parameter[int]
     top_p: Parameter[float]
     n: Parameter[int]
     presence_penalty: Parameter[float]
     frequency_penalty: Parameter[float]
 
-    def __init__(self, env_var_prefix: str):
-        self._prefix = env_var_prefix
+    def __init__(self):
         self.temperature = Parameter.float(name="temperature", required=False, default=0.0, validator=_tv)
         self.max_tokens = Parameter.int(name="max_tokens", required=False, validator=_mtv)
         self.top_p = Parameter.float(name="top_p", required=False)
         self.n = Parameter.int(name="n", required=False, default=1)
         self.presence_penalty = Parameter.float(name="presence_penalty", required=False, validator=_pv)
         self.frequency_penalty = Parameter.float(name="frequency_penalty", required=False, validator=_pv)
 
-    def read_env(self):
-        self.temperature.from_env(self._prefix + "LLM_TEMPERATURE")
-        self.max_tokens.from_env(self._prefix + "LLM_MAX_TOKENS")
-        self.top_p.from_env(self._prefix + "LLM_TOP_P")
-        self.n.from_env(self._prefix + "LLM_N")
-        self.presence_penalty.from_env(self._prefix + "LLM_PRESENCE_PENALTY")
-        self.frequency_penalty.from_env(self._prefix + "LLM_FREQUENCY_PENALTY")
+    def read_env(self, env_var_prefix: str):
+        self.temperature.from_env(env_var_prefix + "LLM_TEMPERATURE")
+        self.max_tokens.from_env(env_var_prefix + "LLM_MAX_TOKENS")
+        self.top_p.from_env(env_var_prefix + "LLM_TOP_P")
+        self.n.from_env(env_var_prefix + "LLM_N")
+        self.presence_penalty.from_env(env_var_prefix + "LLM_PRESENCE_PENALTY")
+        self.frequency_penalty.from_env(env_var_prefix + "LLM_FREQUENCY_PENALTY")
 
     def build_default_payload(self) -> dict[str, Any]:
         payload: dict[str, Any] = {}
         if self.temperature.is_some():
             payload.setdefault(self.temperature.name, self.temperature.unwrap())
         if self.max_tokens.is_some():
             payload.setdefault(self.max_tokens.name, self.max_tokens.unwrap())
```

### Comparing `council_ai-0.0.7/council/llm/llm_message.py` & `council_ai-0.0.8/council/llm/llm_message.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/llm/openai_chat_completions_llm.py` & `council_ai-0.0.8/council/llm/openai_chat_completions_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/llm/openai_llm_configuration.py` & `council_ai-0.0.8/council/llm/openai_llm_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Optional
 
 from council.llm import LLMConfigurationBase
 from council.utils import read_env_str, read_env_int, Option
 
 
 class OpenAILLMConfiguration(LLMConfigurationBase):
     """
@@ -15,30 +15,37 @@
 
     Notes:
         * see https://platform.openai.com/docs/api-reference/chat
     """
 
     api_key: str
     authorization: str  # not a parameter - used to optimize calls
-    model: Option[str] = Option.none()
-    timeout: int = 30
+    model: Option[str]
+    timeout: int
 
-    def __init__(self):
-        super().__init__("OPENAI_")
+    def __init__(self, model: Optional[str] = None, timeout: Optional[int] = None, api_key: Optional[str] = None):
+        super().__init__()
+        self.model = Option(model)
+        self.timeout = timeout or 30
+        if api_key is not None:
+            self._set_api_key(api_key)
 
     def build_default_payload(self) -> dict[str, Any]:
         payload = super().build_default_payload()
         if self.model.is_some():
             payload.setdefault("model", self.model.unwrap())
         return payload
 
     @staticmethod
-    def from_env() -> "OpenAILLMConfiguration":
-        config = OpenAILLMConfiguration()
-        config.read_env()
-
-        config.api_key = read_env_str("OPENAI_API_KEY").unwrap()
-        config.authorization = f"Bearer {config.api_key}"
-        config.model = read_env_str("OPENAI_LLM_MODEL", required=False)
-
+    def from_env(model: Optional[str] = None) -> "OpenAILLMConfiguration":
+        config = OpenAILLMConfiguration(model=model)
+        config.read_env(env_var_prefix="OPENAI_")
+
+        config._set_api_key(read_env_str("OPENAI_API_KEY").unwrap())
+        if config.model.is_none():
+            config.model = read_env_str("OPENAI_LLM_MODEL", required=False, default="gpt-3.5-turbo")
         config.timeout = read_env_int("OPENAI_LLM_TIMEOUT", required=False, default=30).unwrap()
         return config
+
+    def _set_api_key(self, key: str) -> None:
+        self.api_key = key
+        self.authorization = f"Bearer {key}"
```

### Comparing `council_ai-0.0.7/council/mocks/__init__.py` & `council_ai-0.0.8/council/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/prompt/prompt_builder.py` & `council_ai-0.0.8/council/prompt/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/__init__.py` & `council_ai-0.0.8/council/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/budget.py` & `council_ai-0.0.8/council/runners/budget.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/errrors.py` & `council_ai-0.0.8/council/runners/errrors.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/if_runner.py` & `council_ai-0.0.8/council/runners/if_runner.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/parallel.py` & `council_ai-0.0.8/council/runners/parallel.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/parallel_for.py` & `council_ai-0.0.8/council/runners/parallel_for.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/runner_base.py` & `council_ai-0.0.8/council/runners/runner_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/runner_context.py` & `council_ai-0.0.8/council/runners/runner_context.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/sequential.py` & `council_ai-0.0.8/council/runners/sequential.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/runners/skill_runner_base.py` & `council_ai-0.0.8/council/runners/skill_runner_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/scorers/llm_similarity_scorer.py` & `council_ai-0.0.8/council/scorers/llm_similarity_scorer.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/scorers/scorer_base.py` & `council_ai-0.0.8/council/scorers/scorer_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/skills/llm_skill.py` & `council_ai-0.0.8/council/skills/llm_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/skills/skill_base.py` & `council_ai-0.0.8/council/skills/skill_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/skills/google/google_news_skill.py` & `council_ai-0.0.8/council/skills/google/google_news_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/skills/google/google_search_skill.py` & `council_ai-0.0.8/council/skills/google/google_search_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/skills/google/google_context/context_provider.py` & `council_ai-0.0.8/council/skills/google/google_context/context_provider.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/skills/google/google_context/google_news.py` & `council_ai-0.0.8/council/skills/google/google_context/google_news.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/skills/google/google_context/google_search.py` & `council_ai-0.0.8/council/skills/google/google_context/google_search.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/skills/google/google_context/schemas.py` & `council_ai-0.0.8/council/skills/google/google_context/schemas.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/utils/env.py` & `council_ai-0.0.8/council/utils/env.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/utils/option.py` & `council_ai-0.0.8/council/utils/option.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/utils/parameter.py` & `council_ai-0.0.8/council/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/council/utils/result.py` & `council_ai-0.0.8/council/utils/result.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/.readthedocs.yaml` & `council_ai-0.0.8/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/Makefile` & `council_ai-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/make.bat` & `council_ai-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/source/conf.py` & `council_ai-0.0.8/docs/source/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,22 +58,24 @@
 templates_path = ["_templates"]
 exclude_patterns = []
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_title = f"{project} {release}"
+html_short_title = f"{release}"
 html_theme = "furo"
 html_show_copyright = False
 html_show_sphinx = False
 html_static_path = ["_static"]
 html_css_files = [
     "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/fontawesome.min.css",
     "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/solid.min.css",
     "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/brands.min.css",
+    "council.css",
 ]
 # fmt: off
 # so that black does not mess with it
 html_theme_options = {
     "footer_icons": [
         {
             "name": "Discord",
@@ -83,12 +85,13 @@
         },
         {
             "name": "Github",
             "url": "https://github.com/chain-ml/council",
             "html": "",
             "class": "fa-brands fa-solid fa-github",
         },
-    ]
+    ],
+    "dark_logo": "Council_RGB_Horizontal_DarkBKG_Gradient.png",
+    "light_logo": "Council_RGB_Horizontal_LightBKG_Gradient.png",
+    "sidebar_hide_name": False,
 }
 # fmt: on
-
-# html_theme_options = {"dark_logo": "00_chainml_logo.png", "light_logo": "02_chainml_logo_black.png"}
```

### Comparing `council_ai-0.0.7/docs/source/index.rst` & `council_ai-0.0.8/docs/source/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -20,18 +20,28 @@
 
 .. toctree::
     :maxdepth: 2
     :caption: Use Cases
     :hidden:
 
     use_cases/multi_chain_agent.ipynb
+    use_cases/llamaindex_integration.ipynb
     use_cases/langchain_llm_integration.ipynb
 
 .. toctree::
     :maxdepth: 2
+    :caption: Tutorials
+    :hidden:
+
+    tutorials/social.md
+    tutorials/financial.md
+    tutorials/research.md
+
+.. toctree::
+    :maxdepth: 2
     :caption: Reference
     :name: reference
     :hidden:
     :glob:
 
     reference/*
```

### Comparing `council_ai-0.0.7/docs/source/getting_started/first_example.ipynb` & `council_ai-0.0.8/docs/source/getting_started/first_example.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/source/getting_started/installation.md` & `council_ai-0.0.8/docs/source/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/source/introduction/engine_flow.png` & `council_ai-0.0.8/docs/source/introduction/engine_flow.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/source/introduction/key_concepts.md` & `council_ai-0.0.8/docs/source/introduction/key_concepts.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/source/introduction/key_features.md` & `council_ai-0.0.8/docs/source/introduction/key_features.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Key Features
 
 * 🧐 Support for Sophisticated Agents: Reliable agents that can iterate over tasks that require exploring alternatives, creating and completing subgoals, and evaluating quality under budget constraints.
 * 🥰 Built for Data Scientists: Python library, local development environment, integrated with popular frameworks.
 * 🚀 Seamless Production Deployments: Easy packaging, deployment and monitoring at scale on multiple deployment platforms via Kubernetes integration.
-* 🤝 Ecosystem Connectivity: Connected with a growing AI Agent ecosystem, integrated with LangChain.
+* 🤝 Ecosystem Connectivity: Connected with a growing AI Agent ecosystem, integrated with LangChain, LlamaIndex and leading AI models.
 * 👮 Scalable Oversight: Built-in tooling to manage, version, monitor, evaluate and control deployed Agents.
 
 Note: Some of the features listed above are work-in-progress and due in a future release.
```

### Comparing `council_ai-0.0.7/docs/source/introduction/welcome.md` & `council_ai-0.0.8/docs/source/introduction/welcome.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Welcome
 
 
 Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
 
 Council extends the LLM tool ecosystem by enabling advanced control and scalable oversight for AI agents. Users can create sophisticated agents with predictable behavior by leveraging Council's powerful approach to control flow using Controllers, Filters, Evaluators and Budgets for agents. This allows the automated routing between agents, comparing, evaluating and selecting the best results for a (sub-)task. 
 
-The framework provides connectivity to a wide variety of Large Language Models (LLMs) natively and by integrating with popular libraries such as LangChain.
+The framework provides connectivity to a wide variety of Large Language Models (LLMs) natively and by integrating with popular libraries such as LangChain and LlamaIndex.
 
 Council aims to facilitate packaging and seamlessly deploying Agents at scale on multiple deployment platforms while enabling enterprise-grade monitoring and advanced quality control in a future release (contributions are welcome).
 
 # Community
 
 Join our Discord community to connect with the core development team and users <a href="https://discord.gg/uhusYQcP">here</a>.
```

#### html2text {}

```diff
@@ -3,13 +3,13 @@
 `agents` - built in Python and (soon) Rust. Council extends the LLM tool
 ecosystem by enabling advanced control and scalable oversight for AI agents.
 Users can create sophisticated agents with predictable behavior by leveraging
 Council's powerful approach to control flow using Controllers, Filters,
 Evaluators and Budgets for agents. This allows the automated routing between
 agents, comparing, evaluating and selecting the best results for a (sub-)task.
 The framework provides connectivity to a wide variety of Large Language Models
-(LLMs) natively and by integrating with popular libraries such as LangChain.
-Council aims to facilitate packaging and seamlessly deploying Agents at scale
-on multiple deployment platforms while enabling enterprise-grade monitoring and
-advanced quality control in a future release (contributions are welcome). #
-Community Join our Discord community to connect with the core development team
-and users here.
+(LLMs) natively and by integrating with popular libraries such as LangChain and
+LlamaIndex. Council aims to facilitate packaging and seamlessly deploying
+Agents at scale on multiple deployment platforms while enabling enterprise-
+grade monitoring and advanced quality control in a future release
+(contributions are welcome). # Community Join our Discord community to connect
+with the core development team and users here.
```

### Comparing `council_ai-0.0.7/docs/source/reference/runners.rst` & `council_ai-0.0.8/docs/source/reference/runners.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/source/reference/runners/parallel_for.rst` & `council_ai-0.0.8/docs/source/reference/runners/parallel_for.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/docs/source/use_cases/langchain_llm_integration.ipynb` & `council_ai-0.0.8/docs/source/use_cases/langchain_llm_integration.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992761485826002%*

 * *Differences: {"'cells'": "{3: {'execution_count': None, 'source': {insert: [(0, 'from typing import Any, "*

 * *            "List\\n'), (15, '    def _post_chat_request(self, messages: list[LLMMessage], "*

 * *            "**kwargs: Any) -> List[str]:\\n'), (16, '        prompt = messages[-1].content\\n'), "*

 * *            "(17, '        return [self.langchain_llm.__call__(prompt=prompt, **kwargs)]')], "*

 * *            "delete: [17, 16, 15, 0]}}, 5: {'execution_count': None}, 7: {'execution_count': "*

 * *            "None}, 9: {'execution_ […]*

```diff
@@ -46,38 +46,38 @@
             },
             "source": [
                 "Build a `LangchainLLM` to integrate langchain llm into ChainML."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from typing import Any\n",
+                "from typing import Any, List\n",
                 "\n",
                 "from council.llm import LLMBase\n",
                 "from council.llm.llm_message import LLMMessage\n",
                 "\n",
                 "from langchain.llms import BaseLLM\n",
                 "\n",
                 "\n",
                 "class LangChainLLM(LLMBase):\n",
                 "    langchain_llm: BaseLLM\n",
                 "\n",
                 "    def __init__(self, langchain_llm: BaseLLM):\n",
                 "        super().__init__()\n",
                 "        self.langchain_llm = langchain_llm\n",
                 "\n",
-                "    def _post_chat_request(self, messages: list[LLMMessage], **kwargs: Any) -> str:\n",
-                "        prompt = messages[-1].content()\n",
-                "        return self.langchain_llm.__call__(prompt=prompt, **kwargs)"
+                "    def _post_chat_request(self, messages: list[LLMMessage], **kwargs: Any) -> List[str]:\n",
+                "        prompt = messages[-1].content\n",
+                "        return [self.langchain_llm.__call__(prompt=prompt, **kwargs)]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -86,15 +86,15 @@
                 "### HuggingFace pipeline\n",
                 "\n",
                 "Let's create a langchain LLM using the `HuggingFacePipeline`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from langchain import HuggingFacePipeline\n",
                 "\n",
@@ -108,15 +108,15 @@
             },
             "source": [
                 "Wrap the langchain LLM into our newly created `LangchainLLM`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "hugging_face_llm = LangChainLLM(langchain_llm=hf_pipeline)"
             ]
@@ -128,28 +128,19 @@
             },
             "source": [
                 "The `ChainML` LLM is now ready to use!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": "'Blockchains are a type of cryptographic protocol that uses cryptographic hashing to verify'"
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "prompt = LLMMessage.user_message(\"Tell me more about blockchains\")\n",
                 "hugging_face_llm.post_chat_request(messages=[prompt])"
             ]
         },
         {
             "cell_type": "markdown",
@@ -169,15 +160,15 @@
                 "### OpenAI chat model\n",
                 "\n",
                 "Let's build a `LangchainChatLLM` to integrate langchain chat llm into ChainML."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from council.llm.llm_message import LLMMessageRole\n",
                 "from langchain.chat_models.base import BaseChatModel\n",
@@ -190,51 +181,43 @@
                 "    def __init__(self, langchain_llm: BaseChatModel):\n",
                 "        super().__init__()\n",
                 "        self.langchain_llm = langchain_llm\n",
                 "\n",
                 "    @staticmethod\n",
                 "    def convert_message(message: LLMMessage) -> BaseMessage:\n",
                 "        if message.is_of_role(LLMMessageRole.User):\n",
-                "            return HumanMessage(content=message.content())\n",
+                "            return HumanMessage(content=message.content)\n",
                 "        elif message.is_of_role(LLMMessageRole.System):\n",
-                "            return SystemMessage(content=message.content())\n",
+                "            return SystemMessage(content=message.content)\n",
                 "        elif message.is_of_role(LLMMessageRole.Assistant):\n",
-                "            return AIMessage(content=message.content())\n",
+                "            return AIMessage(content=message.content)\n",
                 "        else:\n",
                 "            raise ValueError(f\"Invalid role {message.role}\")\n",
                 "\n",
-                "    def _post_chat_request(self, messages: list[LLMMessage], **kwargs: Any) -> str:\n",
+                "    def _post_chat_request(self, messages: list[LLMMessage], **kwargs: Any) -> List[str]:\n",
                 "        messages = map(lambda msg: LangChainChatLLM.convert_message(msg), messages)\n",
-                "        return self.langchain_llm(messages=list(messages), **kwargs).content"
+                "        return [self.langchain_llm(messages=list(messages), **kwargs).content]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "Let's create a langchain chat llm using the `ChatOpenAI`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Verily, in that mighty continent of South America, there exist three cities of great magnitude. The first is S\u00e3o Paulo, a bustling metropolis in the land of Brazil. The second is Buenos Aires, a city of grandeur and culture in the realm of Argentina. And the third is Lima, a city of ancient civilizations and splendor in the kingdom of Peru."
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "from langchain.chat_models import ChatOpenAI\n",
                 "\n",
                 "lc_chatgpt = ChatOpenAI(model=\"gpt-3.5-turbo\")\n",
                 "\n",
                 "# Wrap `ChatOpenAI` into our newly created `LangChainChatLLM`\n",
                 "chatgpt_llm = LangChainChatLLM(lc_chatgpt)\n",
```

### Comparing `council_ai-0.0.7/docs/source/use_cases/multi_chain_agent.ipynb` & `council_ai-0.0.8/docs/source/use_cases/multi_chain_agent.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/stubs/GoogleNews.pyi` & `council_ai-0.0.8/stubs/GoogleNews.pyi`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/LICENSE` & `council_ai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.7/README.md` & `council_ai-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-<h1><p align="center">Council - AI Agent Platform with Advanced Control and Scalable Oversight</p></h1>
+![Council](council_banner.png "council")
+
+<h1><p align="center">Council: AI Agent Platform with Control Flow and Scalable Oversight</p></h1>
 
 # Welcome
 
-Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
+Council is an open-source platform for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
 
 Council extends the LLM tool ecosystem by enabling advanced control and scalable oversight for AI agents. Users can create sophisticated agents with predictable behavior by leveraging Council's powerful approach to control flow using Controllers, Filters, Evaluators and Budgets for agents. This allows the automated routing between agents, comparing, evaluating and selecting the best results for a (sub-)task. 
 
 The framework provides connectivity to a wide variety of Large Language Models (LLMs) natively and by integrating with popular libraries such as LangChain.
 
 Council aims to facilitate packaging and seamlessly deploying Agents at scale on multiple deployment platforms while enabling enterprise-grade monitoring and advanced quality control in a future release (contributions are welcome).
 
 # Key Features
 
-* 🧐 Support for Sophisticated Agents: Reliable agents that can iterate over tasks that require exploring alternatives, creating and completing subgoals, and evaluating quality under budget constraints.
-* 🥰 Built for Data Scientists: Python library, local development environment, integrated with popular frameworks.
-* 🚀 Seamless Production Deployments: Easy packaging, deployment and monitoring at scale on multiple deployment platforms via Kubernetes integration.
-* 🤝 Ecosystem Connectivity: Connected with a growing AI Agent ecosystem, integrated with LangChain.
-* 👮 Scalable Oversight: Built-in tooling to manage, version, monitor, evaluate and control deployed Agents.
+* 🧐 **Support for Sophisticated Agents**: Reliable agents that can iterate over tasks that require exploring alternatives, creating and completing subgoals, and evaluating quality under budget constraints.
+* 🥰 **Built for Data Scientists**: Python library, local development environment, integrated with popular frameworks.
+* 🚀 **Seamless Production Deployments**: Easy packaging, deployment and monitoring at scale on multiple deployment platforms via Kubernetes integration.
+* 🤝 **Ecosystem Connectivity**: Connected with a growing AI Agent ecosystem, integrated with LangChain, LlamaIndex and leading AI models.
+* 👮 **Scalable Oversight**: Built-in tooling to manage, version, monitor, evaluate and control deployed Agents.
 
 Note: Some of the features listed above are work-in-progress and due in a future release (refer to Roadmap section below).
 
 # Key Concepts
 
 Key components of the framework are shown in below image and further introduced in this section.
```

### Comparing `council_ai-0.0.7/pyproject.toml` & `council_ai-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "council-ai"
-version = "0.0.7"
+version = "0.0.8"
 description = "Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = []
 license = "Apache-2.0"
 
 dynamic = ["dependencies"]
```

### Comparing `council_ai-0.0.7/PKG-INFO` & `council_ai-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: council-ai
-Version: 0.0.7
+Version: 0.0.8
 Summary: Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications
 Project-URL: Source, https://github.com/chain-ml/council
 Project-URL: Documentation, https://council.dev
 License-Expression: Apache-2.0
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: google-api-python-client-stubs
@@ -14,33 +14,35 @@
 Requires-Dist: jinja2~=3.1.2
 Requires-Dist: more-itertools~=9.1.0
 Requires-Dist: progressbar==2.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: requests~=2.31.0
 Description-Content-Type: text/markdown
 
-<h1><p align="center">Council - AI Agent Platform with Advanced Control and Scalable Oversight</p></h1>
+![Council](council_banner.png "council")
+
+<h1><p align="center">Council: AI Agent Platform with Control Flow and Scalable Oversight</p></h1>
 
 # Welcome
 
-Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
+Council is an open-source platform for the rapid development and robust deployment of customized generative AI applications using teams of `agents` - built in Python and (soon) Rust.
 
 Council extends the LLM tool ecosystem by enabling advanced control and scalable oversight for AI agents. Users can create sophisticated agents with predictable behavior by leveraging Council's powerful approach to control flow using Controllers, Filters, Evaluators and Budgets for agents. This allows the automated routing between agents, comparing, evaluating and selecting the best results for a (sub-)task. 
 
 The framework provides connectivity to a wide variety of Large Language Models (LLMs) natively and by integrating with popular libraries such as LangChain.
 
 Council aims to facilitate packaging and seamlessly deploying Agents at scale on multiple deployment platforms while enabling enterprise-grade monitoring and advanced quality control in a future release (contributions are welcome).
 
 # Key Features
 
-* 🧐 Support for Sophisticated Agents: Reliable agents that can iterate over tasks that require exploring alternatives, creating and completing subgoals, and evaluating quality under budget constraints.
-* 🥰 Built for Data Scientists: Python library, local development environment, integrated with popular frameworks.
-* 🚀 Seamless Production Deployments: Easy packaging, deployment and monitoring at scale on multiple deployment platforms via Kubernetes integration.
-* 🤝 Ecosystem Connectivity: Connected with a growing AI Agent ecosystem, integrated with LangChain.
-* 👮 Scalable Oversight: Built-in tooling to manage, version, monitor, evaluate and control deployed Agents.
+* 🧐 **Support for Sophisticated Agents**: Reliable agents that can iterate over tasks that require exploring alternatives, creating and completing subgoals, and evaluating quality under budget constraints.
+* 🥰 **Built for Data Scientists**: Python library, local development environment, integrated with popular frameworks.
+* 🚀 **Seamless Production Deployments**: Easy packaging, deployment and monitoring at scale on multiple deployment platforms via Kubernetes integration.
+* 🤝 **Ecosystem Connectivity**: Connected with a growing AI Agent ecosystem, integrated with LangChain, LlamaIndex and leading AI models.
+* 👮 **Scalable Oversight**: Built-in tooling to manage, version, monitor, evaluate and control deployed Agents.
 
 Note: Some of the features listed above are work-in-progress and due in a future release (refer to Roadmap section below).
 
 # Key Concepts
 
 Key components of the framework are shown in below image and further introduced in this section.
```

