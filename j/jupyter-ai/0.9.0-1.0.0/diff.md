# Comparing `tmp/jupyter_ai-0.9.0.tar.gz` & `tmp/jupyter_ai-1.0.0.tar.gz`

## Comparing `jupyter_ai-0.9.0.tar` & `jupyter_ai-1.0.0.tar`

### file list

```diff
@@ -1,160 +1,152 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.eslintignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.prettierrc
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/babel.config.js
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jest.config.js
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/package.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/project.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/tsconfig.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter-config/nb-config/jupyter_ai.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter-config/server-config/jupyter_ai.json
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/_version.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/engine.py
--rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/extension.py
--rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/handlers.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/models.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/reply_processor.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/task_manager.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/tasks.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/__init__.py
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/ask.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/base.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/chat_provider.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/config.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/default.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/embeddings_provider.py
--rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/generate.py
--rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/learn.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/memory.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/providers.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/document_loaders/__init__.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/document_loaders/directory.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/document_loaders/splitter.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/package.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
--rw-r--r--   0        0        0    26382 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/253.4cb04dcfead6f07b8e7c.js
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
--rw-r--r--   0        0        0    41113 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js.LICENSE.txt
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js
--rw-r--r--   0        0        0   157509 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js.LICENSE.txt
--rw-r--r--   0        0        0  1568438 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js.LICENSE.txt
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/643.23e0a9c561346f879c77.js
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
--rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
--rw-r--r--   0        0        0   443772 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js.LICENSE.txt
--rw-r--r--   0        0        0    91736 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js.LICENSE.txt
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
--rw-r--r--   0        0        0   272943 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/remoteEntry.9095dd2e94ae47ffc04b.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/style.js
--rw-r--r--   0        0        0   111460 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/tests/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/tests/test_handlers.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/schema/plugin.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/chat_handler.ts
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/handler.ts
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/icons.ts
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/index.ts
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/inserter.ts
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/selection-watcher.ts
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/theme-provider.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/utils.ts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/__tests__/jupyter_gai.spec.ts
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat-code-view.tsx
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat-input.tsx
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat-messages.tsx
--rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat-settings.tsx
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/expandable-text-field.tsx
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/jl-theme-provider.tsx
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/scroll-container.tsx
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/select.tsx
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/settings/model-fields.tsx
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/contexts/collaborators-context.tsx
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/contexts/selection-context.tsx
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/types/mui.d.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/types/svg.d.ts
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/widgets/chat-error.tsx
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/widgets/chat-sidebar.tsx
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/base.css
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/chat-settings.css
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/expandable-text-field.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/index.js
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/react-markdown.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/icons/chat.svg
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/icons/jupyternaut.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/tests/jupyter_ai.spec.ts
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/LICENSE
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/README.md
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/.eslintignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/.prettierrc
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/babel.config.js
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/conftest.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jest.config.js
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/package.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/project.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/tsconfig.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter-config/nb-config/jupyter_ai.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter-config/server-config/jupyter_ai.json
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/_version.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/config_manager.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/extension.py
+-rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/handlers.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/models.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/chat_handlers/__init__.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/chat_handlers/ask.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/chat_handlers/base.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/chat_handlers/clear.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/chat_handlers/default.py
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/chat_handlers/generate.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/chat_handlers/help.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/chat_handlers/learn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/document_loaders/directory.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/document_loaders/splitter.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/package.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
+-rw-r--r--   0        0        0    26370 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/253.5c9df1561a4c4c0223da.js
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
+-rw-r--r--   0        0        0    41113 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js.LICENSE.txt
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js
+-rw-r--r--   0        0        0   157509 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js.LICENSE.txt
+-rw-r--r--   0        0        0  1568438 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js.LICENSE.txt
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/643.830710e1337b7cf4cbdd.js
+-rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
+-rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
+-rw-r--r--   0        0        0   443772 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js.LICENSE.txt
+-rw-r--r--   0        0        0    91736 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js.LICENSE.txt
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
+-rw-r--r--   0        0        0   272943 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/remoteEntry.a695d82eb8238716e13d.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/style.js
+-rw-r--r--   0        0        0   111460 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/tests/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/jupyter_ai/tests/test_handlers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/schema/plugin.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/chat_handler.ts
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/handler.ts
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/icons.ts
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/index.ts
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/selection-watcher.ts
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/theme-provider.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/utils.ts
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/__tests__/jupyter_gai.spec.ts
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/chat-code-view.tsx
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/chat-input.tsx
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/chat-messages.tsx
+-rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/chat-settings.tsx
+-rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/chat.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/expandable-text-field.tsx
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/jl-theme-provider.tsx
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/scroll-container.tsx
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/select.tsx
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/components/settings/model-fields.tsx
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/contexts/collaborators-context.tsx
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/contexts/selection-context.tsx
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/types/mui.d.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/types/svg.d.ts
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/widgets/chat-error.tsx
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/src/widgets/chat-sidebar.tsx
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/style/base.css
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/style/chat-settings.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/style/expandable-text-field.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/style/index.js
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/style/react-markdown.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/style/icons/chat.svg
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/style/icons/jupyternaut.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/ui-tests/tests/jupyter_ai.spec.ts
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/README.md
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8260 2020-02-02 00:00:00.000000 jupyter_ai-1.0.0/PKG-INFO
```

### Comparing `jupyter_ai-0.9.0/.eslintrc.js` & `jupyter_ai-1.0.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/RELEASE.md` & `jupyter_ai-1.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jest.config.js` & `jupyter_ai-1.0.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/package.json` & `jupyter_ai-1.0.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'1.0.0'"}*

```diff
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.9.0"
+    "version": "1.0.0"
 }
```

### Comparing `jupyter_ai-0.9.0/tsconfig.json` & `jupyter_ai-1.0.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/handlers.py` & `jupyter_ai-1.0.0/jupyter_ai/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import getpass
 import json
 import time
 import uuid
+from asyncio import AbstractEventLoop
 from dataclasses import asdict
 from typing import Dict, List
 
-import ray
 import tornado
-from jupyter_ai.actors.base import ACTOR_TYPE
+from jupyter_ai.chat_handlers import BaseChatHandler
 from jupyter_server.base.handlers import APIHandler as BaseAPIHandler
 from jupyter_server.base.handlers import JupyterHandler
-from jupyter_server.utils import ensure_async
 from pydantic import ValidationError
 from tornado import web, websocket
 from tornado.web import HTTPError
 
 from .models import (
     AgentChatMessage,
     ChatClient,
@@ -24,76 +23,15 @@
     ChatUser,
     ConnectionMessage,
     GlobalConfig,
     HumanChatMessage,
     ListProvidersEntry,
     ListProvidersResponse,
     Message,
-    PromptRequest,
 )
-from .task_manager import TaskManager
-
-
-class APIHandler(BaseAPIHandler):
-    @property
-    def engines(self):
-        return self.settings["ai_engines"]
-
-    @property
-    def default_tasks(self):
-        return self.settings["ai_default_tasks"]
-
-    @property
-    def task_manager(self):
-        # we have to create the TaskManager lazily, since no event loop is
-        # running in ServerApp.initialize_settings().
-        if "task_manager" not in self.settings:
-            self.settings["task_manager"] = TaskManager(
-                engines=self.engines, default_tasks=self.default_tasks
-            )
-        return self.settings["task_manager"]
-
-
-class PromptAPIHandler(APIHandler):
-    @tornado.web.authenticated
-    async def post(self):
-        try:
-            request = PromptRequest(**self.get_json_body())
-        except ValidationError as e:
-            self.log.exception(e)
-            raise HTTPError(500, str(e)) from e
-
-        if request.engine_id not in self.engines:
-            raise HTTPError(500, f"Model engine not registered: {request.engine_id}")
-
-        engine = self.engines[request.engine_id]
-        task = await self.task_manager.describe_task(request.task_id)
-        if not task:
-            raise HTTPError(404, f"Task not found with ID: {request.task_id}")
-
-        output = await ensure_async(engine.execute(task, request.prompt_variables))
-
-        self.finish(
-            json.dumps({"output": output, "insertion_mode": task.insertion_mode})
-        )
-
-
-class TaskAPIHandler(APIHandler):
-    @tornado.web.authenticated
-    async def get(self, id=None):
-        if id is None:
-            list_tasks_response = await self.task_manager.list_tasks()
-            self.finish(json.dumps(list_tasks_response.dict()))
-            return
-
-        describe_task_response = await self.task_manager.describe_task(id)
-        if describe_task_response is None:
-            raise HTTPError(404, f"Task not found with ID: {id}")
-
-        self.finish(json.dumps(describe_task_response.dict()))
 
 
 class ChatHistoryHandler(BaseAPIHandler):
     """Handler to return message history"""
 
     _messages = []
 
@@ -107,24 +45,30 @@
 
     @tornado.web.authenticated
     async def get(self):
         history = ChatHistory(messages=self.chat_history)
         self.finish(history.json())
 
 
-class ChatHandler(JupyterHandler, websocket.WebSocketHandler):
+class RootChatHandler(JupyterHandler, websocket.WebSocketHandler):
     """
     A websocket handler for chat.
     """
 
     @property
