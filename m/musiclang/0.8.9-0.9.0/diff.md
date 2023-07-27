# Comparing `tmp/musiclang-0.8.9.tar.gz` & `tmp/musiclang-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musiclang-0.8.9.tar", last modified: Wed May  3 09:47:14 2023, max compression
+gzip compressed data, was "musiclang-0.9.0.tar", last modified: Thu Jul 27 15:26:06 2023, max compression
```

## Comparing `musiclang-0.8.9.tar` & `musiclang-0.9.0.tar`

### file list

```diff
@@ -1,215 +1,221 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1302 2023-05-03 09:47:11.000000 musiclang-0.8.9/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2023-05-03 09:47:14.968462 musiclang-0.8.9/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3653 2023-05-03 09:47:11.000000 musiclang-0.8.9/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.952462 musiclang-0.8.9/musiclang/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      694 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.952462 musiclang-0.8.9/musiclang/analyze/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      820 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/analyze/augmented_net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5042 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    69481 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/chord_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4367 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/feature_representation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8996 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/inference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18747 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/input_representations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/keydistance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6149 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/output_representations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6283 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/score_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2667 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2887 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/midi_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12879 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16589 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/pattern_analyzer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/pattern_sampler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10479 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/roman_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10759 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/score_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11992 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/score_formatter_elements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8592 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/to_musiclang.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8870 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/voice_separation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/library.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/arranger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8579 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/arranger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/arranger_trainer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/melody_arranger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6092 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/melody_arranger_trainer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/composer/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/composer/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8888 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/composer/auto_composer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/composer/composer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/composer/harmony.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/predictors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/predictors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3202 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/predictors/hugging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7398 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/predictors/windowed.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/tokenizers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/tokenizers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/tokenizers/chord_tokenizer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/transform/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1559 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7925 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/base_transformer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/transform/chord/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/chord/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/chord/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/composing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/arrange.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11465 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6105 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/layer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6234 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/patternator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13358 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18039 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/voice_leading.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/dynamics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/dynamics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1335 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/dynamics/dynamizer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/features/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/features/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/features/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/generators/rythm_generator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4258 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/library.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19220 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/mask.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/melody/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/melody/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4570 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/melody/basics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/melody/continuation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/melody/filler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/merger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/note/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/note/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/note/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/orchestrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/orchestrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/orchestrations/epic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/orchestrations/nocturne.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/score/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/score/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/score/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/score_merger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/score_merger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/score_merger/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/structure_graphs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/structure_graphs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/structure_graphs/forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/transformer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/utils_random.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/write/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/arrange_utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/arrange_utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4580 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/arrange_utils/arrange_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/arrange_utils/skyline_algorithm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43763 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13534 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4651 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/element.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/elements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/bar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/beat.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/element.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/free_text.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/rhythm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/time_signature.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/tonality.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/voice_leading.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/voicing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13661 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/library.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14138 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/melody.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27070 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/note_pitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8474 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/ornementation.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/out/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12085 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/midi_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3540 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/to_code.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8425 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/to_midi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12321 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/to_mxl.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5393 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/pitches/pitches_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/properties/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/properties/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6890 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/properties/note_properties.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/rhythm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/rhythm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14944 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/rhythm/metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/rhythm/score_rythm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/rhythm/utils_metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37548 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/score.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/sequence/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/sequence/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4656 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/sequence/sequence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12288 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/sequence/sequence_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/time_utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/time_utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5584 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/time_utils/time_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9483 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/tonality.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.952462 musiclang-0.8.9/musiclang.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6212 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      995 2023-05-03 09:47:13.000000 musiclang-0.8.9/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-03 09:47:14.972462 musiclang-0.8.9/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1417 2023-05-03 09:47:13.000000 musiclang-0.8.9/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/tests/analyze/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/analyze/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/analyze/test_analyze.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8605 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/analyze/test_score_formatter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/composing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/composing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/composing/test_counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1176 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/composing/test_project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1920 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/composing/test_voice_leading.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/predict/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/predict/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1951 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/predict/test_auto_composer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/transform/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2557 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_mask.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_transform_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_transforms.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/out/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/out/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3633 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/out/test_to_midi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/pitches/test_pitches_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/properties/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/properties/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/properties/test_note_properties.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/rythm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/rythm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/rythm/test_metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_absolute_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_bass_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2881 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_chord_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_chromatic_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_drum_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_extensions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_melody.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1916 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5994 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_score.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2485 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_tonality.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.510496 musiclang-0.9.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1302 2023-07-27 15:26:03.000000 musiclang-0.9.0/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5705 2023-07-27 15:26:06.510496 musiclang-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3679 2023-07-27 15:26:03.000000 musiclang-0.9.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.486496 musiclang-0.9.0/musiclang/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      694 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.490496 musiclang-0.9.0/musiclang/analyze/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      820 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.490496 musiclang-0.9.0/musiclang/analyze/augmented_net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5042 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    69481 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/chord_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4367 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/feature_representation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9003 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/inference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18747 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/input_representations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/keydistance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6149 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/output_representations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6275 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/score_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2667 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/augmented_net/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7054 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/chord_inference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2544 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/chord_inference_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5794 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/dataset_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6500 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/dataset_trainer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2920 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3435 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/load_score.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6521 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/midi_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15358 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/pattern_analyzer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/pattern_sampler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10479 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/roman_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10759 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/score_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11992 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/score_formatter_elements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3172 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/split.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9213 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/to_musiclang.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8854 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/analyze/voice_separation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/library.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.494496 musiclang-0.9.0/musiclang/predict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.494496 musiclang-0.9.0/musiclang/predict/arranger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/arranger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8579 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/arranger/arranger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/arranger/arranger_trainer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/arranger/melody_arranger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6092 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/arranger/melody_arranger_trainer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.494496 musiclang-0.9.0/musiclang/predict/composer/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/composer/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8888 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/composer/auto_composer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/composer/composer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/composer/harmony.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.494496 musiclang-0.9.0/musiclang/predict/predictors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/predictors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5578 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/predictors/hugging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7398 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/predictors/windowed.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.494496 musiclang-0.9.0/musiclang/predict/tokenizers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/tokenizers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/predict/tokenizers/chord_tokenizer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.494496 musiclang-0.9.0/musiclang/transform/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7925 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/base_transformer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.494496 musiclang-0.9.0/musiclang/transform/chord/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/chord/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/chord/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/composing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/arrange.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11465 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6105 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/layer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6234 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/patternator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13358 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18036 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/composing/voice_leading.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/dynamics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/dynamics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1335 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/dynamics/dynamizer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/features/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/features/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/features/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/generators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/generators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/generators/rythm_generator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4258 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/library.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19220 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/mask.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/melody/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/melody/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4570 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/melody/basics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/melody/continuation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/melody/filler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/merger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/note/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/note/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/note/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/orchestrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/orchestrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/orchestrations/epic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/orchestrations/nocturne.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/pipeline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/score/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/score/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/score/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/score_merger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/score_merger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/score_merger/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.498496 musiclang-0.9.0/musiclang/transform/structure_graphs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/structure_graphs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/structure_graphs/forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/transformer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/transform/utils_random.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.502496 musiclang-0.9.0/musiclang/write/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.502496 musiclang-0.9.0/musiclang/write/arrange_utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/arrange_utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4580 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/arrange_utils/arrange_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/arrange_utils/skyline_algorithm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45096 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13534 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4651 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/element.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.502496 musiclang-0.9.0/musiclang/write/elements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/bar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/beat.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/element.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/free_text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/rhythm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/time_signature.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/tonality.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/voice_leading.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/elements/voicing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14241 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/library.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14138 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/melody.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27348 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/note_pitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8474 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/ornementation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/musiclang/write/out/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/out/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3906 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/out/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13039 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/out/midi_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3540 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/out/to_code.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8425 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/out/to_midi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12321 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/out/to_mxl.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/musiclang/write/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5397 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/pitches/pitches_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/musiclang/write/properties/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/properties/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6890 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/properties/note_properties.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/musiclang/write/rhythm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/rhythm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14944 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/rhythm/metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/rhythm/score_rythm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/rhythm/utils_metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41005 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/score.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/musiclang/write/sequence/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/sequence/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4656 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/sequence/sequence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12288 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/sequence/sequence_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/musiclang/write/time_utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/time_utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5520 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/time_utils/time_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9483 2023-07-27 15:26:03.000000 musiclang-0.9.0/musiclang/write/tonality.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.486496 musiclang-0.9.0/musiclang.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5705 2023-07-27 15:26:06.000000 musiclang-0.9.0/musiclang.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6427 2023-07-27 15:26:06.000000 musiclang-0.9.0/musiclang.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-27 15:26:06.000000 musiclang-0.9.0/musiclang.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-07-27 15:26:06.000000 musiclang-0.9.0/musiclang.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-07-27 15:26:06.000000 musiclang-0.9.0/musiclang.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1005 2023-07-27 15:26:04.000000 musiclang-0.9.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-27 15:26:06.510496 musiclang-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1431 2023-07-27 15:26:04.000000 musiclang-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/tests/analyze/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/analyze/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/analyze/test_analyze.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8605 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/analyze/test_score_formatter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/tests/composing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/composing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/composing/test_counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/composing/test_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1920 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/composing/test_voice_leading.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.506496 musiclang-0.9.0/tests/predict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/predict/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1951 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/predict/test_auto_composer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.510496 musiclang-0.9.0/tests/transform/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/transform/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2557 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/transform/test_mask.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/transform/test_pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/transform/test_transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/transform/test_transform_graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/transform/test_transforms.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.510496 musiclang-0.9.0/tests/write/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.510496 musiclang-0.9.0/tests/write/out/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/out/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3633 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/out/test_to_midi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.510496 musiclang-0.9.0/tests/write/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/pitches/test_pitches_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.510496 musiclang-0.9.0/tests/write/properties/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/properties/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/properties/test_note_properties.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:06.510496 musiclang-0.9.0/tests/write/rythm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/rythm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/rythm/test_metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_absolute_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_bass_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2881 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_chord_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_chromatic_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_drum_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_extensions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_melody.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1916 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5994 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_score.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2485 2023-07-27 15:26:03.000000 musiclang-0.9.0/tests/write/test_tonality.py
```

### Comparing `musiclang-0.8.9/LICENSE.md` & `musiclang-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/PKG-INFO` & `musiclang-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,139 +1,157 @@
 Metadata-Version: 2.1
 Name: musiclang
-Version: 0.8.9
+Version: 0.9.0
 Summary: A python package for music notation and generation
-Home-page: UNKNOWN
 Author: Florian GARDIN
-Author-email: fgardin.pro@gmail.com
-License: UNKNOWN
-Project-URL: Documentation, https://musiclang.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/MusicLang/musiclang/
-Project-URL: Tracker, https://github.com/MusicLang/musiclang/issues
-Description: Musiclang
-        =========
+Author-email: Florian GARDIN <fgardin.pro@gmail.com>
+License: BSD 2-Clause License
         
