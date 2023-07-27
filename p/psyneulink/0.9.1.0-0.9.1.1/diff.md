# Comparing `tmp/psyneulink-0.9.1.0.tar.gz` & `tmp/psyneulink-0.9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psyneulink-0.9.1.0.tar", last modified: Tue Aug 10 00:23:59 2021, max compression
+gzip compressed data, was "dist/psyneulink-0.9.1.1.tar", last modified: Fri Sep 17 02:21:56 2021, max compression
```

## Comparing `psyneulink-0.9.1.0.tar` & `psyneulink-0.9.1.1.tar`

### file list

```diff
@@ -1,521 +1,521 @@
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/
--rw-------   0 katherine  (1000) katherine  (1000)      451 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/CONTRIBUTING.md
--rw-------   0 katherine  (1000) katherine  (1000)     9993 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/CONVENTIONS.md
--rw-------   0 katherine  (1000) katherine  (1000)    11358 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/LICENSE.txt
--rw-------   0 katherine  (1000) katherine  (1000)      209 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/MANIFEST.in
--rw-------   0 katherine  (1000) katherine  (1000)    15089 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/PKG-INFO
--rw-------   0 katherine  (1000) katherine  (1000)    12268 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/README.rst
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/Scripts/
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/Scripts/Debug/
--rw-------   0 katherine  (1000) katherine  (1000)     1662 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Hebbian_Simon.py
--rw-------   0 katherine  (1000) katherine  (1000)    10500 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Jason_Reward_rate_with_penalty_with_inputs.py
--rw-------   0 katherine  (1000) katherine  (1000)     7847 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Jason_Stroop_Stimuli.py
--rw-------   0 katherine  (1000) katherine  (1000)    20545 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Debug/Markus Stroop.py
--rw-------   0 katherine  (1000) katherine  (1000)     6800 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Predator-Prey Sebastian REDUCED.py
--rw-------   0 katherine  (1000) katherine  (1000)    16271 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Predator-Prey Sebastian.py
--rw-------   0 katherine  (1000) katherine  (1000)     8572 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/StabilityFlexibility.py
--rw-------   0 katherine  (1000) katherine  (1000)     7174 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Umemoto_Feb.py
--rw-------   0 katherine  (1000) katherine  (1000)     7261 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Umemoto_Feb2.py
--rw-------   0 katherine  (1000) katherine  (1000)    32747 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Yotam LCA Model LLVM.py
--rw-------   0 katherine  (1000) katherine  (1000)    30275 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/Yotam LCA Model.py
--rw-------   0 katherine  (1000) katherine  (1000)        0 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)     2222 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/bryant_lca_with_termination.py
--rw-------   0 katherine  (1000) katherine  (1000)     2531 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/build_input.py
--rw-------   0 katherine  (1000) katherine  (1000)     4734 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/dndtesting.py
--rw-------   0 katherine  (1000) katherine  (1000)     3863 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/generator_function_as_input.py
--rw-------   0 katherine  (1000) katherine  (1000)    21108 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/laura_test_no_noise_stroop_09_11_2018.py
--rw-------   0 katherine  (1000) katherine  (1000)     8965 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Debug/markus_test_umemoto.py
--rw-------   0 katherine  (1000) katherine  (1000)     6743 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/new_umemoto.py
--rw-------   0 katherine  (1000) katherine  (1000)     7018 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/stability_flexibility_simple.py
--rw-------   0 katherine  (1000) katherine  (1000)     2099 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Debug/testing_dnd.py
--rw-------   0 katherine  (1000) katherine  (1000)     2993 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Debug/testing_dnd_Q.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/Scripts/Examples/
--rw-------   0 katherine  (1000) katherine  (1000)      394 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/BIDS-MDF Example.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/Scripts/Examples/Basics And Primer/
--rw-------   0 katherine  (1000) katherine  (1000)     2309 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Basics And Primer/Stroop Model - Basic.py
--rw-------   0 katherine  (1000) katherine  (1000)     4373 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Basics And Primer/Stroop Model - Conflict Monitoring.py
--rw-------   0 katherine  (1000) katherine  (1000)        0 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Basics And Primer/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)     9399 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Botvinick Model Composition.py
--rw-------   0 katherine  (1000) katherine  (1000)     3554 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/EVC OCM.py
--rw-------   0 katherine  (1000) katherine  (1000)     8503 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/EVC-Gratton Composition.py
--rw-------   0 katherine  (1000) katherine  (1000)     2661 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/EVC-Gratton-GaussianProcess.py
--rw-------   0 katherine  (1000) katherine  (1000)     3949 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Examples/Gating-Mechanism. with UDF.py
--rw-------   0 katherine  (1000) katherine  (1000)    11952 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Gilbert_Shallice_Composition_Model.py
--rw-------   0 katherine  (1000) katherine  (1000)     1883 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/LC Control Mechanism Composition.py
--rw-------   0 katherine  (1000) katherine  (1000)      829 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/LVOC Composition.py
--rw-------   0 katherine  (1000) katherine  (1000)    11551 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Examples/Lena Rumelhart script.py
--rw-------   0 katherine  (1000) katherine  (1000)     1215 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Examples/Mixed-NN-and-DDM.py
--rw-------   0 katherine  (1000) katherine  (1000)     5154 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/Scripts/Examples/Multilayer-Learning.py
--rw-------   0 katherine  (1000) katherine  (1000)     6219 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Examples/RL-DDM.py
--rw-------   0 katherine  (1000) katherine  (1000)     1886 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Rumelhart Semantic Network.py
--rw-------   0 katherine  (1000) katherine  (1000)     8674 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/StabilityFlexibility.py
--rw-------   0 katherine  (1000) katherine  (1000)     4277 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Stroop Model.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/Scripts/Examples/Tutorial/
--rw-------   0 katherine  (1000) katherine  (1000)    14877 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Tutorial/Rumelhart Semantic Network (autodiff).py
--rw-------   0 katherine  (1000) katherine  (1000)     6558 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Tutorial/Stroop Model - EVC.py
--rw-------   0 katherine  (1000) katherine  (1000)        0 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/Tutorial/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)     4758 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/Scripts/Examples/_Gating-Mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)     4739 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Examples/_Leabra-Demo.py
--rw-------   0 katherine  (1000) katherine  (1000)     2543 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/_Leabra-Learning-Demo.py
--rw-------   0 katherine  (1000) katherine  (1000)     3604 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Examples/_Reinforcement-Learning REV.py
--rw-------   0 katherine  (1000) katherine  (1000)     4224 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Examples/_Stroop-Simple.py
--rw-------   0 katherine  (1000) katherine  (1000)        0 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)     1449 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Examples/_nested_learning.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/
--rw-------   0 katherine  (1000) katherine  (1000)     4728 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Adaptive Replay Model.py
--rw-------   0 katherine  (1000) katherine  (1000)     8617 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Bustamante_Stroop_XOR_LVOC_Model.py
--rw-------   0 katherine  (1000) katherine  (1000)     9736 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Bustamante_Stroop_XOR_LVOC_Model_VZ.py
--rw-------   0 katherine  (1000) katherine  (1000)     4667 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/ColorMotionTask_FULL.py
--rw-------   0 katherine  (1000) katherine  (1000)     1015 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/ColorMotionTask_SIMPLE.py
--rw-------   0 katherine  (1000) katherine  (1000)     3401 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/GreedyAgentInteractiveInputs.py
--rw-------   0 katherine  (1000) katherine  (1000)     4167 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/GreedyAgentModel.py
--rw-------   0 katherine  (1000) katherine  (1000)     1804 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/GreedyAgentModel_LLVM_TEST.py
--rw-------   0 katherine  (1000) katherine  (1000)      848 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/GymForagerRandomAgent.py
--rw-------   0 katherine  (1000) katherine  (1000)     6292 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/N-back.py
--rw-------   0 katherine  (1000) katherine  (1000)     1300 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/NeuroML Example.py
--rw-------   0 katherine  (1000) katherine  (1000)     6444 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/PanickyAgentModel.py
--rw-------   0 katherine  (1000) katherine  (1000)    15547 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model DEMO.py
--rw-------   0 katherine  (1000) katherine  (1000)    15801 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model DQN LVOC.py
--rw-------   0 katherine  (1000) katherine  (1000)    16470 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model DQN [ORIG].py
--rw-------   0 katherine  (1000) katherine  (1000)    15378 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model DQN.py
--rw-------   0 katherine  (1000) katherine  (1000)    10424 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model INPUT LAYER.py
--rw-------   0 katherine  (1000) katherine  (1000)    12725 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model I_0 Nested Comp.py
--rw-------   0 katherine  (1000) katherine  (1000)     8520 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model.py
--rw-------   0 katherine  (1000) katherine  (1000)        0 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)     2812 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/bi-percepts.py
--rw-------   0 katherine  (1000) katherine  (1000)     2531 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/build_input.py
--rw-------   0 katherine  (1000) katherine  (1000)     1664 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/build_stimuli_VZ.py
--rw-------   0 katherine  (1000) katherine  (1000)     1478 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/Models (Under Development)/build_stimuli_set.py
--rw-------   0 katherine  (1000) katherine  (1000)        0 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/Scripts/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)       20 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/cuda_requirements.txt
--rw-------   0 katherine  (1000) katherine  (1000)      198 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/dev_requirements.txt
--rw-------   0 katherine  (1000) katherine  (1000)       77 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/doc_requirements.txt
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/docs/
--rw-------   0 katherine  (1000) katherine  (1000)     8025 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/Makefile
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/docs/source/
--rw-------   0 katherine  (1000) katherine  (1000)      334 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/AGT.rst
--rw-------   0 katherine  (1000) katherine  (1000)      242 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/AGTControlMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      260 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/AutoAssociativeLearningMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      228 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/AutoAssociativeProjection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      143 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/AutodiffComposition.rst
--rw-------   0 katherine  (1000) katherine  (1000)    61385 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/BasicsAndPrimer.rst
--rw-------   0 katherine  (1000) katherine  (1000)     5947 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/BotvinickConflictMonitoringModel.rst
--rw-------   0 katherine  (1000) katherine  (1000)      641 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/BustamanteStroopXORLVOCModel.rst
--rw-------   0 katherine  (1000) katherine  (1000)     9581 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Cohen_HustonModel.rst
--rw-------   0 katherine  (1000) katherine  (1000)      308 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/CombinationFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      261 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ComparatorMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)     2673 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Compilation.rst
--rw-------   0 katherine  (1000) katherine  (1000)      576 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Component.rst
--rw-------   0 katherine  (1000) katherine  (1000)      239 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Components.rst
--rw-------   0 katherine  (1000) katherine  (1000)      536 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Composition.rst
--rw-------   0 katherine  (1000) katherine  (1000)      312 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/CompositionFunctionApproximator.rst
--rw-------   0 katherine  (1000) katherine  (1000)      221 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/CompositionInterfaceMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      191 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Compositions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      148 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Condition.rst
--rw-------   0 katherine  (1000) katherine  (1000)      131 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Context.rst
--rw-------   0 katherine  (1000) katherine  (1000)      236 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ContrastiveHebbianMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)     5701 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ContributorsGuide.rst
--rw-------   0 katherine  (1000) katherine  (1000)      399 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ControlMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      445 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ControlMechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      204 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ControlProjection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      166 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ControlProjections.rst
--rw-------   0 katherine  (1000) katherine  (1000)      193 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ControlSignal.rst
--rw-------   0 katherine  (1000) katherine  (1000)     9837 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ConventionsAndDefinitions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      315 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Core.rst
--rw-------   0 katherine  (1000) katherine  (1000)      166 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/DDM.rst
--rw-------   0 katherine  (1000) katherine  (1000)      186 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/DefaultControlMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      223 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Defaults.rst
--rw-------   0 katherine  (1000) katherine  (1000)      215 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/DistributionFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      361 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/EVC.rst
--rw-------   0 katherine  (1000) katherine  (1000)      265 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/EVCAuxiliary.rst
--rw-------   0 katherine  (1000) katherine  (1000)      242 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/EVCControlMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      226 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/EpisodicMemoryMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      307 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/docs/source/Function.rst
--rw-------   0 katherine  (1000) katherine  (1000)      279 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/docs/source/Functions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      205 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/GatingMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)       62 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/GatingMechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      201 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/GatingProjection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      160 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/GatingProjections.rst
--rw-------   0 katherine  (1000) katherine  (1000)      189 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/GatingSignal.rst
--rw-------   0 katherine  (1000) katherine  (1000)     1582 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/GilzenratModel.rst
--rw-------   0 katherine  (1000) katherine  (1000)      163 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/InputPort.rst
--rw-------   0 katherine  (1000) katherine  (1000)      228 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/IntegratorFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      200 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/IntegratorMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      164 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/IntegratorMechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      203 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/KWTAMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      209 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Keywords.rst
--rw-------   0 katherine  (1000) katherine  (1000)      202 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/KohonenMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      191 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LCAMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      239 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LCControlMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      214 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LCMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      191 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LeabraMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      316 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LearningFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      213 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LearningMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      195 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LearningMechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      207 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LearningProjection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      170 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LearningProjections.rst
--rw-------   0 katherine  (1000) katherine  (1000)      195 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/LearningSignal.rst
--rw-------   0 katherine  (1000) katherine  (1000)      116 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Library.rst
--rw-------   0 katherine  (1000) katherine  (1000)      220 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Log.rst
--rw-------   0 katherine  (1000) katherine  (1000)      201 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/MappingProjection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      222 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/MaskedMappingProjection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      484 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Mechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      160 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Mechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      355 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/MemoryFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      373 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Models.rst
--rw-------   0 katherine  (1000) katherine  (1000)      377 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ModulatoryMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      118 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ModulatoryMechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      433 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ModulatoryProjection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      179 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ModulatoryProjections.rst
--rw-------   0 katherine  (1000) katherine  (1000)      418 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ModulatorySignal.rst
--rw-------   0 katherine  (1000) katherine  (1000)     2922 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/MontagueModel.rst
--rw-------   0 katherine  (1000) katherine  (1000)     8526 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/NieuwenhuisModel.rst
--rw-------   0 katherine  (1000) katherine  (1000)      300 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/docs/source/NonStatefulFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      207 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ObjectiveFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      245 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ObjectiveMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      179 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ObjectiveMechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      243 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/OptimizationControlMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      319 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/OptimizationFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      154 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/OutputPort.rst
--rw-------   0 katherine  (1000) katherine  (1000)     8246 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/PCTC_model.rst
--rw-------   0 katherine  (1000) katherine  (1000)      175 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ParameterPort.rst
--rw-------   0 katherine  (1000) katherine  (1000)      155 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Parameters.rst
--rw-------   0 katherine  (1000) katherine  (1000)      125 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Pathway.rst
--rw-------   0 katherine  (1000) katherine  (1000)      397 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/PathwayProjection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      238 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/PathwayProjections.rst
--rw-------   0 katherine  (1000) katherine  (1000)      331 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Port.rst
--rw-------   0 katherine  (1000) katherine  (1000)      219 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/PredictionErrorMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      228 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Preferences.rst
--rw-------   0 katherine  (1000) katherine  (1000)      454 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ProcessingMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      162 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/ProcessingMechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      363 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Projection.rst
--rw-------   0 katherine  (1000) katherine  (1000)      101 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Projections.rst
--rw-------   0 katherine  (1000) katherine  (1000)    16577 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/QuickReference.rst
--rw-------   0 katherine  (1000) katherine  (1000)      233 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/RecurrentTransferMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)     8474 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/RefactoredLearningGuide.rst
--rw-------   0 katherine  (1000) katherine  (1000)     2418 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Registry.rst
--rw-------   0 katherine  (1000) katherine  (1000)      155 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/RegressionCFA.rst
--rw-------   0 katherine  (1000) katherine  (1000)      143 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Report.rst
--rw-------   0 katherine  (1000) katherine  (1000)      148 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Scheduler.rst
--rw-------   0 katherine  (1000) katherine  (1000)       87 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Scheduling.rst
--rw-------   0 katherine  (1000) katherine  (1000)      207 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/SelectionFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      123 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Services.rst
--rw-------   0 katherine  (1000) katherine  (1000)      219 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/StatefulFunction.rst
--rw-------   0 katherine  (1000) katherine  (1000)      274 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/docs/source/StatefulFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      251 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Subystems.rst
--rw-------   0 katherine  (1000) katherine  (1000)      133 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Time.rst
--rw-------   0 katherine  (1000) katherine  (1000)      365 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/TransferFunctions.rst
--rw-------   0 katherine  (1000) katherine  (1000)      194 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/TransferMechanism.rst
--rw-------   0 katherine  (1000) katherine  (1000)      272 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/TransferMechanisms.rst
--rw-------   0 katherine  (1000) katherine  (1000)      230 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/UserDefinedFunction.rst
--rw-------   0 katherine  (1000) katherine  (1000)       83 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/UserGuide.rst
--rw-------   0 katherine  (1000) katherine  (1000)     3775 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/UserGuide_TBD.rst
--rw-------   0 katherine  (1000) katherine  (1000)     1583 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/Visualization.rst
--rw-------   0 katherine  (1000) katherine  (1000)      103 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/globals.rst
--rw-------   0 katherine  (1000) katherine  (1000)    13160 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/docs/source/index.rst
--rw-------   0 katherine  (1000) katherine  (1000)    12851 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/index_logo_with_text.rst
--rw-------   0 katherine  (1000) katherine  (1000)      124 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/docs/source/json.rst
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/
--rw-------   0 katherine  (1000) katherine  (1000)     3712 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)      499 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/_version.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink/core/
--rw-------   0 katherine  (1000) katherine  (1000)      476 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink/core/components/
--rw-------   0 katherine  (1000) katherine  (1000)    13607 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)   179068 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/components/component.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/
--rw-------   0 katherine  (1000) katherine  (1000)     1637 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    44941 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/function.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/
--rw-------   0 katherine  (1000) katherine  (1000)        0 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    93966 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/combinationfunctions.py
--rw-------   0 katherine  (1000) katherine  (1000)    66567 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/distributionfunctions.py
--rw-------   0 katherine  (1000) katherine  (1000)   102361 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/learningfunctions.py
--rw-------   0 katherine  (1000) katherine  (1000)    48803 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/objectivefunctions.py
--rw-------   0 katherine  (1000) katherine  (1000)   125456 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/optimizationfunctions.py
--rw-------   0 katherine  (1000) katherine  (1000)    18199 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/selectionfunctions.py
--rw-------   0 katherine  (1000) katherine  (1000)   176905 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/transferfunctions.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/stateful/
--rw-------   0 katherine  (1000) katherine  (1000)      106 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/stateful/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)   230039 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/stateful/integratorfunctions.py
--rw-------   0 katherine  (1000) katherine  (1000)   145221 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/stateful/memoryfunctions.py
--rw-------   0 katherine  (1000) katherine  (1000)    26845 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/stateful/statefulfunction.py
--rw-------   0 katherine  (1000) katherine  (1000)    31027 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/functions/userdefinedfunction.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/
--rw-------   0 katherine  (1000) katherine  (1000)      257 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)   223729 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/mechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/
--rw-------   0 katherine  (1000) katherine  (1000)      604 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/
--rw-------   0 katherine  (1000) katherine  (1000)      267 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)   102880 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/controlmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    11815 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/defaultcontrolmechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/gating/
--rw-------   0 katherine  (1000) katherine  (1000)      103 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/gating/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    28204 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/gating/gatingmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    83886 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/optimizationcontrolmechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/learning/
--rw-------   0 katherine  (1000) katherine  (1000)      109 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/learning/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    81999 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/learning/learningmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    10462 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/modulatorymechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/
--rw-------   0 katherine  (1000) katherine  (1000)      722 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)     7410 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/compositioninterfacemechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)     3582 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/defaultprocessingmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    11108 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/integratormechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    52099 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/objectivemechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    12374 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/processingmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)   102155 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/transfermechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/
--rw-------   0 katherine  (1000) katherine  (1000)      441 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    81879 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/inputport.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/
--rw-------   0 katherine  (1000) katherine  (1000)      391 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    59442 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/controlsignal.py
--rw-------   0 katherine  (1000) katherine  (1000)    24705 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/gatingsignal.py
--rw-------   0 katherine  (1000) katherine  (1000)    18958 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/learningsignal.py
--rw-------   0 katherine  (1000) katherine  (1000)    41118 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/modulatorysignal.py
--rw-------   0 katherine  (1000) katherine  (1000)    94795 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/outputport.py
--rw-------   0 katherine  (1000) katherine  (1000)    67471 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/parameterport.py
--rw-------   0 katherine  (1000) katherine  (1000)   195326 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/ports/port.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/
--rw-------   0 katherine  (1000) katherine  (1000)      251 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/
--rw-------   0 katherine  (1000) katherine  (1000)      439 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    16883 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/controlprojection.py
--rw-------   0 katherine  (1000) katherine  (1000)    15140 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/gatingprojection.py
--rw-------   0 katherine  (1000) katherine  (1000)    37304 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/learningprojection.py
--rw-------   0 katherine  (1000) katherine  (1000)     7711 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/modulatoryprojection.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/pathway/
--rw-------   0 katherine  (1000) katherine  (1000)      216 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/pathway/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    34071 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/pathway/mappingprojection.py
--rw-------   0 katherine  (1000) katherine  (1000)     4948 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/pathway/pathwayprojection.py
--rw-------   0 katherine  (1000) katherine  (1000)   118640 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/components/projections/projection.py
--rw-------   0 katherine  (1000) katherine  (1000)     5713 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/components/shellclasses.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/compositions/
--rw-------   0 katherine  (1000) katherine  (1000)      432 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/compositions/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)   556248 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/compositions/composition.py
--rw-------   0 katherine  (1000) katherine  (1000)     6890 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/compositions/compositionfunctionapproximator.py
--rw-------   0 katherine  (1000) katherine  (1000)    23518 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/compositions/pathway.py
--rw-------   0 katherine  (1000) katherine  (1000)    95384 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/compositions/report.py
--rw-------   0 katherine  (1000) katherine  (1000)   139905 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/compositions/showgraph.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/globals/
--rw-------   0 katherine  (1000) katherine  (1000)      873 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    30805 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/context.py
--rw-------   0 katherine  (1000) katherine  (1000)     1791 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/defaults.py
--rw-------   0 katherine  (1000) katherine  (1000)    37844 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/json.py
--rw-------   0 katherine  (1000) katherine  (1000)    38951 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/globals/keywords.py
--rw-------   0 katherine  (1000) katherine  (1000)     2759 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/kvo.py
--rw-------   0 katherine  (1000) katherine  (1000)    88253 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/globals/log.py
--rw-------   0 katherine  (1000) katherine  (1000)    84367 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/globals/parameters.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/globals/preferences/
--rw-------   0 katherine  (1000) katherine  (1000)      454 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/preferences/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    22246 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/preferences/basepreferenceset.py
--rw-------   0 katherine  (1000) katherine  (1000)     3560 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/preferences/compositionpreferenceset.py
--rw-------   0 katherine  (1000) katherine  (1000)     9123 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/preferences/mechanismpreferenceset.py
--rw-------   0 katherine  (1000) katherine  (1000)    61417 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/preferences/preferenceset.py
--rw-------   0 katherine  (1000) katherine  (1000)    18253 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/globals/registry.py
--rw-------   0 katherine  (1000) katherine  (1000)    18591 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/sampleiterator.py
--rw-------   0 katherine  (1000) katherine  (1000)     1505 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/socket.py
--rw-------   0 katherine  (1000) katherine  (1000)    65260 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/globals/utilities.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/
--rw-------   0 katherine  (1000) katherine  (1000)     7059 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    19338 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/builder_context.py
--rw-------   0 katherine  (1000) katherine  (1000)    30464 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/builtins.py
--rw-------   0 katherine  (1000) katherine  (1000)    46132 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/codegen.py
--rw-------   0 katherine  (1000) katherine  (1000)     2689 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/debug.py
--rw-------   0 katherine  (1000) katherine  (1000)    30681 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/execution.py
--rw-------   0 katherine  (1000) katherine  (1000)    26207 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/helpers.py
--rw-------   0 katherine  (1000) katherine  (1000)    13395 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/llvm/jit_engine.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/rpc/
--rw-------   0 katherine  (1000) katherine  (1000)       65 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/rpc/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    35165 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/rpc/graph_pb2.py
--rw-------   0 katherine  (1000) katherine  (1000)    15842 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/core/rpc/graph_pb2_grpc.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/core/scheduling/
--rw-------   0 katherine  (1000) katherine  (1000)     2766 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/scheduling/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)     5378 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/scheduling/condition.py
--rw-------   0 katherine  (1000) katherine  (1000)    10887 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/scheduling/scheduler.py
--rw-------   0 katherine  (1000) katherine  (1000)     1369 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/core/scheduling/time.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/
--rw-------   0 katherine  (1000) katherine  (1000)      339 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/
--rw-------   0 katherine  (1000) katherine  (1000)      177 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/
--rw-------   0 katherine  (1000) katherine  (1000)      174 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/
--rw-------   0 katherine  (1000) katherine  (1000)      159 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/control/
--rw-------   0 katherine  (1000) katherine  (1000)       67 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/control/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/control/agt/
--rw-------   0 katherine  (1000) katherine  (1000)      225 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/control/agt/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    21304 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/control/agt/agtcontrolmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    50288 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/control/agt/lccontrolmechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/learning/
--rw-------   0 katherine  (1000) katherine  (1000)      282 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/learning/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    22068 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/learning/autoassociativelearningmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    20987 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/learning/kohonenlearningmechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/
--rw-------   0 katherine  (1000) katherine  (1000)      352 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/integrator/
--rw-------   0 katherine  (1000) katherine  (1000)      192 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/integrator/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    65940 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/integrator/ddm.py
--rw-------   0 katherine  (1000) katherine  (1000)    39647 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/integrator/episodicmemorymechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    28253 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/leabramechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/objective/
--rw-------   0 katherine  (1000) katherine  (1000)      243 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/objective/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    25362 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/objective/comparatormechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    15130 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/objective/predictionerrormechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/
--rw-------   0 katherine  (1000) katherine  (1000)      564 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    69655 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/contrastivehebbianmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    21681 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/kohonenmechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    33070 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/kwtamechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    28046 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/lcamechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    71731 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/recurrenttransfermechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/projections/
--rw-------   0 katherine  (1000) katherine  (1000)       79 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/projections/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/components/projections/pathway/
--rw-------   0 katherine  (1000) katherine  (1000)      258 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/projections/pathway/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    18973 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/components/projections/pathway/autoassociativeprojection.py
--rw-------   0 katherine  (1000) katherine  (1000)     9806 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/components/projections/pathway/maskedmappingprojection.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/
--rw-------   0 katherine  (1000) katherine  (1000)      221 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)    26257 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/autodiffcomposition.py
--rw-------   0 katherine  (1000) katherine  (1000)     3248 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/compiledloss.py
--rw-------   0 katherine  (1000) katherine  (1000)    10643 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/compiledoptimizer.py
--rw-------   0 katherine  (1000) katherine  (1000)    11617 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/compositionrunner.py
--rw-------   0 katherine  (1000) katherine  (1000)     9908 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/gymforagercfa.py
--rw-------   0 katherine  (1000) katherine  (1000)     9165 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/pytorchcomponents.py
--rw-------   0 katherine  (1000) katherine  (1000)     5718 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/pytorchllvmhelper.py
--rw-------   0 katherine  (1000) katherine  (1000)    17308 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/pytorchmodelcreator.py
--rw-------   0 katherine  (1000) katherine  (1000)    32737 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/psyneulink/library/compositions/regressioncfa.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/psyneulink/library/models/
--rw-------   0 katherine  (1000) katherine  (1000)    14915 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/models/Cohen_Huston1994.py
--rw-------   0 katherine  (1000) katherine  (1000)    19995 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/models/Cohen_Huston1994_horse_race.py
--rw-------   0 katherine  (1000) katherine  (1000)     9253 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/models/GilzenratModel.py
--rw-------   0 katherine  (1000) katherine  (1000)    20616 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/models/Kalanthroff_PCTC_2018.py
--rw-------   0 katherine  (1000) katherine  (1000)    10121 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/models/MontagueDayanSejnowski96.py
--rw-------   0 katherine  (1000) katherine  (1000)    12656 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/models/Nieuwenhuis2005Model.py
--rw-------   0 katherine  (1000) katherine  (1000)        0 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/psyneulink/library/models/__init__.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink.egg-info/
--rw-------   0 katherine  (1000) katherine  (1000)    15089 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink.egg-info/PKG-INFO
--rw-------   0 katherine  (1000) katherine  (1000)    19489 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink.egg-info/SOURCES.txt
--rw-------   0 katherine  (1000) katherine  (1000)        1 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink.egg-info/dependency_links.txt
--rw-------   0 katherine  (1000) katherine  (1000)      826 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink.egg-info/requires.txt
--rw-------   0 katherine  (1000) katherine  (1000)       19 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/psyneulink.egg-info/top_level.txt
--rw-------   0 katherine  (1000) katherine  (1000)      451 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/requirements.txt
--rw-------   0 katherine  (1000) katherine  (1000)     2629 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/setup.cfg
--rw-------   0 katherine  (1000) katherine  (1000)     2779 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/setup.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:58.000000 psyneulink-0.9.1.0/tests/
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/api/
--rw-------   0 katherine  (1000) katherine  (1000)     5196 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/api/test_api.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/components/
--rw-------   0 katherine  (1000) katherine  (1000)     3823 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/components/test_component.py
--rw-------   0 katherine  (1000) katherine  (1000)     2595 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/components/test_general.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/composition/
--rw-------   0 katherine  (1000) katherine  (1000)   145271 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/composition/test_autodiffcomposition.py
--rw-------   0 katherine  (1000) katherine  (1000)   297744 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/composition/test_composition.py
--rw-------   0 katherine  (1000) katherine  (1000)   128455 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/composition/test_control.py
--rw-------   0 katherine  (1000) katherine  (1000)     3074 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/composition/test_gating.py
--rw-------   0 katherine  (1000) katherine  (1000)     1248 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/composition/test_graph.py
--rw-------   0 katherine  (1000) katherine  (1000)    38900 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/composition/test_interfaces.py
--rw-------   0 katherine  (1000) katherine  (1000)   295082 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/composition/test_learning.py
--rw-------   0 katherine  (1000) katherine  (1000)    35169 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/composition/test_models.py
--rw-------   0 katherine  (1000) katherine  (1000)   809874 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/composition/test_report.py
--rw-------   0 katherine  (1000) katherine  (1000)    40559 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/composition/test_runtime_params.py
--rw-------   0 katherine  (1000) katherine  (1000)   488058 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/composition/test_show_graph.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/control/
--rw-------   0 katherine  (1000) katherine  (1000)    14792 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/control/test_gilzenrat.py
--rw-------   0 katherine  (1000) katherine  (1000)     6762 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/control/test_param_estimation.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/documentation/
--rw-------   0 katherine  (1000) katherine  (1000)     3737 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/tests/documentation/test_module_docs.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/functions/
--rw-------   0 katherine  (1000) katherine  (1000)     6730 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_accumulator_integrator.py
--rw-------   0 katherine  (1000) katherine  (1000)     8466 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_buffer.py
--rw-------   0 katherine  (1000) katherine  (1000)    14104 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_combination.py
--rw-------   0 katherine  (1000) katherine  (1000)      523 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_default_allocation.py
--rw-------   0 katherine  (1000) katherine  (1000)     3175 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_distance.py
--rw-------   0 katherine  (1000) katherine  (1000)     2822 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_distribution.py
--rw-------   0 katherine  (1000) katherine  (1000)     3252 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_fhn_integrator.py
--rw-------   0 katherine  (1000) katherine  (1000)     4073 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/tests/functions/test_functions.py
--rw-------   0 katherine  (1000) katherine  (1000)      576 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_identity.py
--rw-------   0 katherine  (1000) katherine  (1000)    12310 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_integrator.py
--rw-------   0 katherine  (1000) katherine  (1000)    65528 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_memory.py
--rw-------   0 katherine  (1000) katherine  (1000)      226 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/functions/test_objective.py
--rw-------   0 katherine  (1000) katherine  (1000)     4171 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_optimization.py
--rw-------   0 katherine  (1000) katherine  (1000)     2318 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_selection.py
--rw-------   0 katherine  (1000) katherine  (1000)     1581 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_stability.py
--rw-------   0 katherine  (1000) katherine  (1000)     8301 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/functions/test_transfer.py
--rw-------   0 katherine  (1000) katherine  (1000)    24972 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/tests/functions/test_user_defined_func.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/json/
--rw-------   0 katherine  (1000) katherine  (1000)      225 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/json/model_backprop.py
--rw-------   0 katherine  (1000) katherine  (1000)      518 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/json/model_basic.py
--rw-------   0 katherine  (1000) katherine  (1000)     1125 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/json/model_nested_comp_with_scheduler.py
--rw-------   0 katherine  (1000) katherine  (1000)     2229 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/json/model_with_control.py
--rw-------   0 katherine  (1000) katherine  (1000)      876 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/json/model_with_two_conjoint_comps.py
--rw-------   0 katherine  (1000) katherine  (1000)     1018 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/json/model_with_two_disjoint_comps.py
--rw-------   0 katherine  (1000) katherine  (1000)     2884 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/json/stroop_conflict_monitoring.py
--rw-------   0 katherine  (1000) katherine  (1000)     4130 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/json/test_json.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/llvm/
--rw-------   0 katherine  (1000) katherine  (1000)     1921 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/llvm/test_builtins_intrinsics.py
--rw-------   0 katherine  (1000) katherine  (1000)     7986 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/llvm/test_builtins_matrix.py
--rw-------   0 katherine  (1000) katherine  (1000)     5100 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/llvm/test_builtins_random.py
--rw-------   0 katherine  (1000) katherine  (1000)     2561 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/llvm/test_builtins_vector.py
--rw-------   0 katherine  (1000) katherine  (1000)     1470 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/llvm/test_compile.py
--rw-------   0 katherine  (1000) katherine  (1000)     3791 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/llvm/test_custom_func.py
--rw-------   0 katherine  (1000) katherine  (1000)     2361 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/tests/llvm/test_debug_composition.py
--rw-------   0 katherine  (1000) katherine  (1000)    18380 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/llvm/test_helpers.py
--rw-------   0 katherine  (1000) katherine  (1000)     5306 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/llvm/test_llvm_lite.py
--rw-------   0 katherine  (1000) katherine  (1000)     9753 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/llvm/test_multiple_executions.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/log/
--rw-------   0 katherine  (1000) katherine  (1000)    64315 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/log/test_log.py
--rw-------   0 katherine  (1000) katherine  (1000)    33890 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/log/test_rpc.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/mechanisms/
--rw-------   0 katherine  (1000) katherine  (1000)     6513 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_contrastive_hebbian_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    15017 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_control_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    24957 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_ddm_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)     3347 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_drift_diffusion_analytical.py
--rw-------   0 katherine  (1000) katherine  (1000)    12209 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_episodic_memory.py
--rw-------   0 katherine  (1000) katherine  (1000)     6218 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_gating_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    15331 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/mechanisms/test_input_output_labels.py
--rw-------   0 katherine  (1000) katherine  (1000)    39125 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_input_state_spec.py
--rw-------   0 katherine  (1000) katherine  (1000)    53567 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_integrator_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    19873 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_kwta.py
--rw-------   0 katherine  (1000) katherine  (1000)    16336 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_lca.py
--rw-------   0 katherine  (1000) katherine  (1000)    13916 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_leabra_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)     8245 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/mechanisms/test_mechanisms.py
--rw-------   0 katherine  (1000) katherine  (1000)     2468 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/mechanisms/test_modulatory_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)      755 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_objective_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    16270 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_processing_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    59905 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_recurrent_transfer_mechanism.py
--rw-------   0 katherine  (1000) katherine  (1000)    76702 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/mechanisms/test_transfer_mechanism.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/misc/
--rw-------   0 katherine  (1000) katherine  (1000)     1763 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/misc/test_notebooks.py
--rw-------   0 katherine  (1000) katherine  (1000)    13637 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/misc/test_parameters.py
--rw-------   0 katherine  (1000) katherine  (1000)      380 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/misc/test_user_seed.py
--rw-------   0 katherine  (1000) katherine  (1000)     1933 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/misc/test_utilities.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/models/
--rw-------   0 katherine  (1000) katherine  (1000)     8909 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/models/test_bi_percepts.py
--rw-------   0 katherine  (1000) katherine  (1000)    16914 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/models/test_botvinick.py
--rw-------   0 katherine  (1000) katherine  (1000)     3564 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/models/test_documentation_models.py
--rw-------   0 katherine  (1000) katherine  (1000)    10660 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/models/test_greedy_agent.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/naming/
--rw-------   0 katherine  (1000) katherine  (1000)    11267 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/naming/test_naming.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/ports/
--rw-------   0 katherine  (1000) katherine  (1000)     5201 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/ports/test_input_ports.py
--rw-------   0 katherine  (1000) katherine  (1000)     3042 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/ports/test_modulatory_signals.py
--rw-------   0 katherine  (1000) katherine  (1000)     3181 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/ports/test_output_ports.py
--rw-------   0 katherine  (1000) katherine  (1000)     7987 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/ports/test_parameter_ports.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/projections/
--rw-------   0 katherine  (1000) katherine  (1000)      706 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/projections/test_projection.py
--rw-------   0 katherine  (1000) katherine  (1000)    24046 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/projections/test_projection_specifications.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tests/scheduling/
--rw-------   0 katherine  (1000) katherine  (1000)     1033 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/scheduling/conftest.py
--rw-------   0 katherine  (1000) katherine  (1000)    42122 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/tests/scheduling/test_condition.py
--rw-------   0 katherine  (1000) katherine  (1000)    69059 2021-08-10 00:23:57.000000 psyneulink-0.9.1.0/tests/scheduling/test_scheduler.py
--rw-------   0 katherine  (1000) katherine  (1000)    22296 2021-06-22 02:06:49.000000 psyneulink-0.9.1.0/tests/scheduling/test_system_newsched.py
--rw-------   0 katherine  (1000) katherine  (1000)     2238 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tests/scheduling/test_time.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2021-08-10 00:23:59.000000 psyneulink-0.9.1.0/tutorial/
--rw-------   0 katherine  (1000) katherine  (1000)   150549 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tutorial/PsyNeuLink Tutorial.ipynb
--rw-------   0 katherine  (1000) katherine  (1000)       48 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/tutorial_requirements.txt
--rw-------   0 katherine  (1000) katherine  (1000)    68611 2021-05-11 04:55:31.000000 psyneulink-0.9.1.0/versioneer.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/
+-rw-------   0 katherine  (1000) katherine  (1000)      451 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/CONTRIBUTING.md
+-rw-------   0 katherine  (1000) katherine  (1000)     9993 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/CONVENTIONS.md
+-rw-------   0 katherine  (1000) katherine  (1000)    11358 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/LICENSE.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      209 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/MANIFEST.in
+-rw-------   0 katherine  (1000) katherine  (1000)    15089 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/PKG-INFO
+-rw-------   0 katherine  (1000) katherine  (1000)    12268 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/README.rst
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/Scripts/
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/Scripts/Debug/
+-rw-------   0 katherine  (1000) katherine  (1000)     1662 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Hebbian_Simon.py
+-rw-------   0 katherine  (1000) katherine  (1000)    10500 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Jason_Reward_rate_with_penalty_with_inputs.py
+-rw-------   0 katherine  (1000) katherine  (1000)     7847 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Jason_Stroop_Stimuli.py
+-rw-------   0 katherine  (1000) katherine  (1000)    20545 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Markus Stroop.py
+-rw-------   0 katherine  (1000) katherine  (1000)     6800 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Predator-Prey Sebastian REDUCED.py
+-rw-------   0 katherine  (1000) katherine  (1000)    16271 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Predator-Prey Sebastian.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8572 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/StabilityFlexibility.py
+-rw-------   0 katherine  (1000) katherine  (1000)     7174 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Umemoto_Feb.py
+-rw-------   0 katherine  (1000) katherine  (1000)     7261 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Umemoto_Feb2.py
+-rw-------   0 katherine  (1000) katherine  (1000)    32747 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Yotam LCA Model LLVM.py
+-rw-------   0 katherine  (1000) katherine  (1000)    30275 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/Yotam LCA Model.py
+-rw-------   0 katherine  (1000) katherine  (1000)        0 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2222 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/bryant_lca_with_termination.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2531 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/build_input.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4734 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/dndtesting.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3863 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/generator_function_as_input.py
+-rw-------   0 katherine  (1000) katherine  (1000)    21108 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/laura_test_no_noise_stroop_09_11_2018.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8965 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/markus_test_umemoto.py
+-rw-------   0 katherine  (1000) katherine  (1000)     6743 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/new_umemoto.py
+-rw-------   0 katherine  (1000) katherine  (1000)     7018 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/stability_flexibility_simple.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2099 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/testing_dnd.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2993 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Debug/testing_dnd_Q.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/Scripts/Examples/
+-rw-------   0 katherine  (1000) katherine  (1000)      394 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/BIDS-MDF Example.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/Scripts/Examples/Basics And Primer/
+-rw-------   0 katherine  (1000) katherine  (1000)     2309 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Basics And Primer/Stroop Model - Basic.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4373 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Basics And Primer/Stroop Model - Conflict Monitoring.py
+-rw-------   0 katherine  (1000) katherine  (1000)        0 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Basics And Primer/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9399 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Botvinick Model Composition.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3554 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/EVC OCM.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8503 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/EVC-Gratton Composition.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2661 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/EVC-Gratton-GaussianProcess.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3949 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Gating-Mechanism. with UDF.py
+-rw-------   0 katherine  (1000) katherine  (1000)    11952 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Gilbert_Shallice_Composition_Model.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1883 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/LC Control Mechanism Composition.py
+-rw-------   0 katherine  (1000) katherine  (1000)      829 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/LVOC Composition.py
+-rw-------   0 katherine  (1000) katherine  (1000)    11551 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Lena Rumelhart script.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1215 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Mixed-NN-and-DDM.py
+-rw-------   0 katherine  (1000) katherine  (1000)     5154 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Multilayer-Learning.py
+-rw-------   0 katherine  (1000) katherine  (1000)     6219 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/RL-DDM.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1886 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Rumelhart Semantic Network.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8674 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/StabilityFlexibility.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4277 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Stroop Model.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/Scripts/Examples/Tutorial/
+-rw-------   0 katherine  (1000) katherine  (1000)    14877 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Tutorial/Rumelhart Semantic Network (autodiff).py
+-rw-------   0 katherine  (1000) katherine  (1000)     6558 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Tutorial/Stroop Model - EVC.py
+-rw-------   0 katherine  (1000) katherine  (1000)        0 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/Tutorial/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4758 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/_Gating-Mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4739 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/_Leabra-Demo.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2543 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/_Leabra-Learning-Demo.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3604 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/_Reinforcement-Learning REV.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4224 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/_Stroop-Simple.py
+-rw-------   0 katherine  (1000) katherine  (1000)        0 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1449 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Examples/_nested_learning.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/
+-rw-------   0 katherine  (1000) katherine  (1000)     4728 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Adaptive Replay Model.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8617 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Bustamante_Stroop_XOR_LVOC_Model.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9736 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Bustamante_Stroop_XOR_LVOC_Model_VZ.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4667 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/ColorMotionTask_FULL.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1015 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/ColorMotionTask_SIMPLE.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3401 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/GreedyAgentInteractiveInputs.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4167 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/GreedyAgentModel.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1804 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/GreedyAgentModel_LLVM_TEST.py
+-rw-------   0 katherine  (1000) katherine  (1000)      848 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/GymForagerRandomAgent.py
+-rw-------   0 katherine  (1000) katherine  (1000)     6292 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/N-back.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1300 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/NeuroML Example.py
+-rw-------   0 katherine  (1000) katherine  (1000)     6444 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/PanickyAgentModel.py
+-rw-------   0 katherine  (1000) katherine  (1000)    15547 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model DEMO.py
+-rw-------   0 katherine  (1000) katherine  (1000)    15801 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model DQN LVOC.py
+-rw-------   0 katherine  (1000) katherine  (1000)    16470 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model DQN [ORIG].py
+-rw-------   0 katherine  (1000) katherine  (1000)    15378 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model DQN.py
+-rw-------   0 katherine  (1000) katherine  (1000)    10424 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model INPUT LAYER.py
+-rw-------   0 katherine  (1000) katherine  (1000)    12725 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model I_0 Nested Comp.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8520 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model.py
+-rw-------   0 katherine  (1000) katherine  (1000)        0 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2812 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/bi-percepts.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2531 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/build_input.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1664 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/build_stimuli_VZ.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1478 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/Models (Under Development)/build_stimuli_set.py
+-rw-------   0 katherine  (1000) katherine  (1000)        0 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/Scripts/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)       20 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/cuda_requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      198 2021-09-17 02:21:55.000000 psyneulink-0.9.1.1/dev_requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)       77 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/doc_requirements.txt
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/docs/
+-rw-------   0 katherine  (1000) katherine  (1000)     8348 2021-09-17 02:21:55.000000 psyneulink-0.9.1.1/docs/Makefile
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/docs/source/
+-rw-------   0 katherine  (1000) katherine  (1000)      334 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/AGT.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      242 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/AGTControlMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      260 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/AutoAssociativeLearningMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      228 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/AutoAssociativeProjection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      143 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/AutodiffComposition.rst
+-rw-------   0 katherine  (1000) katherine  (1000)    61385 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/BasicsAndPrimer.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     5947 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/BotvinickConflictMonitoringModel.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      641 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/BustamanteStroopXORLVOCModel.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     9581 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Cohen_HustonModel.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      308 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/CombinationFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      261 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ComparatorMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     2673 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Compilation.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      576 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Component.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      239 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Components.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      536 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Composition.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      312 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/CompositionFunctionApproximator.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      221 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/CompositionInterfaceMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      191 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Compositions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      148 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Condition.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      131 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Context.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      236 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ContrastiveHebbianMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     5701 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ContributorsGuide.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      399 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ControlMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      445 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ControlMechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      204 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ControlProjection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      166 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ControlProjections.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      193 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ControlSignal.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     9837 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ConventionsAndDefinitions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      315 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Core.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      166 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/DDM.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      186 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/DefaultControlMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      223 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Defaults.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      215 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/DistributionFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      361 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/EVC.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      265 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/EVCAuxiliary.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      242 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/EVCControlMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      226 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/EpisodicMemoryMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      307 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Function.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      279 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Functions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      205 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/GatingMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)       62 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/GatingMechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      201 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/GatingProjection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      160 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/GatingProjections.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      189 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/GatingSignal.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     1582 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/GilzenratModel.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      163 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/InputPort.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      228 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/IntegratorFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      200 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/IntegratorMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      164 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/IntegratorMechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      203 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/KWTAMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      209 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Keywords.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      202 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/KohonenMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      191 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LCAMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      239 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LCControlMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      214 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LCMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      191 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LeabraMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      316 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LearningFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      213 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LearningMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      195 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LearningMechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      207 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LearningProjection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      170 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LearningProjections.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      195 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/LearningSignal.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      116 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Library.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      220 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Log.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      201 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/MappingProjection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      222 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/MaskedMappingProjection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      484 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Mechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      160 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Mechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      355 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/MemoryFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      373 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Models.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      377 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ModulatoryMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      118 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ModulatoryMechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      433 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ModulatoryProjection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      179 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ModulatoryProjections.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      418 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ModulatorySignal.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     2922 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/MontagueModel.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     8526 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/NieuwenhuisModel.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      300 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/NonStatefulFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      207 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ObjectiveFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      245 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ObjectiveMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      179 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ObjectiveMechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      243 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/OptimizationControlMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      319 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/OptimizationFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      154 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/OutputPort.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     8246 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/PCTC_model.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      175 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ParameterPort.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      155 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Parameters.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      125 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Pathway.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      397 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/PathwayProjection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      238 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/PathwayProjections.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      331 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Port.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      219 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/PredictionErrorMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      228 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Preferences.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      454 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ProcessingMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      162 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/ProcessingMechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      363 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Projection.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      101 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Projections.rst
+-rw-------   0 katherine  (1000) katherine  (1000)    16577 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/QuickReference.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      233 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/RecurrentTransferMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     8474 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/RefactoredLearningGuide.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     2418 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Registry.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      155 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/RegressionCFA.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      143 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Report.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      148 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Scheduler.rst
+-rw-------   0 katherine  (1000) katherine  (1000)       87 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Scheduling.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      207 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/SelectionFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      123 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Services.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      219 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/StatefulFunction.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      274 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/StatefulFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      251 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Subystems.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      133 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Time.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      365 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/TransferFunctions.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      194 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/TransferMechanism.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      272 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/TransferMechanisms.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      230 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/UserDefinedFunction.rst
+-rw-------   0 katherine  (1000) katherine  (1000)       83 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/UserGuide.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     3775 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/UserGuide_TBD.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     1583 2021-08-24 20:29:10.000000 psyneulink-0.9.1.1/docs/source/Visualization.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      103 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/docs/source/globals.rst
+-rw-------   0 katherine  (1000) katherine  (1000)    13160 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/docs/source/index.rst
+-rw-------   0 katherine  (1000) katherine  (1000)    12851 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/docs/source/index_logo_with_text.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      124 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/docs/source/json.rst
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/
+-rw-------   0 katherine  (1000) katherine  (1000)     3712 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)      499 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/_version.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/
+-rw-------   0 katherine  (1000) katherine  (1000)      476 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/
+-rw-------   0 katherine  (1000) katherine  (1000)    13607 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)   179070 2021-09-17 02:21:55.000000 psyneulink-0.9.1.1/psyneulink/core/components/component.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/
+-rw-------   0 katherine  (1000) katherine  (1000)     1637 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    44941 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/function.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/
+-rw-------   0 katherine  (1000) katherine  (1000)        0 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    93966 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/combinationfunctions.py
+-rw-------   0 katherine  (1000) katherine  (1000)    66567 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/distributionfunctions.py
+-rw-------   0 katherine  (1000) katherine  (1000)   102361 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/learningfunctions.py
+-rw-------   0 katherine  (1000) katherine  (1000)    48803 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/objectivefunctions.py
+-rw-------   0 katherine  (1000) katherine  (1000)   125456 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/optimizationfunctions.py
+-rw-------   0 katherine  (1000) katherine  (1000)    18199 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/selectionfunctions.py
+-rw-------   0 katherine  (1000) katherine  (1000)   176905 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/transferfunctions.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/stateful/
+-rw-------   0 katherine  (1000) katherine  (1000)      106 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/stateful/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)   230039 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/stateful/integratorfunctions.py
+-rw-------   0 katherine  (1000) katherine  (1000)   145221 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/stateful/memoryfunctions.py
+-rw-------   0 katherine  (1000) katherine  (1000)    26845 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/stateful/statefulfunction.py
+-rw-------   0 katherine  (1000) katherine  (1000)    31027 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/functions/userdefinedfunction.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/
+-rw-------   0 katherine  (1000) katherine  (1000)      257 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)   223729 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/mechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/
+-rw-------   0 katherine  (1000) katherine  (1000)      604 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/
+-rw-------   0 katherine  (1000) katherine  (1000)      267 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)   102880 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/controlmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    11815 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/defaultcontrolmechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/gating/
+-rw-------   0 katherine  (1000) katherine  (1000)      103 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/gating/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    28204 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/gating/gatingmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    83886 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/optimizationcontrolmechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/learning/
+-rw-------   0 katherine  (1000) katherine  (1000)      109 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/learning/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    81999 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/learning/learningmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    10462 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/modulatorymechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/
+-rw-------   0 katherine  (1000) katherine  (1000)      722 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)     7410 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/compositioninterfacemechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3582 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/defaultprocessingmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    11108 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/integratormechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    52099 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/objectivemechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    12374 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/processingmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)   102155 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/transfermechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/
+-rw-------   0 katherine  (1000) katherine  (1000)      441 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    81879 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/inputport.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/
+-rw-------   0 katherine  (1000) katherine  (1000)      391 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    59442 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/controlsignal.py
+-rw-------   0 katherine  (1000) katherine  (1000)    24705 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/gatingsignal.py
+-rw-------   0 katherine  (1000) katherine  (1000)    18958 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/learningsignal.py
+-rw-------   0 katherine  (1000) katherine  (1000)    41118 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/modulatorysignal.py
+-rw-------   0 katherine  (1000) katherine  (1000)    94795 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/outputport.py
+-rw-------   0 katherine  (1000) katherine  (1000)    67471 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/parameterport.py
+-rw-------   0 katherine  (1000) katherine  (1000)   195326 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/ports/port.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/
+-rw-------   0 katherine  (1000) katherine  (1000)      251 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/
+-rw-------   0 katherine  (1000) katherine  (1000)      439 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    16883 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/controlprojection.py
+-rw-------   0 katherine  (1000) katherine  (1000)    15140 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/gatingprojection.py
+-rw-------   0 katherine  (1000) katherine  (1000)    37304 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/learningprojection.py
+-rw-------   0 katherine  (1000) katherine  (1000)     7711 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/modulatoryprojection.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/pathway/
+-rw-------   0 katherine  (1000) katherine  (1000)      216 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/pathway/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    34071 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/pathway/mappingprojection.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4948 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/pathway/pathwayprojection.py
+-rw-------   0 katherine  (1000) katherine  (1000)   118640 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/projections/projection.py
+-rw-------   0 katherine  (1000) katherine  (1000)     5713 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/components/shellclasses.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/compositions/
+-rw-------   0 katherine  (1000) katherine  (1000)      432 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/compositions/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)   556353 2021-09-17 02:21:55.000000 psyneulink-0.9.1.1/psyneulink/core/compositions/composition.py
+-rw-------   0 katherine  (1000) katherine  (1000)     6890 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/compositions/compositionfunctionapproximator.py
+-rw-------   0 katherine  (1000) katherine  (1000)    23518 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/compositions/pathway.py
+-rw-------   0 katherine  (1000) katherine  (1000)    95384 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/compositions/report.py
+-rw-------   0 katherine  (1000) katherine  (1000)   139905 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/compositions/showgraph.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/globals/
+-rw-------   0 katherine  (1000) katherine  (1000)      873 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    30805 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/context.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1791 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/defaults.py
+-rw-------   0 katherine  (1000) katherine  (1000)    37844 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/json.py
+-rw-------   0 katherine  (1000) katherine  (1000)    38951 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/keywords.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2759 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/kvo.py
+-rw-------   0 katherine  (1000) katherine  (1000)    88253 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/log.py
+-rw-------   0 katherine  (1000) katherine  (1000)    84367 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/parameters.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/globals/preferences/
+-rw-------   0 katherine  (1000) katherine  (1000)      454 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/preferences/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    22246 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/preferences/basepreferenceset.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3560 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/preferences/compositionpreferenceset.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9123 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/preferences/mechanismpreferenceset.py
+-rw-------   0 katherine  (1000) katherine  (1000)    61417 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/preferences/preferenceset.py
+-rw-------   0 katherine  (1000) katherine  (1000)    18253 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/registry.py
+-rw-------   0 katherine  (1000) katherine  (1000)    18591 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/sampleiterator.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1505 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/globals/socket.py
+-rw-------   0 katherine  (1000) katherine  (1000)    65581 2021-09-17 02:21:55.000000 psyneulink-0.9.1.1/psyneulink/core/globals/utilities.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/
+-rw-------   0 katherine  (1000) katherine  (1000)     7059 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    19338 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/builder_context.py
+-rw-------   0 katherine  (1000) katherine  (1000)    30464 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/builtins.py
+-rw-------   0 katherine  (1000) katherine  (1000)    46132 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/codegen.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2689 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/debug.py
+-rw-------   0 katherine  (1000) katherine  (1000)    30681 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/execution.py
+-rw-------   0 katherine  (1000) katherine  (1000)    26207 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/helpers.py
+-rw-------   0 katherine  (1000) katherine  (1000)    13395 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/llvm/jit_engine.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/rpc/
+-rw-------   0 katherine  (1000) katherine  (1000)       65 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/rpc/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    35165 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/rpc/graph_pb2.py
+-rw-------   0 katherine  (1000) katherine  (1000)    15842 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/rpc/graph_pb2_grpc.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/core/scheduling/
+-rw-------   0 katherine  (1000) katherine  (1000)     2766 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/scheduling/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)     5378 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/scheduling/condition.py
+-rw-------   0 katherine  (1000) katherine  (1000)    10887 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/scheduling/scheduler.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1369 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/core/scheduling/time.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/
+-rw-------   0 katherine  (1000) katherine  (1000)      339 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/
+-rw-------   0 katherine  (1000) katherine  (1000)      177 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/
+-rw-------   0 katherine  (1000) katherine  (1000)      174 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/
+-rw-------   0 katherine  (1000) katherine  (1000)      159 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/control/
+-rw-------   0 katherine  (1000) katherine  (1000)       67 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/control/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/control/agt/
+-rw-------   0 katherine  (1000) katherine  (1000)      225 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/control/agt/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    21304 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/control/agt/agtcontrolmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    50288 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/control/agt/lccontrolmechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/learning/
+-rw-------   0 katherine  (1000) katherine  (1000)      282 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/learning/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    22068 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/learning/autoassociativelearningmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    20987 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/learning/kohonenlearningmechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/
+-rw-------   0 katherine  (1000) katherine  (1000)      352 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/integrator/
+-rw-------   0 katherine  (1000) katherine  (1000)      192 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/integrator/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    65940 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/integrator/ddm.py
+-rw-------   0 katherine  (1000) katherine  (1000)    39647 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/integrator/episodicmemorymechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    28253 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/leabramechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/objective/
+-rw-------   0 katherine  (1000) katherine  (1000)      243 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/objective/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    25362 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/objective/comparatormechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    15130 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/objective/predictionerrormechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/
+-rw-------   0 katherine  (1000) katherine  (1000)      564 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    69655 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/contrastivehebbianmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    21681 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/kohonenmechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    33070 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/kwtamechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    28046 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/lcamechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    71731 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/recurrenttransfermechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/projections/
+-rw-------   0 katherine  (1000) katherine  (1000)       79 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/projections/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/components/projections/pathway/
+-rw-------   0 katherine  (1000) katherine  (1000)      258 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/projections/pathway/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    18973 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/projections/pathway/autoassociativeprojection.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9806 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/components/projections/pathway/maskedmappingprojection.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/
+-rw-------   0 katherine  (1000) katherine  (1000)      221 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)    26257 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/autodiffcomposition.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3248 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/compiledloss.py
+-rw-------   0 katherine  (1000) katherine  (1000)    10643 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/compiledoptimizer.py
+-rw-------   0 katherine  (1000) katherine  (1000)    11617 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/compositionrunner.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9908 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/gymforagercfa.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9165 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/pytorchcomponents.py
+-rw-------   0 katherine  (1000) katherine  (1000)     5718 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/pytorchllvmhelper.py
+-rw-------   0 katherine  (1000) katherine  (1000)    17308 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/pytorchmodelcreator.py
+-rw-------   0 katherine  (1000) katherine  (1000)    32737 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/compositions/regressioncfa.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink/library/models/
+-rw-------   0 katherine  (1000) katherine  (1000)    14915 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/models/Cohen_Huston1994.py
+-rw-------   0 katherine  (1000) katherine  (1000)    19995 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/models/Cohen_Huston1994_horse_race.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9253 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/models/GilzenratModel.py
+-rw-------   0 katherine  (1000) katherine  (1000)    20616 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/models/Kalanthroff_PCTC_2018.py
+-rw-------   0 katherine  (1000) katherine  (1000)    10121 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/models/MontagueDayanSejnowski96.py
+-rw-------   0 katherine  (1000) katherine  (1000)    12656 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/models/Nieuwenhuis2005Model.py
+-rw-------   0 katherine  (1000) katherine  (1000)        0 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/psyneulink/library/models/__init__.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink.egg-info/
+-rw-------   0 katherine  (1000) katherine  (1000)    15089 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink.egg-info/PKG-INFO
+-rw-------   0 katherine  (1000) katherine  (1000)    19489 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink.egg-info/SOURCES.txt
+-rw-------   0 katherine  (1000) katherine  (1000)        1 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink.egg-info/dependency_links.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      827 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink.egg-info/requires.txt
+-rw-------   0 katherine  (1000) katherine  (1000)       19 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/psyneulink.egg-info/top_level.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      452 2021-09-17 02:21:55.000000 psyneulink-0.9.1.1/requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)     2629 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/setup.cfg
+-rw-------   0 katherine  (1000) katherine  (1000)     2779 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/setup.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/api/
+-rw-------   0 katherine  (1000) katherine  (1000)     5196 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/api/test_api.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/components/
+-rw-------   0 katherine  (1000) katherine  (1000)     3823 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/components/test_component.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2595 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/components/test_general.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/composition/
+-rw-------   0 katherine  (1000) katherine  (1000)   145271 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_autodiffcomposition.py
+-rw-------   0 katherine  (1000) katherine  (1000)   297744 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_composition.py
+-rw-------   0 katherine  (1000) katherine  (1000)   128455 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_control.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3074 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_gating.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1248 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_graph.py
+-rw-------   0 katherine  (1000) katherine  (1000)    38900 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_interfaces.py
+-rw-------   0 katherine  (1000) katherine  (1000)   295082 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_learning.py
+-rw-------   0 katherine  (1000) katherine  (1000)    35169 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_models.py
+-rw-------   0 katherine  (1000) katherine  (1000)   809874 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_report.py
+-rw-------   0 katherine  (1000) katherine  (1000)    40559 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_runtime_params.py
+-rw-------   0 katherine  (1000) katherine  (1000)   488058 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/composition/test_show_graph.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/control/
+-rw-------   0 katherine  (1000) katherine  (1000)    14792 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/control/test_gilzenrat.py
+-rw-------   0 katherine  (1000) katherine  (1000)     6762 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/control/test_param_estimation.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/documentation/
+-rw-------   0 katherine  (1000) katherine  (1000)     3737 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/documentation/test_module_docs.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/functions/
+-rw-------   0 katherine  (1000) katherine  (1000)     6730 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_accumulator_integrator.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8466 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_buffer.py
+-rw-------   0 katherine  (1000) katherine  (1000)    14104 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_combination.py
+-rw-------   0 katherine  (1000) katherine  (1000)      523 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_default_allocation.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3175 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_distance.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2822 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_distribution.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3252 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_fhn_integrator.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4073 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_functions.py
+-rw-------   0 katherine  (1000) katherine  (1000)      576 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_identity.py
+-rw-------   0 katherine  (1000) katherine  (1000)    12310 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_integrator.py
+-rw-------   0 katherine  (1000) katherine  (1000)    65528 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_memory.py
+-rw-------   0 katherine  (1000) katherine  (1000)      226 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_objective.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4171 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_optimization.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2318 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_selection.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1581 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_stability.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8301 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_transfer.py
+-rw-------   0 katherine  (1000) katherine  (1000)    24972 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/functions/test_user_defined_func.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/json/
+-rw-------   0 katherine  (1000) katherine  (1000)      225 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/json/model_backprop.py
+-rw-------   0 katherine  (1000) katherine  (1000)      518 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/json/model_basic.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1125 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/json/model_nested_comp_with_scheduler.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2229 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/json/model_with_control.py
+-rw-------   0 katherine  (1000) katherine  (1000)      876 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/json/model_with_two_conjoint_comps.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1018 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/json/model_with_two_disjoint_comps.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2884 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/json/stroop_conflict_monitoring.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4130 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/json/test_json.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/llvm/
+-rw-------   0 katherine  (1000) katherine  (1000)     1921 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_builtins_intrinsics.py
+-rw-------   0 katherine  (1000) katherine  (1000)     7986 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_builtins_matrix.py
+-rw-------   0 katherine  (1000) katherine  (1000)     5100 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_builtins_random.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2561 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_builtins_vector.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1470 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_compile.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3791 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_custom_func.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2361 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_debug_composition.py
+-rw-------   0 katherine  (1000) katherine  (1000)    18380 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_helpers.py
+-rw-------   0 katherine  (1000) katherine  (1000)     5306 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_llvm_lite.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9753 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/llvm/test_multiple_executions.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/log/
+-rw-------   0 katherine  (1000) katherine  (1000)    64315 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/log/test_log.py
+-rw-------   0 katherine  (1000) katherine  (1000)    33890 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/log/test_rpc.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/mechanisms/
+-rw-------   0 katherine  (1000) katherine  (1000)     6513 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_contrastive_hebbian_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    15017 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_control_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    24957 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_ddm_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3347 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_drift_diffusion_analytical.py
+-rw-------   0 katherine  (1000) katherine  (1000)    12209 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_episodic_memory.py
+-rw-------   0 katherine  (1000) katherine  (1000)     6218 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_gating_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    15331 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_input_output_labels.py
+-rw-------   0 katherine  (1000) katherine  (1000)    39125 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_input_state_spec.py
+-rw-------   0 katherine  (1000) katherine  (1000)    53567 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_integrator_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    19873 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_kwta.py
+-rw-------   0 katherine  (1000) katherine  (1000)    16336 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_lca.py
+-rw-------   0 katherine  (1000) katherine  (1000)    13916 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_leabra_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8245 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_mechanisms.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2468 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_modulatory_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)      755 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_objective_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    16270 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_processing_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    59905 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_recurrent_transfer_mechanism.py
+-rw-------   0 katherine  (1000) katherine  (1000)    76702 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/mechanisms/test_transfer_mechanism.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/misc/
+-rw-------   0 katherine  (1000) katherine  (1000)     1763 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/misc/test_notebooks.py
+-rw-------   0 katherine  (1000) katherine  (1000)    13637 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/misc/test_parameters.py
+-rw-------   0 katherine  (1000) katherine  (1000)      380 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/misc/test_user_seed.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1933 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/misc/test_utilities.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/models/
+-rw-------   0 katherine  (1000) katherine  (1000)     8909 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/models/test_bi_percepts.py
+-rw-------   0 katherine  (1000) katherine  (1000)    16914 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/models/test_botvinick.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3564 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/models/test_documentation_models.py
+-rw-------   0 katherine  (1000) katherine  (1000)    10660 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/models/test_greedy_agent.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/naming/
+-rw-------   0 katherine  (1000) katherine  (1000)    11267 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/naming/test_naming.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/ports/
+-rw-------   0 katherine  (1000) katherine  (1000)     5201 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/ports/test_input_ports.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3042 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/ports/test_modulatory_signals.py
+-rw-------   0 katherine  (1000) katherine  (1000)     3181 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/ports/test_output_ports.py
+-rw-------   0 katherine  (1000) katherine  (1000)     7987 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/ports/test_parameter_ports.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/projections/
+-rw-------   0 katherine  (1000) katherine  (1000)      706 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/projections/test_projection.py
+-rw-------   0 katherine  (1000) katherine  (1000)    24046 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/projections/test_projection_specifications.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tests/scheduling/
+-rw-------   0 katherine  (1000) katherine  (1000)     1033 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/scheduling/conftest.py
+-rw-------   0 katherine  (1000) katherine  (1000)    42122 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/scheduling/test_condition.py
+-rw-------   0 katherine  (1000) katherine  (1000)    69059 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/scheduling/test_scheduler.py
+-rw-------   0 katherine  (1000) katherine  (1000)    22296 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/scheduling/test_system_newsched.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2238 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tests/scheduling/test_time.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2021-09-17 02:21:56.000000 psyneulink-0.9.1.1/tutorial/
+-rw-------   0 katherine  (1000) katherine  (1000)   150549 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/tutorial/PsyNeuLink Tutorial.ipynb
+-rw-------   0 katherine  (1000) katherine  (1000)       48 2021-09-17 02:21:55.000000 psyneulink-0.9.1.1/tutorial_requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)    68611 2021-08-24 20:29:11.000000 psyneulink-0.9.1.1/versioneer.py
```

### Comparing `psyneulink-0.9.1.0/CONVENTIONS.md` & `psyneulink-0.9.1.1/CONVENTIONS.md`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/LICENSE.txt` & `psyneulink-0.9.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/PKG-INFO` & `psyneulink-0.9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyneulink
-Version: 0.9.1.0
+Version: 0.9.1.1
 Summary: A block modeling system for cognitive neuroscience
 Home-page: https://github.com/PrincetonUniversity/PsyNeuLink
 Author: Jonathan Cohen, Princeton University, Intel
 Author-email: jdc@princeton.edu
 License: Apache
 Description: .. image:: https://badge.fury.io/py/psyneulink.svg
             :target: https://badge.fury.io/py/psyneulink
@@ -260,11 +260,11 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
-Provides-Extra: doc
+Provides-Extra: cuda
 Provides-Extra: dev
 Provides-Extra: tutorial
-Provides-Extra: cuda
+Provides-Extra: doc
```