-    def chat_handlers(self) -> Dict[str, "ChatHandler"]:
-        """Dictionary mapping client IDs to their WebSocket handler
+    def root_chat_handlers(self) -> Dict[str, "RootChatHandler"]:
+        """Dictionary mapping client IDs to their corresponding RootChatHandler
         instances."""
-        return self.settings["chat_handlers"]
+        return self.settings["jai_root_chat_handlers"]
+
+    @property
+    def chat_handlers(self) -> Dict[str, "BaseChatHandler"]:
+        """Dictionary mapping chat commands to their corresponding
+        BaseChatHandler instances."""
+        return self.settings["jai_chat_handlers"]
 
     @property
     def chat_clients(self) -> Dict[str, ChatClient]:
         """Dictionary mapping client IDs to their ChatClient objects that store
         metadata."""
         return self.settings["chat_clients"]
 
@@ -133,14 +77,18 @@
         """Returns ChatClient object associated with the current connection."""
         return self.chat_clients[self.client_id]
 
     @property
     def chat_history(self) -> List[ChatMessage]:
         return self.settings["chat_history"]
 
+    @property
+    def loop(self) -> AbstractEventLoop:
+        return self.settings["jai_event_loop"]
+
     def initialize(self):
         self.log.debug("Initializing websocket connection %s", self.request.path)
 
     def pre_get(self):
         """Handles authentication/authorization."""
         # authenticate the request before opening the websocket
         user = self.current_user
@@ -183,32 +131,32 @@
     def open(self):
         """Handles opening of a WebSocket connection. Client ID can be retrieved
         from `self.client_id`."""
 
         current_user = self.get_chat_user().dict()
         client_id = self.generate_client_id()
 
-        self.chat_handlers[client_id] = self
+        self.root_chat_handlers[client_id] = self
         self.chat_clients[client_id] = ChatClient(**current_user, id=client_id)
         self.client_id = client_id
         self.write_message(ConnectionMessage(client_id=client_id).dict())
 
         self.log.info(f"Client connected. ID: {client_id}")
-        self.log.debug("Clients are : %s", self.chat_handlers.keys())
+        self.log.debug("Clients are : %s", self.root_chat_handlers.keys())
 
     def broadcast_message(self, message: Message):
         """Broadcasts message to all connected clients.
         Appends message to `self.chat_history`.
         """
 
         self.log.debug("Broadcasting message: %s to all clients...", message)
-        client_ids = self.chat_handlers.keys()
+        client_ids = self.root_chat_handlers.keys()
 
         for client_id in client_ids:
-            client = self.chat_handlers[client_id]
+            client = self.root_chat_handlers[client_id]
             if client:
                 client.write_message(message.dict())
 
         # Only append ChatMessage instances to history, not control messages
         if isinstance(message, HumanChatMessage) or isinstance(
             message, AgentChatMessage
         ):
@@ -232,45 +180,59 @@
             body=chat_request.prompt,
             client=self.chat_client,
         )
 
         # broadcast the message to other clients
         self.broadcast_message(message=chat_message)
 
-        # Clear the message history if given the /clear command
-        if chat_request.prompt.startswith("/"):
-            command = chat_request.prompt.split(" ", 1)[0]
-            if command == "/clear":
-                self.chat_history.clear()
-
-        # process through the router
-        router = ray.get_actor("router")
-        router.process_message.remote(chat_message)
+        # do not await this, as it blocks the parent task responsible for
+        # handling messages from a websocket.  instead, process each message
+        # as a distinct concurrent task.
+        self.loop.create_task(self._route(chat_message))
+
+    async def _route(self, message):
+        """Method that routes an incoming message to the appropriate handler."""
+        default = self.chat_handlers["default"]
+        maybe_command = message.body.split(" ", 1)[0]
+        is_command = (
+            message.body.startswith("/")
+            and maybe_command in self.chat_handlers.keys()
+            and maybe_command != "default"
+        )
+        command = maybe_command if is_command else "default"
+
+        start = time.time()
+        if is_command:
+            await self.chat_handlers[command].process_message(message)
+        else:
+            await default.process_message(message)
+
+        latency_ms = round((time.time() - start) * 1000)
+        command_readable = "Default" if command == "default" else command
+        self.log.info(f"{command_readable} chat handler resolved in {latency_ms} ms.")
 
     def on_close(self):
         self.log.debug("Disconnecting client with user %s", self.client_id)
 
-        self.chat_handlers.pop(self.client_id, None)
+        self.root_chat_handlers.pop(self.client_id, None)
         self.chat_clients.pop(self.client_id, None)
 
         self.log.info(f"Client disconnected. ID: {self.client_id}")
-        self.log.debug("Chat clients: %s", self.chat_handlers.keys())
+        self.log.debug("Chat clients: %s", self.root_chat_handlers.keys())
 
 
 class ModelProviderHandler(BaseAPIHandler):
     @property
-    def chat_providers(self):
-        actor = ray.get_actor("providers")
-        o = actor.get_model_providers.remote()
-        return ray.get(o)
+    def lm_providers(self):
+        return self.settings["lm_providers"]
 
     @web.authenticated
     def get(self):
         providers = []
-        for provider in self.chat_providers.values():
+        for provider in self.lm_providers.values():
             # skip old legacy OpenAI chat provider used only in magics
             if provider.id == "openai-chat":
                 continue
 
             providers.append(
                 ListProvidersEntry(
                     id=provider.id,
@@ -286,23 +248,21 @@
             providers=sorted(providers, key=lambda p: p.name)
         )
         self.finish(response.json())
 
 
 class EmbeddingsModelProviderHandler(BaseAPIHandler):
     @property
-    def embeddings_providers(self):
-        actor = ray.get_actor("providers")
-        o = actor.get_embeddings_providers.remote()
-        return ray.get(o)
+    def em_providers(self):
+        return self.settings["em_providers"]
 
     @web.authenticated
     def get(self):
         providers = []
-        for provider in self.embeddings_providers.values():
+        for provider in self.em_providers.values():
             providers.append(
                 ListProvidersEntry(
                     id=provider.id,
                     name=provider.name,
                     models=provider.models,
                     auth_strategy=provider.auth_strategy,
                     registry=provider.registry,
@@ -317,33 +277,33 @@
 
 
 class GlobalConfigHandler(BaseAPIHandler):
     """API handler for fetching and setting the
     model and emebddings config.
     """
 
+    @property
+    def config_manager(self):
+        return self.settings["jai_config_manager"]
+
     @web.authenticated
     def get(self):
-        actor = ray.get_actor(ACTOR_TYPE.CONFIG)
-        config = ray.get(actor.get_config.remote())
+        config = self.config_manager.get_config()
         if not config:
             raise HTTPError(500, "No config found.")
 
         self.finish(config.json())
 
     @web.authenticated
     def post(self):
         try:
             config = GlobalConfig(**self.get_json_body())
-            actor = ray.get_actor(ACTOR_TYPE.CONFIG)
-            ray.get(actor.update.remote(config))
-
+            self.config_manager.update(config)
             self.set_status(204)
             self.finish()
-
         except ValidationError as e:
             self.log.exception(e)
             raise HTTPError(500, str(e)) from e
         except ValueError as e:
             self.log.exception(e)
             raise HTTPError(500, str(e.cause) if hasattr(e, "cause") else str(e))
         except Exception as e:
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/actors/ask.py` & `jupyter_ai-1.0.0/jupyter_ai/chat_handlers/ask.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,63 @@
 import argparse
-from typing import Dict, List, Type
+from typing import Dict, Type
 
-import ray
-from jupyter_ai.actors.base import ACTOR_TYPE, BaseActor, Logger
 from jupyter_ai.models import HumanChatMessage
 from jupyter_ai_magics.providers import BaseProvider
 from langchain.chains import ConversationalRetrievalChain
-from langchain.schema import BaseRetriever, Document
-from ray.util.queue import Queue
 
+from .base import BaseChatHandler
 
-@ray.remote
-class AskActor(BaseActor):
+
+class AskChatHandler(BaseChatHandler):
     """Processes messages prefixed with /ask. This actor will
     send the message as input to a RetrieverQA chain, that
     follows the Retrieval and Generation (RAG) tehnique to
     query the documents from the index, and sends this context
     to the LLM to generate the final reply.
     """
 
-    def __init__(self, reply_queue: Queue, log: Logger):
-        super().__init__(reply_queue=reply_queue, log=log)
+    def __init__(self, retriever, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
+        self._retriever = retriever
         self.parser.prog = "/ask"
         self.parser.add_argument("query", nargs=argparse.REMAINDER)
 
     def create_llm_chain(
         self, provider: Type[BaseProvider], provider_params: Dict[str, str]
     ):
-        retriever = Retriever()
         self.llm = provider(**provider_params)
         self.chat_history = []
-        self.llm_chain = ConversationalRetrievalChain.from_llm(self.llm, retriever)
+        self.llm_chain = ConversationalRetrievalChain.from_llm(
+            self.llm, self._retriever
+        )
 
-    def _process_message(self, message: HumanChatMessage):
+    async def _process_message(self, message: HumanChatMessage):
         args = self.parse_args(message)
         if args is None:
             return
         query = " ".join(args.query)
         if not query:
             self.reply(f"{self.parser.format_usage()}", message)
             return
 
         self.get_llm_chain()
 
         try:
             # limit chat history to last 2 exchanges
             self.chat_history = self.chat_history[-2:]
-            result = self.llm_chain(
+
+            result = await self.llm_chain.acall(
                 {"question": query, "chat_history": self.chat_history}
             )
             response = result["answer"]
             self.chat_history.append((query, response))
             self.reply(response, message)
         except AssertionError as e:
             self.log.error(e)
             response = """Sorry, an error occurred while reading the from the learned documents.
             If you have changed the embedding provider, try deleting the existing index by running
             `/learn -d` command and then re-submitting the `learn <directory>` to learn the documents,
             and then asking the question again.
             """
             self.reply(response, message)
-
-
-class Retriever(BaseRetriever):
-    """Wrapper retriever class to get relevant docs
-    from the vector store, this is important because
-    of inconsistent de-serialization of index when it's
-    accessed directly from the ask actor.
-    """
-
-    def get_relevant_documents(self, question: str):
-        index_actor = ray.get_actor(ACTOR_TYPE.LEARN.value)
-        docs = ray.get(index_actor.get_relevant_documents.remote(question))
-        return docs
-
-    async def aget_relevant_documents(self, query: str) -> List[Document]:
-        return await super().aget_relevant_documents(query)
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/actors/default.py` & `jupyter_ai-1.0.0/jupyter_ai/chat_handlers/default.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from typing import Dict, List, Type
 
-import ray
-from jupyter_ai.actors.base import ACTOR_TYPE, BaseActor
-from jupyter_ai.actors.memory import RemoteMemory
 from jupyter_ai.models import ChatMessage, ClearMessage, HumanChatMessage
 from jupyter_ai_magics.providers import BaseProvider
 from langchain import ConversationChain
+from langchain.memory import ConversationBufferWindowMemory
 from langchain.prompts import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     MessagesPlaceholder,
     SystemMessagePromptTemplate,
 )
 from langchain.schema import AIMessage
 
+from .base import BaseChatHandler
+
 SYSTEM_PROMPT = """
 You are Jupyternaut, a conversational assistant living in JupyterLab to help users.
 You are not a language model, but rather an application built on a foundation model from {provider_name} called {local_model_id}.
 You are talkative and you provide lots of specific details from the foundation model's context.
 You may use Markdown to format your response.
 Code blocks must be formatted in Markdown.
 Math should be rendered with inline TeX markup, surrounded by $.
 If you do not know the answer to a question, answer truthfully by responding that you do not know.
 The following is a friendly conversation between you and a human.
 """.strip()
 
 
-@ray.remote
-class DefaultActor(BaseActor):
+class DefaultChatHandler(BaseChatHandler):
     def __init__(self, chat_history: List[ChatMessage], *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.memory = None
+        self.memory = ConversationBufferWindowMemory(return_messages=True, k=2)
         self.chat_history = chat_history
 
     def create_llm_chain(
         self, provider: Type[BaseProvider], provider_params: Dict[str, str]
     ):
         llm = provider(**provider_params)
-        self.memory = RemoteMemory(actor_name=ACTOR_TYPE.MEMORY)
         prompt_template = ChatPromptTemplate.from_messages(
             [
                 SystemMessagePromptTemplate.from_template(SYSTEM_PROMPT).format(
                     provider_name=llm.name, local_model_id=llm.model_id
                 ),
                 MessagesPlaceholder(variable_name="history"),
                 HumanMessagePromptTemplate.from_template("{input}"),
@@ -56,17 +54,17 @@
     def clear_memory(self):
         # clear chain memory
         if self.memory:
             self.memory.clear()
 
         # clear transcript for existing chat clients
         reply_message = ClearMessage()
-        self.reply_queue.put(reply_message)
+        self.reply(reply_message)
 
         # clear transcript for new chat clients
         if self.chat_history:
             self.chat_history.clear()
 
-    def _process_message(self, message: HumanChatMessage):
+    async def _process_message(self, message: HumanChatMessage):
         self.get_llm_chain()
-        response = self.llm_chain.predict(input=message.body, stop=["\nHuman:"])
+        response = await self.llm_chain.apredict(input=message.body, stop=["\nHuman:"])
         self.reply(response, message)
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/actors/generate.py` & `jupyter_ai-1.0.0/jupyter_ai/chat_handlers/generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
+import asyncio
 import json
 import os
 from typing import Dict, Type
 
 import nbformat
-import ray
-from jupyter_ai.actors.base import BaseActor, Logger
+from jupyter_ai.chat_handlers import BaseChatHandler
 from jupyter_ai.models import HumanChatMessage
-from jupyter_ai_magics.providers import BaseProvider, ChatOpenAINewProvider
+from jupyter_ai_magics.providers import BaseProvider
 from langchain.chains import LLMChain
 from langchain.llms import BaseLLM
 from langchain.prompts import PromptTemplate
-from ray.util.queue import Queue
 
 schema = """{
   "$schema": "http://json-schema.org/draft-07/schema#",
   "type": "object",
   "properties": {
     "description": {
       "type": "string"
@@ -54,18 +53,18 @@
         prompt = PromptTemplate(
             template=task_creation_template,
             input_variables=["description", "schema"],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
 
-def generate_outline(description, llm=None, verbose=False):
+async def generate_outline(description, llm=None, verbose=False):
     """Generate an outline of sections given a description of a notebook."""
     chain = NotebookOutlineChain.from_llm(llm=llm, verbose=verbose)
-    outline = chain.predict(description=description, schema=schema)
+    outline = await chain.apredict(description=description, schema=schema)
     return json.loads(outline)
 
 
 class CodeImproverChain(LLMChain):
     """Chain to improve source code."""
 
     @classmethod
@@ -79,62 +78,34 @@
             input_variables=[
                 "code",
             ],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
 
-def improve_code(code, llm=None, verbose=False):
-    """Improve source code using an LLM."""
-    chain = CodeImproverChain.from_llm(llm=llm, verbose=verbose)
-    improved_code = chain.predict(code=code)
-    improved_code = "\n".join(
-        [line for line in improved_code.split("/n") if not line.startswith("```")]
-    )
-    return improved_code
-
-
 class NotebookSectionCodeChain(LLMChain):
     """Chain to generate source code for a notebook section."""
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, verbose: bool = False) -> LLMChain:
         task_creation_template = (
             "You are an AI that writes code for a single section of a Jupyter notebook.\n"
             "Overall topic of the notebook: {description}\n"
             "Title of the notebook section: {title}\n"
             "Description of the notebok section: {content}\n"
             "Given this information, write all the code for this section and this section only."
             " Your output should be valid code with inline comments.\n"
-            "Code in the notebook so far:\n"
-            "{code_so_far}"
         )
         prompt = PromptTemplate(
             template=task_creation_template,
-            input_variables=["description", "title", "content", "code_so_far"],
+            input_variables=["description", "title", "content"],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
 
-def generate_code(outline, llm=None, verbose=False):
-    """Generate source code for a section given a description of the notebook and section."""
-    chain = NotebookSectionCodeChain.from_llm(llm=llm, verbose=verbose)
-    code_so_far = []
-    for section in outline["sections"]:
-        code = chain.predict(
-            description=outline["description"],
-            title=section["title"],
-            content=section["content"],
-            code_so_far="\n".join(code_so_far),
-        )
-        section["code"] = improve_code(code, llm=llm, verbose=verbose)
-        code_so_far.append(section["code"])
-    return outline
-
-
 class NotebookSummaryChain(LLMChain):
     """Chain to generate a short summary of a notebook."""
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, verbose: bool = False) -> LLMChain:
         task_creation_template = (
             "Create a markdown summary for a Jupyter notebook with the following content."
@@ -164,23 +135,65 @@
             input_variables=[
                 "content",
             ],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
 
-def generate_title_and_summary(outline, llm=None, verbose=False):
+async def improve_code(code, llm=None, verbose=False):
+    """Improve source code using an LLM."""
+    chain = CodeImproverChain.from_llm(llm=llm, verbose=verbose)
+    improved_code = await chain.apredict(code=code)
+    improved_code = "\n".join(
+        [line for line in improved_code.split("/n") if not line.startswith("```")]
+    )
+    return improved_code
+
+
+async def generate_code(section, description, llm=None, verbose=False) -> None:
+    """
+    Function that accepts a section and adds code under the "code" key when
+    awaited.
+    """
+    chain = NotebookSectionCodeChain.from_llm(llm=llm, verbose=verbose)
+    code = await chain.apredict(
+        description=description,
+        title=section["title"],
+        content=section["content"],
+    )
+    improved_code = await improve_code(code, llm=llm, verbose=verbose)
+    section["code"] = improved_code
+
+
+async def generate_title(outline, llm=None, verbose: bool = False):
     """Generate a title and summary of a notebook outline using an LLM."""
-    summary_chain = NotebookSummaryChain.from_llm(llm=llm, verbose=verbose)
     title_chain = NotebookTitleChain.from_llm(llm=llm, verbose=verbose)
-    summary = summary_chain.predict(content=outline)
-    title = title_chain.predict(content=outline)
+    title = await title_chain.apredict(content=outline)
+    title = title.strip()
+    title = title.strip("'\"")
+    outline["title"] = title
+
+
+async def generate_summary(outline, llm=None, verbose: bool = False):
+    summary_chain = NotebookSummaryChain.from_llm(llm=llm, verbose=verbose)
+    summary = await summary_chain.apredict(content=outline)
     outline["summary"] = summary
-    outline["title"] = title.strip('"')
-    return outline
+
+
+async def fill_outline(outline, llm, verbose=False):
+    shared_kwargs = {"outline": outline, "llm": llm, "verbose": verbose}
+
+    all_coros = []
+    all_coros.append(generate_title(**shared_kwargs))
+    all_coros.append(generate_summary(**shared_kwargs))
+    for section in outline["sections"]:
+        all_coros.append(
+            generate_code(section, outline["description"], llm=llm, verbose=verbose)
+        )
+    await asyncio.gather(*all_coros)
 
 
 def create_notebook(outline):
     """Create an nbformat Notebook object for a notebook outline."""
     nbf = nbformat.v4
     nb = nbf.new_notebook()
     nb["cells"].append(nbf.new_markdown_cell("# " + outline["title"]))
@@ -192,42 +205,46 @@
     for section in outline["sections"][1:]:
         nb["cells"].append(nbf.new_markdown_cell("## " + section["title"]))
         for code_block in section["code"].split("\n\n"):
             nb["cells"].append(nbf.new_code_cell(code_block))
     return nb
 
 
-@ray.remote
-class GenerateActor(BaseActor):
-    """A Ray actor to generate a Jupyter notebook given a description."""
+class GenerateChatHandler(BaseChatHandler):
+    """Generates a Jupyter notebook given a description."""
 
-    def __init__(self, reply_queue: Queue, root_dir: str, log: Logger):
-        super().__init__(log=log, reply_queue=reply_queue)
+    def __init__(self, root_dir: str, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.root_dir = os.path.abspath(os.path.expanduser(root_dir))
         self.llm = None
 
     def create_llm_chain(
         self, provider: Type[BaseProvider], provider_params: Dict[str, str]
     ):
         llm = provider(**provider_params)
         self.llm = llm
         return llm
 
-    def _process_message(self, message: HumanChatMessage):
+    async def _process_message(self, message: HumanChatMessage):
         self.get_llm_chain()
 
+        # first send a verification message to user
         response = "👍 Great, I will get started on your notebook. It may take a few minutes, but I will reply here when the notebook is ready. In the meantime, you can continue to ask me other questions."
         self.reply(response, message)
 
+        # generate notebook outline
         prompt = message.body
-        outline = generate_outline(prompt, llm=self.llm, verbose=True)
+        outline = await generate_outline(prompt, llm=self.llm, verbose=True)
         # Save the user input prompt, the description property is now LLM generated.
         outline["prompt"] = prompt
-        outline = generate_code(outline, llm=self.llm, verbose=True)
-        outline = generate_title_and_summary(outline, llm=self.llm)
+
+        # fill the outline concurrently
+        await fill_outline(outline, llm=self.llm, verbose=True)
+
+        # create and write the notebook to disk
         notebook = create_notebook(outline)
         final_path = os.path.join(self.root_dir, outline["title"] + ".ipynb")
         nbformat.write(notebook, final_path)
         response = f"""🎉 I have created your notebook and saved it to the location {final_path}. I am still learning how to create notebooks, so please review all code before running it."""
         self.reply(response, message)
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/actors/learn.py` & `jupyter_ai-1.0.0/jupyter_ai/chat_handlers/learn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,94 @@
 import argparse
 import json
 import os
-import time
-from typing import List
+from typing import Any, Awaitable, Coroutine, List
 
-import ray
-from jupyter_ai.actors.base import BaseActor, Logger
-from jupyter_ai.document_loaders.directory import RayRecursiveDirectoryLoader
+from dask.distributed import Client as DaskClient
+from jupyter_ai.document_loaders.directory import get_embeddings, split
 from jupyter_ai.document_loaders.splitter import ExtensionSplitter, NotebookSplitter
-from jupyter_ai.models import HumanChatMessage, IndexedDir, IndexMetadata
+from jupyter_ai.models import (
+    DEFAULT_CHUNK_OVERLAP,
+    DEFAULT_CHUNK_SIZE,
+    HumanChatMessage,
+    IndexedDir,
+    IndexMetadata,
+)
 from jupyter_core.paths import jupyter_data_dir
 from langchain import FAISS
-from langchain.schema import Document
+from langchain.schema import BaseRetriever, Document
 from langchain.text_splitter import (
     LatexTextSplitter,
     MarkdownTextSplitter,
     PythonCodeTextSplitter,
     RecursiveCharacterTextSplitter,
 )
-from ray.util.queue import Queue
+
+from .base import BaseChatHandler
 
 INDEX_SAVE_DIR = os.path.join(jupyter_data_dir(), "jupyter_ai", "indices")
 METADATA_SAVE_PATH = os.path.join(INDEX_SAVE_DIR, "metadata.json")
 
 
-@ray.remote
-class LearnActor(BaseActor):
-    def __init__(self, reply_queue: Queue, log: Logger, root_dir: str):
-        super().__init__(reply_queue=reply_queue, log=log)
+class LearnChatHandler(BaseChatHandler, BaseRetriever):
+    def __init__(
+        self, root_dir: str, dask_client_future: Awaitable[DaskClient], *args, **kwargs
+    ):
+        super().__init__(*args, **kwargs)
         self.root_dir = root_dir
-        self.chunk_size = 2000
-        self.chunk_overlap = 100
+        self.dask_client_future = dask_client_future
         self.parser.prog = "/learn"
         self.parser.add_argument("-v", "--verbose", action="store_true")
         self.parser.add_argument("-d", "--delete", action="store_true")
         self.parser.add_argument("-l", "--list", action="store_true")
+        self.parser.add_argument(
+            "-c", "--chunk-size", action="store", default=DEFAULT_CHUNK_SIZE, type=int
+        )
+        self.parser.add_argument(
+            "-o",
+            "--chunk-overlap",
+            action="store",
+            default=DEFAULT_CHUNK_OVERLAP,
+            type=int,
+        )
         self.parser.add_argument("path", nargs=argparse.REMAINDER)
         self.index_name = "default"
         self.index = None
         self.metadata = IndexMetadata(dirs=[])
+        self.prev_em_id = None
 
         if not os.path.exists(INDEX_SAVE_DIR):
             os.makedirs(INDEX_SAVE_DIR)
 
-        self.load_or_create()
+        self._load_or_create()
+
+    def _load_or_create(self):
+        """Loads the vector store and creates a new one if none exists."""
+        embeddings = self.get_embedding_model()
+        if not embeddings:
+            return
+        if self.index is None:
+            try:
+                self.index = FAISS.load_local(
+                    INDEX_SAVE_DIR, embeddings, index_name=self.index_name
+                )
+                self.load_metadata()
+            except Exception as e:
+                self.create()
 
-    def _process_message(self, message: HumanChatMessage):
+    async def _process_message(self, message: HumanChatMessage):
         if not self.index:
-            self.load_or_create()
+            self._load_or_create()
 
         # If index is not still there, embeddings are not present
         if not self.index:
             self.reply(
                 "Sorry, please select an embedding provider before using the `/learn` command."
             )
+            return
 
         args = self.parse_args(message)
         if args is None:
             return
 
         if args.delete:
             self.delete()
@@ -75,18 +106,21 @@
         short_path = args.path[0]
         load_path = os.path.join(self.root_dir, short_path)
         if not os.path.exists(load_path):
             response = f"Sorry, that path doesn't exist: {load_path}"
             self.reply(response, message)
             return
 
+        # delete and relearn index if embedding model was changed
+        await self.delete_and_relearn()
+
         if args.verbose:
             self.reply(f"Loading and splitting files for {load_path}", message)
 
-        self.learn_dir(load_path)
+        await self.learn_dir(load_path, args.chunk_size, args.chunk_overlap)
         self.save()
 
         response = f"""🎉 I have learned documents at **{load_path}** and I am ready to answer questions about them.
         You can ask questions about these docs by prefixing your message with **/ask**."""
         self.reply(response, message)
 
     def _build_list_response(self):
@@ -95,93 +129,117 @@
 
         dirs = [dir.path for dir in self.metadata.dirs]
         dir_list = "\n- " + "\n- ".join(dirs) + "\n\n"
         message = f"""I can answer questions from docs in these directories:
         {dir_list}"""
         return message
 
-    def learn_dir(self, path: str):
+    async def learn_dir(self, path: str, chunk_size: int, chunk_overlap: int):
+        dask_client = await self.dask_client_future
+        splitter_kwargs = {"chunk_size": chunk_size, "chunk_overlap": chunk_overlap}
         splitters = {
-            ".py": PythonCodeTextSplitter(
-                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
-            ),
-            ".md": MarkdownTextSplitter(
-                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
-            ),
-            ".tex": LatexTextSplitter(
-                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
-            ),
-            ".ipynb": NotebookSplitter(
-                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
-            ),
+            ".py": PythonCodeTextSplitter(**splitter_kwargs),
+            ".md": MarkdownTextSplitter(**splitter_kwargs),
+            ".tex": LatexTextSplitter(**splitter_kwargs),
+            ".ipynb": NotebookSplitter(**splitter_kwargs),
         }
         splitter = ExtensionSplitter(
             splitters=splitters,
-            default_splitter=RecursiveCharacterTextSplitter(
-                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
-            ),
+            default_splitter=RecursiveCharacterTextSplitter(**splitter_kwargs),
         )
 
-        loader = RayRecursiveDirectoryLoader(path)
-        texts = loader.load_and_split(text_splitter=splitter)
-        self.index.add_documents(texts)
-        self._add_dir_to_metadata(path)
+        delayed = split(path, splitter=splitter)
+        doc_chunks = await dask_client.compute(delayed)
 
-    def _add_dir_to_metadata(self, path: str):
+        em_provider_cls, em_provider_args = self.get_embedding_provider()
+        delayed = get_embeddings(doc_chunks, em_provider_cls, em_provider_args)
+        embedding_records = await dask_client.compute(delayed)
+        self.index.add_embeddings(*embedding_records)
+        self._add_dir_to_metadata(path, chunk_size, chunk_overlap)
+        self.prev_em_id = em_provider_cls.id + ":" + em_provider_args["model_id"]
+
+    def _add_dir_to_metadata(self, path: str, chunk_size: int, chunk_overlap: int):
         dirs = self.metadata.dirs
         index = next((i for i, dir in enumerate(dirs) if dir.path == path), None)
         if not index:
-            dirs.append(IndexedDir(path=path))
+            dirs.append(
+                IndexedDir(
+                    path=path, chunk_size=chunk_size, chunk_overlap=chunk_overlap
+                )
+            )
         self.metadata.dirs = dirs
 
-    def delete_and_relearn(self):
+    async def delete_and_relearn(self):
+        """Delete the vector store and relearn all indexed directories if
+        necessary. If the embedding model is unchanged, this method does
+        nothing."""
         if not self.metadata.dirs:
             self.delete()
             return
-        message = """🔔 Hi there, It seems like you have updated the embeddings model. For the **/ask**
-        command to work with the new model, I have to re-learn the documents you had previously
-        submitted for learning. Please wait to use the **/ask** command until I am done with this task."""
+
+        em_provider_cls, em_provider_args = self.get_embedding_provider()
+        curr_em_id = em_provider_cls.id + ":" + em_provider_args["model_id"]
+        prev_em_id = self.prev_em_id
+
+        # TODO: Fix this condition to read the previous EM id from some
+        # persistent source. Right now, we just skip this validation on server
+        # init, meaning a user could switch embedding models in the config file
+        # directly and break their instance.
+        if (prev_em_id is None) or (prev_em_id == curr_em_id):
+            return
+
+        self.log.info(
+            f"Switching embedding provider from {prev_em_id} to {curr_em_id}."
+        )
+        message = f"""🔔 Hi there, it seems like you have updated the embeddings
+        model from `{prev_em_id}` to `{curr_em_id}`. I have to re-learn the
+        documents you had previously submitted for learning. Please wait to use
+        the **/ask** command until I am done with this task."""
+
         self.reply(message)
 
         metadata = self.metadata
         self.delete()
-        self.relearn(metadata)
+        await self.relearn(metadata)
+        self.prev_em_id = curr_em_id
 
     def delete(self):
         self.index = None
         self.metadata = IndexMetadata(dirs=[])
         paths = [
             os.path.join(INDEX_SAVE_DIR, self.index_name + ext)
             for ext in [".pkl", ".faiss"]
         ]
         for path in paths:
             if os.path.isfile(path):
                 os.remove(path)
         self.create()
 
-    def relearn(self, metadata: IndexMetadata):
+    async def relearn(self, metadata: IndexMetadata):
         # Index all dirs in the metadata
         if not metadata.dirs:
             return
 
         for dir in metadata.dirs:
-            self.learn_dir(dir.path)
+            # TODO: do not relearn directories in serial, but instead
+            # concurrently or in parallel
+            await self.learn_dir(dir.path, dir.chunk_size, dir.chunk_overlap)
 
         self.save()
 
         dir_list = (
             "\n- " + "\n- ".join([dir.path for dir in self.metadata.dirs]) + "\n\n"
         )
         message = f"""🎉 I am done learning docs in these directories:
         {dir_list} I am ready to answer questions about them.
         You can ask questions about these docs by prefixing your message with **/ask**."""
         self.reply(message)
 
     def create(self):
-        embeddings = self.get_embeddings()
+        embeddings = self.get_embedding_model()
         if not embeddings:
             return
         self.index = FAISS.from_texts(
             [
                 "Jupyternaut knows about your filesystem, to ask questions first use the /learn command."
             ],
             embeddings,
@@ -194,33 +252,40 @@
 
         self.save_metadata()
 
     def save_metadata(self):
         with open(METADATA_SAVE_PATH, "w") as f:
             f.write(self.metadata.json())
 
-    def load_or_create(self):
-        embeddings = self.get_embeddings()
-        if not embeddings:
-            return
-        if self.index is None:
-            try:
-                self.index = FAISS.load_local(
-                    INDEX_SAVE_DIR, embeddings, index_name=self.index_name
-                )
-                self.load_metadata()
-            except Exception as e:
-                self.create()
-
     def load_metadata(self):
         if not os.path.exists(METADATA_SAVE_PATH):
             return
 
         with open(METADATA_SAVE_PATH, encoding="utf-8") as f:
             j = json.loads(f.read())
             self.metadata = IndexMetadata(**j)
 
-    def get_relevant_documents(self, question: str) -> List[Document]:
-        if self.index:
-            docs = self.index.similarity_search(question)
-            return docs
-        return []
+    def get_relevant_documents(self, query: str) -> List[Document]:
+        raise NotImplementedError()
+
+    async def aget_relevant_documents(
+        self, query: str
+    ) -> Coroutine[Any, Any, List[Document]]:
+        if not self.index:
+            return []
+
+        await self.delete_and_relearn()
+        docs = self.index.similarity_search(query)
+        return docs
+
+    def get_embedding_provider(self):
+        em_provider_cls = self.config_manager.get_em_provider()
+        em_provider_args = self.config_manager.get_em_provider_params()
+
+        return em_provider_cls, em_provider_args
+
+    def get_embedding_model(self):
+        em_provider_cls, em_provider_args = self.get_embedding_provider()
+        if em_provider_cls is None:
+            return None
+
+        return em_provider_cls(**em_provider_args)
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/document_loaders/splitter.py` & `jupyter_ai-1.0.0/jupyter_ai/document_loaders/splitter.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/package.json` & `jupyter_ai-1.0.0/jupyter_ai/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a695d82eb8238716e13d.js'}}",*

 * * "'version'": "'1.0.0'"}*

```diff
@@ -59,15 +59,15 @@
         "schema/*.json",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9095dd2e94ae47ffc04b.js",
+            "load": "static/remoteEntry.a695d82eb8238716e13d.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_ai"
                 },
@@ -126,9 +126,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.9.0"
+    "version": "1.0.0"
 }
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig` & `jupyter_ai-1.0.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'1.0.0'"}*

```diff
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.9.0"
+    "version": "1.0.0"
 }
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json` & `jupyter_ai-1.0.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/253.4cb04dcfead6f07b8e7c.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/253.5c9df1561a4c4c0223da.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -158,26 +158,26 @@
             }
             var f = n(30535),
                 v = n.n(f),
                 y = n(96707),
                 E = n.n(y),
                 _ = n(40532),
                 b = n.n(_),
-                C = (n(38662), n(55351)),
-                x = n(7464),
-                w = n(6277);
-            const S = "jp-ai-code";
+                x = (n(38662), n(55351)),
+                C = n(7464),
+                S = n(6277);
+            const w = "jp-ai-code";
 
             function k({
                 className: e,
                 children: t,
                 ...n
             }) {
                 return i().createElement("code", Object.assign({}, n, {
-                    className: (0, w.Z)(S, e)
+                    className: (0, S.Z)(w, e)
                 }), t)
             }
             var j;
             ! function(e) {
                 e[e.None = 0] = "None", e[e.Copying = 1] = "Copying", e[e.Copied = 2] = "Copied"
             }(j || (j = {}));
             const I = {
@@ -194,18 +194,18 @@
                 const r = (0, l.useMemo)((() => String(t).replace(/\n$/, "")), [t]),
                     [o, a] = (0, l.useState)(j.None);
                 return i().createElement(c.Box, {
                     sx: {
                         display: "flex",
                         flexDirection: "column"
                     }
-                }, i().createElement(C.Prism, Object.assign({}, n, {
-                    className: (0, w.Z)(n.className, S),
+                }, i().createElement(x.Prism, Object.assign({}, n, {
+                    className: (0, S.Z)(n.className, w),
                     children: r,
-                    style: x.Z,
+                    style: C.Z,
                     language: e,
                     PreTag: "div"
                 })), i().createElement(c.Button, {
                     onClick: async () => {
                         a(j.Copying);
                         try {
                             await navigator.clipboard.writeText(r)
@@ -255,20 +255,20 @@
                 }, t) : t
             }
             var A = n(61745);
             const N = new A.LabIcon({
                     name: "jupyter-ai::chat",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M0 0h24v24H0V0z" fill="none"/>\n    <path d="M15 4v7H5.17L4 12.17V4h11m1-2H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm5 4h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1z"/>\n  </g>\n</svg>\n'
                 }),
-                T = new A.LabIcon({
+                R = new A.LabIcon({
                     name: "jupyter-ai::jupyternaut",
                     svgstr: '<svg viewBox="0 0 38 38" fill="none"\n    xmlns="http://www.w3.org/2000/svg">\n    <g clip-path="url(#clip0_0_2356)">\n        <rect width="38" height="38" fill="white" />\n        <circle cx="19" cy="19" r="19" fill="#F37726" />\n        <path fill-rule="evenodd" clip-rule="evenodd"\n            d="M19.9483 6.83653C20.5827 6.6205 21.0391 6.0196 21.0391 5.31212C21.0391 4.42296 20.3183 3.70215 19.4291 3.70215C18.5399 3.70215 17.8191 4.42296 17.8191 5.31212C17.8191 6.01951 18.2753 6.62033 18.9096 6.83644V8.00387H18.3702C12.0844 8.00387 6.97151 13.1171 6.97151 19.4026C6.97151 25.6885 12.0848 30.8013 18.3702 30.8013H19.7682C26.0541 30.8013 31.167 25.6881 31.167 19.4026C31.167 13.1773 26.1511 8.10183 19.9483 8.00527V6.83653ZM18.3702 29H19.7682C25.1351 29 29.4985 24.0213 29.4985 20.6545C29.4985 15.2876 25.1351 10.9242 19.7682 10.9242H18.3702C13.0034 10.9242 8.64 15.2876 8.64 20.6545C8.64 24.0213 13.0034 29 18.3702 29ZM32.8926 23.997C33.6267 23.997 33.6301 23.4847 33.6348 22.7562V22.7562V22.7562V22.7561C33.636 22.5714 33.6373 22.3728 33.6506 22.1651C33.7079 21.3027 33.7245 20.4643 33.7079 19.6759L33.7046 19.5569C33.6673 18.2251 33.661 17.999 32.3999 17.7511L32.252 17.7265L32.2535 17.776C32.2611 18.0225 32.2686 18.269 32.2686 18.515C32.2686 20.3168 31.9974 22.0628 31.4956 23.704C31.3593 24.1499 31.8389 24.5669 32.249 24.3451L32.8926 23.997ZM5.28037 23.997C4.54628 23.997 4.54296 23.4847 4.53822 22.7563C4.53702 22.5715 4.53573 22.3729 4.52241 22.1651C4.46511 21.3027 4.44849 20.4644 4.4651 19.6759L4.46846 19.557C4.50567 18.2251 4.51198 17.9991 5.77316 17.7512L5.921 17.7265L5.91949 17.776L5.91949 17.776C5.91193 18.0225 5.90438 18.269 5.90438 18.515C5.90438 20.3169 6.17557 22.0628 6.67738 23.704C6.81372 24.1499 6.33412 24.5669 5.92398 24.3451L5.28037 23.997ZM19.5225 11.9922C14.8928 11.9922 11.0449 14.9283 10.0641 18.7499C9.93031 19.2711 10.6154 19.4434 10.9411 19.0152C12.324 17.1972 14.0829 16.8622 15.6479 16.5641C17.7622 16.1614 19.5225 15.8262 19.5225 11.9922Z"\n            fill="white" />\n    </g>\n    <defs>\n        <clipPath id="clip0_0_2356">\n            <rect width="38" height="38" fill="white" />\n        </clipPath>\n    </defs>\n</svg>\n'
                 }).react;
 
-            function R(e) {
+            function T(e) {
                 var t;
                 const n = (0, l.useContext)(M),
                     r = {
                         height: "24px",
                         width: "24px"
                     };
                 let o;
@@ -288,15 +288,15 @@
                         }
                     }, e.message.client.initials))
                 } else o = i().createElement(c.Avatar, {
                     sx: {
                         ...r,
                         bgcolor: "var(--jp-jupyter-icon-color)"
                     }
-                }, i().createElement(T, {
+                }, i().createElement(R, {
                     display: "block",
                     height: "100%",
                     width: "100%"
                 }));
                 const a = "human" === e.message.type ? e.message.client.display_name : "Jupyternaut";
                 return i().createElement(c.Box, {
                     sx: {
@@ -348,15 +348,15 @@
                         }
                     }
                 }, e.messages.map(((e, n) => i().createElement(c.Box, {
                     key: n,
                     sx: {
                         padding: 4
                     }
-                }, i().createElement(R, {
+                }, i().createElement(T, {
                     message: e,
                     timestamp: t[e.id],
                     sx: {
                         marginBottom: 3
                     }
                 }), i().createElement(v(), {
                     className: "jp-RenderedHTMLCommon jp-ai-react-markdown",
@@ -382,15 +382,15 @@
                     onChange: t => e.onChange(t.target.value),
                     fullWidth: !0,
                     variant: "outlined",
                     multiline: !0,
                     onKeyDown: function(t) {
                         "Enter" === t.key && (e.sendWithShiftEnter && t.shiftKey || !e.sendWithShiftEnter && !t.shiftKey) && (e.onSend(), t.stopPropagation(), t.preventDefault())
                     },
-                    placeholder: "Ask Jupyternaut anything",
+                    placeholder: "Ask Jupyternaut",
                     InputProps: {
                         endAdornment: i().createElement(c.InputAdornment, {
                             position: "end"
                         }, i().createElement(c.IconButton, {
                             size: "small",
                             color: "primary",
                             onClick: e.onSend,
@@ -462,38 +462,48 @@
                 }
                 if (!o.ok) throw new J.ServerConnection.ResponseError(o, l.message || l);
                 return l
             }
 
             function $(e) {
                 var t, n;
+                const [r, o] = (0, l.useState)(null);
 
-                function r(t) {
+                function a(t) {
+                    if ("json" === e.field.format) try {
+                        JSON.parse(t.target.value), o(null)
+                    } catch (e) {
+                        o("You must specify a value in JSON format.")
+                    }
                     e.setConfig({
                         ...e.config,
                         fields: {
                             ...e.config.fields,
                             [e.gmid]: {
                                 ...e.config.fields[e.gmid],
                                 [e.field.key]: t.target.value
                             }
                         }
                     })
                 }
                 return "text" === e.field.type ? i().createElement(c.TextField, {
                     label: e.field.label,
                     value: null === (t = e.config.fields[e.gmid]) || void 0 === t ? void 0 : t[e.field.key],
-                    onChange: r,
+                    onChange: a,
+                    error: !!r,
+                    helperText: null != r ? r : void 0,
                     fullWidth: !0
                 }) : "text-multiline" === e.field.type ? i().createElement(c.TextField, {
                     label: e.field.label,
                     value: null === (n = e.config.fields[e.gmid]) || void 0 === n ? void 0 : n[e.field.key],
-                    onChange: r,
+                    onChange: a,
                     fullWidth: !0,
                     multiline: !0,
+                    error: !!r,
+                    helperText: null != r ? r : void 0,
                     minRows: 2
                 }) : i().createElement(i().Fragment, null)
             }
 
             function G(e) {
                 var t;
                 return (null === (t = e.fields) || void 0 === t ? void 0 : t.length) ? i().createElement(i().Fragment, null, e.fields.map(((t, n) => i().createElement($, Object.assign({}, e, {
@@ -507,36 +517,36 @@
             }
 
             function K(e, t) {
                 const n = U(e);
                 return t.providers.find((e => e.id === n))
             }
 
-            function Q() {
+            function Y() {
                 var e;
                 const [t, n] = (0, l.useState)(Z.Loading), [r, o] = (0, l.useState)(), [a, d] = (0, l.useState)(), [u, m] = (0, l.useState)(), [h, p] = (0, l.useState)(), [g, f] = (0, l.useState)({
                     model_provider_id: null,
                     embeddings_provider_id: null,
                     api_keys: {},
                     send_with_shift_enter: null,
                     fields: {}
-                }), [v, y] = (0, l.useState)(!1), [E, _] = (0, l.useState)(), [b, C] = (0, l.useState)(!1), [x, w] = (0, l.useState)("*"), S = (0, l.useMemo)((() => {
+                }), [v, y] = (0, l.useState)(!1), [E, _] = (0, l.useState)(), [b, x] = (0, l.useState)(!1), [C, S] = (0, l.useState)("*"), w = (0, l.useMemo)((() => {
                     if (g.model_provider_id && u) return K(g.model_provider_id, u)
-                }), [g.model_provider_id, u]), k = (0, l.useMemo)((() => g.model_provider_id && S ? (null == S ? void 0 : S.registry) ? `${S.id}:${x}` : g.model_provider_id : null), [g.model_provider_id, S, u, x]);
+                }), [g.model_provider_id, u]), k = (0, l.useMemo)((() => g.model_provider_id && w ? (null == w ? void 0 : w.registry) ? `${w.id}:${C}` : g.model_provider_id : null), [g.model_provider_id, w, u, C]);
                 return (0, l.useEffect)((() => {
                     !async function() {
                         try {
                             const [e, t, r] = await Promise.all([O.getConfig(), O.listLmProviders(), O.listEmProviders()]);
                             if (d(e), m(t), p(r), function(e, t) {
                                     var n, r;
                                     return null !== (r = null === (n = K(e, t)) || void 0 === n ? void 0 : n.registry) && void 0 !== r && r
                                 }(e.model_provider_id, t)) {
-                                C(!0);
+                                x(!0);
                                 const t = U(e.model_provider_id);
-                                w(function(e) {
+                                S(function(e) {
                                     if (!e) return null;
                                     const t = e.split(":");
                                     return t[t.length - 1]
                                 }(e.model_provider_id)), f({
                                     ...e,
                                     model_provider_id: `${t}:*`
                                 })
@@ -588,36 +598,36 @@
                     label: "Language model",
                     onChange: e => {
                         f((t => ({
                             ...t,
                             model_provider_id: e.target.value
                         })));
                         const t = K(e.target.value, u);
-                        (null == t ? void 0 : t.registry) ? (C(!0), w("*")) : C(!1)
+                        (null == t ? void 0 : t.registry) ? (x(!0), S("*")) : x(!1)
                     },
                     MenuProps: {
                         sx: {
                             maxHeight: "50%",
                             minHeight: 400
                         }
                     }
                 }, i().createElement(c.MenuItem, {
                     value: "null"
                 }, "None"), u.providers.map((e => e.models.map((t => i().createElement(c.MenuItem, {
                     value: `${e.id}:${t}`
                 }, e.name, " :: ", t)))))), b && i().createElement(c.TextField, {
                     label: "Local model ID",
-                    value: x,
-                    onChange: e => w(e.target.value),
+                    value: C,
+                    onChange: e => S(e.target.value),
                     fullWidth: !0
                 }), k && i().createElement(G, {
                     gmid: k,
                     config: g,
                     setConfig: f,
-                    fields: null == S ? void 0 : S.fields
+                    fields: null == w ? void 0 : w.fields
                 }), i().createElement("h2", {
                     className: "jp-ai-ChatSettings-header"
                 }, "Embedding model"), i().createElement(H, {
                     value: g.embeddings_provider_id,
                     label: "Embedding model",
                     onChange: e => f((t => ({
                         ...t,
@@ -713,30 +723,15 @@
                         padding: 4,
                         boxSizing: "border-box"
                     }
                 }, i().createElement(c.Alert, {
                     severity: "error"
                 }, r ? `An error occurred. Error details:\n\n${r}` : "An unknown error occurred. Check the console for more details."))
             }! function(e) {
-                e.sendPrompt = async function(e) {
-                    let t;
-                    try {
-                        t = await V("prompt", {
-                            method: "POST",
-                            body: JSON.stringify(e)
-                        })
-                    } catch (e) {
-                        return Promise.reject(e)
-                    }
-                    return t
-                }, e.listTasks = async function() {
-                    return V("tasks")
-                }, e.describeTask = async function(e) {
-                    return V(`tasks/${e}`)
-                }, e.getConfig = async function() {
+                e.getConfig = async function() {
                     return V("config")
                 }, e.listLmProviders = async function() {
                     return V("providers")
                 }, e.listEmProviders = async function() {
                     return V("providers/embeddings")
                 }, e.updateConfig = async function(e) {
                     return V("config", {
@@ -744,30 +739,30 @@
                         body: JSON.stringify(e)
                     })
                 }
             }(O || (O = {})),
             function(e) {
                 e[e.Loading = 0] = "Loading", e[e.Ready = 1] = "Ready", e[e.FetchError = 2] = "FetchError", e[e.SubmitError = 3] = "SubmitError", e[e.Success = 4] = "Success"
             }(Z || (Z = {}));
-            const Y = i().createContext([null, () => {}]);
+            const Q = i().createContext([null, () => {}]);
 
             function q({
                 selectionWatcher: e,
                 children: t
             }) {
                 const [n, r] = (0, l.useState)(null);
                 (0, l.useEffect)((() => {
                     e.selectionChanged.connect(((e, t) => {
                         r(t)
                     }))
                 }), []);
                 const o = (0, l.useCallback)((t => {
                     e.replaceSelection(t)
                 }), [e]);
-                return i().createElement(Y.Provider, {
+                return i().createElement(Q.Provider, {
                     value: [n, o]
                 }, t)
             }
 
             function X(e) {
                 const t = (0, l.useMemo)((() => "jupyter-ai-scroll-container-" + Date.now().toString()), []);
                 return (0, l.useEffect)((() => {
@@ -804,15 +799,15 @@
                 }))
             }
 
             function ee({
                 chatHandler: e,
                 setChatView: t
             }) {
-                const [n, r] = (0, l.useState)([]), [o, a] = (0, l.useState)(!1), [u, m] = (0, l.useState)(!0), [h, p] = (0, l.useState)(!1), [g, f] = (0, l.useState)(""), [v, y] = (0, l.useContext)(Y), [E, _] = (0, l.useState)(!0);
+                const [n, r] = (0, l.useState)([]), [o, a] = (0, l.useState)(!1), [u, m] = (0, l.useState)(!0), [h, p] = (0, l.useState)(!1), [g, f] = (0, l.useState)(""), [v, y] = (0, l.useContext)(Q), [E, _] = (0, l.useState)(!0);
                 return (0, l.useEffect)((() => {
                     !async function() {
                         var t;
                         try {
                             const [n, o] = await Promise.all([e.getHistory(), O.getConfig()]);
                             _(null !== (t = o.send_with_shift_enter) && void 0 !== t && t), r(n.messages), o.model_provider_id || a(!0)
                         } catch (e) {
@@ -833,15 +828,17 @@
                         display: "flex",
                         flexGrow: 1,
                         alignItems: "top",
                         justifyContent: "space-around"
                     }
                 }, i().createElement(c.Stack, {
                     spacing: 4
-                }, i().createElement("p", null, "Welcome to Jupyter AI! To get started, please select a language model to chat with from the settings panel. You will also likely need to provide API credentials, so be sure to have those handy."), i().createElement(c.Button, {
+                }, i().createElement("p", {
+                    className: "jp-ai-ChatSettings-welcome"
+                }, "Welcome to Jupyter AI! To get started, please select a language model to chat with from the settings panel. You may also need to provide API credentials, so have those handy."), i().createElement(c.Button, {
                     variant: "contained",
                     startIcon: i().createElement(d.Z, null),
                     size: "large",
                     onClick: () => (a(!1), void t(te.Settings))
                 }, "Start Here"))) : i().createElement(i().Fragment, null, i().createElement(X, {
                     sx: {
                         flexGrow: 1
@@ -912,15 +909,15 @@
                 }, t !== te.Chat ? i().createElement(c.IconButton, {
                     onClick: () => n(te.Chat)
                 }, i().createElement(u.Z, null)) : i().createElement(s.Z, null), t === te.Chat ? i().createElement(c.IconButton, {
                     onClick: () => n(te.Settings)
                 }, i().createElement(d.Z, null)) : i().createElement(s.Z, null)), t === te.Chat && i().createElement(ee, {
                     chatHandler: e.chatHandler,
                     setChatView: n
-                }), t === te.Settings && i().createElement(Q, null)))))
+                }), t === te.Settings && i().createElement(Y, null)))))
             }! function(e) {
                 e[e.Chat = 0] = "Chat", e[e.Settings = 1] = "Settings"
             }(te || (te = {}));
             var re = n(68020),
                 oe = n(59235),
                 le = n(40763),
                 ie = n(80127),
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/643.23e0a9c561346f879c77.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/643.830710e1337b7cf4cbdd.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -5,30 +5,30 @@
             t.d(n, {
                 Z: () => l
             });
             var r = t(82609),
                 i = t.n(r),
                 o = t(83055),
                 a = t(98814),
-                s = t(22299),
-                c = i()((function(e) {
+                c = t(22299),
+                s = i()((function(e) {
                     return e[1]
                 }));
-            c.i(o.Z), c.i(a.Z), c.i(s.Z), c.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n", ""]);
-            const l = c
+            s.i(o.Z), s.i(a.Z), s.i(c.Z), s.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n", ""]);
+            const l = s
         },
         22299: (e, n, t) => {
             t.d(n, {
                 Z: () => o
             });
             var r = t(82609),
                 i = t.n(r)()((function(e) {
                     return e[1]
                 }));
-            i.push([e.id, ".jp-ai-ChatSettings-header {\n  font-size: var(--jp-ui-font-size3);\n  font-weight: 400;\n  color: var(--jp-ui-font-color1);\n}\n", ""]);
+            i.push([e.id, ".jp-ai-ChatSettings-header {\n  font-size: var(--jp-ui-font-size3);\n  font-weight: 400;\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-ai-ChatSettings-welcome {\n  color: var(--jp-ui-font-color1);\n}\n", ""]);
             const o = i
         },
         83055: (e, n, t) => {
             t.d(n, {
                 Z: () => o
             });
             var r = t(82609),
@@ -42,15 +42,15 @@
             t.d(n, {
                 Z: () => o
             });
             var r = t(82609),
                 i = t.n(r)()((function(e) {
                     return e[1]
                 }));
-            i.push([e.id, ".jp-RenderedHTMLCommon.jp-ai-react-markdown > pre {\n  margin: 0;\n}\n\n.jp-RenderedHTMLCommon.jp-ai-react-markdown {\n  padding: 0;\n}\n\n/* !important specifier required to override inline styles from Prism */\n.jp-ai-code {\n  font-family: var(--jp-code-font-family) !important;\n  font-size: var(--jp-code-font-size) !important;\n  line-height: var(--jp-code-line-height) !important;\n}\n", ""]);
+            i.push([e.id, ".jp-RenderedHTMLCommon.jp-ai-react-markdown > pre {\n  margin: 0;\n}\n\n.jp-RenderedHTMLCommon.jp-ai-react-markdown {\n  padding: 0;\n}\n\n.jp-RenderedHTMLCommon.jp-ai-react-markdown ul:not(.list-inline) {\n  padding-left: 1em;\n}\n\n/* !important specifier required to override inline styles from Prism */\n.jp-ai-code {\n  font-family: var(--jp-code-font-family) !important;\n  font-size: var(--jp-code-font-size) !important;\n  line-height: var(--jp-code-line-height) !important;\n}\n", ""]);
             const o = i
         },
         82609: e => {
             e.exports = function(e) {
                 var n = [];
                 return n.toString = function() {
                     return this.map((function(n) {
@@ -63,17 +63,17 @@
                     ]);
                     var i = {};
                     if (r)
                         for (var o = 0; o < this.length; o++) {
                             var a = this[o][0];
                             null != a && (i[a] = !0)
                         }
-                    for (var s = 0; s < e.length; s++) {
-                        var c = [].concat(e[s]);
-                        r && i[c[0]] || (t && (c[2] ? c[2] = "".concat(t, " and ").concat(c[2]) : c[2] = t), n.push(c))
+                    for (var c = 0; c < e.length; c++) {
+                        var s = [].concat(e[c]);
+                        r && i[s[0]] || (t && (s[2] ? s[2] = "".concat(t, " and ").concat(s[2]) : s[2] = t), n.push(s))
                     }
                 }, n
             }
         },
         46062: (e, n, t) => {
             var r, i = function() {
                     var e = {};
@@ -96,36 +96,36 @@
                 for (var n = -1, t = 0; t < o.length; t++)
                     if (o[t].identifier === e) {
                         n = t;
                         break
                     } return n
             }
 
-            function s(e, n) {
+            function c(e, n) {
                 for (var t = {}, r = [], i = 0; i < e.length; i++) {
-                    var s = e[i],
-                        c = n.base ? s[0] + n.base : s[0],
-                        l = t[c] || 0,
-                        d = "".concat(c, " ").concat(l);
-                    t[c] = l + 1;
+                    var c = e[i],
+                        s = n.base ? c[0] + n.base : c[0],
+                        l = t[s] || 0,
+                        d = "".concat(s, " ").concat(l);
+                    t[s] = l + 1;
                     var u = a(d),
                         f = {
-                            css: s[1],
-                            media: s[2],
-                            sourceMap: s[3]
+                            css: c[1],
+                            media: c[2],
+                            sourceMap: c[3]
                         }; - 1 !== u ? (o[u].references++, o[u].updater(f)) : o.push({
                         identifier: d,
                         updater: h(f, n),
                         references: 1
                     }), r.push(d)
                 }
                 return r
             }
 
-            function c(e) {
+            function s(e) {
                 var n = document.createElement("style"),
                     r = e.attributes || {};
                 if (void 0 === r.nonce) {
                     var o = t.nc;
                     o && (r.nonce = o)
                 }
                 if (Object.keys(r).forEach((function(e) {
@@ -165,16 +165,16 @@
             var p = null,
                 v = 0;
 
             function h(e, n) {
                 var t, r, i;
                 if (n.singleton) {
                     var o = v++;
-                    t = p || (p = c(n)), r = u.bind(null, t, o, !1), i = u.bind(null, t, o, !0)
-                } else t = c(n), r = f.bind(null, t, n), i = function() {
+                    t = p || (p = s(n)), r = u.bind(null, t, o, !1), i = u.bind(null, t, o, !0)
+                } else t = s(n), r = f.bind(null, t, n), i = function() {
                     ! function(e) {
                         if (null === e.parentNode) return !1;
                         e.parentNode.removeChild(e)
                     }(t)
                 };
                 return r(e),
                     function(n) {
@@ -182,26 +182,26 @@
                             if (n.css === e.css && n.media === e.media && n.sourceMap === e.sourceMap) return;
                             r(e = n)
                         } else i()
                     }
             }
             e.exports = function(e, n) {
                 (n = n || {}).singleton || "boolean" == typeof n.singleton || (n.singleton = (void 0 === r && (r = Boolean(window && document && document.all && !window.atob)), r));
-                var t = s(e = e || [], n);
+                var t = c(e = e || [], n);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
                         for (var r = 0; r < t.length; r++) {
                             var i = a(t[r]);
                             o[i].references--
                         }
-                        for (var c = s(e, n), l = 0; l < t.length; l++) {
+                        for (var s = c(e, n), l = 0; l < t.length; l++) {
                             var d = a(t[l]);
                             0 === o[d].references && (o[d].updater(), o.splice(d, 1))
                         }
-                        t = c
+                        t = s
                     }
                 }
             }
         },
         76643: (e, n, t) => {
             t.r(n);
             var r = t(46062),
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/remoteEntry.9095dd2e94ae47ffc04b.js` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/remoteEntry.a695d82eb8238716e13d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, f, u, c, d, s, p, h, b, m, v, y, g, j, P, w, k, _, O, S = {
+    var e, r, t, a, o, n, i, f, l, c, u, d, s, p, h, b, m, v, y, g, j, P, w, k, _, O, S = {
             22399: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(253)]).then((() => () => t(30253))),
                         "./extension": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(253)]).then((() => () => t(30253))),
                         "./style": () => t.e(643).then((() => () => t(76643)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -56,49 +56,49 @@
         return n.default = () => t, x.d(o, n), o
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
-        253: "4cb04dcfead6f07b8e7c",
+        253: "5c9df1561a4c4c0223da",
         271: "69215afaecf754ef22b8",
         296: "c1fab29ee6698d164796",
         341: "f8070bd4be2814acfc0d",
         342: "d3a98882c7231544e992",
         365: "d20799d043a171f06d37",
         380: "367f93b5ced659dcbadd",
         407: "6b1f897f3ceb4355d6ac",
         456: "3766abc0ca49db318bcd",
         527: "96409770f04a31a6ae7e",
         564: "43eaeac5fe02580e918d",
         598: "168be006d4b42d34521a",
-        643: "23e0a9c561346f879c77",
+        643: "830710e1337b7cf4cbdd",
         675: "e2778aeb06575c94bca0",
         693: "970d9a45469683adfff5",
         703: "3d0d8b7012529f0dd511",
         819: "5279f5daf1d1f505f15f",
         860: "03421bb262ea8bfa0af1",
         861: "c7c12ea31e8b5552473d",
         900: "899d3fbf00938382f665",
         963: "59c8f2feb6aaf0b34378"
     } [e] + ".js?v=" + {
-        253: "4cb04dcfead6f07b8e7c",
+        253: "5c9df1561a4c4c0223da",
         271: "69215afaecf754ef22b8",
         296: "c1fab29ee6698d164796",
         341: "f8070bd4be2814acfc0d",
         342: "d3a98882c7231544e992",
         365: "d20799d043a171f06d37",
         380: "367f93b5ced659dcbadd",
         407: "6b1f897f3ceb4355d6ac",
         456: "3766abc0ca49db318bcd",
         527: "96409770f04a31a6ae7e",
         564: "43eaeac5fe02580e918d",
         598: "168be006d4b42d34521a",
-        643: "23e0a9c561346f879c77",
+        643: "830710e1337b7cf4cbdd",
         675: "e2778aeb06575c94bca0",
         693: "970d9a45469683adfff5",
         703: "3d0d8b7012529f0dd511",
         819: "5279f5daf1d1f505f15f",
         860: "03421bb262ea8bfa0af1",
         861: "c7c12ea31e8b5552473d",
         900: "899d3fbf00938382f665",
@@ -109,34 +109,34 @@
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupyter-ai/core:", x.l = (e, r, o, n) => {
         if (t[e]) t[e].push(r);
         else {
-            var i, l;
+            var i, f;
             if (void 0 !== o)
-                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
-                    var c = f[u];
-                    if (c.getAttribute("src") == e || c.getAttribute("data-webpack") == a + o) {
-                        i = c;
+                for (var l = document.getElementsByTagName("script"), c = 0; c < l.length; c++) {
+                    var u = l[c];
+                    if (u.getAttribute("src") == e || u.getAttribute("data-webpack") == a + o) {
+                        i = u;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
+            i || (f = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
             var d = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var o = t[e];
                     if (delete t[e], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
                 s = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), f && document.head.appendChild(i)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -148,25 +148,25 @@
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
                 x.o(x.S, t) || (x.S[t] = {});
                 var n = x.S[t],
                     i = "@jupyter-ai/core",
-                    l = (e, r, t, a) => {
+                    f = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
+                            f = o[r];
+                        (!f || !f.loaded && (!a != !f.eager ? a : i > f.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    f = [];
-                return "default" === t && (l("@emotion/react", "11.11.0", (() => Promise.all([x.e(296), x.e(527), x.e(271), x.e(342)]).then((() => () => x(26527))))), l("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(271), x.e(564), x.e(407)]).then((() => () => x(52675))))), l("@jupyter-ai/core", "0.9.0", (() => Promise.all([x.e(341), x.e(380), x.e(271), x.e(963), x.e(253)]).then((() => () => x(30253))))), l("@mui/material", "5.13.1", (() => Promise.all([x.e(296), x.e(860), x.e(341), x.e(271), x.e(564), x.e(963), x.e(456)]).then((() => () => x(30860))))), l("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(271)]).then((() => () => x(81861))))), l("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(271)]).then((() => () => x(95598))))), l("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), l("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (f("@emotion/react", "11.11.0", (() => Promise.all([x.e(296), x.e(527), x.e(271), x.e(342)]).then((() => () => x(26527))))), f("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(271), x.e(564), x.e(407)]).then((() => () => x(52675))))), f("@jupyter-ai/core", "1.0.0", (() => Promise.all([x.e(341), x.e(380), x.e(271), x.e(963), x.e(253)]).then((() => () => x(30253))))), f("@mui/material", "5.13.1", (() => Promise.all([x.e(296), x.e(860), x.e(341), x.e(271), x.e(564), x.e(963), x.e(456)]).then((() => () => x(30860))))), f("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(271)]).then((() => () => x(81861))))), f("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(271)]).then((() => () => x(95598))))), f("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), f("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,100 +185,100 @@
         e = o(e), r = o(r);
         for (var t = 0;;) {
             if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
             var a = e[t],
                 n = (typeof a)[0];
             if (t >= r.length) return "u" == n;
             var i = r[t],
-                l = (typeof i)[0];
-            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
+                f = (typeof i)[0];
+            if (n != f) return "o" == n && "n" == f || "s" == f || "u" == n;
             if ("o" != n && "u" != n && a != i) return a < i;
             t++
         }
     }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(f = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, f);
             return t
         }
         var n = [];
         for (o = 1; o < e.length; o++) {
-            var l = e[o];
-            n.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? n.pop() + " " + n.pop() : i(l))
+            var f = e[o];
+            n.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? n.pop() + " " + n.pop() : i(f))
         }
-        return f();
+        return l();
 
-        function f() {
+        function l() {
             return n.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, l = (e, r) => {
+    }, f = (e, r) => {
         if (0 in e) {
             r = o(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
-            for (var n = 0, i = 1, f = !0;; i++, n++) {
-                var u, c, d = i < e.length ? (typeof e[i])[0] : "";
-                if (n >= r.length || "o" == (c = (typeof(u = r[n]))[0])) return !f || ("u" == d ? i > t && !a : "" == d != a);
-                if ("u" == c) {
-                    if (!f || "u" != d) return !1
-                } else if (f)
-                    if (d == c)
+            for (var n = 0, i = 1, l = !0;; i++, n++) {
+                var c, u, d = i < e.length ? (typeof e[i])[0] : "";
+                if (n >= r.length || "o" == (u = (typeof(c = r[n]))[0])) return !l || ("u" == d ? i > t && !a : "" == d != a);
+                if ("u" == u) {
+                    if (!l || "u" != d) return !1
+                } else if (l)
+                    if (d == u)
                         if (i <= t) {
-                            if (u != e[i]) return !1
+                            if (c != e[i]) return !1
                         } else {
-                            if (a ? u > e[i] : u < e[i]) return !1;
-                            u != e[i] && (f = !1)
+                            if (a ? c > e[i] : c < e[i]) return !1;
+                            c != e[i] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (a || i <= t) return !1;
-                    f = !1, i--
+                    l = !1, i--
                 } else {
-                    if (i <= t || c < d != a) return !1;
-                    f = !1
-                } else "s" != d && "n" != d && (f = !1, i--)
+                    if (i <= t || u < d != a) return !1;
+                    l = !1
+                } else "s" != d && "n" != d && (l = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (n = 1; n < e.length; n++) {
             var h = e[n];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? l(h, r) : !p())
+            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? f(h, r) : !p())
         }
         return !!p()
-    }, f = (e, r) => {
+    }, l = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, u = (e, r) => {
+    }, c = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
-    }, c = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(a) + ")", s = (e, r, t, a) => {
-        var o = c(e, t);
-        return l(a, o) || b(d(e, t, o, a)), v(e[t][o])
+        var o = u(e, t);
+        return f(a, o) || b(d(e, t, o, a)), v(e[t][o])
     }, p = (e, r, t) => {
         var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !l(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+        return (r = Object.keys(a).reduce(((e, r) => !f(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, h = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + i(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, m = (e, r, t, a) => {
         b(h(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), g = (y = e => function(r, t, a, o) {
         var n = x.I(r);
         return n && n.then ? n.then(e.bind(e, r, x.S[r], t, a, o)) : e(r, x.S[r], t, a, o)
-    })(((e, r, t, a) => r && x.o(r, t) ? v(u(r, t)) : a())), j = y(((e, r, t, a) => (f(e, t), v(p(r, t, a) || m(r, e, t, a) || u(r, t))))), P = y(((e, r, t, a) => (f(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
+    })(((e, r, t, a) => r && x.o(r, t) ? v(c(r, t)) : a())), j = y(((e, r, t, a) => (l(e, t), v(p(r, t, a) || m(r, e, t, a) || c(r, t))))), P = y(((e, r, t, a) => (l(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
         var n = r && x.o(r, t) && p(r, t, a);
         return n ? v(n) : o()
     })), k = {}, _ = {
         56271: () => P("default", "react", [1, 17, 0, 1]),
         79510: () => w("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([x.e(296), x.e(527), x.e(365)]).then((() => () => x(26527))))),
         92764: () => w("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([x.e(675), x.e(564), x.e(407)]).then((() => () => x(52675))))),
         344: () => P("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
@@ -348,21 +348,21 @@
                             n = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, i, l] = t,
-                    f = 0;
+                var a, o, [n, i, f] = t,
+                    l = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in i) x.o(i, a) && (x.m[a] = i[a]);
-                    l && l(x)
+                    f && f(x)
                 }
-                for (r && r(t); f < n.length; f++) o = n[f], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < n.length; l++) o = n[l], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), x.nc = void 0;
     var T = x(22399);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter-ai/core"] = T
 })();
```

### Comparing `jupyter_ai-0.9.0/jupyter_ai/labextension/static/third-party-licenses.json` & `jupyter_ai-1.0.0/jupyter_ai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/schema/plugin.json` & `jupyter_ai-1.0.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/chat_handler.ts` & `jupyter_ai-1.0.0/src/chat_handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/handler.ts` & `jupyter_ai-1.0.0/src/handler.ts`

 * *Files 18% similar despite different names*

```diff
@@ -47,23 +47,14 @@
   /**
    * The instantiation options for a data registry handler.
    */
   export interface IOptions {
     serverSettings?: ServerConnection.ISettings;
   }
 
-  export interface IPromptRequest {
-    task_id: string;
-    engine_id: string;
-    prompt_variables: {
-      body: string;
-      [key: string]: string;
-    };
-  }
-
   export type ChatRequest = {
     prompt: string;
   };
 
   export type Collaborator = {
     username: string;
     initials: string;
@@ -109,66 +100,14 @@
     | ConnectionMessage
     | ClearMessage;
 
   export type ChatHistory = {
     messages: ChatMessage[];
   };
 
-  export interface IPromptResponse {
-    output: string;
-    insertion_mode: 'above' | 'below' | 'replace';
-  }
-
-  export async function sendPrompt(
-    request: IPromptRequest
-  ): Promise<IPromptResponse> {
-    let data;
-
-    try {
-      data = await requestAPI('prompt', {
-        method: 'POST',
-        body: JSON.stringify(request)
-      });
-    } catch (e) {
-      return Promise.reject(e);
-    }
-    return data as IPromptResponse;
-  }
-
-  export type ListTasksEntry = {
-    id: string;
-    name: string;
-  };
-
-  export type ListTasksResponse = {
-    tasks: ListTasksEntry[];
-  };
-
-  export async function listTasks(): Promise<ListTasksResponse> {
-    return requestAPI<ListTasksResponse>('tasks');
-  }
-
-  export type ListEnginesEntry = {
-    id: string;
-    name: string;
-  };
-
-  export type DescribeTaskResponse = {
-    name: string;
-    insertion_mode: string;
-    prompt_template: string;
-    engines: ListEnginesEntry[];
-  };
-
-  export async function describeTask(
-    id: string
-  ): Promise<DescribeTaskResponse> {
-    return requestAPI<DescribeTaskResponse>(`tasks/${id}`);
-  }
-
   export type Config = {
     model_provider_id: string | null;
     embeddings_provider_id: string | null;
     api_keys: Record<string, string>;
     send_with_shift_enter: boolean | null;
     fields: Record<string, Record<string, any>>;
   };
@@ -192,20 +131,22 @@
 
   export type AuthStrategy = EnvAuthStrategy | AwsAuthStrategy | null;
 
   export type TextField = {
     type: 'text';
     key: string;
     label: string;
+    format: string;
   };
 
   export type MultilineTextField = {
     type: 'text-multiline';
     key: string;
     label: string;
+    format: string;
   };
 
   export type Field = TextField | MultilineTextField;
 
   export type ListProvidersEntry = {
     id: string;
     name: string;
```

### Comparing `jupyter_ai-0.9.0/src/icons.ts` & `jupyter_ai-1.0.0/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/index.ts` & `jupyter_ai-1.0.0/src/index.ts`

 * *Files 12% similar despite different names*

```diff
@@ -57,8 +57,7 @@
     if (restorer) {
       restorer.add(chatWidget, 'jupyter-ai-chat');
     }
   }
 };
 
 export default plugin;
-export type { InsertionContext } from './inserter';
```

### Comparing `jupyter_ai-0.9.0/src/selection-watcher.ts` & `jupyter_ai-1.0.0/src/selection-watcher.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/theme-provider.ts` & `jupyter_ai-1.0.0/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/utils.ts` & `jupyter_ai-1.0.0/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/components/chat-code-view.tsx` & `jupyter_ai-1.0.0/src/components/chat-code-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/components/chat-input.tsx` & `jupyter_ai-1.0.0/src/components/chat-input.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         <TextField
           value={props.value}
           onChange={e => props.onChange(e.target.value)}
           fullWidth
           variant="outlined"
           multiline
           onKeyDown={handleKeyDown}
-          placeholder="Ask Jupyternaut anything"
+          placeholder="Ask Jupyternaut"
           InputProps={{
             endAdornment: (
               <InputAdornment position="end">
                 <IconButton
                   size="small"
                   color="primary"
                   onClick={props.onSend}
```

### Comparing `jupyter_ai-0.9.0/src/components/chat-messages.tsx` & `jupyter_ai-1.0.0/src/components/chat-messages.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/components/chat-settings.tsx` & `jupyter_ai-1.0.0/src/components/chat-settings.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/components/chat.tsx` & `jupyter_ai-1.0.0/src/components/chat.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -121,18 +121,18 @@
           display: 'flex',
           flexGrow: 1,
           alignItems: 'top',
           justifyContent: 'space-around'
         }}
       >
         <Stack spacing={4}>
-          <p>
+          <p className="jp-ai-ChatSettings-welcome">
             Welcome to Jupyter AI! To get started, please select a language
-            model to chat with from the settings panel. You will also likely
-            need to provide API credentials, so be sure to have those handy.
+            model to chat with from the settings panel. You may also need to
+            provide API credentials, so have those handy.
           </p>
           <Button
             variant="contained"
             startIcon={<SettingsIcon />}
             size={'large'}
             onClick={() => openSettingsView()}
           >
```

### Comparing `jupyter_ai-0.9.0/src/components/expandable-text-field.tsx` & `jupyter_ai-1.0.0/src/components/expandable-text-field.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/components/jl-theme-provider.tsx` & `jupyter_ai-1.0.0/src/components/jl-theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/components/scroll-container.tsx` & `jupyter_ai-1.0.0/src/components/scroll-container.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/components/select.tsx` & `jupyter_ai-1.0.0/src/components/select.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/components/settings/model-fields.tsx` & `jupyter_ai-1.0.0/src/components/settings/model-fields.tsx`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,46 @@
-import React from 'react';
+import React, { useState } from 'react';
 import { AiService } from '../../handler';
 import { TextField } from '@mui/material';
 
 export type ModelFieldProps = {
   /**
    * The global model ID to which these fields belong.
    */
   gmid: string;
   field: AiService.Field;
   config: AiService.Config;
   setConfig: (newConfig: AiService.Config) => unknown;
 };
 
 export function ModelField(props: ModelFieldProps): JSX.Element {
+  const [errorMessage, setErrorMessage] = useState<string | null>(null);
+
   function handleChange(
     e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>
   ) {
+    // Perform validation based on the field format
+    switch (props.field.format) {
+      case 'json':
+        try {
+          // JSON.parse does not allow single quotes or trailing commas
+          JSON.parse(e.target.value);
+          setErrorMessage(null);
+        } catch (exc) {
+          setErrorMessage('You must specify a value in JSON format.');
+        }
+        break;
+      case 'jsonpath':
+        // TODO: Do JSONPath validation
+        break;
+      default:
+        // No validation performed
+        break;
+    }
+
     props.setConfig({
       ...props.config,
       fields: {
         ...props.config.fields,
         [props.gmid]: {
           ...props.config.fields[props.gmid],
           [props.field.key]: e.target.value
@@ -30,27 +51,31 @@
 
   if (props.field.type === 'text') {
     return (
       <TextField
         label={props.field.label}
         value={props.config.fields[props.gmid]?.[props.field.key]}
         onChange={handleChange}
+        error={!!errorMessage}
+        helperText={errorMessage ?? undefined}
         fullWidth
       />
     );
   }
 
   if (props.field.type === 'text-multiline') {
     return (
       <TextField
         label={props.field.label}
         value={props.config.fields[props.gmid]?.[props.field.key]}
         onChange={handleChange}
         fullWidth
         multiline
+        error={!!errorMessage}
+        helperText={errorMessage ?? undefined}
         minRows={2}
       />
     );
   }
 
   return <></>;
 }
```

### Comparing `jupyter_ai-0.9.0/src/contexts/collaborators-context.tsx` & `jupyter_ai-1.0.0/src/contexts/collaborators-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/contexts/selection-context.tsx` & `jupyter_ai-1.0.0/src/contexts/selection-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/widgets/chat-error.tsx` & `jupyter_ai-1.0.0/src/widgets/chat-error.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/src/widgets/chat-sidebar.tsx` & `jupyter_ai-1.0.0/src/widgets/chat-sidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/style/icons/jupyternaut.svg` & `jupyter_ai-1.0.0/style/icons/jupyternaut.svg`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/ui-tests/README.md` & `jupyter_ai-1.0.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/ui-tests/jupyter_server_test_config.py` & `jupyter_ai-1.0.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/ui-tests/tests/jupyter_ai.spec.ts` & `jupyter_ai-1.0.0/ui-tests/tests/jupyter_ai.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/.gitignore` & `jupyter_ai-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/LICENSE` & `jupyter_ai-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.9.0/README.md` & `jupyter_ai-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -12,65 +12,34 @@
 - JupyterLab >= 3.5 (not JupyterLab 4)
 - Jupyter Server >= 2.0.0
 
 ## Installation
 
 You can use `conda` or `pip` to install Jupyter AI. If you're using macOS on an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), we strongly recommend using `conda`.
 
-Because of Ray's incompatibility with Python 3.11, you must use Python 3.9, or 3.10 with Jupyter AI. The instructions below presume that you are using Python 3.10.
-
 Before you can use Jupyter AI, you will need to install any packages and set environment variables with API keys for the model providers that you will use. See [our documentation](https://jupyter-ai.readthedocs.io/en/latest/users/index.html) for details about what you'll need.
 
 ### With pip
 
     $ pip install jupyter_ai
 
 ### With conda
 
-First, install [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) and create an environment that uses Python 3.10:
+First, install [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) and create an environment that uses Python 3.11:
 
-    $ conda create -n jupyter-ai python=3.10
+    $ conda create -n jupyter-ai python=3.11
     $ conda activate jupyter-ai
     $ pip install jupyter_ai
 
-If you are using an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), you need to uninstall the `pip` provided version of `grpcio` and install the version provided by `conda` instead.
-
-    $ pip uninstall grpcio; conda install grpcio
-
 ## Uninstall
 
 To remove the extension, execute:
 
     $ pip uninstall jupyter_ai
 
-## Usage with GPT-3
-
-To use the `GPT3ModelEngine` in `jupyter_ai`, you will need an OpenAI API key.
-Copy the API key and then create a Jupyter config file locally at `config.py` to
-store the API key.
-
-```python
-c.GPT3ModelEngine.api_key = "<your-api-key>"
-```
-
-Finally, start a new JupyterLab instance pointing to this configuration file.
-
-```bash
-jupyter lab --config=config.py
-```
-
-If you are doing this in a Git repository, you can ensure you never commit this
-file on accident by adding it to `.git/info/exclude`.
-
-Alternately, you can also specify your API key while launching JupyterLab.
-
-```bash
-jupyter lab --GPT3ModelEngine.api_key=<api-key>
-```
-
 ## Troubleshoot
 
 If you can see the extension UI, but it is not working, check
 that the server extension is enabled:
 
 ```bash
 jupyter server extension list
```

### Comparing `jupyter_ai-0.9.0/pyproject.toml` & `jupyter_ai-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,48 +2,46 @@
 requires = ["hatchling>=1.4.0", "jupyterlab>=3.4.7,<4.0.0", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_ai"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.8,<3.11"
+requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 3",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "jupyter_server>=1.6,<3",
     "jupyterlab>=3.5,<4",
     "pydantic",
     "openai~=0.26",
     "aiosqlite~=0.18",
     "importlib_metadata~=5.2.0",
-    "langchain==0.0.159",
+    "langchain==0.0.220",
     "tiktoken", # required for OpenAIEmbeddings
     "jupyter_ai_magics",
-    "ray~=2.4.0", # Requires grpcio installation from conda
+    "dask[distributed]",
     "faiss-cpu", # Not distributed by official repo
     "typing_extensions==4.5.0"
 ]
 
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
-[project.entry-points."jupyter_ai.model_engine_classes"]
-gpt3 = "jupyter_ai:GPT3ModelEngine"
-
 [project.entry-points."jupyter_ai.default_tasks"]
 core_default_tasks = "jupyter_ai:tasks"
 
 [project.optional-dependencies]
 test = [
     "jupyter-server[test]>=1.6,<3",
     "coverage",
```

### Comparing `jupyter_ai-0.9.0/PKG-INFO` & `jupyter_ai-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai
-Version: 0.9.0
+Version: 1.0.0
 Summary: A generative AI extension for JupyterLab
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -43,25 +43,26 @@
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Requires-Dist: aiosqlite~=0.18
+Requires-Dist: dask[distributed]
 Requires-Dist: faiss-cpu
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: jupyter-ai-magics
 Requires-Dist: jupyter-server<3,>=1.6
 Requires-Dist: jupyterlab<4,>=3.5
-Requires-Dist: langchain==0.0.159
+Requires-Dist: langchain==0.0.220
 Requires-Dist: openai~=0.26
 Requires-Dist: pydantic
-Requires-Dist: ray~=2.4.0
 Requires-Dist: tiktoken
 Requires-Dist: typing-extensions==4.5.0
 Provides-Extra: all
 Requires-Dist: jupyter-ai-magics[all]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: jupyter-ai-magics[dev]; extra == 'dev'
 Provides-Extra: test
@@ -87,65 +88,34 @@
 - JupyterLab >= 3.5 (not JupyterLab 4)
 - Jupyter Server >= 2.0.0
 
 ## Installation
 
 You can use `conda` or `pip` to install Jupyter AI. If you're using macOS on an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), we strongly recommend using `conda`.
 
-Because of Ray's incompatibility with Python 3.11, you must use Python 3.9, or 3.10 with Jupyter AI. The instructions below presume that you are using Python 3.10.
-
 Before you can use Jupyter AI, you will need to install any packages and set environment variables with API keys for the model providers that you will use. See [our documentation](https://jupyter-ai.readthedocs.io/en/latest/users/index.html) for details about what you'll need.
 
 ### With pip
 
     $ pip install jupyter_ai
 
 ### With conda
 
-First, install [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) and create an environment that uses Python 3.10:
+First, install [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) and create an environment that uses Python 3.11:
 
-    $ conda create -n jupyter-ai python=3.10
+    $ conda create -n jupyter-ai python=3.11
     $ conda activate jupyter-ai
     $ pip install jupyter_ai
 
-If you are using an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), you need to uninstall the `pip` provided version of `grpcio` and install the version provided by `conda` instead.
-
-    $ pip uninstall grpcio; conda install grpcio
-
 ## Uninstall
 
 To remove the extension, execute:
 
     $ pip uninstall jupyter_ai
 
-## Usage with GPT-3
-
-To use the `GPT3ModelEngine` in `jupyter_ai`, you will need an OpenAI API key.
-Copy the API key and then create a Jupyter config file locally at `config.py` to
-store the API key.
-
-```python
-c.GPT3ModelEngine.api_key = "<your-api-key>"
-```
-
-Finally, start a new JupyterLab instance pointing to this configuration file.
-
-```bash
-jupyter lab --config=config.py
-```
-
-If you are doing this in a Git repository, you can ensure you never commit this
-file on accident by adding it to `.git/info/exclude`.
-
-Alternately, you can also specify your API key while launching JupyterLab.
-
-```bash
-jupyter lab --GPT3ModelEngine.api_key=<api-key>
-```
-
 ## Troubleshoot
 
 If you can see the extension UI, but it is not working, check
 that the server extension is enabled:
 
 ```bash
 jupyter server extension list
```