-        ![MusicLang logo](https://github.com/MusicLang/musiclang/blob/main/documentation/images/MusicLang.png?raw=true "MusicLang")
+        Copyright (c) 2023, Florian GARDIN
         
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
         
-        [![Documentation Status](https://readthedocs.org/projects/musiclang/badge/?version=latest)](https://musiclang.readthedocs.io/en/latest/?badge=latest)
-        
-        The Python framework to write, analyze, transform and predict music.
-        
-        
-        What is MusicLang ?
-        --------------------
-        
-        MusicLang which simply stands for "music language" is a Python framework
-        that allows composers to write symbolic music in a condensed and high level manner.
-        It can be used to write, arrange, transform or predict new music.
-        This framework is not only another notation software but also
-        an assistant that is able to automate some tasks that would normally be tedious for a composer.
-        It is naturally good at analyzing and manipulating existing
-        pieces of music in musicxml or midi format.
-        
-        [Read our documentation](https://musiclang.readthedocs.io/en/latest).
-        
-        
-        How to install
-        --------------
-        
-        MusicLang is available on Pypi :
-        
-        ```
-        pip install musiclang
-        ```
-        
-        Or use this repo for the latest version :
-        
-        ```
-        pip install git+https://github.com/MusicLang/musiclang
-        ```
-            
-        
-        Examples
-        ---------
-        
-        1. A hello world example to create a C-major chord in musiclang and save it to midi :
-        
-        ```python
-        from musiclang.library import *
-        
-        # Write A C major chord
-        score = (I % I.M)(piano=[s0, s2, s4])
-        
-        # Store it to midi
-        score.to_midi('c_major.mid')
-        ```
-        
-        2. Create, transform and harmonize a theme quickly : 
-        
-        ```python
-        from musiclang.library import *
-        
-        # Create a cool melody (the beginning of happy birthday, independant of any harmonic context)
-        melody = s4.ed + s4.s + s5 + s4 + s0.o(1) + s6.h
-        
-        # Create a simple accompaniment with a cello and a oboe
-        acc_melody = r + s0.o(-1).q * 3 + s0.o(-1).h
-        accomp = {'cello__0': acc_melody, 'oboe__0': acc_melody.o(1)}
-        
-        # Play it in F-major
-        score = (I % IV.M)(violin__0=melody, **accomp)
-        
-        # Repeat the score a second time in F-minor and forte
-        score += (score % I.m).f
-        
-        # Just to create an anachrusis at the first bar
-        score = (I % I.M)(violin__0=r.h) + score
-        
-        # Transform a bit the accompaniment by applying counterpoint rules automatically
-        from musiclang.transform.library import create_counterpoint_on_score
-        score = create_counterpoint_on_score(score, fixed_parts=['violin__0'])
-        
-        # Save it to musicxml
-        score.to_musicxml('happy_birthday.musicxml', signature=(3, 4), title='Happy birthday !')
-        
-        # Et voilà !
-        ```
-        ![Happy birthday score](https://github.com/MusicLang/musiclang/blob/main/documentation/images/happy_birthday.png?raw=true "Happy Birthday")
-        
-        
-        3. Predict a score using a deep learning model trained on musiclang language :
-        
-        ```python
-        from musiclang.library import *
-        from musiclang import Score
-        
-        # Some random bar of chopin op18 Waltz
-        score = ((V % III.b.M)(
-        	piano__0=s0 + s2.e.mp + s3.e.mp, 
-        	piano__4=s0.e.o(-2).p + r.e + s0.ed.o(-1).mp + r.s, 
-        	piano__5=r + s4.ed.o(-1).mp + r.s, 
-        	piano__6=r + s6.ed.o(-1).mp + r.s)+ 
-        (V['7'] % III.b.M)(
-        	piano__0=s2.ed.mp + r.s, 
-        	piano__2=s4.ed.mp + r.s, 
-        	piano__4=s6.ed.o(-1).mp + r.s, 
-        	piano__5=s0.ed.o(-1).mp + r.s, 
-        	piano__6=s4.ed.o(-1).mp + r.s))
-        
-        # Predict the next two chords of the score using huggingface musiclang model
-        predicted_score = score.predict_score(n_chords=2, temperature=0.5)
-        # Save it to midi
-        predicted_score.to_midi('test.mid')
-        ```
-        
-        Please note that this feature is still experimental, it will only work with
-        piano music for now and the model is not yet trained on a large corpus of music.
-        If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
-        
-        
-        4. Mix everything together to create a new pieces of music !
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Project-URL: Homepage, https://github.com/MusicLang/musiclang
+Keywords: music,ai,notation
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
+Musiclang
+=========
+
+![MusicLang logo](https://github.com/MusicLang/musiclang/blob/main/documentation/images/MusicLang.png?raw=true "MusicLang")
+
+
+[![Documentation Status](https://readthedocs.org/projects/musiclang/badge/?version=latest)](https://musiclang.readthedocs.io/en/latest/?badge=latest)
+
+The Python framework to write, analyze, transform and predict music.
+
+
+What is MusicLang ?
+--------------------
+
+MusicLang which simply stands for "music language" is a Python framework
+implementing a new language for tonal music.
+This language allows composers to load, write, transform and predict symbolic music in a simple,
+condensed and high level manner.
+MusicLang internally uses  a [LLM (Large Language Model)](https://huggingface.co/floriangardin/musiclang)  to predict what could happen next in a musical score.
+This framework is well suited to :
+- Generate musical ideas quickly.
+- Predict what could happen next in an existing midi file
+- Create an interpretable and information rich text representation of a midi file
+
+[Read our documentation](https://musiclang.readthedocs.io/en/latest).
+
+
+How to install
+--------------
+
+MusicLang is available on Pypi :
+
+```
+pip install musiclang
+```
+    
+
+Examples
+---------
+
+1. A hello world example to create a C-major chord in musiclang and save it to midi :
+
+```python
+from musiclang.library import *
+
+# Write A C major chord
+score = (I % I.M)(piano=[s0, s2, s4])
+
+# Store it to midi
+score.to_midi('c_major.mid')
+```
+
+2. Create, transform and harmonize a theme quickly : 
+
+```python
+from musiclang.library import *
+
+# Create a cool melody (the beginning of happy birthday, independant of any harmonic context)
+melody = s4.ed + s4.s + s5 + s4 + s0.o(1) + s6.h
+
+# Create a simple accompaniment with a cello and a oboe
+acc_melody = r + s0.o(-1).q * 3 + s0.o(-1).h
+accomp = {'cello__0': acc_melody, 'oboe__0': acc_melody.o(1)}
+
+# Play it in F-major
+score = (I % IV.M)(violin__0=melody, **accomp)
+
+# Repeat the score a second time in F-minor and forte
+score += (score % I.m).f
+
+# Just to create an anachrusis at the first bar
+score = (I % I.M)(violin__0=r.h) + score
+
+# Transform a bit the accompaniment by applying counterpoint rules automatically
+from musiclang.transform.library import create_counterpoint_on_score
+score = create_counterpoint_on_score(score, fixed_parts=['violin__0'])
+
+# Save it to musicxml
+score.to_musicxml('happy_birthday.musicxml', signature=(3, 4), title='Happy birthday !')
+
+# Et voilà !
+```
+![Happy birthday score](https://github.com/MusicLang/musiclang/blob/main/documentation/images/happy_birthday.png?raw=true "Happy Birthday")
+
+
+3. Predict a score using a deep learning model trained on musiclang language :
+
+```python
+from musiclang.library import *
+from musiclang import Score
+
+# Some random bar of chopin op18 Waltz
+score = ((V % III.b.M)(
+	piano__0=s0 + s2.e.mp + s3.e.mp, 
+	piano__4=s0.e.o(-2).p + r.e + s0.ed.o(-1).mp + r.s, 
+	piano__5=r + s4.ed.o(-1).mp + r.s, 
+	piano__6=r + s6.ed.o(-1).mp + r.s)+ 
+(V['7'] % III.b.M)(
+	piano__0=s2.ed.mp + r.s, 
+	piano__2=s4.ed.mp + r.s, 
+	piano__4=s6.ed.o(-1).mp + r.s, 
+	piano__5=s0.ed.o(-1).mp + r.s, 
+	piano__6=s4.ed.o(-1).mp + r.s))
+
+# Predict the next two chords of the score using huggingface musiclang model
+predicted_score = score.predict_score(n_chords=4, temperature=0.5)
+# Save it to midi
+predicted_score.to_midi('test.mid')
+```
+
+Please note that this feature is still experimental, it will only work with
+piano music for now and the model is not yet trained on a large corpus of music.
+If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
+
+
+4. Mix everything together to create a new pieces of music !
+
```

### Comparing `musiclang-0.8.9/README.md` & `musiclang-0.9.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,38 +9,34 @@
 The Python framework to write, analyze, transform and predict music.
 
 
 What is MusicLang ?
 --------------------
 
 MusicLang which simply stands for "music language" is a Python framework
-that allows composers to write symbolic music in a condensed and high level manner.
-It can be used to write, arrange, transform or predict new music.
-This framework is not only another notation software but also
-an assistant that is able to automate some tasks that would normally be tedious for a composer.
-It is naturally good at analyzing and manipulating existing
-pieces of music in musicxml or midi format.
+implementing a new language for tonal music.
+This language allows composers to load, write, transform and predict symbolic music in a simple,
+condensed and high level manner.
+MusicLang internally uses  a [LLM (Large Language Model)](https://huggingface.co/floriangardin/musiclang)  to predict what could happen next in a musical score.
+This framework is well suited to :
+- Generate musical ideas quickly.
+- Predict what could happen next in an existing midi file
+- Create an interpretable and information rich text representation of a midi file
 
 [Read our documentation](https://musiclang.readthedocs.io/en/latest).
 
 
 How to install
 --------------
 
 MusicLang is available on Pypi :
 
 ```
 pip install musiclang
 ```
-
-Or use this repo for the latest version :
-
-```
-pip install git+https://github.com/MusicLang/musiclang
-```
     
 
 Examples
 ---------
 
 1. A hello world example to create a C-major chord in musiclang and save it to midi :
 
@@ -103,15 +99,15 @@
 	piano__0=s2.ed.mp + r.s, 
 	piano__2=s4.ed.mp + r.s, 
 	piano__4=s6.ed.o(-1).mp + r.s, 
 	piano__5=s0.ed.o(-1).mp + r.s, 
 	piano__6=s4.ed.o(-1).mp + r.s))
 
 # Predict the next two chords of the score using huggingface musiclang model
-predicted_score = score.predict_score(n_chords=2, temperature=0.5)
+predicted_score = score.predict_score(n_chords=4, temperature=0.5)
 # Save it to midi
 predicted_score.to_midi('test.mid')
 ```
 
 Please note that this feature is still experimental, it will only work with
 piano music for now and the model is not yet trained on a large corpus of music.
 If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
```

### Comparing `musiclang-0.8.9/musiclang/__init__.py` & `musiclang-0.9.0/musiclang/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/__init__.py` & `musiclang-0.9.0/musiclang/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/cache.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/cache.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/chord_vocabulary.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/chord_vocabulary.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/feature_representation.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/feature_representation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/inference.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 
 modelPath = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'AugmentedNet.hdf5')
 
 MODEL = None
 
 def get_model():
     global MODEL
+    print('LOADING MODEL')
     if MODEL is not None:
         return MODEL
     else:
         disableGPU()
         MODEL = keras.models.load_model(modelPath)
         return MODEL
 
-MODEL = get_model()
 
 
 inversions = {
     "triad": {
         0: "",
         1: "6",
         2: "64",
```

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/input_representations.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/input_representations.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/keydistance.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/keydistance.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/models.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/models.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/output_representations.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/output_representations.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/score_parser.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/score_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 def m21Parse(f, fmt=None, remove_perc=True):
     """
 
     Parameters
     ----------
     f :
-        
+
     fmt :
          (Default value = None)
 
     Returns
     -------
 
     """
```

### Comparing `musiclang-0.8.9/musiclang/analyze/augmented_net/utils.py` & `musiclang-0.9.0/musiclang/analyze/augmented_net/utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/constants.py` & `musiclang-0.9.0/musiclang/analyze/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/item.py` & `musiclang-0.9.0/musiclang/analyze/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,12 +98,13 @@
     for note in notes:
         start = note[0]
         end = start + note[2]
         vel = int(note[3])
         pitch = int(note[1])
         track = int(note[4])
         channel = int(note[5])
-        items.append(Item("name", start, end, vel=vel, pitch=pitch, track=track, channel=channel, voice=0))
+        voice = int(note[6])
+        items.append(Item("name", start, end, vel=vel, pitch=pitch, track=track, channel=channel, voice=voice))
 
     # Quantize notes in integer
     items = quantize_notes_raw(items)
     return items
```

### Comparing `musiclang-0.8.9/musiclang/analyze/midi_parser.py` & `musiclang-0.9.0/musiclang/analyze/midi_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
 
 import pandas as pd
 import numpy as np
 from mido import MidiFile
-
+import time
+import warnings
 
 TYPE = "type"
 TIME = "time"
 NOTE = "note"
 VEL = "vel"
 CHANNEL = "channel"
 DURATION = "duration"
@@ -35,18 +36,19 @@
     **kwargs :
         
 
     Returns
     -------
 
     """
-    notes, config = _load_midi(filename, **kwargs)
+    notes, config, bars = _load_midi(filename, **kwargs)
     instruments = config['instruments']
     tempo = config['tempo']
-    return notes, instruments, tempo
+    time_signature = config['bar_duration']
+    return notes, instruments, tempo, time_signature, bars
 
 
 """
 Below, some loader helpers :
 """
 
 class MusicLangIgnoreException(Exception):
@@ -66,22 +68,23 @@
     **kwargs :
         
 
     Returns
     -------
 
     """
-    notes, config = _parse(filename)
+    notes, config, bars = _parse(filename)
     if len(config['bar_durations']) > 1 and ignore_file_with_bar_change:
         raise MusicLangIgnoreException('Bar duration change events in midifile, MusicLang cannot parse that')
     elif len(config['bar_durations']) == 1:
         config['bar_duration'] = config['bar_durations'][0]
     else:
         config['bar_duration'] = None
-    return notes, config
+    return notes, config, bars
+
 
 
 def _parse(filename, **kwargs):
     """
 
     Parameters
     ----------
@@ -91,43 +94,56 @@
         
 
     Returns
     -------
 
     """
     from fractions import Fraction as frac
-
+    from .load_score import load_score
     mf = MidiFile(filename)
     instruments = _infer_instruments(mf)
     notes = []
     bar_durations = []
     tempos = []
-
     for track_idx, track in enumerate(mf.tracks):
-        time = 0
+        t = 0
         for note in track:
             if note.type == 'note_on':
-                notes.append([1, time + note.time, note.note, note.velocity, note.channel, track_idx])
+                notes.append([1, t + note.time, note.note, note.velocity, note.channel, track_idx])
             elif note.type == 'note_off':
-                notes.append([0, time + note.time, note.note, note.velocity, note.channel, track_idx])
+                notes.append([0, t + note.time, note.note, note.velocity, note.channel, track_idx])
             elif note.type == 'time_signature':
                 bar_durations.append(note.numerator * frac(4, note.denominator))
             elif note.type == 'set_tempo':
                 tempos.append((time, note.tempo))
-            time = time + note.time
-    notes = np.asarray(notes)
+            t = t + note.time
     first_tempo = int(60/(tempos[0][1]/1e6))
     config = {'ticks_per_beats': mf.ticks_per_beat,
              'instruments': instruments,
              'tempo': first_tempo, 'tempos': tempos, 'bar_durations': bar_durations}
-
-    notes = _get_notes_dataframe(notes)
-    notes = _get_notes_in_beats(notes, mf.ticks_per_beat)
-    notes = np.asarray(notes[[START_TIME, NOTE, DURATION, VEL, TRACK, CHANNEL, VOICE]])
-    return notes, config
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        notes_score, bars = load_score(filename, ticks_per_beat=mf.ticks_per_beat)
+    notes_score_df = pd.DataFrame(notes_score, columns=[START_TIME, END_TIME, VEL, NOTE, TRACK, CHANNEL, VOICE])
+    notes_score_df[TRACK] = (notes_score_df[TRACK] + 1).astype(int)
+    notes_score_df[DURATION] = notes_score_df[END_TIME] - notes_score_df[START_TIME]
+    notes_score_df[VOICE] = (notes_score_df[VOICE] - 1).astype(int)
+
+    if notes_score_df[START_TIME].min() < 0:
+        # Add bar duration in notes_score[START_TIME]
+        bar_duration = config['bar_durations'][0]
+        notes_score_df[START_TIME] += bar_duration
+        for idx in range(len(bars)):
+            bars[idx] = bars[idx][0] + bar_duration, bars[idx][1] + bar_duration
+
+    if len(bars) > 1 and (bars[-1][1] - bars[-1][0] != bars[-2][1] - bars[-2][0]):
+        bars[-1] = bars[-1][0], bars[-1][0] + bars[-2][1] - bars[-2][0]
+    #notes_score_df[START_TIME] = notes_score_df[START_TIME] - notes_score_df[START_TIME].min() # Start at 0
+    notes = np.asarray(notes_score_df[[START_TIME, NOTE, DURATION, VEL, TRACK, CHANNEL, VOICE]])
+    return notes, config, bars
 
 
 def _get_notes_in_beats(df, ticks_per_beats):
     """By default notes are stored in ticks from midi file, convert it to beats
     :return:
 
     Parameters
```

### Comparing `musiclang-0.8.9/musiclang/analyze/parser.py` & `musiclang-0.9.0/musiclang/analyze/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 LICENSE file in the root directory of this source tree.
 """
 
 """
 This file groups a set of functions to parse files into MusicLang objects
 """
 
-def parse_to_musiclang(input_file: str):
+def parse_to_musiclang(input_file: str, **kwargs):
     """Parse an input file into a musiclang Score
     - Get chords with the AugmentedNet (https://github.com/napulen/AugmentedNet)
     - Get voice separation and parsing
 
     Parameters
     ----------
     input_file : str
@@ -27,21 +27,21 @@
 
     config: dict
         Dict of score configuration
 
     """
     extension = input_file.split('.')[-1]
     if extension.lower() in ['mid', 'midi']:
-        return parse_midi_to_musiclang(input_file)
+        return parse_midi_to_musiclang(input_file, **kwargs)
     elif extension.lower() in ['mxl', 'xml', 'musicxml', 'krn']:
-        return parse_mxl_to_musiclang(input_file)
+        return parse_mxl_to_musiclang(input_file, **kwargs)
     else:
         raise Exception('Unknown extension {}'.format(extension))
 
-def parse_midi_to_musiclang(input_file: str):
+def parse_midi_to_musiclang(input_file: str, **kwargs):
     """Parse a midi input file into a musiclang Score
     - Get chords with the AugmentedNet (https://github.com/napulen/AugmentedNet)
     - Get voice separation and parsing
 
     Parameters
     ----------
     input_file : str
@@ -55,26 +55,25 @@
     config: dict
      Dict of score configuration
 
     """
     import tempfile
     import os
     import shutil
-    from .augmented_net import m21Parse
     with tempfile.TemporaryDirectory() as di:
         midi_file = os.path.join(di, 'data.mid')
         mxl_file = os.path.join(di, 'data.mxl')
-        obj = m21Parse(input_file, remove_perc=True)
-        obj.write('musicxml', fp=os.path.join(di, mxl_file))
+        #obj = _m21Parse(input_file, remove_perc=True)
+        #obj.write('musicxml', fp=os.path.join(di, mxl_file))
         shutil.copy(input_file, midi_file)
-        result = parse_directory_to_musiclang(di)
+        result = parse_directory_to_musiclang(di, **kwargs)
     return result
 
 
-def parse_mxl_to_musiclang(input_file: str):
+def parse_mxl_to_musiclang(input_file: str, **kwargs):
     """Parse a music xml input file into a musiclang Score
     - Get chords with the AugmentedNet (https://github.com/napulen/AugmentedNet)
     - Separate into monophonic voice with the proper instrument
 
     Parameters
     ----------
     input_file: str :
@@ -89,25 +88,24 @@
 
     """
 
     import tempfile
     import os
     import music21
     import shutil
-    from .augmented_net import m21Parse
     with tempfile.TemporaryDirectory() as di:
         midi_file = os.path.join(di, 'data.mid')
         mxl_file = os.path.join(di, 'data.mxl')
-        obj = m21Parse(input_file)
+        obj = _m21Parse(input_file)
         obj.write('midi', fp=os.path.join(di, midi_file))
         shutil.copy(input_file, mxl_file)
-        result = parse_directory_to_musiclang(di)
+        result = parse_directory_to_musiclang(di, **kwargs)
     return result
 
-def parse_directory_to_musiclang(directory: str):
+def parse_directory_to_musiclang(directory: str, fast_chord_inference=True, **kwargs):
     """Parse a directory containing a 'data.mid' and 'data_annotated.rntxt' file (midi file and chord annotation file)
 
     Parameters
     ----------
     directory : str
         Directory with a "data.mid" file and a "data_annotated.rntxt" annotation file
 
@@ -117,26 +115,55 @@
         MusicLang score parsed
 
     config: dict
         Dict of score configuration
 
     """
     import os
-    from .augmented_net import infer_chords
-    print('1/4 : Analyze the score (This may takes a while)')
-    annotation_file = os.path.join(directory, 'data_annotated.rntxt')
     midi_file = os.path.join(directory, 'data.mid')
     mxl_file = os.path.join(directory, 'data.mxl')
-    infer_chords(mxl_file)
-    score, config = parse_midi_to_musiclang_with_annotation(midi_file, annotation_file)
-    score = score.clean()
+    if not fast_chord_inference:
+        from .augmented_net import infer_chords
+        print('1/4 : Analyze the score (This may takes a while)')
+        annotation_file = os.path.join(directory, 'data_annotated.rntxt')
+        infer_chords(mxl_file)
+        score, config = parse_midi_to_musiclang_with_annotation(midi_file, annotation_file)
+    else:
+        score, config = parse_midi_to_musiclang_without_annotation(midi_file)
+
+    score = score.to_drum()
     return score, config
 
 
 
+def parse_midi_to_musiclang_without_annotation(midi_file: str):
+    """
+
+    Parameters
+    ----------
+    midi_file: str :
+        Filepath to the midi file to parse
+
+    annotation_file: str :
+        Filepath to the anotation file to parse
+
+
+    Returns
+    -------
+    score: Score
+        MusicLang score parsed
+
+    config: dict
+        Config of the score
+
+    """
+    config = {}
+    score, tempo = parse_musiclang_sequence_and_chords(midi_file)
+    config.update({'tempo': tempo})
+    return score, config
 
 def parse_midi_to_musiclang_with_annotation(midi_file: str, annotation_file: str):
     """
 
     Parameters
     ----------
     midi_file: str :
@@ -147,19 +174,20 @@
 
 
     Returns
     -------
     score: Score
         MusicLang score parsed
 
-    tempo: int
-        Tempo of the score
+    config: dict
+        Config of the score
 
     """
 
+
     chords = get_chords_from_analysis(annotation_file)
     config = chords.config
     score, tempo = parse_musiclang_sequence(midi_file, chords)
     config.update({'tempo': tempo})
     return score, config
 
 
@@ -311,14 +339,45 @@
         result, fractions.Fraction with denominator limited to 8
 
     """
     from fractions import Fraction as frac
     return frac(roman.duration.quarterLength).limit_denominator(8)
 
 
+def parse_musiclang_sequence_and_chords(midi_file):
+    """Parse a midi file into MusicLang and chords
+
+    Parameters
+    ----------
+    midi_file : str
+        Path to the midi file
+    """
+    from musiclang import Score
+    from .midi_parser import parse_midi
+    from .item import convert_to_items
+    from .to_musiclang import infer_score_with_chords_durations
+    from .chord_inference import fast_chord_inference
+
+    print('1/4 : Performing voice separation (This may takes a while)')
+    notes, instruments, tempo, time_signature, bars = parse_midi(midi_file)
+    print('2/4 : Now infering chords with fast inference')
+    chords = fast_chord_inference(notes, bars)
+    sequence = convert_to_items(notes)
+    print('3/4 : Create the score')
+    import time
+    start = time.time()
+    score = infer_score_with_chords_durations(sequence, chords, instruments)
+    print('Finished creating score in {} seconds'.format(time.time() - start))
+    print('Finished creating score')
+    print('4/4 Normalize the score...')
+    score = score.normalize()
+
+    return score, tempo
+
+
 def parse_musiclang_sequence(midi_file, chords):
     """Parse a midi file into MusicLang and chords with chords duration
 
     Parameters
     ----------
     midi_file :
 
@@ -328,23 +387,25 @@
     Returns
     -------
 
     """
     from musiclang import Score
     from .midi_parser import parse_midi
     from .item import convert_to_items
-    from .to_musiclang import infer_voices_per_tracks, infer_score_with_chords_durations
-    notes, instruments, tempo = parse_midi(midi_file)
-    sequence = convert_to_items(notes)
+    from .to_musiclang import infer_score_with_chords_durations
+
+
     print('2/4 : Performing voice separation (This may takes a while)')
-    sequence = infer_voices_per_tracks(sequence)
+    notes, instruments, tempo, time_signature, bars = parse_midi(midi_file)
+    sequence = convert_to_items(notes)
     print('3/4 : Create the score')
     score = infer_score_with_chords_durations(sequence, chords, instruments)
     print('Finished creating score')
-    print('4/4 Create a copy of the score...')
+    print('4/4 Normalize the score...')
+    score = score.normalize()
 
     return score, tempo
 
 
 def get_chords_from_mxl(input_file):
     """Given a mxl file, return a MusicLang score parsing only the chord progression
 
@@ -487,7 +548,39 @@
 
 def old_annotation_to_musiclang(file):
     import music21
     analysis = music21.converter.parse(file, format="romanText")
     chords = music21_roman_analysis_to_chords(analysis)
     score = chords_to_musiclang(chords)
     return score
+
+
+def _m21Parse(f, fmt=None, remove_perc=True):
+    """
+
+    Parameters
+    ----------
+    f :
+
+    fmt :
+         (Default value = None)
+
+    Returns
+    -------
+
+    """
+    import music21
+    s = music21.converter.parse(f, format=fmt, forceSource=True)
+    if remove_perc:
+
+        for el in s.recurse():
+            if set(el.classes).intersection(['PercussionChord', 'Unpitched']):  # or 'Piano'
+                # el.activeSite.replace(el, instrument.Violin())
+                el.activeSite.remove(el)
+
+        # perc = [
+        #     p
+        #     for p in s.parts
+        #     if list(p.recurse().getElementsByClass(["PercussionClef", "PercussionChord"]))
+        # ]
+        # s.remove(perc, recurse=True)
+    return s
```

### Comparing `musiclang-0.8.9/musiclang/analyze/pattern_analyzer.py` & `musiclang-0.9.0/musiclang/analyze/pattern_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import time
+
 from musiclang.write.pitches.pitches_utils import get_relative_scale_value
-from musiclang import Note
+from musiclang import Note, Melody
 import numpy as np
 from musiclang.library import *
 from musiclang import Score
 from musiclang.write.out import get_pitches, get_pitches_instruments
 
 
 def get_candidate(candidates, scale, new_pitch, last_pitch):
@@ -55,17 +57,19 @@
 def transform_note_to_relative_note_with_chord_note(note, chord, last_pitch, voicing, idx_instrument):
     if not note.is_note:
         return note, last_pitch, voicing
     # First transform to chord extension note if possible
     chord_pitch_classes = chord.chord_extension_pitch_classes
     new_pitch = chord.to_pitch(note)
     pitch_class = new_pitch % 12
+    start = time.time()
     if pitch_class in chord_pitch_classes:
         # Transform to chord extension note
         real_note = transform_note_to_chord_extension(note, chord)
+
         # If voicing is None, then attribute voicing
         if voicing is None:
             new_note = real_note.copy()
             voicing = new_note.set_duration(1).set_amp('mf')
             new_note.type = "x"
             new_note.val = idx_instrument
             new_note.octave = 0
@@ -84,20 +88,25 @@
     return new_note, new_pitch, voicing
 
 
 def transform_melody_to_relative(melody, chord, idx_instrument, prev_voicing=None):
     last_pitch = None
     new_melody = None
     voicing = None
+    new_melody = []
     for note in melody.notes:
         new_note, last_pitch, voicing = transform_note_to_relative_note_with_chord_note(note, chord,
                                                                                         last_pitch, voicing,
                                                                                         idx_instrument)
-        new_melody += new_note
+        if isinstance(new_note, Note):
+            new_melody.append(new_note)
+        else:
+            new_melody += new_note.notes
 
+    new_melody = Melody(new_melody)
     if voicing is None:
         voicing = prev_voicing
 
     return new_melody, voicing
 
 
 def exclude_instruments(chord, nb, ascending=True):
@@ -226,17 +235,19 @@
     def extract(self, chord):
 
         if self.melody:
             result_score, voicing, instruments, bar_duration = transform_chord_to_relative(chord,
                                                                                             len(chord.score.items()) - 1,
                                                                                                 ascending=False)
         else:
+            start = time.time()
             result_score, voicing, instruments, bar_duration = transform_chord_to_relative(chord,
                                                                                             self.nb_excluded_instruments,
                                                                                             ascending=True)
+            print('transform chord to relative', time.time() - start)
 
         if self.instruments is not None:
             instruments = self.instruments[:len(instruments)] + instruments[len(self.instruments):]
         if self.voicing is not None:
             voicing = self.voicing[:len(voicing)] + voicing[len(self.voicing):]
 
         dict_pattern = {
```

### Comparing `musiclang-0.8.9/musiclang/analyze/pattern_sampler.py` & `musiclang-0.9.0/musiclang/analyze/pattern_sampler.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/roman_parser.py` & `musiclang-0.9.0/musiclang/analyze/roman_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/score_formatter.py` & `musiclang-0.9.0/musiclang/analyze/score_formatter.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/score_formatter_elements.py` & `musiclang-0.9.0/musiclang/analyze/score_formatter_elements.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/analyze/to_musiclang.py` & `musiclang-0.9.0/musiclang/analyze/to_musiclang.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
 
 from .voice_separation import separate_voices
 from musiclang.write.note import Silence, Continuation
 from musiclang.write.constants import OCTAVES
-
+from musiclang import Score
 
 def infer_score_with_chords_durations(sequence, chords, instruments):
     """Get the score from a note sequence, the chords with durations and the instruments assigned to each tracks
 
     Parameters
     ----------
     sequence :
@@ -26,52 +26,49 @@
     Returns
     -------
 
     """
     # Split each chords, instruments, voices
     time_start = 0
     time_end = 0
-    score = None
+    score = []
     continuations = {}
     offsets_voices = {}  # Store the offset of voice to deduplicate voice idx between tracks
     offsets_voices_raw = {}  # Store the offset of voice to deduplicate voice idx between tracks
     tracks = list(set([s.track for s in sequence]))
-
     for channel, instrument in instruments.items():
         for track_idx in tracks:
             track_notes = [n for n in sequence if n.track == track_idx]
             voices = {n.voice for n in track_notes}
             offsets_voices[track_idx] = offsets_voices_raw.get(channel, 0)
             if channel not in offsets_voices_raw.keys():
                 offsets_voices_raw[channel] = max(voices) + 1
             else:
                 offsets_voices_raw[channel] += max(voices) + 1
-
     for idx, chord in enumerate(chords):
         time_start = 0 if idx == 0 else time_start + chords[idx - 1].duration
         time_end += chord.duration
         chord_notes = [n for n in sequence if time_start <= n.start < time_end]
         chord_dict = {}
         for track in tracks:
             track_notes = [n for n in chord_notes if n.track == track]
             voices = {n.voice for n in track_notes}
             for voice in voices:
                 voice_notes = [n for n in track_notes if n.voice == voice]
                 if len(voice_notes) > 0:
-                    instrument = instruments[voice_notes[0].channel]
-                    voice_name = instrument + '__' + str(offsets_voices[track] + int(voice))
+                    instrument = instruments.get(voice_notes[0].channel, 'piano')
+                    voice_name = instrument + '__' + str(offsets_voices.get(track, 0) + int(voice))
                     cont = continuations.get(voice_name, None)
-                    chord_dict[voice_name], cont = _parse_voice(voice_notes, chord,
-                                                            time_start, time_end, 1, cont)
+                    chord_dict[voice_name], cont = _parse_voice(voice_notes, chord,time_start, time_end, 1, cont, is_drum=instrument.startswith('drum'))
                     if cont is not None:
                         continuations[voice_name] = cont
-                    chord_dict[voice_name] = chord_dict[voice_name].o(- OCTAVES.get(instrument, 0))
 
-        score += chord(**chord_dict)
-    return score
+        score.append(chord(**chord_dict))
+
+    return Score(score)
 
 
 def infer_score(sequence, chords, instruments, bar_duration_in_ticks, offset_in_ticks, tick_value):
     """
 
     Parameters
     ----------
@@ -170,15 +167,15 @@
 
 
 """
 Utils
 """
 
 
-def _parse_voice(voice_notes, chord, bar_time_start, bar_time_end, tick_value, cont):
+def _parse_voice(voice_notes, chord, bar_time_start, bar_time_end, tick_value, cont, is_drum=False):
     """Parse a single voice to a musicLang melody between start time and end time
 
     Parameters
     ----------
     voice_notes :
         list of notes from sequence that represents a voice
     chord :
@@ -217,54 +214,72 @@
 
         """
         value = chord.parse(note.pitch - 60)
         value = value.augment(duration)
         value.amp = note.vel
         return value.augment(tick_value)
 
-    melody = None
+    melody = []
     return_cont = None
     local_time_end = voice_notes[0].start
     if cont is not None:
-        melody += cont
+        if cont.duration > 0:
+            melody.append(cont)
         local_time_end = bar_time_start + (cont.duration / tick_value)
 
     elif local_time_end > bar_time_start:
-        melody += Silence((local_time_end - bar_time_start) * tick_value)
+        duration = (local_time_end - bar_time_start) * tick_value
+        if duration > 0:
+            melody.append(Silence(duration))
+
+    for idx, note in enumerate(voice_notes):
+        if is_drum:
+            if idx < len(voice_notes) - 1:
+                next_note = voice_notes[idx + 1]
+                note.end = next_note.start
+            else:
+                note.end = bar_time_end
 
-    for note in voice_notes:
         overlap = local_time_end - note.start
         if overlap > 0:
-            melody.notes[-1].duration -= overlap * tick_value
-            if melody.notes[-1].duration == 0:
-                melody.notes.pop()
+            melody[-1].duration -= overlap * tick_value
+            if melody[-1].duration == 0:
+                melody.pop()
             duration = note.end - note.start
-            melody += _parse_note(note, duration, chord, tick_value)
+            n = _parse_note(note, duration, chord, tick_value)
+            if n.duration > 0:
+                melody.append(n)
         elif overlap < 0:
-            melody += Silence(- overlap * tick_value)
+            melody.append(Silence(- overlap * tick_value))
             duration = note.end - note.start
             if duration > 0:
-                melody += _parse_note(note, duration, chord, tick_value)
+                n = _parse_note(note, duration, chord, tick_value)
+                if n.duration > 0:
+                    melody.append(n)
         else:
             duration = note.end - note.start
             if duration > 0:
-                melody += _parse_note(note, duration, chord, tick_value)
+                n = _parse_note(note, duration, chord, tick_value)
+                if n.duration > 0:
+                    melody.append(n)
 
         local_time_end = note.end
         # Find scale note
     if local_time_end < bar_time_end:
-        melody += Silence((bar_time_end - local_time_end) * tick_value)
+        melody.append(Silence((bar_time_end - local_time_end) * tick_value))
     if local_time_end > bar_time_end:
         return_cont = Continuation((local_time_end - bar_time_end) * tick_value)
-        melody.notes[-1].duration -= (local_time_end - bar_time_end) * tick_value
-        if melody.notes[-1].duration == 0:
-            melody.notes.pop()
+        melody[-1].duration -= (local_time_end - bar_time_end) * tick_value
+        if melody[-1].duration == 0:
+            melody.pop()
 
-    from musiclang import Note
+    from musiclang import Note, Melody
+    melody = Melody(melody)
     assert all([isinstance(m, Note) for m in melody.notes])
-    assert melody.duration == (bar_time_end - bar_time_start) * tick_value
-
+    delta_t = abs(melody.duration -  ((bar_time_end - bar_time_start) * tick_value))
+    assert delta_t < 0.25, f"Issue with melody duration {delta_t}"
+    assert melody.notes[0].duration >0, "Issue with note duration"
     return melody, return_cont
```

### Comparing `musiclang-0.8.9/musiclang/analyze/voice_separation.py` & `musiclang-0.9.0/musiclang/analyze/voice_separation.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,17 +81,17 @@
     Parameters
     ----------
     S :
         param logprob:
     n :
         param beam_size:
     logprob :
-        
+
     beam_size :
-        
+
 
     Returns
     -------
 
     """
     probas = generate_probas_for_one(S, n)
     assert len(probas) > 0
```

### Comparing `musiclang-0.8.9/musiclang/predict/arranger/arranger.py` & `musiclang-0.9.0/musiclang/predict/arranger/arranger.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/predict/arranger/arranger_trainer.py` & `musiclang-0.9.0/musiclang/predict/arranger/arranger_trainer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/predict/arranger/melody_arranger_trainer.py` & `musiclang-0.9.0/musiclang/predict/arranger/melody_arranger_trainer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/predict/composer/auto_composer.py` & `musiclang-0.9.0/musiclang/predict/composer/auto_composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     fixed_voices = [f'm__{i}' for i in range(len(melodies))]
     if fixed_bass:
         fixed_voices = fixed_voices + [bass for bass, fixed_bass in zip(basses, fixed_basses) if fixed_bass]
     for instruments, voice_leading in zip(temp_instrumentss, voice_leadings):
         if not voice_leading:
             fixed_voices = fixed_voices + instruments[1:]
 
-    score = VoiceLeading(fixed_voices=fixed_voices)(score, max_norm=3, max_norm_rules=1)
+    score = VoiceLeading(fixed_voices=fixed_voices)(score, max_norm=2, max_norm_rules=2)
 
     patternator = Patternator(**patternator)
     for orchestra, temp_instruments in zip(orchestras, temp_instrumentss):
         realized_orchestra = NC(**Pattern.from_json(orchestra, instruments=temp_instruments))
         score = patternator(realized_orchestra.set_amp(acc_amp), score)
 
     score = score.replace_instruments(**{temp_instr: instr for temp_instruments, instruments in zip(temp_instrumentss, instrumentss)
```

### Comparing `musiclang-0.8.9/musiclang/predict/composer/composer.py` & `musiclang-0.9.0/musiclang/predict/composer/composer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/predict/composer/harmony.py` & `musiclang-0.9.0/musiclang/predict/composer/harmony.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/predict/predictors/windowed.py` & `musiclang-0.9.0/musiclang/predict/predictors/windowed.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/predict/tokenizers/chord_tokenizer.py` & `musiclang-0.9.0/musiclang/predict/tokenizers/chord_tokenizer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/__init__.py` & `musiclang-0.9.0/musiclang/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/base_transformer.py` & `musiclang-0.9.0/musiclang/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/chord/basics.py` & `musiclang-0.9.0/musiclang/transform/chord/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/composing/arrange.py` & `musiclang-0.9.0/musiclang/transform/composing/arrange.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/composing/counterpoint.py` & `musiclang-0.9.0/musiclang/transform/composing/counterpoint.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/composing/layer.py` & `musiclang-0.9.0/musiclang/transform/composing/layer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/composing/pattern.py` & `musiclang-0.9.0/musiclang/transform/composing/pattern.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/composing/patternator.py` & `musiclang-0.9.0/musiclang/transform/composing/patternator.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/composing/project.py` & `musiclang-0.9.0/musiclang/transform/composing/project.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/composing/voice_leading.py` & `musiclang-0.9.0/musiclang/transform/composing/voice_leading.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     It has automatically solved the parallel dissonnance issue.
     """
 
     TYPES = ['b', 'c', 's', 'h']
     RULES = Rules
 
-    def __init__(self, types=None, rules=None, exclude_rules=None, fixed_voices=None, change_octave_fixed=True, seed=None, method='voices_and_rules', **kwargs):
+    def __init__(self, types=None, rules=None, exclude_rules=None, fixed_voices=None, change_octave_fixed=True, seed=34, method='voices_and_rules', **kwargs):
         """
 
         Parameters
         ----------
         types: None or list[str], default will be ['b', 'c', 's', 'h']
             List of types on which to apply the algorithm, if not present the notes will act as fixed voices
         rules: list of str in ALL_RULES
@@ -262,15 +262,15 @@
     def random_optim(self, dvals, max_iter=250, max_norm=3, **kwargs):
         solutions = [dvals + self.rg.randint(-max_norm, max_norm + 1, dvals.shape) for i in range(max_iter - 1)]
         solutions.append(dvals)
         scores = [self.eval_solution(sol) for sol in solutions]
         best = np.argmin(scores)
         return solutions[best]
 
-    def voices_optim(self, dvals, max_iter=1000, max_norm=3, temperature=8, min_temperature=1, **kwargs):
+    def voices_optim(self, dvals, max_iter=100, max_norm=3, temperature=8, min_temperature=1, **kwargs):
         min_score = self.eval_solution(dvals)
         start_temp = temperature
         end_temp = min_temperature
         for it in range(max_iter):
             pitches = self.get_pitch_solution(dvals)
             mov = self.get_movement(pitches).astype(np.float32)  # Find movements
             mov *= self.dvalsmask[:, :-1]
@@ -291,15 +291,15 @@
                 dvals = proposed_sol
             coeff = (it / max_iter)
             temperature = coeff * end_temp + (1 - coeff) * start_temp
         return dvals
         # Move in direction of sgn
 
 
-    def optimize_rules(self, dvals, max_iter_rules=200, max_norm_rules=1, temperature=1, **kwargs):
+    def optimize_rules(self, dvals, max_iter_rules=100, max_norm_rules=1, temperature=1, **kwargs):
 
         def eval_solution(dvals):
             pitches = self.get_pitch_solution(dvals)
             problems = self.get_problems(pitches)
             return np.sum(problems)
 
         pitches = self.get_pitch_solution(dvals)
```

### Comparing `musiclang-0.8.9/musiclang/transform/dynamics/dynamizer.py` & `musiclang-0.9.0/musiclang/transform/dynamics/dynamizer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/features/basics.py` & `musiclang-0.9.0/musiclang/transform/features/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/graph.py` & `musiclang-0.9.0/musiclang/transform/graph.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/library.py` & `musiclang-0.9.0/musiclang/transform/library.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/mask.py` & `musiclang-0.9.0/musiclang/transform/mask.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/melody/basics.py` & `musiclang-0.9.0/musiclang/transform/melody/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/melody/continuation.py` & `musiclang-0.9.0/musiclang/transform/melody/continuation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/note/basics.py` & `musiclang-0.9.0/musiclang/transform/note/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/orchestrations/epic.py` & `musiclang-0.9.0/musiclang/transform/orchestrations/epic.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/orchestrations/nocturne.py` & `musiclang-0.9.0/musiclang/transform/orchestrations/nocturne.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/pipeline.py` & `musiclang-0.9.0/musiclang/transform/pipeline.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/score_merger/basics.py` & `musiclang-0.9.0/musiclang/transform/score_merger/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/structure_graphs/forms.py` & `musiclang-0.9.0/musiclang/transform/structure_graphs/forms.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/transformer.py` & `musiclang-0.9.0/musiclang/transform/transformer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/transform/utils_random.py` & `musiclang-0.9.0/musiclang/transform/utils_random.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/arrange_utils/arrange_utils.py` & `musiclang-0.9.0/musiclang/write/arrange_utils/arrange_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/arrange_utils/skyline_algorithm.py` & `musiclang-0.9.0/musiclang/write/arrange_utils/skyline_algorithm.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/chord.py` & `musiclang-0.9.0/musiclang/write/chord.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2023, Florian GARDIN
 All rights reserved.
 
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
+from functools import cached_property
 
 from .constants import *
 import re
 
 class Chord:
     """
     Represents a chord in MusicLang.
@@ -367,15 +368,15 @@
         if not note.is_note:
             return None
         return note_to_pitch_result(note, self, last_pitch=last_pitch)
 
     def to_absolute_note(self):
         return self(**{part: melody.to_absolute_note(self) for part, melody in self.score.items()})
 
-    @property
+    @cached_property
     def bass_pitch(self):
         return self.chord_extension_pitches[0]
 
     def to_sequence(self):
         """
         See :func:`~Score.to_sequence()
         """
@@ -402,48 +403,48 @@
         return self.to_score().to_musicxml(*args, **kwargs)
 
 
     def to_music21(self, *args, **kwargs):
         return self.to_score().to_music21(*args, **kwargs)
 
 
-    @property
+    @cached_property
     def scale_degree(self):
         """
 
         Returns
         -------
 
         """
         tonic = self.scale_pitches[0]
         return DEGREE_TO_SCALE_DEGREE[tonic % 12] + tonic // 12
 
-    @property
+    @cached_property
     def pitch_set(self):
         """
         Get a frozenset of :func:`~Chord.chord_pitches`
         """
         return frozenset({s % 12 for s in self.chord_pitches})
 
     @property
     def pitch_dict(self):
         chromatic_dict = {self.to_pitch(note): note for note in self.chromatic_scale_notes}
         diatonic_dict = {self.to_pitch(note): note for note in self.scale_notes}
 
         return {**chromatic_dict, **diatonic_dict}
 
 
-    @property
+    @cached_property
     def scale_set(self):
         """
         Get a frozenset of :func:`~Chord.scale_pitches`
         """
         return frozenset({s % 12 for s in self.scale_pitches})
 
-    @property
+    @cached_property
     def chord_pitches(self):
         """
         Get the chord absolute pitches (integers) starting with the chord root.
 
         See Also
         --------
         :func:`~Tonality.scale_pitches`
@@ -526,18 +527,18 @@
             return self.scale_pitches
         elif type == "b":
             return self.chord_extension_pitches
         elif type == "c":
             return self.chord_pitches
         else:
             raise ValueError("This type is not associated to a scale")
-    @property
+    @cached_property
     def chromatic_pitches(self):
         return [self.scale_pitches[0] + i for i in range(12)]
-    @property
+    @cached_property
     def scale_pitches(self):
         """
         Get the scale absolute pitches (integers) starting with the chord root.
 
         See Also
         --------
         :func:`~Tonality.scale_pitches`
@@ -561,20 +562,20 @@
         tonality_scale_pitches = self.tonality.scale_pitches
         start_idx = self.element
         scale_pitches = tonality_scale_pitches[start_idx:] + [t + 12 for t in tonality_scale_pitches[:start_idx]]
         scale_pitches = [n + 12 * self.octave for n in scale_pitches]
         return scale_pitches
 
 
-    @property
+    @cached_property
     def chromatic_scale_pitches(self):
         """ """
         return [self.scale_pitches[0] + i for i in range(12)]
 
-    @property
+    @cached_property
     def chord_extension_pitches(self):
         """
         Get the chord absolute pitches (integers) starting with the chord bass as indicated by the extension.
 
         See Also
         --------
         :func:`~Tonality.chord_pitches`
@@ -1045,15 +1046,15 @@
                  nb_excluded_instruments=0,
                  fixed_bass=True,
                  voice_leading=True,
                  melody=False,
                  instruments=None,
                  voicing=None,
                  add_metadata=True,
-                   max_duration=16,
+                   max_duration=32,
                    **kwargs):
         """
         Extract the pattern from the chord
 
         Parameters
         ----------
         nb_excluded_instruments: int (Default value = 0)
@@ -1095,19 +1096,24 @@
         if add_metadata:
             from musiclang.analyze.pattern_analyzer import PatternFeatureExtractor
             dict_pattern = PatternFeatureExtractor().extract(dict_pattern,
                                                              self,
                                                              melody=melody,
                                                              nb_excluded_instruments=nb_excluded_instruments,
                                                              )
+        dict_pattern['multi_chord'] = False
         return dict_pattern, pattern
 
     def project_pattern(self, score, restart_each_chord=False):
         return self.to_score().project_pattern(score, restart_each_chord=restart_each_chord)
 
+    def remove_drums(self):
+        return self(**{ins: val for ins, val in self.score.items() if not ins.startswith('drums')})
+
+
     def o(self, octave):
         """Chord up or down the amount of octave in parameter, it will change the chord octave, not the melody
 
         Parameters
         ----------
         octave :
             return:
@@ -1317,14 +1323,44 @@
     def __repr__(self):
         return f"{self.to_code()}({self.melody_to_str()})"
 
     @property
     def full_octave(self):
         return self.octave + self.tonality.octave
 
+
+    def replace_instruments_names(self, **instruments_dict):
+        """
+        Replace any instrument with another (use part name (eg: piano__0)
+
+        Parameters
+        ----------
+        instruments_dict: dict[str, str]
+            Dictionary of parts name to replace
+
+        Returns
+        -------
+        chord: Chord
+
+        """
+        new_chord_dict = {}
+        idx_instruments = {}
+        instruments = sorted(self.score.keys(), key=lambda x: (x.split('__')[0], int(x.split('__')[1])))
+        for ins in instruments:
+            name, idx = ins.split('__')
+            idx = int(idx)
+            new_name = instruments_dict.get(name, name)
+            if new_name not in idx_instruments.keys():
+                idx_instruments[new_name] = -1
+            chosen_idx = idx_instruments[new_name] + 1 if idx <= idx_instruments[new_name] else idx
+            new_chord_dict[new_name + '__' + str(chosen_idx)] = self.score[ins]
+            idx_instruments[new_name] = max(idx, idx_instruments[new_name])
+
+        return self(**new_chord_dict)
+
     def replace_instruments(self, **instruments_dict):
         """
         Replace any instrument with another (use full part name (eg: piano__0)
 
         Parameters
         ----------
         instruments_dict: dict[str, str]
```

### Comparing `musiclang-0.8.9/musiclang/write/constants.py` & `musiclang-0.9.0/musiclang/write/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/element.py` & `musiclang-0.9.0/musiclang/write/element.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/elements/chord.py` & `musiclang-0.9.0/musiclang/write/elements/chord.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/library.py` & `musiclang-0.9.0/musiclang/write/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,26 @@
 x5 = Note('x', 5, 0, 1)
 x6 = Note('x', 6, 0, 1)
 x7 = Note('x', 7, 0, 1)
 x8 = Note('x', 8, 0, 1)
 x9 = Note('x', 9, 0, 1)
 x10 = Note('x', 10, 0, 1)
 x11 = Note('x', 11, 0, 1)
+x12 = Note('x', 12, 0, 1)
+x13 = Note('x', 13, 0, 1)
+x14 = Note('x', 14, 0, 1)
+x15 = Note('x', 15, 0, 1)
+x16 = Note('x', 16, 0, 1)
+x17 = Note('x', 17, 0, 1)
+x18 = Note('x', 18, 0, 1)
+x19 = Note('x', 19, 0, 1)
+x20 = Note('x', 20, 0, 1)
+x21 = Note('x', 21, 0, 1)
+x22 = Note('x', 22, 0, 1)
+
 
 
 bdd = Note('d', 11, -3, 1)  # bassdrum
 bd = Note('d', 0, -2, 1)  # bassdrum
 rs = Note('d', 1, -2, 1)     # rimshot
 sn = Note('d', 2, -2, 1)  # Snare drum 1
 cp = Note('d', 3, -2, 1)   # Clap
@@ -157,14 +169,27 @@
 hh = Note('d', 6, -2, 1)  # Bass tom
 lt = Note('d', 7, -2, 1)  # Low tom
 ch = Note('d', 8, -2, 1)  # Closed hat
 mt = Note('d', 9, -2, 1)  # Medium tom
 oh = Note('d', 10, -2, 1)  # Open hat
 ht = Note('d', 11, -2, 1)  # High tom
 
+d0 = Note('d', 0, 0, 1)
+d1 = Note('d', 1, 0, 1)
+d2 = Note('d', 2, 0, 1)
+d3 = Note('d', 3, 0, 1)
+d4 = Note('d', 4, 0, 1)
+d5 = Note('d', 5, 0, 1)
+d6 = Note('d', 6, 0, 1)
+d7 = Note('d', 7, 0, 1)
+d8 = Note('d', 8, 0, 1)
+d9 = Note('d', 9, 0, 1)
+d10 = Note('d', 10, 0, 1)
+d11 = Note('d', 11, 0, 1)
+
 hht = Note('d', 0, -1, 1)
 crash = Note('d', 1, -1, 1)
 other_hht = Note('d', 2, -1, 1)
 ride = Note('d', 3, -1, 1)
 ride_hard = Note('d', 4, -1, 1)
 dr050 = Note('d', 5, -1, 1)
 dr060 = Note('d', 6, -1, 1)
```

### Comparing `musiclang-0.8.9/musiclang/write/melody.py` & `musiclang-0.9.0/musiclang/write/melody.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/note.py` & `musiclang-0.9.0/musiclang/write/note.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 All rights reserved.
 
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
 
 from .constants import *
-
+LIMIT_DENOM = int(1e4)
 
 class Note:
     """
     Represents a note in MusicLang.
 
     **The specificity of MusicLang is that notes are always represented relatively to a chord inside a tonality.**
 
@@ -123,15 +123,15 @@
     """
     DEFAULT_AMP = 66
 
     def __init__(self, type, val, octave, duration, mode=None, accident=None, amp=DEFAULT_AMP, tags=None, pedal=None, tempo=None):
         self.type = type
         self.val = val
         self.octave = octave
-        self.duration = duration
+        self.duration = frac(duration).limit_denominator(LIMIT_DENOM)
         self.amp = amp
         self.accident = accident
         self.mode = mode
         self.properties = self.init_properties()
         self.tags = tags if tags is not None else set()
         self.pedal = pedal
         self.tempo = tempo
@@ -470,19 +470,20 @@
 
 
         Returns
         -------
 
         """
         if isinstance(value, float):
-            value = frac(value).limit_denominator(8)
+            value = frac(value).limit_denominator(LIMIT_DENOM)
         elif isinstance(value, int):
             value = frac(value, 1)
         result = self.copy()
         result.duration = value
+        result.duration = result.duration.limit_denominator(LIMIT_DENOM)
         return result
 
     def augment(self, value):
         """
         Returns a copy with augmented duration (multiply current duration by the value)
 
         Parameters
@@ -502,19 +503,20 @@
         >>> from musiclang.library import s0
         >>> from fractions import Fraction
         >>> s0.augment(Fraction(8, 7))
         s0.augment(frac(8, 7))
 
         """
         if isinstance(value, float):
-            value = frac(value).limit_denominator(8)
+            value = frac(value).limit_denominator(LIMIT_DENOM)
         if isinstance(value, int):
             value = frac(value, 1)
         result = self.copy()
         result.duration *= value
+        result.duration = result.duration.limit_denominator(LIMIT_DENOM)
         return result
 
     def change_type(self, new_type):
         """
 
         Parameters
         ----------
@@ -686,15 +688,17 @@
         A string representation of the note valid using standard musiclang library
 
         """
 
         if self.is_note:
             result = f"{self.type}{self.val}"
         elif self.is_drum:
-            result = DRUMS_DICT.get((self.val, self.octave), 'r')
+            result = f'd{self.val}'
+            if self.octave != 0:
+                result += f".oabs({self.octave})"
         elif self.type == 'x':
             result = f"{self.type}{self.val}"
         else:
             result = f"{self.type}"
 
         if self.duration != Q:
             if self.duration in DURATION_TO_STR:
```

### Comparing `musiclang-0.8.9/musiclang/write/note_pitch.py` & `musiclang-0.9.0/musiclang/write/note_pitch.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/ornementation.py` & `musiclang-0.9.0/musiclang/write/ornementation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/out/constants.py` & `musiclang-0.9.0/musiclang/write/out/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "accordion": 21,
     "harmonica": 22,
     "tango_accordion": 23,
     "acoustic_guitar": 24,
     "steel_guitar": 25,
     "jazz_guitar": 26,
     "clean_guitar": 27,
+    "muted_guitar": 28,
     "overdriven_guitar": 29,
     "distortion_guitar": 30,
     "harmonic_guitar": 31,
     "acoustic_bass": 32,
     "electric_bass_finger": 33,
     "electric_bass_pick": 34,
     "fretless_bass": 35,
```

### Comparing `musiclang-0.8.9/musiclang/write/out/midi_utils.py` & `musiclang-0.9.0/musiclang/write/out/midi_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 All rights reserved.
 
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
 
 import numpy as np
+import mido
 
 def voice_to_channel(instrument_list, voice, instruments):
     """
 
     Parameters
     ----------
     instrument_list :
@@ -27,29 +28,30 @@
     instrument_of_voice = instruments.get(voice, 0)
     return instrument_list.index(instrument_of_voice)
 
 
 
 def matrix_to_events(matrix, 
                      output_file=None, 
-                     ticks_per_beat=480, 
+                     ticks_per_beat=384,
                      tempo=120, 
                      instruments={}, 
                      time_signature=(4, 4),
                      instrument_names=None):
     matrix = np.asarray(matrix)
     events = [] # [(time, instrument, duration, message)]
     for el in matrix:
         pitch, offset, duration, velocity, track, silence, continuation, tempo, pedal = el
         # Add note on, note off for each track
 
     return events
 
 def matrix_to_mid(matrix, output_file=None, ticks_per_beat=480, tempo=120, instruments={}, time_signature=(4, 4),
-                  instrument_names=None, **kwargs):
+                  anachrusis_time=0,
+                  instrument_names=None, one_track_per_instrument=False, **kwargs):
     """
 
     Parameters
     ----------
     matrix :
         
     output_file :
@@ -71,14 +73,34 @@
         instrument_names = []
     from mido import MidiFile, MidiTrack, Message, MetaMessage
     from ..constants import SILENCE, CONTINUATION, PITCH, TRACK, OFFSET, VELOCITY, DURATION, TEMPO, PEDAL
     from .constants import OCTAVES
     import os
 
     matrix = np.asarray(matrix)
+
+
+    #
+
+    if one_track_per_instrument:
+        # instrument
+        instrument_group = {}
+        for track_nb, program in instruments.items():
+            instrument_group[program] = instrument_group.get(program, []) + [track_nb]
+
+        # Change the tracks associated to each instrument
+        instruments = {i: program for i, program in enumerate(instrument_group.keys())}
+        invert_instruments = {program: i for i, program in instruments.items()}
+
+        # Associate each track to the right new track
+        for program, tracks in instrument_group.items():
+            for i, track in enumerate(tracks):
+                matrix[matrix[:, TRACK] == track, TRACK] = invert_instruments[program]
+
+
     def number_to_channel(n):
         """
 
         Parameters
         ----------
         n :
             
@@ -92,14 +114,17 @@
         if n >= 9:
             return n + 1
 
     mid = MidiFile()
     mid.ticks_per_beat = ticks_per_beat
     mid.type = 1
 
+    bar_duration = time_signature[0] * 4 / time_signature[1]
+    start_time = (-anachrusis_time) % bar_duration
+    matrix[:, OFFSET] = matrix[:, OFFSET] + start_time
     # Take care of continuation
     # matrix = matrix[(matrix['pitch'] > 0) | (matrix['continuation'] > 0)]
     # Remove all continuations that follows a silence
     # Put all instruments with same name in same track
     # For each voice assign right track
     instrument_list = list(sorted(list(set([0] + list(instruments.values())))))
     # Replace with track in matrix
@@ -120,15 +145,15 @@
             track.append(Message('program_change', program=0, time=0, channel=channels[i]))
         mid.tracks.append(track)
 
     if isinstance(output_file, str):
         mid.tracks[0].append(MetaMessage("track_name", name=os.path.split(output_file)[1], time=int(0)))
     else:
         mid.tracks[0].append(MetaMessage("track_name", name='track', time=int(0)))
-    mid.tracks[0].append(MetaMessage("set_tempo", tempo=(480000 * 120) // tempo, time=int(0)))
+    mid.tracks[0].append(MetaMessage("set_tempo", tempo=mido.bpm2tempo(tempo), time=int(0)))
     mid.tracks[0].append(MetaMessage("time_signature", numerator=time_signature[0], denominator=time_signature[1], time=int(0)))
 
 
 
     sort_events = []
     last_silence = True
     for row in matrix:
```

### Comparing `musiclang-0.8.9/musiclang/write/out/to_code.py` & `musiclang-0.9.0/musiclang/write/out/to_code.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/out/to_midi.py` & `musiclang-0.9.0/musiclang/write/out/to_midi.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/out/to_mxl.py` & `musiclang-0.9.0/musiclang/write/out/to_mxl.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/pitches/pitches_utils.py` & `musiclang-0.9.0/musiclang/write/pitches/pitches_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     """
     scale_mod = list(sorted([i % 12 for i in scale_pitches]))
     # Get scale index
     if delta == 0:
         new_pitch = last_pitch
     else:
-        whole_scale = [s + octave * 12 for octave in range(-7, 7) for s in scale_mod]
+        whole_scale = [s + octave * 12 for octave in range(-10, 10) for s in scale_mod]
         dists = np.asarray(whole_scale) - last_pitch
         dists = dists[dists >= 0] + last_pitch
         new_pitch = dists[delta - 1 * (last_pitch not in whole_scale)]
 
     return new_pitch
 
 
@@ -51,15 +51,15 @@
 
     """
     scale_mod = list(sorted([i % 12 for i in scale_pitches]))
     # Get scale index
     if delta == 0:
         new_pitch = last_pitch
     else:
-        whole_scale = [s + octave * 12 for octave in range(-7, 7) for s in scale_mod]
+        whole_scale = [s + octave * 12 for octave in range(-10, 10) for s in scale_mod]
         dists = np.asarray(whole_scale) - last_pitch
         dists = dists[dists <= 0] + last_pitch
         new_pitch = dists[-(delta + 1) + 1 * (last_pitch not in whole_scale)]
     return new_pitch
 
 
 def get_relative_scale_value(note, last_pitch, scale_pitches):
```

### Comparing `musiclang-0.8.9/musiclang/write/properties/note_properties.py` & `musiclang-0.9.0/musiclang/write/properties/note_properties.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/rhythm/metric.py` & `musiclang-0.9.0/musiclang/write/rhythm/metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/rhythm/score_rythm.py` & `musiclang-0.9.0/musiclang/write/rhythm/score_rythm.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/rhythm/utils_metric.py` & `musiclang-0.9.0/musiclang/write/rhythm/utils_metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/score.py` & `musiclang-0.9.0/musiclang/write/score.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,24 +235,24 @@
 
         Returns
         -------
         score: Score
         Normalize score
         """
         from musiclang import Silence
-        score = None
+        score = []
         instruments = set(self.instruments)
         for chord_raw in self.chords:
             chord = chord_raw.copy()
             missing_instruments = set(instruments) - set(chord.instruments)
             chord_score = chord.score
             for instrument in missing_instruments:
                 chord_score[instrument] = Silence(chord.duration)
-            score += chord(**chord_score)
-        return score
+            score.append(chord(**chord_score))
+        return Score(score)
 
     def remove_silenced_instruments(self):
         """
         Inverse operation of :func:`~Score.normalize_instruments`
         For each chord remove all instruments that are silenced
         Returns
         -------
@@ -268,38 +268,80 @@
                 if all([n.type == 'r' for n in chord_score[instrument]]):
                     del chord_score[instrument]
 
             chords.append(chord(**chord_score))
 
         return sum(chords, None)
 
+    def normalize_instrument_names(self):
+        """
+        Normalize the instrument idx for all instrument.
+        The first voice of an instrument encountered will always have idx 0, the second idx 1, etc...
+        Returns
+        -------
+        score: Score
+        """
+
+        instruments = self.instruments
+
+        replace_dic = {}
+        replace_dic_ins = {}
+        for ins in instruments:
+            name, idx = '__'.join(ins.split('__')[:-1]), ins.split('__')[-1]
+            replace_dic_ins[name] = replace_dic_ins.get(name, -1) + 1
+            replace_dic[ins] = name + '__' + str(replace_dic_ins[name])
+
+        score = self.replace_instruments(**replace_dic)
+        return score
+
     def replace_instruments(self, **instruments_dict):
         """
         Replace any instrument with another (use full part name (eg: piano__0)
 
         Parameters
         ----------
         instruments_dict: dict[str, str]
             Dictionary of parts name to replace
 
         Returns
         -------
         score: Score
 
         """
-        score = None
+        score = []
         instruments_dict = {key: instruments_dict[key] if key in instruments_dict.keys() else key for key in self.parts}
         for chord in self.chords:
             new_chord_dict = {}
             for ins_name, new_ins_name in instruments_dict.items():
                 if ins_name in chord.score.keys():
                     new_chord_dict[new_ins_name] = chord.score[ins_name]
-            score += chord(**new_chord_dict)
+            score.append(chord(**new_chord_dict))
 
-        return score
+        return Score(score)
+
+
+    def replace_instruments_names(self, **instruments_dict):
+        """
+        Replace any instrument name with another (use only instrument name (eg: piano)
+
+        Parameters
+        ----------
+        instruments_dict: dict[str, str]
+            Dictionary of parts name to replace
+
+        Returns
+        -------
+        score: Score
+
+        """
+        score = []
+        for chord in self.chords:
+            score.append(chord.replace_instruments_names(**instruments_dict))
+
+        return Score(score)
 
 
     def clean(self):
         return self.to_drum().decompose_duration()
 
     def to_drum(self):
         return Score([chord.to_drum() for chord in self.chords], tags=set(self.tags))
@@ -381,48 +423,61 @@
 
         Returns
         -------
         type
             :return:
 
         """
+
+        def f7(seq):
+            seen = set()
+            seen_add = seen.add
+            return [x for x in seq if not (x in seen or seen_add(x))]
+
         result = []
         for chord in self:
             insts = list(chord.score.keys())
             result += insts
-            result = list(set(result))
-
-        return list(sorted(result, key=lambda x: (x.split('__')[0], int(x.split('__')[1]))))
+            result = f7(result)
+        return result
 
 
     def normalize(self):
         """
         Normalize the score to be standardized for the language model
         - Normalize instruments in each chord
         - Convert relative notes to real notes
         - Correct chord octaves to minimize distance with central C
         FIXME : Relative notes should be converted first
 
         Returns
         -------
         score: Score
         """
+        import time
+        start = time.time()
         score = self.to_standard_note()
         score = score.correct_chord_octave()
+        score = score.normalize_instrument_names()
         score = score.split_too_long_chords(8)
+        #score = score.remove_drums()
+        score = score.remove_empty_chords()
         return score
 
+    def remove_empty_chords(self):
+        return Score([c for c in self.chords if c.duration > 0])
+
     def correct_chord_octave(self):
         """
         Correct chord octaves to minimize distance with central C
         Returns
         -------
         score: Score
         """
-        return sum([c.correct_chord_octave() for c in self.chords], None)
+        return Score([c.correct_chord_octave() for c in self.chords])
 
     def octaver(self, **instruments_octaves):
         """
         Transpose down octave per instrument
 
 
         Parameters
@@ -734,21 +789,21 @@
         Returns
         -------
         score: Score
             The score with shorter chords
 
         """
 
-        new_score = None
+        new_score = []
         for chord in self:
             if chord.duration > max_length:
-                new_score += chord.split(max_length)
+                new_score += (chord.split(max_length)).chords
             else:
-                new_score += chord
-        return new_score
+                new_score.append(chord)
+        return Score(new_score)
 
     def to_text_file(self, filepath, create_dir=False):
         """
         Save as a musiclang txt file
         Parameters
         ----------
         filepath
@@ -778,14 +833,54 @@
         """
         from musiclang import PartComposer
         score = PartComposer.compose(data)
         return score
 
 
 
+    def patternize(self,
+                   **kwargs):
+        """
+        Extract the pattern from the chord
+
+        Parameters
+        ----------
+        nb_excluded_instruments: int (Default value = 0)
+            Number of instruments to exclude from the pattern
+        fixed_bass: bool (Default value = True)
+            If True, the bass will be fixed in the pattern response
+        voice_leading: bool (Default value = True)
+            If True, the voice leading will be applied in the pattern response
+        melody: bool (Default value = False)
+            Do you want to extract a melody or an accompaniment pattern
+        instruments: list[str] (Default value = None)
+            List of instruments to use for the pattern
+        voicing: list[Note] or None (Default value = None)
+            Voicing to use for the pattern, otherwise extract the good one
+        add_metadata: bool (Default value = True)
+            If True, add metadata and features to the pattern
+        Returns
+        -------
+        score_pattern: Chord
+            Patternized chord or score
+        pattern: dict
+            Pattern data of the score
+
+        """
+        # Project all on same chord
+        first_chord = self.chords[0].to_chord().augment(self.duration)
+        one_chord_score = self.project_on_score(first_chord, voice_leading=False)
+        chord = one_chord_score.chords[0]
+        pattern, score_pattern = chord.patternize(**kwargs)
+        pattern['chords'] = [str(chord.to_chord()(r.augment(chord.duration))) for chord in self.chords]
+        pattern['multi_chord'] = True
+        return pattern, score_pattern
+
+
+
     def get_patterns(self, nb_excluded_instruments=0, **kwargs):
         metadata_base = {
             "tempo": self.config['tempo']
         }
         metadata_base = {**metadata_base, **kwargs}
         data = []
         patterns = []
@@ -918,26 +1013,26 @@
         return get_chord_between(chord, start, end)
 
     @property
     def pedal_each_chord(self):
         return Score([c.pedal for c in self.chords], tags=set(self.tags))
 
     def doubling(self, **args):
-        new_score = None
+        new_score = []
         for chord in self.chords:
             score = chord.copy().score
             for part, new_parts in args.items():
                 if isinstance(new_parts, str):
                     new_parts = [new_parts]
                 for new_part in new_parts:
                     if part in score.keys():
                         score[new_part] = score[part].copy()
-            new_score += chord(**score)
+            new_score.append(chord(**score))
 
-        return new_score
+        return Score(new_score)
 
     def get_score_between(self, start=None, end=None):
         """
         Get the score between start and end time.
 
         Parameters
         ----------
@@ -998,15 +1093,15 @@
     @classmethod
     def from_annotation(cls, text):
         from musiclang.analyze import ScoreFormatter
         return ScoreFormatter(text).parse()
 
 
     @classmethod
-    def from_midi(cls, filename):
+    def from_midi(cls, filename, fast_chord_inference=True):
         """
         Load a midi score into musiclang
 
         .. warning:: This step can take some time depending on the length of the file
 
         Parameters
         ----------
@@ -1016,32 +1111,31 @@
         Returns
         -------
         score: Score
                The loaded score
 
         """
         from musiclang.analyze import parse_to_musiclang
-        score, config = parse_to_musiclang(filename)
+        score, config = parse_to_musiclang(filename, fast_chord_inference=fast_chord_inference)
         real_config = {**score.config, **config}
-        score = score.normalize()
         score.config = real_config
         return score
 
     def to_extension_note(self):
         return Score([chord.to_extension_note() for chord in self.chords], tags=set(self.tags))
 
     def to_chord_note(self):
         return Score([chord.to_chord_note() for chord in self.chords], tags=set(self.tags))
 
     def to_standard_note(self):
         return Score([chord.to_standard_note() for chord in self.chords], tags=set(self.tags))
 
 
     @classmethod
-    def from_xml(cls, filename):
+    def from_xml(cls, filename, fast_chord_inference=False):
         """
         Load a musicxml score into musiclang
 
         .. warning:: This step can take some time depending on the length of the file
 
 
         Parameters
@@ -1054,15 +1148,15 @@
         -------
 
         score: Score
                The loaded score
 
         """
         from musiclang.analyze import parse_to_musiclang
-        score, config = parse_to_musiclang(filename)
+        score, config = parse_to_musiclang(filename, fast_chord_inference=fast_chord_inference)
         score.config.update(config)
         return score
 
     def decompose_duration(self):
         """
         Decompose the duration in a note + continuations. It recursively call
         :func:`~Note.decompose_duration()`
@@ -1166,14 +1260,17 @@
             return Score([c % other for c in self.chords], config=self.config.copy(), tags=self.tags)
         else:
             raise Exception('Following % should be a Tonality')
 
     def remove_accidents(self):
         return Score([chord.remove_accidents() for chord in self.chords], tags=set(self.tags))
 
+    def remove_drums(self):
+        return Score([chord.remove_drums() for chord in self.chords])
+
 
     def __mul__(self, other):
         """
         If other is Integer, repeat the note other times
         """
         if isinstance(other, int):
             return sum([self.copy() for i in range(other)], None)
```

### Comparing `musiclang-0.8.9/musiclang/write/sequence/sequence.py` & `musiclang-0.9.0/musiclang/write/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/sequence/sequence_utils.py` & `musiclang-0.9.0/musiclang/write/sequence/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang/write/time_utils/time_utils.py` & `musiclang-0.9.0/musiclang/write/time_utils/time_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Copyright (c) 2023, Florian GARDIN
 All rights reserved.
 
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
+from musiclang import Melody
+
 
 def put_on_same_chord(score):
     """Take the first chord as reference,
     Put everything into the first chord preserving the note value (It will change the piece to a static harmony)
 
     Parameters
     ----------
@@ -101,15 +103,15 @@
         chord, Chord, modified chord
 
     """
     new_parts = {ins: None for ins in chord.instruments}
     for part in chord.score.keys():
         time = 0
         voice = chord.score[part]
-        new_voice = None
+        new_voice = []
         to_break = False
         for note in voice:
             add_continuation = False
             note_duration = note.duration
             new_note = note.copy()
             if time >= end:
                 break
@@ -122,29 +124,28 @@
             if time < start:
                 new_note.duration = new_note.duration - (start - time)
                 time += start - time
                 add_continuation = True
 
             if add_continuation:
                 from ..note import Continuation
-                new_voice += Continuation(new_note.duration)
+                new_voice.append(Continuation(new_note.duration))
             else:
-                new_voice += new_note
+                new_voice.append(new_note)
 
 
             if new_note.duration < 0:
                 raise Exception('Get a negative duration in get_chord_between')
-            if new_voice.duration > end - start:
-                raise Exception('New voice duration should never be more than boundaries')
+
 
             time += new_note.duration
 
             if to_break:
                 break
-
+        new_voice = Melody(new_voice)
         new_parts[part] = new_voice
 
     if len(new_parts.keys()) == 0:
         from ..note import Silence
         return chord(**{'piano__0': Silence(end - start)})
         # if new_voice.duration != chord.duration:
         #    from pdb import set_trace; set_trace()
```

### Comparing `musiclang-0.8.9/musiclang/write/tonality.py` & `musiclang-0.9.0/musiclang/write/tonality.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/musiclang.egg-info/PKG-INFO` & `musiclang-0.9.0/musiclang.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,139 +1,157 @@
 Metadata-Version: 2.1
 Name: musiclang
-Version: 0.8.9
+Version: 0.9.0
 Summary: A python package for music notation and generation
-Home-page: UNKNOWN
 Author: Florian GARDIN
-Author-email: fgardin.pro@gmail.com
-License: UNKNOWN
-Project-URL: Documentation, https://musiclang.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/MusicLang/musiclang/
-Project-URL: Tracker, https://github.com/MusicLang/musiclang/issues
-Description: Musiclang
-        =========
+Author-email: Florian GARDIN <fgardin.pro@gmail.com>
+License: BSD 2-Clause License
         
-        ![MusicLang logo](https://github.com/MusicLang/musiclang/blob/main/documentation/images/MusicLang.png?raw=true "MusicLang")
+        Copyright (c) 2023, Florian GARDIN
         
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
         
-        [![Documentation Status](https://readthedocs.org/projects/musiclang/badge/?version=latest)](https://musiclang.readthedocs.io/en/latest/?badge=latest)
-        
-        The Python framework to write, analyze, transform and predict music.
-        
-        
-        What is MusicLang ?
-        --------------------
-        
-        MusicLang which simply stands for "music language" is a Python framework
-        that allows composers to write symbolic music in a condensed and high level manner.
-        It can be used to write, arrange, transform or predict new music.
-        This framework is not only another notation software but also
-        an assistant that is able to automate some tasks that would normally be tedious for a composer.
-        It is naturally good at analyzing and manipulating existing
-        pieces of music in musicxml or midi format.
-        
-        [Read our documentation](https://musiclang.readthedocs.io/en/latest).
-        
-        
-        How to install
-        --------------
-        
-        MusicLang is available on Pypi :
-        
-        ```
-        pip install musiclang
-        ```
-        
-        Or use this repo for the latest version :
-        
-        ```
-        pip install git+https://github.com/MusicLang/musiclang
-        ```
-            
-        
-        Examples
-        ---------
-        
-        1. A hello world example to create a C-major chord in musiclang and save it to midi :
-        
-        ```python
-        from musiclang.library import *
-        
-        # Write A C major chord
-        score = (I % I.M)(piano=[s0, s2, s4])
-        
-        # Store it to midi
-        score.to_midi('c_major.mid')
-        ```
-        
-        2. Create, transform and harmonize a theme quickly : 
-        
-        ```python
-        from musiclang.library import *
-        
-        # Create a cool melody (the beginning of happy birthday, independant of any harmonic context)
-        melody = s4.ed + s4.s + s5 + s4 + s0.o(1) + s6.h
-        
-        # Create a simple accompaniment with a cello and a oboe
-        acc_melody = r + s0.o(-1).q * 3 + s0.o(-1).h
-        accomp = {'cello__0': acc_melody, 'oboe__0': acc_melody.o(1)}
-        
-        # Play it in F-major
-        score = (I % IV.M)(violin__0=melody, **accomp)
-        
-        # Repeat the score a second time in F-minor and forte
-        score += (score % I.m).f
-        
-        # Just to create an anachrusis at the first bar
-        score = (I % I.M)(violin__0=r.h) + score
-        
-        # Transform a bit the accompaniment by applying counterpoint rules automatically
-        from musiclang.transform.library import create_counterpoint_on_score
-        score = create_counterpoint_on_score(score, fixed_parts=['violin__0'])
-        
-        # Save it to musicxml
-        score.to_musicxml('happy_birthday.musicxml', signature=(3, 4), title='Happy birthday !')
-        
-        # Et voilà !
-        ```
-        ![Happy birthday score](https://github.com/MusicLang/musiclang/blob/main/documentation/images/happy_birthday.png?raw=true "Happy Birthday")
-        
-        
-        3. Predict a score using a deep learning model trained on musiclang language :
-        
-        ```python
-        from musiclang.library import *
-        from musiclang import Score
-        
-        # Some random bar of chopin op18 Waltz
-        score = ((V % III.b.M)(
-        	piano__0=s0 + s2.e.mp + s3.e.mp, 
-        	piano__4=s0.e.o(-2).p + r.e + s0.ed.o(-1).mp + r.s, 
-        	piano__5=r + s4.ed.o(-1).mp + r.s, 
-        	piano__6=r + s6.ed.o(-1).mp + r.s)+ 
-        (V['7'] % III.b.M)(
-        	piano__0=s2.ed.mp + r.s, 
-        	piano__2=s4.ed.mp + r.s, 
-        	piano__4=s6.ed.o(-1).mp + r.s, 
-        	piano__5=s0.ed.o(-1).mp + r.s, 
-        	piano__6=s4.ed.o(-1).mp + r.s))
-        
-        # Predict the next two chords of the score using huggingface musiclang model
-        predicted_score = score.predict_score(n_chords=2, temperature=0.5)
-        # Save it to midi
-        predicted_score.to_midi('test.mid')
-        ```
-        
-        Please note that this feature is still experimental, it will only work with
-        piano music for now and the model is not yet trained on a large corpus of music.
-        If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
-        
-        
-        4. Mix everything together to create a new pieces of music !
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Project-URL: Homepage, https://github.com/MusicLang/musiclang
+Keywords: music,ai,notation
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
+Musiclang
+=========
+
+![MusicLang logo](https://github.com/MusicLang/musiclang/blob/main/documentation/images/MusicLang.png?raw=true "MusicLang")
+
+
+[![Documentation Status](https://readthedocs.org/projects/musiclang/badge/?version=latest)](https://musiclang.readthedocs.io/en/latest/?badge=latest)
+
+The Python framework to write, analyze, transform and predict music.
+
+
+What is MusicLang ?
+--------------------
+
+MusicLang which simply stands for "music language" is a Python framework
+implementing a new language for tonal music.
+This language allows composers to load, write, transform and predict symbolic music in a simple,
+condensed and high level manner.
+MusicLang internally uses  a [LLM (Large Language Model)](https://huggingface.co/floriangardin/musiclang)  to predict what could happen next in a musical score.
+This framework is well suited to :
+- Generate musical ideas quickly.
+- Predict what could happen next in an existing midi file
+- Create an interpretable and information rich text representation of a midi file
+
+[Read our documentation](https://musiclang.readthedocs.io/en/latest).
+
+
+How to install
+--------------
+
+MusicLang is available on Pypi :
+
+```
+pip install musiclang
+```
+    
+
+Examples
+---------
+
+1. A hello world example to create a C-major chord in musiclang and save it to midi :
+
+```python
+from musiclang.library import *
+
+# Write A C major chord
+score = (I % I.M)(piano=[s0, s2, s4])
+
+# Store it to midi
+score.to_midi('c_major.mid')
+```
+
+2. Create, transform and harmonize a theme quickly : 
+
+```python
+from musiclang.library import *
+
+# Create a cool melody (the beginning of happy birthday, independant of any harmonic context)
+melody = s4.ed + s4.s + s5 + s4 + s0.o(1) + s6.h
+
+# Create a simple accompaniment with a cello and a oboe
+acc_melody = r + s0.o(-1).q * 3 + s0.o(-1).h
+accomp = {'cello__0': acc_melody, 'oboe__0': acc_melody.o(1)}
+
+# Play it in F-major
+score = (I % IV.M)(violin__0=melody, **accomp)
+
+# Repeat the score a second time in F-minor and forte
+score += (score % I.m).f
+
+# Just to create an anachrusis at the first bar
+score = (I % I.M)(violin__0=r.h) + score
+
+# Transform a bit the accompaniment by applying counterpoint rules automatically
+from musiclang.transform.library import create_counterpoint_on_score
+score = create_counterpoint_on_score(score, fixed_parts=['violin__0'])
+
+# Save it to musicxml
+score.to_musicxml('happy_birthday.musicxml', signature=(3, 4), title='Happy birthday !')
+
+# Et voilà !
+```
+![Happy birthday score](https://github.com/MusicLang/musiclang/blob/main/documentation/images/happy_birthday.png?raw=true "Happy Birthday")
+
+
+3. Predict a score using a deep learning model trained on musiclang language :
+
+```python
+from musiclang.library import *
+from musiclang import Score
+
+# Some random bar of chopin op18 Waltz
+score = ((V % III.b.M)(
+	piano__0=s0 + s2.e.mp + s3.e.mp, 
+	piano__4=s0.e.o(-2).p + r.e + s0.ed.o(-1).mp + r.s, 
+	piano__5=r + s4.ed.o(-1).mp + r.s, 
+	piano__6=r + s6.ed.o(-1).mp + r.s)+ 
+(V['7'] % III.b.M)(
+	piano__0=s2.ed.mp + r.s, 
+	piano__2=s4.ed.mp + r.s, 
+	piano__4=s6.ed.o(-1).mp + r.s, 
+	piano__5=s0.ed.o(-1).mp + r.s, 
+	piano__6=s4.ed.o(-1).mp + r.s))
+
+# Predict the next two chords of the score using huggingface musiclang model
+predicted_score = score.predict_score(n_chords=4, temperature=0.5)
+# Save it to midi
+predicted_score.to_midi('test.mid')
+```
+
+Please note that this feature is still experimental, it will only work with
+piano music for now and the model is not yet trained on a large corpus of music.
+If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
+
+
+4. Mix everything together to create a new pieces of music !
+
```

### Comparing `musiclang-0.8.9/musiclang.egg-info/SOURCES.txt` & `musiclang-0.9.0/musiclang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,29 @@
 musiclang/library.py
 musiclang.egg-info/PKG-INFO
 musiclang.egg-info/SOURCES.txt
 musiclang.egg-info/dependency_links.txt
 musiclang.egg-info/requires.txt
 musiclang.egg-info/top_level.txt
 musiclang/analyze/__init__.py
+musiclang/analyze/chord_inference.py
+musiclang/analyze/chord_inference_utils.py
 musiclang/analyze/constants.py
+musiclang/analyze/dataset_extractor.py
+musiclang/analyze/dataset_trainer.py
 musiclang/analyze/item.py
+musiclang/analyze/load_score.py
 musiclang/analyze/midi_parser.py
 musiclang/analyze/parser.py
 musiclang/analyze/pattern_analyzer.py
 musiclang/analyze/pattern_sampler.py
 musiclang/analyze/roman_parser.py
 musiclang/analyze/score_formatter.py
 musiclang/analyze/score_formatter_elements.py
+musiclang/analyze/split.py
 musiclang/analyze/to_musiclang.py
 musiclang/analyze/voice_separation.py
 musiclang/analyze/augmented_net/__init__.py
 musiclang/analyze/augmented_net/cache.py
 musiclang/analyze/augmented_net/chord_vocabulary.py
 musiclang/analyze/augmented_net/feature_representation.py
 musiclang/analyze/augmented_net/inference.py
```

### Comparing `musiclang-0.8.9/pyproject.toml` & `musiclang-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "musiclang"
-version = "0.8.9"
+version = "0.9.0"
 description = "A python package for music notation and generation"
 readme = "README.md"
 authors = [{ name = "Florian GARDIN", email = "fgardin.pro@gmail.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["music", "ai", "notation"]
 dependencies = [
-    "lxml==4.9.1",
+    "lxml",
     "mido==1.2.10",
     "music21==8.1.0",
     "numpy",
     "pandas==1.5.3",
     "scikit-learn==1.1.3",
-    "scipy==1.9.3",
+    "scipy",
     "tensorflow",
     "toml==0.10.2",
     "tomli==2.0.1",
     "xmlschema==2.1.1",
     "transformers==4.26.1",
     "tokenizers==0.13.2",
+    "partitura==1.2.1",
     "torch"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest"]
```

### Comparing `musiclang-0.8.9/setup.py` & `musiclang-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="musiclang",
-    version="0.8.9",
+    version="0.9.0",
     author="Florian GARDIN",
     author_email="fgardin.pro@gmail.com",
     description=("A python package for music notation and generation"
                 ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
@@ -20,27 +20,28 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "lxml==4.9.1",
+        "lxml",
         "mido==1.2.10",
         "music21==8.1.0",
         "numpy",
         "pandas==1.5.3",
         "scikit-learn==1.1.3",
-        "scipy==1.9.3",
+        "scipy",
         "tensorflow",
         "toml==0.10.2",
         "tomli==2.0.1",
         "xmlschema==2.1.1",
         "transformers==4.26.1",
         "tokenizers==0.13.2",
+        "partitura==1.2.1",
         "torch"
                       ],
     packages=setuptools.find_packages(include='*'),
     package_data={'musiclang': ['augmented_net/*.hdf5']},
     include_package_data=True,
     python_requires=">=3.6",
 )
```

### Comparing `musiclang-0.8.9/tests/analyze/test_score_formatter.py` & `musiclang-0.9.0/tests/analyze/test_score_formatter.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/composing/test_project.py` & `musiclang-0.9.0/tests/composing/test_project.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/composing/test_voice_leading.py` & `musiclang-0.9.0/tests/composing/test_voice_leading.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/predict/test_auto_composer.py` & `musiclang-0.9.0/tests/predict/test_auto_composer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/transform/test_mask.py` & `musiclang-0.9.0/tests/transform/test_mask.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/transform/test_pipeline.py` & `musiclang-0.9.0/tests/transform/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/transform/test_transforms.py` & `musiclang-0.9.0/tests/transform/test_transforms.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/out/test_to_midi.py` & `musiclang-0.9.0/tests/write/out/test_to_midi.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/pitches/test_pitches_utils.py` & `musiclang-0.9.0/tests/write/pitches/test_pitches_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/properties/test_note_properties.py` & `musiclang-0.9.0/tests/write/properties/test_note_properties.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/rythm/test_metric.py` & `musiclang-0.9.0/tests/write/rythm/test_metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/test_bass_notes.py` & `musiclang-0.9.0/tests/write/test_bass_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/test_chord.py` & `musiclang-0.9.0/tests/write/test_chord.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/test_chord_notes.py` & `musiclang-0.9.0/tests/write/test_chord_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/test_drum_notes.py` & `musiclang-0.9.0/tests/write/test_drum_notes.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
     chord = (I % I.M)(drums=s0.o(-2))
     assert chord == (I % I.M)(drums=bd)
 
 def test_unexisting_drum_lead_to_error():
 
     chord = (I % I.M)(drums=s0.o(-2) + s0)
-    assert chord == (I % I.M)(drums=s0.o(-2) + r)
+    assert chord == (I % I.M)(drums=s0.o(-2) + d0)
 
 def test_drum_note_evaluation_ok():
     score = (I % I.M)(drums=[sn + bd, hh + hh]) + (I % I.M)(drums=[sn + bd, hh + hh])
     assert Score.from_str(str(score)) == score
```

### Comparing `musiclang-0.8.9/tests/write/test_extensions.py` & `musiclang-0.9.0/tests/write/test_extensions.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/test_note.py` & `musiclang-0.9.0/tests/write/test_note.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/test_score.py` & `musiclang-0.9.0/tests/write/test_score.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.9/tests/write/test_tonality.py` & `musiclang-0.9.0/tests/write/test_tonality.py`

 * *Files identical despite different names*