### Comparing `psyneulink-0.9.1.0/README.rst` & `psyneulink-0.9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Hebbian_Simon.py` & `psyneulink-0.9.1.1/Scripts/Debug/Hebbian_Simon.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Jason_Reward_rate_with_penalty_with_inputs.py` & `psyneulink-0.9.1.1/Scripts/Debug/Jason_Reward_rate_with_penalty_with_inputs.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Jason_Stroop_Stimuli.py` & `psyneulink-0.9.1.1/Scripts/Debug/Jason_Stroop_Stimuli.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Markus Stroop.py` & `psyneulink-0.9.1.1/Scripts/Debug/Markus Stroop.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Predator-Prey Sebastian REDUCED.py` & `psyneulink-0.9.1.1/Scripts/Debug/Predator-Prey Sebastian REDUCED.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Predator-Prey Sebastian.py` & `psyneulink-0.9.1.1/Scripts/Debug/Predator-Prey Sebastian.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/StabilityFlexibility.py` & `psyneulink-0.9.1.1/Scripts/Debug/StabilityFlexibility.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Umemoto_Feb.py` & `psyneulink-0.9.1.1/Scripts/Debug/Umemoto_Feb.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Umemoto_Feb2.py` & `psyneulink-0.9.1.1/Scripts/Debug/Umemoto_Feb2.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Yotam LCA Model LLVM.py` & `psyneulink-0.9.1.1/Scripts/Debug/Yotam LCA Model LLVM.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/Yotam LCA Model.py` & `psyneulink-0.9.1.1/Scripts/Debug/Yotam LCA Model.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/bryant_lca_with_termination.py` & `psyneulink-0.9.1.1/Scripts/Debug/bryant_lca_with_termination.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/build_input.py` & `psyneulink-0.9.1.1/Scripts/Debug/build_input.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/dndtesting.py` & `psyneulink-0.9.1.1/Scripts/Debug/dndtesting.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/generator_function_as_input.py` & `psyneulink-0.9.1.1/Scripts/Debug/generator_function_as_input.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/laura_test_no_noise_stroop_09_11_2018.py` & `psyneulink-0.9.1.1/Scripts/Debug/laura_test_no_noise_stroop_09_11_2018.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/markus_test_umemoto.py` & `psyneulink-0.9.1.1/Scripts/Debug/markus_test_umemoto.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/new_umemoto.py` & `psyneulink-0.9.1.1/Scripts/Debug/new_umemoto.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/stability_flexibility_simple.py` & `psyneulink-0.9.1.1/Scripts/Debug/stability_flexibility_simple.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/testing_dnd.py` & `psyneulink-0.9.1.1/Scripts/Debug/testing_dnd.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Debug/testing_dnd_Q.py` & `psyneulink-0.9.1.1/Scripts/Debug/testing_dnd_Q.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Basics And Primer/Stroop Model - Basic.py` & `psyneulink-0.9.1.1/Scripts/Examples/Basics And Primer/Stroop Model - Basic.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Basics And Primer/Stroop Model - Conflict Monitoring.py` & `psyneulink-0.9.1.1/Scripts/Examples/Basics And Primer/Stroop Model - Conflict Monitoring.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Botvinick Model Composition.py` & `psyneulink-0.9.1.1/Scripts/Examples/Botvinick Model Composition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/EVC OCM.py` & `psyneulink-0.9.1.1/Scripts/Examples/EVC OCM.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/EVC-Gratton Composition.py` & `psyneulink-0.9.1.1/Scripts/Examples/EVC-Gratton Composition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/EVC-Gratton-GaussianProcess.py` & `psyneulink-0.9.1.1/Scripts/Examples/EVC-Gratton-GaussianProcess.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Gating-Mechanism. with UDF.py` & `psyneulink-0.9.1.1/Scripts/Examples/Gating-Mechanism. with UDF.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Gilbert_Shallice_Composition_Model.py` & `psyneulink-0.9.1.1/Scripts/Examples/Gilbert_Shallice_Composition_Model.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/LC Control Mechanism Composition.py` & `psyneulink-0.9.1.1/Scripts/Examples/LC Control Mechanism Composition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/LVOC Composition.py` & `psyneulink-0.9.1.1/Scripts/Examples/LVOC Composition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Lena Rumelhart script.py` & `psyneulink-0.9.1.1/Scripts/Examples/Lena Rumelhart script.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Mixed-NN-and-DDM.py` & `psyneulink-0.9.1.1/Scripts/Examples/Mixed-NN-and-DDM.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Multilayer-Learning.py` & `psyneulink-0.9.1.1/Scripts/Examples/Multilayer-Learning.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/RL-DDM.py` & `psyneulink-0.9.1.1/Scripts/Examples/RL-DDM.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Rumelhart Semantic Network.py` & `psyneulink-0.9.1.1/Scripts/Examples/Rumelhart Semantic Network.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/StabilityFlexibility.py` & `psyneulink-0.9.1.1/Scripts/Examples/StabilityFlexibility.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Stroop Model.py` & `psyneulink-0.9.1.1/Scripts/Examples/Stroop Model.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Tutorial/Rumelhart Semantic Network (autodiff).py` & `psyneulink-0.9.1.1/Scripts/Examples/Tutorial/Rumelhart Semantic Network (autodiff).py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/Tutorial/Stroop Model - EVC.py` & `psyneulink-0.9.1.1/Scripts/Examples/Tutorial/Stroop Model - EVC.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/_Gating-Mechanism.py` & `psyneulink-0.9.1.1/Scripts/Examples/_Gating-Mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/_Leabra-Demo.py` & `psyneulink-0.9.1.1/Scripts/Examples/_Leabra-Demo.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/_Leabra-Learning-Demo.py` & `psyneulink-0.9.1.1/Scripts/Examples/_Leabra-Learning-Demo.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/_Reinforcement-Learning REV.py` & `psyneulink-0.9.1.1/Scripts/Examples/_Reinforcement-Learning REV.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/_Stroop-Simple.py` & `psyneulink-0.9.1.1/Scripts/Examples/_Stroop-Simple.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Examples/_nested_learning.py` & `psyneulink-0.9.1.1/Scripts/Examples/_nested_learning.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Adaptive Replay Model.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Adaptive Replay Model.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Bustamante_Stroop_XOR_LVOC_Model.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Bustamante_Stroop_XOR_LVOC_Model.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Bustamante_Stroop_XOR_LVOC_Model_VZ.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Bustamante_Stroop_XOR_LVOC_Model_VZ.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/ColorMotionTask_FULL.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/ColorMotionTask_FULL.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/ColorMotionTask_SIMPLE.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/ColorMotionTask_SIMPLE.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/GreedyAgentInteractiveInputs.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/GreedyAgentInteractiveInputs.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/GreedyAgentModel.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/GreedyAgentModel.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/GreedyAgentModel_LLVM_TEST.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/GreedyAgentModel_LLVM_TEST.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/GymForagerRandomAgent.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/GymForagerRandomAgent.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/N-back.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/N-back.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/NeuroML Example.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/NeuroML Example.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/PanickyAgentModel.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/PanickyAgentModel.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model DEMO.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model DEMO.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model DQN LVOC.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model DQN LVOC.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model DQN [ORIG].py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model DQN [ORIG].py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model DQN.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model DQN.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model INPUT LAYER.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model INPUT LAYER.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model I_0 Nested Comp.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model I_0 Nested Comp.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/Predator-Prey Model.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/Predator-Prey Model.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/bi-percepts.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/bi-percepts.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/build_input.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/build_input.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/build_stimuli_VZ.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/build_stimuli_VZ.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/Scripts/Models (Under Development)/build_stimuli_set.py` & `psyneulink-0.9.1.1/Scripts/Models (Under Development)/build_stimuli_set.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/Makefile` & `psyneulink-0.9.1.1/docs/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -47,154 +47,154 @@
 	@echo "  dummy      to check syntax errors of document sources"
 
 .PHONY: clean
 clean:
 	rm -rf $(BUILDDIR)/*
 
 .PHONY: html
-html:
+html: generated
 	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
 
 .PHONY: dirhtml
-dirhtml:
+dirhtml: generated
 	$(SPHINXBUILD) -b dirhtml $(ALLSPHINXOPTS) $(BUILDDIR)/dirhtml
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/dirhtml."
 
 .PHONY: singlehtml
-singlehtml:
+singlehtml: generated
 	$(SPHINXBUILD) -b singlehtml $(ALLSPHINXOPTS) $(BUILDDIR)/singlehtml
 	@echo
 	@echo "Build finished. The HTML page is in $(BUILDDIR)/singlehtml."
 
 .PHONY: pickle
-pickle:
+pickle: generated
 	$(SPHINXBUILD) -b pickle $(ALLSPHINXOPTS) $(BUILDDIR)/pickle
 	@echo
 	@echo "Build finished; now you can process the pickle files."
 
 .PHONY: json
-json:
+json: generated
 	$(SPHINXBUILD) -b json $(ALLSPHINXOPTS) $(BUILDDIR)/json
 	@echo
 	@echo "Build finished; now you can process the JSON files."
 
 .PHONY: htmlhelp
-htmlhelp:
+htmlhelp: generated
 	$(SPHINXBUILD) -b htmlhelp $(ALLSPHINXOPTS) $(BUILDDIR)/htmlhelp
 	@echo
 	@echo "Build finished; now you can run HTML Help Workshop with the" \
 	      ".hhp project file in $(BUILDDIR)/htmlhelp."
 
 .PHONY: qthelp
-qthelp:
+qthelp: generated
 	$(SPHINXBUILD) -b qthelp $(ALLSPHINXOPTS) $(BUILDDIR)/qthelp
 	@echo
 	@echo "Build finished; now you can run "qcollectiongenerator" with the" \
 	      ".qhcp project file in $(BUILDDIR)/qthelp, like this:"
 	@echo "# qcollectiongenerator $(BUILDDIR)/qthelp/PsyNeuLink.qhcp"
 	@echo "To view the help file:"
 	@echo "# assistant -collectionFile $(BUILDDIR)/qthelp/PsyNeuLink.qhc"
 
 .PHONY: applehelp
-applehelp:
+applehelp: generated
 	$(SPHINXBUILD) -b applehelp $(ALLSPHINXOPTS) $(BUILDDIR)/applehelp
 	@echo
 	@echo "Build finished. The help book is in $(BUILDDIR)/applehelp."
 	@echo "N.B. You won't be able to view it unless you put it in" \
 	      "~/Library/Documentation/Help or install it in your application" \
 	      "bundle."
 
 .PHONY: devhelp
-devhelp:
+devhelp: generated
 	$(SPHINXBUILD) -b devhelp $(ALLSPHINXOPTS) $(BUILDDIR)/devhelp
 	@echo
 	@echo "Build finished."
 	@echo "To view the help file:"
 	@echo "# mkdir -p $$HOME/.local/share/devhelp/PsyNeuLink"
 	@echo "# ln -s $(BUILDDIR)/devhelp $$HOME/.local/share/devhelp/PsyNeuLink"
 	@echo "# devhelp"
 
 .PHONY: epub
-epub:
+epub: generated
 	$(SPHINXBUILD) -b epub $(ALLSPHINXOPTS) $(BUILDDIR)/epub
 	@echo
 	@echo "Build finished. The epub file is in $(BUILDDIR)/epub."
 
 .PHONY: epub3
-epub3:
+epub3: generated
 	$(SPHINXBUILD) -b epub3 $(ALLSPHINXOPTS) $(BUILDDIR)/epub3
 	@echo
 	@echo "Build finished. The epub3 file is in $(BUILDDIR)/epub3."
 
 .PHONY: latex
-latex:
+latex: generated
 	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) $(BUILDDIR)/latex
 	@echo
 	@echo "Build finished; the LaTeX files are in $(BUILDDIR)/latex."
 	@echo "Run \`make' in that directory to run these through (pdf)latex" \
 	      "(use \`make latexpdf' here to do that automatically)."
 
 .PHONY: latexpdf
-latexpdf:
+latexpdf: generated
 	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) $(BUILDDIR)/latex
 	@echo "Running LaTeX files through pdflatex..."
 	$(MAKE) -C $(BUILDDIR)/latex all-pdf
 	@echo "pdflatex finished; the PDF files are in $(BUILDDIR)/latex."
 
 .PHONY: latexpdfja
-latexpdfja:
+latexpdfja: generated
 	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) $(BUILDDIR)/latex
 	@echo "Running LaTeX files through platex and dvipdfmx..."
 	$(MAKE) -C $(BUILDDIR)/latex all-pdf-ja
 	@echo "pdflatex finished; the PDF files are in $(BUILDDIR)/latex."
 
 .PHONY: text
-text:
+text: generated
 	$(SPHINXBUILD) -b text $(ALLSPHINXOPTS) $(BUILDDIR)/text
 	@echo
 	@echo "Build finished. The text files are in $(BUILDDIR)/text."
 
 .PHONY: man
-man:
+man: generated
 	$(SPHINXBUILD) -b man $(ALLSPHINXOPTS) $(BUILDDIR)/man
 	@echo
 	@echo "Build finished. The manual pages are in $(BUILDDIR)/man."
 
 .PHONY: texinfo
-texinfo:
+texinfo: generated
 	$(SPHINXBUILD) -b texinfo $(ALLSPHINXOPTS) $(BUILDDIR)/texinfo
 	@echo
 	@echo "Build finished. The Texinfo files are in $(BUILDDIR)/texinfo."
 	@echo "Run \`make' in that directory to run these through makeinfo" \
 	      "(use \`make info' here to do that automatically)."
 
 .PHONY: info
-info:
+info: generated
 	$(SPHINXBUILD) -b texinfo $(ALLSPHINXOPTS) $(BUILDDIR)/texinfo
 	@echo "Running Texinfo files through makeinfo..."
 	make -C $(BUILDDIR)/texinfo info
 	@echo "makeinfo finished; the Info files are in $(BUILDDIR)/texinfo."
 
 .PHONY: gettext
-gettext:
+gettext: generated
 	$(SPHINXBUILD) -b gettext $(I18NSPHINXOPTS) $(BUILDDIR)/locale
 	@echo
 	@echo "Build finished. The message catalogs are in $(BUILDDIR)/locale."
 
 .PHONY: changes
-changes:
+changes: generated
 	$(SPHINXBUILD) -b changes $(ALLSPHINXOPTS) $(BUILDDIR)/changes
 	@echo
 	@echo "The overview file is in $(BUILDDIR)/changes."
 
 .PHONY: linkcheck
-linkcheck:
+linkcheck: generated
 	$(SPHINXBUILD) -b linkcheck $(ALLSPHINXOPTS) $(BUILDDIR)/linkcheck
 	@echo
 	@echo "Link check complete; look for any errors in the above output " \
 	      "or in $(BUILDDIR)/linkcheck/output.txt."
 
 .PHONY: doctest
 doctest:
@@ -205,21 +205,21 @@
 .PHONY: coverage
 coverage:
 	$(SPHINXBUILD) -b coverage $(ALLSPHINXOPTS) $(BUILDDIR)/coverage
 	@echo "Testing of coverage in the sources finished, look at the " \
 	      "results in $(BUILDDIR)/coverage/python.txt."
 
 .PHONY: xml
-xml:
+xml: generated
 	$(SPHINXBUILD) -b xml $(ALLSPHINXOPTS) $(BUILDDIR)/xml
 	@echo
 	@echo "Build finished. The XML files are in $(BUILDDIR)/xml."
 
 .PHONY: pseudoxml
-pseudoxml:
+pseudoxml: generated
 	$(SPHINXBUILD) -b pseudoxml $(ALLSPHINXOPTS) $(BUILDDIR)/pseudoxml
 	@echo
 	@echo "Build finished. The pseudo-XML files are in $(BUILDDIR)/pseudoxml."
 
 .PHONY: dummy
 dummy:
 	$(SPHINXBUILD) -b dummy $(ALLSPHINXOPTS) $(BUILDDIR)/dummy
@@ -235,7 +235,11 @@
 	cd ..
 	rm -rf *
 	mv ~/tmp_gh-pages_dir/* .
 	rm -rf ~/tmp_gh-pages_dir
 	git add -A
 	git ci -m "Generated gh-pages for `git log devel -1 --pretty=short --abbrev-commit`" && git push origin gh-pages ; git checkout devel
 	make clean
+
+.PHONY: generated
+generated:
+	find source/generator_scripts -name "*.py" -exec python {} \;
```

### Comparing `psyneulink-0.9.1.0/docs/source/BasicsAndPrimer.rst` & `psyneulink-0.9.1.1/docs/source/BasicsAndPrimer.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/BotvinickConflictMonitoringModel.rst` & `psyneulink-0.9.1.1/docs/source/BotvinickConflictMonitoringModel.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/BustamanteStroopXORLVOCModel.rst` & `psyneulink-0.9.1.1/docs/source/BustamanteStroopXORLVOCModel.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/Cohen_HustonModel.rst` & `psyneulink-0.9.1.1/docs/source/Cohen_HustonModel.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/Compilation.rst` & `psyneulink-0.9.1.1/docs/source/Compilation.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/Component.rst` & `psyneulink-0.9.1.1/docs/source/Component.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/Composition.rst` & `psyneulink-0.9.1.1/docs/source/Composition.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/ContributorsGuide.rst` & `psyneulink-0.9.1.1/docs/source/ContributorsGuide.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/ConventionsAndDefinitions.rst` & `psyneulink-0.9.1.1/docs/source/ConventionsAndDefinitions.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/GilzenratModel.rst` & `psyneulink-0.9.1.1/docs/source/GilzenratModel.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/MontagueModel.rst` & `psyneulink-0.9.1.1/docs/source/MontagueModel.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/NieuwenhuisModel.rst` & `psyneulink-0.9.1.1/docs/source/NieuwenhuisModel.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/PCTC_model.rst` & `psyneulink-0.9.1.1/docs/source/PCTC_model.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/QuickReference.rst` & `psyneulink-0.9.1.1/docs/source/QuickReference.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/RefactoredLearningGuide.rst` & `psyneulink-0.9.1.1/docs/source/RefactoredLearningGuide.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/Registry.rst` & `psyneulink-0.9.1.1/docs/source/Registry.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/UserGuide_TBD.rst` & `psyneulink-0.9.1.1/docs/source/UserGuide_TBD.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/Visualization.rst` & `psyneulink-0.9.1.1/docs/source/Visualization.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/index.rst` & `psyneulink-0.9.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/docs/source/index_logo_with_text.rst` & `psyneulink-0.9.1.1/docs/source/index_logo_with_text.rst`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/__init__.py` & `psyneulink-0.9.1.1/psyneulink/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/__init__.py` & `psyneulink-0.9.1.1/psyneulink/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/component.py` & `psyneulink-0.9.1.1/psyneulink/core/components/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,36 +419,36 @@
   irrespective of its `is_finished` method;  if it is True then, depending on how its class implements and handles its
   `is_finished` method, the Component may execute more than once per call to its `execute <Component.execute>` method.
 
 .. _Component_Num_Executions_Before_Finished:
 
 * **num_executions_before_finished** -- contains the number of times the Component has executed prior to finishing
   (and since it last finished);  depending upon the class, these may all be within a single call to the Component's
-  `execute <Component.execute>` method, or extend over several calls.  It is set to 0 each time `is_finished` evalutes
+  `execute <Component.execute>` method, or extend over several calls.  It is set to 0 each time `is_finished` evaluates
   to True. Note that this is distinct from the `execution_count <Component_Execution_Count>` and `num_executions
   <Component_Num_Executions>` attributes.
 
 .. _Component_Max_Executions_Before_Finished:
 
 * **max_executions_before_finished** -- determines the maximum number of executions allowed before finishing
-  (i.e., the maxmium allowable value of `num_executions_before_finished <Component.num_executions_before_finished>`).
+  (i.e., the maximum allowable value of `num_executions_before_finished <Component.num_executions_before_finished>`).
   If it is exceeded, a warning message is generated.  Note that this only pertains to `num_executions_before_finished
   <Component_Num_Executions_Before_Finished>`, and not its `execution_count <Component_Execution_Count>`, which can be
   unlimited.
 
 .. _Component_Execution_Count_and_Time:
 
 *Count and Time*
 ~~~~~~~~~~~~~~~~
 
 .. _Component_Execution_Count:
 
 * **execution_count** -- maintains a record of the number of times a Component has executed since it was constructed,
   *excluding*  executions carried out during initialization and validation, but including all others whether they are
-  of the Component on its own are as part of a `Composition`, and irresective of the `context <Context>` in which
+  of the Component on its own are as part of a `Composition`, and irrespective of the `context <Context>` in which
   they are occur. The value can be changed "manually" or programmatically by assigning an integer
   value directly to the attribute.  Note that this is the distinct from the `num_executions <Component_Num_Executions>`
   and `num_executions_before_finished <Component_Num_Executions_Before_Finished>` attributes.
 
 .. _Component_Num_Executions:
 
 * **num_executions** -- maintains a record, in a `Time` object, of the number of times a Component has executed in a
```

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/__init__.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/function.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/function.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/combinationfunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/combinationfunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/distributionfunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/distributionfunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/learningfunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/learningfunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/objectivefunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/optimizationfunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/optimizationfunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/selectionfunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/selectionfunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/nonstateful/transferfunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/nonstateful/transferfunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/stateful/integratorfunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/stateful/integratorfunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/stateful/memoryfunctions.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/stateful/memoryfunctions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/stateful/statefulfunction.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/stateful/statefulfunction.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/functions/userdefinedfunction.py` & `psyneulink-0.9.1.1/psyneulink/core/components/functions/userdefinedfunction.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/mechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/__init__.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/controlmechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/controlmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/defaultcontrolmechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/defaultcontrolmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/gating/gatingmechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/gating/gatingmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/control/optimizationcontrolmechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/control/optimizationcontrolmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/learning/learningmechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/learning/learningmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/modulatory/modulatorymechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/modulatory/modulatorymechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/__init__.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/compositioninterfacemechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/compositioninterfacemechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/defaultprocessingmechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/defaultprocessingmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/integratormechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/integratormechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/objectivemechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/objectivemechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/processingmechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/processingmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/mechanisms/processing/transfermechanism.py` & `psyneulink-0.9.1.1/psyneulink/core/components/mechanisms/processing/transfermechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/ports/inputport.py` & `psyneulink-0.9.1.1/psyneulink/core/components/ports/inputport.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/controlsignal.py` & `psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/controlsignal.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/gatingsignal.py` & `psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/gatingsignal.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/learningsignal.py` & `psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/learningsignal.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/ports/modulatorysignals/modulatorysignal.py` & `psyneulink-0.9.1.1/psyneulink/core/components/ports/modulatorysignals/modulatorysignal.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/ports/outputport.py` & `psyneulink-0.9.1.1/psyneulink/core/components/ports/outputport.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/ports/parameterport.py` & `psyneulink-0.9.1.1/psyneulink/core/components/ports/parameterport.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/ports/port.py` & `psyneulink-0.9.1.1/psyneulink/core/components/ports/port.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/controlprojection.py` & `psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/controlprojection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/gatingprojection.py` & `psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/gatingprojection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/learningprojection.py` & `psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/learningprojection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/projections/modulatory/modulatoryprojection.py` & `psyneulink-0.9.1.1/psyneulink/core/components/projections/modulatory/modulatoryprojection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/projections/pathway/mappingprojection.py` & `psyneulink-0.9.1.1/psyneulink/core/components/projections/pathway/mappingprojection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/projections/pathway/pathwayprojection.py` & `psyneulink-0.9.1.1/psyneulink/core/components/projections/pathway/pathwayprojection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/projections/projection.py` & `psyneulink-0.9.1.1/psyneulink/core/components/projections/projection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/components/shellclasses.py` & `psyneulink-0.9.1.1/psyneulink/core/components/shellclasses.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/compositions/composition.py` & `psyneulink-0.9.1.1/psyneulink/core/compositions/composition.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,15 +771,15 @@
 <Composition_Learning_Components>`.  This is shown in an animation of the XOR network from the `example above
 <Composition_XOR_Example>`:
 
 .. _Composition_Learning_Animation_Figure:
 
     **Composition with Learning**
 
-    .. figure:: _static/Composition_XOR_animation.gif
+    .. figure:: _images/Composition_XOR_animation.gif
        :alt: Animation of Composition with learning
        :scale: 50 %
 
        Animation of XOR Composition in example above when it is executed by calling its `learn <Composition.learn>`
        method with the argument ``animate={'show_learning':True}``.
 
 .. note::
@@ -9910,15 +9910,18 @@
     def _get_parsed_variable(self, *args, **kwargs):
         raise TypeError(f'_get_parsed_variable unsupported for {self.__class__.__name__}')
 
     def _delete_contexts(self, *contexts, check_simulation_storage=False, visited=None):
         super()._delete_contexts(*contexts, check_simulation_storage=check_simulation_storage, visited=visited)
 
         for c in contexts:
-            self.scheduler._delete_counts(c.execution_id)
+            try:
+                self.scheduler._delete_counts(c.execution_id)
+            except AttributeError:
+                self.scheduler._delete_counts(c)
 
     # ******************************************************************************************************************
     #                                           LLVM
     # ******************************************************************************************************************
 
     @property
     def _inner_projections(self):
```

### Comparing `psyneulink-0.9.1.0/psyneulink/core/compositions/compositionfunctionapproximator.py` & `psyneulink-0.9.1.1/psyneulink/core/compositions/compositionfunctionapproximator.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/compositions/pathway.py` & `psyneulink-0.9.1.1/psyneulink/core/compositions/pathway.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/compositions/report.py` & `psyneulink-0.9.1.1/psyneulink/core/compositions/report.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/compositions/showgraph.py` & `psyneulink-0.9.1.1/psyneulink/core/compositions/showgraph.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/__init__.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/context.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/context.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/defaults.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/defaults.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/json.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/json.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/keywords.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/keywords.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/kvo.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/kvo.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/log.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/log.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/parameters.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/parameters.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/preferences/basepreferenceset.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/preferences/basepreferenceset.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/preferences/compositionpreferenceset.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/preferences/compositionpreferenceset.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/preferences/mechanismpreferenceset.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/preferences/mechanismpreferenceset.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/preferences/preferenceset.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/preferences/preferenceset.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/registry.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/registry.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/sampleiterator.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/sampleiterator.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/socket.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/socket.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/globals/utilities.py` & `psyneulink-0.9.1.1/psyneulink/core/globals/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1735,28 +1735,40 @@
         -------
             a string corresponding to **string** that is an attribute
             of psyneulink if it exists, otherwise None
 
             The output of this function will cause
             getattr(psyneulink, <output>) to return a psyneulink object
     """
-    try:
-        eval(f'psyneulink.{string}')
+    def is_pnl_obj(string):
+        try:
+            # remove parens to get rid of class instantiations
+            string = re.sub(r'\(.*?\)', '', string)
+            attr_sequence = string.split('.')
+            obj = getattr(psyneulink, attr_sequence[0])
+
+            for item in attr_sequence[1:]:
+                obj = getattr(obj, item)
+
+            return True
+        except (AttributeError, TypeError):
+            return False
+
+    if is_pnl_obj(string):
         return string
-    except (AttributeError, SyntaxError, TypeError):
-        pass
 
     # handle potential psyneulink keyword
     try:
         # insert space between camel case words
         keyword = re.sub('([a-z])([A-Z])', r'\1 \2', string)
         keyword = keyword.upper().replace(' ', '_')
-        eval(f'psyneulink.{keyword}')
-        return keyword
-    except (AttributeError, SyntaxError, TypeError):
+
+        if is_pnl_obj(keyword):
+            return keyword
+    except TypeError:
         pass
 
     return None
 
 
 def get_all_explicit_arguments(cls_, func_str):
     """
```

### Comparing `psyneulink-0.9.1.0/psyneulink/core/llvm/__init__.py` & `psyneulink-0.9.1.1/psyneulink/core/llvm/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/llvm/builder_context.py` & `psyneulink-0.9.1.1/psyneulink/core/llvm/builder_context.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/llvm/builtins.py` & `psyneulink-0.9.1.1/psyneulink/core/llvm/builtins.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/llvm/codegen.py` & `psyneulink-0.9.1.1/psyneulink/core/llvm/codegen.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/llvm/debug.py` & `psyneulink-0.9.1.1/psyneulink/core/llvm/debug.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/llvm/execution.py` & `psyneulink-0.9.1.1/psyneulink/core/llvm/execution.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/llvm/helpers.py` & `psyneulink-0.9.1.1/psyneulink/core/llvm/helpers.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/llvm/jit_engine.py` & `psyneulink-0.9.1.1/psyneulink/core/llvm/jit_engine.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/rpc/graph_pb2.py` & `psyneulink-0.9.1.1/psyneulink/core/rpc/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/rpc/graph_pb2_grpc.py` & `psyneulink-0.9.1.1/psyneulink/core/rpc/graph_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/scheduling/__init__.py` & `psyneulink-0.9.1.1/psyneulink/core/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/scheduling/condition.py` & `psyneulink-0.9.1.1/psyneulink/core/scheduling/condition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/scheduling/scheduler.py` & `psyneulink-0.9.1.1/psyneulink/core/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/core/scheduling/time.py` & `psyneulink-0.9.1.1/psyneulink/core/scheduling/time.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/control/agt/agtcontrolmechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/control/agt/agtcontrolmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/control/agt/lccontrolmechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/control/agt/lccontrolmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/learning/autoassociativelearningmechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/learning/autoassociativelearningmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/modulatory/learning/kohonenlearningmechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/modulatory/learning/kohonenlearningmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/integrator/ddm.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/integrator/ddm.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/integrator/episodicmemorymechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/integrator/episodicmemorymechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/leabramechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/leabramechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/objective/comparatormechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/objective/comparatormechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/objective/predictionerrormechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/objective/predictionerrormechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/__init__.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/contrastivehebbianmechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/contrastivehebbianmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/kohonenmechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/kohonenmechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/kwtamechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/kwtamechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/lcamechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/lcamechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/mechanisms/processing/transfer/recurrenttransfermechanism.py` & `psyneulink-0.9.1.1/psyneulink/library/components/mechanisms/processing/transfer/recurrenttransfermechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/projections/pathway/autoassociativeprojection.py` & `psyneulink-0.9.1.1/psyneulink/library/components/projections/pathway/autoassociativeprojection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/components/projections/pathway/maskedmappingprojection.py` & `psyneulink-0.9.1.1/psyneulink/library/components/projections/pathway/maskedmappingprojection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/autodiffcomposition.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/autodiffcomposition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/compiledloss.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/compiledloss.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/compiledoptimizer.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/compiledoptimizer.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/compositionrunner.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/compositionrunner.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/gymforagercfa.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/gymforagercfa.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/pytorchcomponents.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/pytorchcomponents.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/pytorchllvmhelper.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/pytorchllvmhelper.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/pytorchmodelcreator.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/pytorchmodelcreator.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/compositions/regressioncfa.py` & `psyneulink-0.9.1.1/psyneulink/library/compositions/regressioncfa.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/models/Cohen_Huston1994.py` & `psyneulink-0.9.1.1/psyneulink/library/models/Cohen_Huston1994.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/models/Cohen_Huston1994_horse_race.py` & `psyneulink-0.9.1.1/psyneulink/library/models/Cohen_Huston1994_horse_race.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/models/GilzenratModel.py` & `psyneulink-0.9.1.1/psyneulink/library/models/GilzenratModel.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/models/Kalanthroff_PCTC_2018.py` & `psyneulink-0.9.1.1/psyneulink/library/models/Kalanthroff_PCTC_2018.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/models/MontagueDayanSejnowski96.py` & `psyneulink-0.9.1.1/psyneulink/library/models/MontagueDayanSejnowski96.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink/library/models/Nieuwenhuis2005Model.py` & `psyneulink-0.9.1.1/psyneulink/library/models/Nieuwenhuis2005Model.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/psyneulink.egg-info/PKG-INFO` & `psyneulink-0.9.1.1/psyneulink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyneulink
-Version: 0.9.1.0
+Version: 0.9.1.1
 Summary: A block modeling system for cognitive neuroscience
 Home-page: https://github.com/PrincetonUniversity/PsyNeuLink
 Author: Jonathan Cohen, Princeton University, Intel
 Author-email: jdc@princeton.edu
 License: Apache
 Description: .. image:: https://badge.fury.io/py/psyneulink.svg
             :target: https://badge.fury.io/py/psyneulink
@@ -260,11 +260,11 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
-Provides-Extra: doc
+Provides-Extra: cuda
 Provides-Extra: dev
 Provides-Extra: tutorial
-Provides-Extra: cuda
+Provides-Extra: doc
```

### Comparing `psyneulink-0.9.1.0/psyneulink.egg-info/SOURCES.txt` & `psyneulink-0.9.1.1/psyneulink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/setup.cfg` & `psyneulink-0.9.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/setup.py` & `psyneulink-0.9.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/api/test_api.py` & `psyneulink-0.9.1.1/tests/api/test_api.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/components/test_component.py` & `psyneulink-0.9.1.1/tests/components/test_component.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/components/test_general.py` & `psyneulink-0.9.1.1/tests/components/test_general.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_autodiffcomposition.py` & `psyneulink-0.9.1.1/tests/composition/test_autodiffcomposition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_composition.py` & `psyneulink-0.9.1.1/tests/composition/test_composition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_control.py` & `psyneulink-0.9.1.1/tests/composition/test_control.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_gating.py` & `psyneulink-0.9.1.1/tests/composition/test_gating.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_graph.py` & `psyneulink-0.9.1.1/tests/composition/test_graph.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_interfaces.py` & `psyneulink-0.9.1.1/tests/composition/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_learning.py` & `psyneulink-0.9.1.1/tests/composition/test_learning.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_models.py` & `psyneulink-0.9.1.1/tests/composition/test_models.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_report.py` & `psyneulink-0.9.1.1/tests/composition/test_report.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_runtime_params.py` & `psyneulink-0.9.1.1/tests/composition/test_runtime_params.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/composition/test_show_graph.py` & `psyneulink-0.9.1.1/tests/composition/test_show_graph.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/control/test_gilzenrat.py` & `psyneulink-0.9.1.1/tests/control/test_gilzenrat.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/control/test_param_estimation.py` & `psyneulink-0.9.1.1/tests/control/test_param_estimation.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/documentation/test_module_docs.py` & `psyneulink-0.9.1.1/tests/documentation/test_module_docs.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_accumulator_integrator.py` & `psyneulink-0.9.1.1/tests/functions/test_accumulator_integrator.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_buffer.py` & `psyneulink-0.9.1.1/tests/functions/test_buffer.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_combination.py` & `psyneulink-0.9.1.1/tests/functions/test_combination.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_default_allocation.py` & `psyneulink-0.9.1.1/tests/functions/test_default_allocation.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_distance.py` & `psyneulink-0.9.1.1/tests/functions/test_distance.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_distribution.py` & `psyneulink-0.9.1.1/tests/functions/test_distribution.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_fhn_integrator.py` & `psyneulink-0.9.1.1/tests/functions/test_fhn_integrator.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_functions.py` & `psyneulink-0.9.1.1/tests/functions/test_functions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_identity.py` & `psyneulink-0.9.1.1/tests/functions/test_identity.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_integrator.py` & `psyneulink-0.9.1.1/tests/functions/test_integrator.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_memory.py` & `psyneulink-0.9.1.1/tests/functions/test_memory.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_optimization.py` & `psyneulink-0.9.1.1/tests/functions/test_optimization.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_selection.py` & `psyneulink-0.9.1.1/tests/functions/test_selection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_stability.py` & `psyneulink-0.9.1.1/tests/functions/test_stability.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_transfer.py` & `psyneulink-0.9.1.1/tests/functions/test_transfer.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/functions/test_user_defined_func.py` & `psyneulink-0.9.1.1/tests/functions/test_user_defined_func.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/json/model_basic.py` & `psyneulink-0.9.1.1/tests/json/model_basic.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/json/model_nested_comp_with_scheduler.py` & `psyneulink-0.9.1.1/tests/json/model_nested_comp_with_scheduler.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/json/model_with_control.py` & `psyneulink-0.9.1.1/tests/json/model_with_control.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/json/model_with_two_conjoint_comps.py` & `psyneulink-0.9.1.1/tests/json/model_with_two_conjoint_comps.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/json/model_with_two_disjoint_comps.py` & `psyneulink-0.9.1.1/tests/json/model_with_two_disjoint_comps.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/json/stroop_conflict_monitoring.py` & `psyneulink-0.9.1.1/tests/json/stroop_conflict_monitoring.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/json/test_json.py` & `psyneulink-0.9.1.1/tests/json/test_json.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_builtins_intrinsics.py` & `psyneulink-0.9.1.1/tests/llvm/test_builtins_intrinsics.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_builtins_matrix.py` & `psyneulink-0.9.1.1/tests/llvm/test_builtins_matrix.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_builtins_random.py` & `psyneulink-0.9.1.1/tests/llvm/test_builtins_random.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_builtins_vector.py` & `psyneulink-0.9.1.1/tests/llvm/test_builtins_vector.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_compile.py` & `psyneulink-0.9.1.1/tests/llvm/test_compile.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_custom_func.py` & `psyneulink-0.9.1.1/tests/llvm/test_custom_func.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_debug_composition.py` & `psyneulink-0.9.1.1/tests/llvm/test_debug_composition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_helpers.py` & `psyneulink-0.9.1.1/tests/llvm/test_helpers.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_llvm_lite.py` & `psyneulink-0.9.1.1/tests/llvm/test_llvm_lite.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/llvm/test_multiple_executions.py` & `psyneulink-0.9.1.1/tests/llvm/test_multiple_executions.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/log/test_log.py` & `psyneulink-0.9.1.1/tests/log/test_log.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/log/test_rpc.py` & `psyneulink-0.9.1.1/tests/log/test_rpc.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_contrastive_hebbian_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_contrastive_hebbian_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_control_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_control_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_ddm_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_ddm_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_drift_diffusion_analytical.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_drift_diffusion_analytical.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_episodic_memory.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_episodic_memory.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_gating_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_gating_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_input_output_labels.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_input_output_labels.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_input_state_spec.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_input_state_spec.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_integrator_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_integrator_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_kwta.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_kwta.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_lca.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_lca.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_leabra_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_leabra_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_mechanisms.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_mechanisms.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_modulatory_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_modulatory_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_objective_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_objective_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_processing_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_processing_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_recurrent_transfer_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_recurrent_transfer_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/mechanisms/test_transfer_mechanism.py` & `psyneulink-0.9.1.1/tests/mechanisms/test_transfer_mechanism.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/misc/test_notebooks.py` & `psyneulink-0.9.1.1/tests/misc/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/misc/test_parameters.py` & `psyneulink-0.9.1.1/tests/misc/test_parameters.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/misc/test_utilities.py` & `psyneulink-0.9.1.1/tests/misc/test_utilities.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/models/test_bi_percepts.py` & `psyneulink-0.9.1.1/tests/models/test_bi_percepts.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/models/test_botvinick.py` & `psyneulink-0.9.1.1/tests/models/test_botvinick.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/models/test_documentation_models.py` & `psyneulink-0.9.1.1/tests/models/test_documentation_models.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/models/test_greedy_agent.py` & `psyneulink-0.9.1.1/tests/models/test_greedy_agent.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/naming/test_naming.py` & `psyneulink-0.9.1.1/tests/naming/test_naming.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/ports/test_input_ports.py` & `psyneulink-0.9.1.1/tests/ports/test_input_ports.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/ports/test_modulatory_signals.py` & `psyneulink-0.9.1.1/tests/ports/test_modulatory_signals.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/ports/test_output_ports.py` & `psyneulink-0.9.1.1/tests/ports/test_output_ports.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/ports/test_parameter_ports.py` & `psyneulink-0.9.1.1/tests/ports/test_parameter_ports.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/projections/test_projection.py` & `psyneulink-0.9.1.1/tests/projections/test_projection.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/projections/test_projection_specifications.py` & `psyneulink-0.9.1.1/tests/projections/test_projection_specifications.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/scheduling/conftest.py` & `psyneulink-0.9.1.1/tests/scheduling/conftest.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/scheduling/test_condition.py` & `psyneulink-0.9.1.1/tests/scheduling/test_condition.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/scheduling/test_scheduler.py` & `psyneulink-0.9.1.1/tests/scheduling/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/scheduling/test_system_newsched.py` & `psyneulink-0.9.1.1/tests/scheduling/test_system_newsched.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tests/scheduling/test_time.py` & `psyneulink-0.9.1.1/tests/scheduling/test_time.py`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/tutorial/PsyNeuLink Tutorial.ipynb` & `psyneulink-0.9.1.1/tutorial/PsyNeuLink Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `psyneulink-0.9.1.0/versioneer.py` & `psyneulink-0.9.1.1/versioneer.py`

 * *Files identical despite different names*

