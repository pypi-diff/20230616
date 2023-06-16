# Comparing `tmp/jupyter_ai-0.7.3.tar.gz` & `tmp/jupyter_ai-0.8.0.tar.gz`

## Comparing `jupyter_ai-0.7.3.tar` & `jupyter_ai-0.8.0.tar`

### file list

```diff
@@ -1,161 +1,163 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.eslintignore
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/CHANGELOG.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/babel.config.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jest.config.js
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/package.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/project.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/tsconfig.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter-config/nb-config/jupyter_ai.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter-config/server-config/jupyter_ai.json
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/_version.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/engine.py
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/extension.py
--rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/handlers.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/models.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/reply_processor.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/task_manager.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/tasks.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/ask.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/base.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/chat_provider.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/config.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/default.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/embeddings_provider.py
--rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/generate.py
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/learn.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/memory.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/providers.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/actors/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/document_loaders/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/document_loaders/directory.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/document_loaders/splitter.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/package.json
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
--rw-r--r--   0        0        0    41113 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js.LICENSE.txt
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js
--rw-r--r--   0        0        0   157509 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js.LICENSE.txt
--rw-r--r--   0        0        0  1568438 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js.LICENSE.txt
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
--rw-r--r--   0        0        0    23774 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/639.b63fa10cbcf2eccddd7d.js
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/643.d05f12a52798d8475b12.js
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
--rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
--rw-r--r--   0        0        0   443772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js.LICENSE.txt
--rw-r--r--   0        0        0    91736 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js.LICENSE.txt
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
--rw-r--r--   0        0        0   272943 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/900.aad7c14c6d8f76011810.js
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
--rw-r--r--   0        0        0    11319 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/remoteEntry.df84a6245b68ae8abd9f.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/style.js
--rw-r--r--   0        0        0   111460 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/tests/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/jupyter_ai/tests/test_handlers.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/schema/plugin.json
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/chat_handler.ts
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/handler.ts
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/icons.ts
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/index.ts
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/inserter.ts
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/selection-watcher.ts
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/theme-provider.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/utils.ts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/__tests__/jupyter_gai.spec.ts
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/__tests__/widgets/closable-dialog.spec.tsx
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat-code-view.tsx
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat-input.tsx
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat-messages.tsx
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat-settings.tsx
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/chat.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/expandable-text-field.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/jl-theme-provider.tsx
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/open-task-dialog.tsx
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/scroll-container.tsx
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/components/select.tsx
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/contexts/collaborators-context.tsx
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/contexts/selection-context.tsx
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/types/mui.d.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/types/svg.d.ts
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/widgets/chat-error.tsx
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/widgets/chat-sidebar.tsx
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/src/widgets/closable-dialog.tsx
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/base.css
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/expandable-text-field.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/index.js
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/react-markdown.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/icons/chat.svg
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/style/icons/jupyternaut.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/ui-tests/tests/jupyter_ai.spec.ts
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/LICENSE
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/README.md
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 jupyter_ai-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.eslintignore
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/babel.config.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/conftest.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jest.config.js
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/package.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/project.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/tsconfig.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter-config/nb-config/jupyter_ai.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter-config/server-config/jupyter_ai.json
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/_version.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/engine.py
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/extension.py
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/handlers.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/models.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/reply_processor.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/task_manager.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/tasks.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/ask.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/base.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/chat_provider.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/config.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/default.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/embeddings_provider.py
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/generate.py
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/learn.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/memory.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/providers.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/document_loaders/directory.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/document_loaders/splitter.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/package.json
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
+-rw-r--r--   0        0        0    26351 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/253.0b5d158f3577d0bfbee5.js
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
+-rw-r--r--   0        0        0    41113 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js.LICENSE.txt
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js
+-rw-r--r--   0        0        0   157509 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js.LICENSE.txt
+-rw-r--r--   0        0        0  1568438 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js.LICENSE.txt
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/643.ca949b2ea9d252cbcc23.js
+-rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
+-rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
+-rw-r--r--   0        0        0   443772 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js.LICENSE.txt
+-rw-r--r--   0        0        0    91736 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js.LICENSE.txt
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
+-rw-r--r--   0        0        0   272943 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
+-rw-r--r--   0        0        0    11319 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/remoteEntry.e77e7c805bbe3d26eec6.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/style.js
+-rw-r--r--   0        0        0   111460 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/tests/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/tests/test_handlers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/schema/plugin.json
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/chat_handler.ts
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/handler.ts
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/icons.ts
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/index.ts
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/inserter.ts
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/selection-watcher.ts
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/theme-provider.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/utils.ts
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/__tests__/jupyter_gai.spec.ts
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/__tests__/widgets/closable-dialog.spec.tsx
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat-code-view.tsx
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat-input.tsx
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat-messages.tsx
+-rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat-settings.tsx
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/expandable-text-field.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/jl-theme-provider.tsx
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/open-task-dialog.tsx
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/scroll-container.tsx
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/select.tsx
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/settings/model-fields.tsx
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/contexts/collaborators-context.tsx
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/contexts/selection-context.tsx
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/types/mui.d.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/types/svg.d.ts
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/widgets/chat-error.tsx
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/widgets/chat-sidebar.tsx
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/widgets/closable-dialog.tsx
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/base.css
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/chat-settings.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/expandable-text-field.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/index.js
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/react-markdown.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/icons/chat.svg
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/icons/jupyternaut.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/tests/jupyter_ai.spec.ts
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/README.md
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/PKG-INFO
```

### Comparing `jupyter_ai-0.7.3/.eslintrc.js` & `jupyter_ai-0.8.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/RELEASE.md` & `jupyter_ai-0.8.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jest.config.js` & `jupyter_ai-0.8.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/package.json` & `jupyter_ai-0.8.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.8.0'"}*

```diff
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.3"
+    "version": "0.8.0"
 }
```

### Comparing `jupyter_ai-0.7.3/tsconfig.json` & `jupyter_ai-0.8.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/__init__.py` & `jupyter_ai-0.8.0/jupyter_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/engine.py` & `jupyter_ai-0.8.0/jupyter_ai/engine.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/extension.py` & `jupyter_ai-0.8.0/jupyter_ai/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/handlers.py` & `jupyter_ai-0.8.0/jupyter_ai/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,15 +275,17 @@
                 continue
 
             providers.append(
                 ListProvidersEntry(
                     id=provider.id,
                     name=provider.name,
                     models=provider.models,
-                    auth_strategy=provider.auth_strategy
+                    auth_strategy=provider.auth_strategy,
+                    registry=provider.registry,
+                    fields=provider.fields,
                 )
             )
         
         response = ListProvidersResponse(providers=sorted(providers, key=lambda p: p.name))
         self.finish(response.json())
 
 
@@ -300,15 +302,17 @@
         providers = []
         for provider in self.embeddings_providers.values():
             providers.append(
                 ListProvidersEntry(
                     id=provider.id,
                     name=provider.name,
                     models=provider.models,
-                    auth_strategy=provider.auth_strategy
+                    auth_strategy=provider.auth_strategy,
+                    registry=provider.registry,
+                    fields=provider.fields,
                 )
             )
         
         response = ListProvidersResponse(providers=sorted(providers, key=lambda p: p.name))
         self.finish(response.json())
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/models.py` & `jupyter_ai-0.8.0/jupyter_ai/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from jupyter_ai_magics.providers import AuthStrategy
+from jupyter_ai_magics.providers import AuthStrategy, Field
 
 from pydantic import BaseModel 
-from typing import Dict, List, Union, Literal, Optional
+from typing import Any, Dict, List, Union, Literal, Optional
 
 class PromptRequest(BaseModel):
     task_id: str
     engine_id: str
     prompt_variables: Dict[str, str]
 
 # the type of message used to chat with the agent
@@ -88,14 +88,16 @@
     """Model provider with supported models
     and provider's authentication strategy
     """
     id: str
     name: str
     models: List[str]
     auth_strategy: AuthStrategy
+    registry: bool
+    fields: List[Field]
 
 
 class ListProvidersResponse(BaseModel):
     providers: List[ListProvidersEntry]
 
 class IndexedDir(BaseModel):
     path: str
@@ -104,7 +106,8 @@
     dirs: List[IndexedDir]
 
 class GlobalConfig(BaseModel):
     model_provider_id: Optional[str] = None
     embeddings_provider_id: Optional[str] = None
     api_keys: Dict[str, str] = {}
     send_with_shift_enter: Optional[bool] = None
+    fields: Dict[str, Dict[str, Any]] = {}
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/reply_processor.py` & `jupyter_ai-0.8.0/jupyter_ai/reply_processor.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/task_manager.py` & `jupyter_ai-0.8.0/jupyter_ai/task_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/tasks.py` & `jupyter_ai-0.8.0/jupyter_ai/tasks.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/ask.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/ask.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/base.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/base.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/chat_provider.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/chat_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         local_model_id, provider = ray.get(
             actor.get_model_provider_data.remote(model_id)
         )
         
         if not provider:
             raise ValueError(f"No provider and model found with '{model_id}'")
         
-        provider_params = { "model_id": local_model_id}
+        fields = config.fields.get(model_id, {})
+        provider_params = { "model_id": local_model_id, **fields }
         
         auth_strategy = provider.auth_strategy
         if auth_strategy and auth_strategy.type == "env":
             api_keys = config.api_keys
             name = auth_strategy.name
             if name not in api_keys:
                 raise ValueError(f"Missing value for '{auth_strategy.name}' in the config.")
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/config.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/default.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/default.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from jupyter_ai.actors.memory import RemoteMemory
 from jupyter_ai.models import HumanChatMessage, ClearMessage, ChatMessage
 from jupyter_ai_magics.providers import BaseProvider
 
 SYSTEM_PROMPT = """
 You are Jupyternaut, a conversational assistant living in JupyterLab to help users.
 You are not a language model, but rather an application built on a foundation model from {provider_name} called {local_model_id}.
-You are talkative and provides lots of specific details from its context.
+You are talkative and you provide lots of specific details from the foundation model's context.
 You may use Markdown to format your response.
 Code blocks must be formatted in Markdown.
 Math should be rendered with inline TeX markup, surrounded by $.
 If you do not know the answer to a question, answer truthfully by responding that you do not know.
 The following is a friendly conversation between you and a human.
 """.strip()
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/embeddings_provider.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/generate.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/generate.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/learn.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/learn.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/memory.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/memory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/providers.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/actors/router.py` & `jupyter_ai-0.8.0/jupyter_ai/actors/router.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/document_loaders/directory.py` & `jupyter_ai-0.8.0/jupyter_ai/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/document_loaders/splitter.py` & `jupyter_ai-0.8.0/jupyter_ai/document_loaders/splitter.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/package.json` & `jupyter_ai-0.8.0/jupyter_ai/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e77e7c805bbe3d26eec6.js'}}",*

 * * "'version'": "'0.8.0'"}*

```diff
@@ -59,15 +59,15 @@
         "schema/*.json",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.df84a6245b68ae8abd9f.js",
+            "load": "static/remoteEntry.e77e7c805bbe3d26eec6.js",
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
-    "version": "0.7.3"
+    "version": "0.8.0"
 }
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig` & `jupyter_ai-0.8.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.8.0'"}*

```diff
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.3"
+    "version": "0.8.0"
 }
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json` & `jupyter_ai-0.8.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/639.b63fa10cbcf2eccddd7d.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/253.0b5d158f3577d0bfbee5.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
-    [639], {
-        11639: (e, t, n) => {
+    [253], {
+        30253: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => se
+                default: () => me
             });
-            var r = n(45687),
-                o = n(35059),
+            var r = n(96175),
+                o = n(75884),
                 l = n(56271),
                 i = n.n(l),
-                a = n(73033),
+                a = n(49764),
                 s = n(53959),
                 c = n(35048),
                 d = n(13264),
                 u = n(28504),
                 m = n(28066),
                 h = n(53626);
 
@@ -156,18 +156,18 @@
                     theme: t
                 }, e.children)
             }
             var f = n(30535),
                 v = n.n(f),
                 y = n(96707),
                 E = n.n(y),
-                b = n(40532),
-                x = n.n(b),
+                _ = n(40532),
+                b = n.n(_),
                 C = (n(38662), n(55351)),
-                _ = n(7464),
+                x = n(7464),
                 S = n(6277);
             const w = "jp-ai-code";
 
             function k({
                 className: e,
                 children: t,
                 ...n
@@ -197,15 +197,15 @@
                     sx: {
                         display: "flex",
                         flexDirection: "column"
                     }
                 }, i().createElement(C.Prism, Object.assign({}, n, {
                     className: (0, S.Z)(n.className, w),
                     children: r,
-                    style: _.Z,
+                    style: x.Z,
                     language: e,
                     PreTag: "div"
                 })), i().createElement(c.Button, {
                     onClick: async () => {
                         a(j.Copying);
                         try {
                             await navigator.clipboard.writeText(r)
@@ -229,15 +229,15 @@
                 const r = /language-(\w+)/.exec(t || "");
                 return e ? i().createElement(k, Object.assign({}, n)) : i().createElement(P, Object.assign({}, n, {
                     language: r ? r[1] : void 0
                 }))
             }
             const M = i().createContext({});
 
-            function A({
+            function F({
                 globalAwareness: e,
                 children: t
             }) {
                 const [n, r] = (0, l.useState)({});
                 return (0, l.useEffect)((() => {
                     function t() {
                         var t;
@@ -250,25 +250,25 @@
                     return null == e || e.on("change", t), () => {
                         null == e || e.off("change", t)
                     }
                 }), [e]), e ? i().createElement(M.Provider, {
                     value: n
                 }, t) : t
             }
-            var F = n(22502);
-            const R = new F.LabIcon({
+            var A = n(78667);
+            const N = new A.LabIcon({
                     name: "jupyter-ai::chat",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M0 0h24v24H0V0z" fill="none"/>\n    <path d="M15 4v7H5.17L4 12.17V4h11m1-2H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm5 4h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1z"/>\n  </g>\n</svg>\n'
                 }),
-                T = new F.LabIcon({
+                T = new A.LabIcon({
                     name: "jupyter-ai::jupyternaut",
                     svgstr: '<svg viewBox="0 0 38 38" fill="none"\n    xmlns="http://www.w3.org/2000/svg">\n    <g clip-path="url(#clip0_0_2356)">\n        <rect width="38" height="38" fill="white" />\n        <circle cx="19" cy="19" r="19" fill="#F37726" />\n        <path fill-rule="evenodd" clip-rule="evenodd"\n            d="M19.9483 6.83653C20.5827 6.6205 21.0391 6.0196 21.0391 5.31212C21.0391 4.42296 20.3183 3.70215 19.4291 3.70215C18.5399 3.70215 17.8191 4.42296 17.8191 5.31212C17.8191 6.01951 18.2753 6.62033 18.9096 6.83644V8.00387H18.3702C12.0844 8.00387 6.97151 13.1171 6.97151 19.4026C6.97151 25.6885 12.0848 30.8013 18.3702 30.8013H19.7682C26.0541 30.8013 31.167 25.6881 31.167 19.4026C31.167 13.1773 26.1511 8.10183 19.9483 8.00527V6.83653ZM18.3702 29H19.7682C25.1351 29 29.4985 24.0213 29.4985 20.6545C29.4985 15.2876 25.1351 10.9242 19.7682 10.9242H18.3702C13.0034 10.9242 8.64 15.2876 8.64 20.6545C8.64 24.0213 13.0034 29 18.3702 29ZM32.8926 23.997C33.6267 23.997 33.6301 23.4847 33.6348 22.7562V22.7562V22.7562V22.7561C33.636 22.5714 33.6373 22.3728 33.6506 22.1651C33.7079 21.3027 33.7245 20.4643 33.7079 19.6759L33.7046 19.5569C33.6673 18.2251 33.661 17.999 32.3999 17.7511L32.252 17.7265L32.2535 17.776C32.2611 18.0225 32.2686 18.269 32.2686 18.515C32.2686 20.3168 31.9974 22.0628 31.4956 23.704C31.3593 24.1499 31.8389 24.5669 32.249 24.3451L32.8926 23.997ZM5.28037 23.997C4.54628 23.997 4.54296 23.4847 4.53822 22.7563C4.53702 22.5715 4.53573 22.3729 4.52241 22.1651C4.46511 21.3027 4.44849 20.4644 4.4651 19.6759L4.46846 19.557C4.50567 18.2251 4.51198 17.9991 5.77316 17.7512L5.921 17.7265L5.91949 17.776L5.91949 17.776C5.91193 18.0225 5.90438 18.269 5.90438 18.515C5.90438 20.3169 6.17557 22.0628 6.67738 23.704C6.81372 24.1499 6.33412 24.5669 5.92398 24.3451L5.28037 23.997ZM19.5225 11.9922C14.8928 11.9922 11.0449 14.9283 10.0641 18.7499C9.93031 19.2711 10.6154 19.4434 10.9411 19.0152C12.324 17.1972 14.0829 16.8622 15.6479 16.5641C17.7622 16.1614 19.5225 15.8262 19.5225 11.9922Z"\n            fill="white" />\n    </g>\n    <defs>\n        <clipPath id="clip0_0_2356">\n            <rect width="38" height="38" fill="white" />\n        </clipPath>\n    </defs>\n</svg>'
                 }).react;
 
-            function B(e) {
+            function R(e) {
                 var t;
                 const n = (0, l.useContext)(M),
                     r = {
                         height: "24px",
                         width: "24px"
                     };
                 let o;
@@ -325,15 +325,15 @@
                         fontSize: "0.8em",
                         color: "var(--jp-ui-font-color2)",
                         fontWeight: 300
                     }
                 }, e.timestamp)))
             }
 
-            function N(e) {
+            function W(e) {
                 const [t, n] = (0, l.useState)({});
                 return (0, l.useEffect)((() => {
                     const r = {
                         ...t
                     };
                     let o = !1;
                     for (const t of e.messages) t.id in r || (r[t.id] = new Date(1e3 * t.time).toLocaleTimeString([], {
@@ -348,32 +348,32 @@
                         }
                     }
                 }, e.messages.map(((e, n) => i().createElement(c.Box, {
                     key: n,
                     sx: {
                         padding: 4
                     }
-                }, i().createElement(B, {
+                }, i().createElement(R, {
                     message: e,
                     timestamp: t[e.id],
                     sx: {
                         marginBottom: 3
                     }
                 }), i().createElement(v(), {
                     className: "jp-RenderedHTMLCommon jp-ai-react-markdown",
                     components: {
                         code: L
                     },
                     remarkPlugins: [E()],
-                    rehypePlugins: [x()]
+                    rehypePlugins: [b()]
                 }, e.body)))))
             }
-            var H = n(17380);
+            var z = n(17380);
 
-            function z(e) {
+            function B(e) {
                 const t = e.sendWithShiftEnter ? i().createElement("span", null, "Press ", i().createElement("b", null, "Shift"), "+", i().createElement("b", null, "Enter"), " to send message") : i().createElement("span", null, "Press ", i().createElement("b", null, "Shift"), "+", i().createElement("b", null, "Enter"), " to add a new line");
                 return i().createElement(c.Box, {
                     sx: e.sx
                 }, i().createElement(c.Box, {
                     sx: {
                         display: "flex"
                     }
@@ -392,15 +392,15 @@
                             position: "end"
                         }, i().createElement(c.IconButton, {
                             size: "small",
                             color: "primary",
                             onClick: e.onSend,
                             disabled: !e.value.trim().length,
                             title: "Send message (SHIFT+ENTER)"
-                        }, i().createElement(H.Z, null)))
+                        }, i().createElement(z.Z, null)))
                     },
                     FormHelperTextProps: {
                         sx: {
                             marginLeft: "auto",
                             marginRight: 0
                         }
                     },
@@ -421,15 +421,15 @@
                         checked: e.replaceSelection,
                         onChange: e.toggleReplaceSelection
                     }),
                     label: "Replace selection"
                 })))
             }
 
-            function W(e) {
+            function H(e) {
                 return i().createElement(c.FormControl, {
                     fullWidth: !0
                 }, i().createElement(c.InputLabel, null, e.label), i().createElement(c.Select, Object.assign({}, e, {
                     value: null === e.value ? "null" : e.value,
                     label: e.label,
                     onChange: (t, n) => {
                         var r;
@@ -439,105 +439,187 @@
                         sx: {
                             maxHeight: "50%",
                             minHeight: 400
                         }
                     }
                 }), e.children))
             }
-            var Z, D, O = n(28142),
-                V = n(48820);
-            async function J(e = "", t = {}) {
-                const n = V.ServerConnection.makeSettings(),
-                    r = O.URLExt.join(n.baseUrl, "api/ai", e);
+            var O, Z, D = n(83058),
+                J = n(11872);
+            async function V(e = "", t = {}) {
+                const n = J.ServerConnection.makeSettings(),
+                    r = D.URLExt.join(n.baseUrl, "api/ai", e);
                 let o;
                 try {
-                    o = await V.ServerConnection.makeRequest(r, t, n)
+                    o = await J.ServerConnection.makeRequest(r, t, n)
                 } catch (e) {
-                    throw new V.ServerConnection.NetworkError(e)
+                    throw new J.ServerConnection.NetworkError(e)
                 }
                 let l = await o.text();
                 if (l.length > 0) try {
                     l = JSON.parse(l)
                 } catch (e) {
                     console.log("Not a JSON response body.", o)
                 }
-                if (!o.ok) throw new V.ServerConnection.ResponseError(o, l.message || l);
+                if (!o.ok) throw new J.ServerConnection.ResponseError(o, l.message || l);
                 return l
             }
 
-            function $() {
+            function $(e) {
+                var t, n;
+
+                function r(t) {
+                    e.setConfig({
+                        ...e.config,
+                        fields: {
+                            ...e.config.fields,
+                            [e.gmid]: {
+                                ...e.config.fields[e.gmid],
+                                [e.field.key]: t.target.value
+                            }
+                        }
+                    })
+                }
+                return "text" === e.field.type ? i().createElement(c.TextField, {
+                    label: e.field.label,
+                    value: null === (t = e.config.fields[e.gmid]) || void 0 === t ? void 0 : t[e.field.key],
+                    onChange: r,
+                    fullWidth: !0
+                }) : "text-multiline" === e.field.type ? i().createElement(c.TextField, {
+                    label: e.field.label,
+                    value: null === (n = e.config.fields[e.gmid]) || void 0 === n ? void 0 : n[e.field.key],
+                    onChange: r,
+                    fullWidth: !0,
+                    multiline: !0,
+                    minRows: 2
+                }) : i().createElement(i().Fragment, null)
+            }
+
+            function G(e) {
+                var t;
+                return (null === (t = e.fields) || void 0 === t ? void 0 : t.length) ? i().createElement(i().Fragment, null, e.fields.map(((t, n) => i().createElement($, Object.assign({}, e, {
+                    field: t,
+                    key: n
+                }))))) : null
+            }
+
+            function U(e) {
+                return e ? e.split(":")[0] : null
+            }
+
+            function K(e, t) {
+                const n = U(e);
+                return t.providers.find((e => e.id === n))
+            }
+
+            function Q() {
                 var e;
-                const [t, n] = (0, l.useState)(D.Loading), [r, o] = (0, l.useState)(), [a, d] = (0, l.useState)(), [u, m] = (0, l.useState)(), [h, p] = (0, l.useState)(), [g, f] = (0, l.useState)({
+                const [t, n] = (0, l.useState)(Z.Loading), [r, o] = (0, l.useState)(), [a, d] = (0, l.useState)(), [u, m] = (0, l.useState)(), [h, p] = (0, l.useState)(), [g, f] = (0, l.useState)({
                     model_provider_id: null,
                     embeddings_provider_id: null,
                     api_keys: {},
-                    send_with_shift_enter: null
-                }), [v, y] = (0, l.useState)(!1), [E, b] = (0, l.useState)();
+                    send_with_shift_enter: null,
+                    fields: {}
+                }), [v, y] = (0, l.useState)(!1), [E, _] = (0, l.useState)(), [b, C] = (0, l.useState)(!1), [x, S] = (0, l.useState)("*"), w = (0, l.useMemo)((() => {
+                    if (g.model_provider_id && u) return K(g.model_provider_id, u)
+                }), [g.model_provider_id, u]), k = (0, l.useMemo)((() => g.model_provider_id && w ? (null == w ? void 0 : w.registry) ? `${w.id}:${x}` : g.model_provider_id : null), [g.model_provider_id, w, u, x]);
                 return (0, l.useEffect)((() => {
                     !async function() {
                         try {
-                            const [e, t, r] = await Promise.all([Z.getConfig(), Z.listLmProviders(), Z.listEmProviders()]);
-                            d(e), f(e), m(t), p(r), n(D.Ready)
+                            const [e, t, r] = await Promise.all([O.getConfig(), O.listLmProviders(), O.listEmProviders()]);
+                            if (d(e), m(t), p(r), function(e, t) {
+                                    var n, r;
+                                    return null !== (r = null === (n = K(e, t)) || void 0 === n ? void 0 : n.registry) && void 0 !== r && r
+                                }(e.model_provider_id, t)) {
+                                C(!0);
+                                const t = U(e.model_provider_id);
+                                S(function(e) {
+                                    if (!e) return null;
+                                    const t = e.split(":");
+                                    return t[t.length - 1]
+                                }(e.model_provider_id)), f({
+                                    ...e,
+                                    model_provider_id: `${t}:*`
+                                })
+                            } else f(e);
+                            n(Z.Ready)
                         } catch (e) {
-                            console.error(e), e instanceof Error && o(e.message), n(D.FetchError)
+                            console.error(e), e instanceof Error && o(e.message), n(Z.FetchError)
                         }
                     }()
                 }), []), (0, l.useEffect)((() => {
-                    var e, t;
-                    const n = null === (e = g.model_provider_id) || void 0 === e ? void 0 : e.split(":")[0],
-                        r = null === (t = g.embeddings_provider_id) || void 0 === t ? void 0 : t.split(":")[0],
-                        o = null == u ? void 0 : u.providers.find((e => e.id === n)),
-                        l = null == h ? void 0 : h.providers.find((e => e.id === r)),
-                        i = {};
-                    (null == o ? void 0 : o.auth_strategy) && "env" === o.auth_strategy.type && (i[o.auth_strategy.name] = (null == a ? void 0 : a.api_keys[o.auth_strategy.name]) || ""), (null == l ? void 0 : l.auth_strategy) && "env" === l.auth_strategy.type && (i[l.auth_strategy.name] = (null == a ? void 0 : a.api_keys[l.auth_strategy.name]) || ""), f((e => ({
+                    const e = U(g.model_provider_id),
+                        t = U(g.embeddings_provider_id),
+                        n = null == u ? void 0 : u.providers.find((t => t.id === e)),
+                        r = null == h ? void 0 : h.providers.find((e => e.id === t)),
+                        o = {};
+                    (null == n ? void 0 : n.auth_strategy) && "env" === n.auth_strategy.type && (o[n.auth_strategy.name] = (null == a ? void 0 : a.api_keys[n.auth_strategy.name]) || ""), (null == r ? void 0 : r.auth_strategy) && "env" === r.auth_strategy.type && (o[r.auth_strategy.name] = (null == a ? void 0 : a.api_keys[r.auth_strategy.name]) || ""), f((e => ({
                         ...e,
                         api_keys: {
                             ...null == a ? void 0 : a.api_keys,
-                            ...i
+                            ...o
                         }
                     })))
-                }), [g.model_provider_id, g.embeddings_provider_id]), t === D.Loading ? i().createElement(s.Z, {
+                }), [g.model_provider_id, g.embeddings_provider_id]), t === Z.Loading ? i().createElement(s.Z, {
                     sx: {
                         width: "100%",
                         height: "100%",
                         boxSizing: "border-box",
                         display: "flex",
                         alignItems: "center",
                         justifyContent: "space-around"
                     }
-                }, i().createElement(c.CircularProgress, null)) : t !== D.FetchError && u && h && a ? i().createElement(s.Z, {
+                }, i().createElement(c.CircularProgress, null)) : t !== Z.FetchError && u && h && a ? i().createElement(s.Z, {
                     sx: {
                         padding: 4,
                         boxSizing: "border-box",
                         "& > .MuiAlert-root": {
                             marginBottom: 2
                         }
                     }
-                }, t === D.SubmitError && i().createElement(c.Alert, {
+                }, t === Z.SubmitError && i().createElement(c.Alert, {
                     severity: "error"
-                }, E ? `An error occurred. Error details:\n\n${E}` : "An unknown error occurred. Check the console for more details."), t === D.Success && i().createElement(c.Alert, {
+                }, E ? `An error occurred. Error details:\n\n${E}` : "An unknown error occurred. Check the console for more details."), t === Z.Success && i().createElement(c.Alert, {
                     severity: "success"
-                }, "Settings saved successfully."), i().createElement(W, {
+                }, "Settings saved successfully."), i().createElement("h2", {
+                    className: "jp-ai-ChatSettings-header"
+                }, "Language model"), i().createElement(H, {
                     value: g.model_provider_id,
                     label: "Language model",
-                    onChange: e => f((t => ({
-                        ...t,
-                        model_provider_id: e.target.value
-                    }))),
+                    onChange: e => {
+                        f((t => ({
+                            ...t,
+                            model_provider_id: e.target.value
+                        })));
+                        const t = K(e.target.value, u);
+                        (null == t ? void 0 : t.registry) ? (C(!0), S("*")) : C(!1)
+                    },
                     MenuProps: {
                         sx: {
                             maxHeight: "50%",
                             minHeight: 400
                         }
                     }
                 }, i().createElement(c.MenuItem, {
                     value: "null"
-                }, "None"), u.providers.map((e => e.models.filter((e => "*" !== e)).map((t => i().createElement(c.MenuItem, {
+                }, "None"), u.providers.map((e => e.models.map((t => i().createElement(c.MenuItem, {
                     value: `${e.id}:${t}`
-                }, e.name, " :: ", t)))))), i().createElement(W, {
+                }, e.name, " :: ", t)))))), b && i().createElement(c.TextField, {
+                    label: "Local model ID",
+                    value: x,
+                    onChange: e => S(e.target.value),
+                    fullWidth: !0
+                }), k && i().createElement(G, {
+                    gmid: k,
+                    config: g,
+                    setConfig: f,
+                    fields: null == w ? void 0 : w.fields
+                }), i().createElement("h2", {
+                    className: "jp-ai-ChatSettings-header"
+                }, "Embedding model"), i().createElement(H, {
                     value: g.embeddings_provider_id,
                     label: "Embedding model",
                     onChange: e => f((t => ({
                         ...t,
                         embeddings_provider_id: e.target.value
                     }))),
                     MenuProps: {
@@ -546,28 +628,32 @@
                             minHeight: 400
                         }
                     }
                 }, i().createElement(c.MenuItem, {
                     value: "null"
                 }, "None"), h.providers.map((e => e.models.filter((e => "*" !== e)).map((t => i().createElement(c.MenuItem, {
                     value: `${e.id}:${t}`
-                }, e.name, " :: ", t)))))), Object.entries(g.api_keys).map((([e, t], n) => i().createElement(c.TextField, {
+                }, e.name, " :: ", t)))))), i().createElement("h2", {
+                    className: "jp-ai-ChatSettings-header"
+                }, "API Keys"), Object.entries(g.api_keys).map((([e, t], n) => i().createElement(c.TextField, {
                     key: n,
                     label: e,
                     value: t,
                     fullWidth: !0,
                     type: "password",
                     onChange: t => f((n => ({
                         ...n,
                         api_keys: {
                             ...n.api_keys,
                             [e]: t.target.value
                         }
                     })))
-                }))), i().createElement(c.FormControl, null, i().createElement(c.FormLabel, {
+                }))), i().createElement("h2", {
+                    className: "jp-ai-ChatSettings-header"
+                }, "Input"), i().createElement(c.FormControl, null, i().createElement(c.FormLabel, {
                     id: "send-radio-buttons-group-label"
                 }, "When writing a message, press ", i().createElement("kbd", null, "Enter"), " to:"), i().createElement(c.RadioGroup, {
                     "aria-labelledby": "send-radio-buttons-group-label",
                     value: null !== (e = g.send_with_shift_enter) && void 0 !== e && e ? "newline" : "send",
                     name: "send-radio-buttons-group",
                     onChange: e => f((t => ({
                         ...t,
@@ -588,27 +674,39 @@
                     }
                 }, i().createElement(c.Button, {
                     variant: "contained",
                     onClick: async () => {
                         var e;
                         const t = {
                             ...g,
+                            model_provider_id: k,
                             api_keys: {
                                 ...g.api_keys
                             },
                             send_with_shift_enter: null === (e = g.send_with_shift_enter) || void 0 === e || e
                         };
                         for (const e in t.api_keys) "" === t.api_keys[e] && delete t.api_keys[e];
+                        for (const e in t.fields)
+                            for (const n in t.fields[e]) {
+                                const r = t.fields[e][n];
+                                if ("string" == typeof r) try {
+                                    const o = JSON.parse(r),
+                                        l = JSON.stringify(o);
+                                    t.fields[e][n] = l
+                                } catch (e) {
+                                    continue
+                                }
+                            }
                         y(!0);
                         try {
-                            await Z.updateConfig(t)
+                            await O.updateConfig(t)
                         } catch (e) {
-                            console.error(e), e instanceof Error && b(e.message), n(D.SubmitError)
+                            console.error(e), e instanceof Error && _(e.message), n(Z.SubmitError)
                         }
-                        n(D.Success), y(!1)
+                        n(Z.Success), y(!1)
                     },
                     disabled: v
                 }, v ? "Saving..." : "Save changes"))) : i().createElement(s.Z, {
                     sx: {
                         width: "100%",
                         height: "100%",
                         padding: 4,
@@ -617,63 +715,63 @@
                 }, i().createElement(c.Alert, {
                     severity: "error"
                 }, r ? `An error occurred. Error details:\n\n${r}` : "An unknown error occurred. Check the console for more details."))
             }! function(e) {
                 e.sendPrompt = async function(e) {
                     let t;
                     try {
-                        t = await J("prompt", {
+                        t = await V("prompt", {
                             method: "POST",
                             body: JSON.stringify(e)
                         })
                     } catch (e) {
                         return Promise.reject(e)
                     }
                     return t
                 }, e.listTasks = async function() {
-                    return J("tasks")
+                    return V("tasks")
                 }, e.describeTask = async function(e) {
-                    return J(`tasks/${e}`)
+                    return V(`tasks/${e}`)
                 }, e.getConfig = async function() {
-                    return J("config")
+                    return V("config")
                 }, e.listLmProviders = async function() {
-                    return J("providers")
+                    return V("providers")
                 }, e.listEmProviders = async function() {
-                    return J("providers/embeddings")
+                    return V("providers/embeddings")
                 }, e.updateConfig = async function(e) {
-                    return J("config", {
+                    return V("config", {
                         method: "POST",
                         body: JSON.stringify(e)
                     })
                 }
-            }(Z || (Z = {})),
+            }(O || (O = {})),
             function(e) {
                 e[e.Loading = 0] = "Loading", e[e.Ready = 1] = "Ready", e[e.FetchError = 2] = "FetchError", e[e.SubmitError = 3] = "SubmitError", e[e.Success = 4] = "Success"
-            }(D || (D = {}));
-            const G = i().createContext([null, () => {}]);
+            }(Z || (Z = {}));
+            const q = i().createContext([null, () => {}]);
 
-            function U({
+            function Y({
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
-                return i().createElement(G.Provider, {
+                return i().createElement(q.Provider, {
                     value: [n, o]
                 }, t)
             }
 
-            function K(e) {
+            function X(e) {
                 const t = (0, l.useMemo)((() => "jupyter-ai-scroll-container-" + Date.now().toString()), []);
                 return (0, l.useEffect)((() => {
                     const e = document.querySelector(`#${t}`);
                     if (!e) return;
                     const n = new IntersectionObserver((t => {
                         t.forEach((t => {
                             t.isIntersecting && e.scroll({
@@ -701,25 +799,25 @@
                     sx: {
                         overflowAnchor: "auto",
                         height: "1px"
                     }
                 }))
             }
 
-            function Q({
+            function ee({
                 chatHandler: e,
                 setChatView: t
             }) {
-                const [n, r] = (0, l.useState)([]), [o, a] = (0, l.useState)(!1), [u, m] = (0, l.useState)(!0), [h, p] = (0, l.useState)(!1), [g, f] = (0, l.useState)(""), [v, y] = (0, l.useContext)(G), [E, b] = (0, l.useState)(!0);
+                const [n, r] = (0, l.useState)([]), [o, a] = (0, l.useState)(!1), [u, m] = (0, l.useState)(!0), [h, p] = (0, l.useState)(!1), [g, f] = (0, l.useState)(""), [v, y] = (0, l.useContext)(q), [E, _] = (0, l.useState)(!0);
                 return (0, l.useEffect)((() => {
                     !async function() {
                         var t;
                         try {
-                            const [n, o] = await Promise.all([e.getHistory(), Z.getConfig()]);
-                            b(null !== (t = o.send_with_shift_enter) && void 0 !== t && t), r(n.messages), o.model_provider_id || a(!0)
+                            const [n, o] = await Promise.all([e.getHistory(), O.getConfig()]);
+                            _(null !== (t = o.send_with_shift_enter) && void 0 !== t && t), r(n.messages), o.model_provider_id || a(!0)
                         } catch (e) {
                             console.error(e)
                         }
                     }()
                 }), [e]), (0, l.useEffect)((() => {
                     function t(e) {
                         "connection" !== e.type && ("clear" !== e.type ? r((t => [...t, e])) : r([]))
@@ -738,22 +836,22 @@
                     }
                 }, i().createElement(c.Stack, {
                     spacing: 4
                 }, i().createElement("p", null, "Welcome to Jupyter AI! To get started, please select a language model to chat with from the settings panel. You will also likely need to provide API credentials, so be sure to have those handy."), i().createElement(c.Button, {
                     variant: "contained",
                     startIcon: i().createElement(d.Z, null),
                     size: "large",
-                    onClick: () => (a(!1), void t(q.Settings))
-                }, "Start Here"))) : i().createElement(i().Fragment, null, i().createElement(K, {
+                    onClick: () => (a(!1), void t(te.Settings))
+                }, "Start Here"))) : i().createElement(i().Fragment, null, i().createElement(X, {
                     sx: {
                         flexGrow: 1
                     }
-                }, i().createElement(N, {
+                }, i().createElement(W, {
                     messages: n
-                })), i().createElement(z, {
+                })), i().createElement(B, {
                     value: g,
                     onChange: f,
                     onSend: async () => {
                         f("");
                         const t = g + (u && (null == v ? void 0 : v.text) ? "\n\n```\n" + v.text + "\n```" : ""),
                             n = await e.sendMessage({
                                 prompt: t
@@ -784,21 +882,21 @@
                         paddingTop: 3.5,
                         paddingBottom: 0,
                         borderTop: "1px solid var(--jp-border-color1)"
                     },
                     sendWithShiftEnter: E
                 }))
             }
-            var q;
+            var te;
 
-            function Y(e) {
-                const [t, n] = (0, l.useState)(e.chatView || q.Chat);
-                return i().createElement(g, null, i().createElement(U, {
+            function ne(e) {
+                const [t, n] = (0, l.useState)(e.chatView || te.Chat);
+                return i().createElement(g, null, i().createElement(Y, {
                     selectionWatcher: e.selectionWatcher
-                }, i().createElement(A, {
+                }, i().createElement(F, {
                     globalAwareness: e.globalAwareness
                 }, i().createElement(s.Z, {
                     sx: {
                         width: "100%",
                         height: "100%",
                         boxSizing: "border-box",
                         background: "var(--jp-layout-color0)",
@@ -806,78 +904,78 @@
                         flexDirection: "column"
                     }
                 }, i().createElement(s.Z, {
                     sx: {
                         display: "flex",
                         justifyContent: "space-between"
                     }
-                }, t !== q.Chat ? i().createElement(c.IconButton, {
-                    onClick: () => n(q.Chat)
-                }, i().createElement(u.Z, null)) : i().createElement(s.Z, null), t === q.Chat ? i().createElement(c.IconButton, {
-                    onClick: () => n(q.Settings)
-                }, i().createElement(d.Z, null)) : i().createElement(s.Z, null)), t === q.Chat && i().createElement(Q, {
+                }, t !== te.Chat ? i().createElement(c.IconButton, {
+                    onClick: () => n(te.Chat)
+                }, i().createElement(u.Z, null)) : i().createElement(s.Z, null), t === te.Chat ? i().createElement(c.IconButton, {
+                    onClick: () => n(te.Settings)
+                }, i().createElement(d.Z, null)) : i().createElement(s.Z, null)), t === te.Chat && i().createElement(ee, {
                     chatHandler: e.chatHandler,
                     setChatView: n
-                }), t === q.Settings && i().createElement($, null)))))
+                }), t === te.Settings && i().createElement(Q, null)))))
             }! function(e) {
                 e[e.Chat = 0] = "Chat", e[e.Settings = 1] = "Settings"
-            }(q || (q = {}));
-            var X = n(80819),
-                ee = n(26413),
-                te = n(51473),
-                ne = n(41123),
-                re = n(78918),
-                oe = n(71840);
+            }(te || (te = {}));
+            var re = n(26676),
+                oe = n(36705),
+                le = n(82883),
+                ie = n(76779),
+                ae = n(78918),
+                se = n(71840);
 
-            function le(e) {
+            function ce(e) {
                 var t;
-                if (!(e instanceof X.DocumentWidget)) return null;
+                if (!(e instanceof re.DocumentWidget)) return null;
                 let n;
                 const {
                     content: r
                 } = e;
-                return r instanceof te.FileEditor ? n = r.editor : r instanceof ne.Notebook && (n = null === (t = r.activeCell) || void 0 === t ? void 0 : t.editor), n instanceof ee.CodeMirrorEditor ? n : void 0
+                return r instanceof le.FileEditor ? n = r.editor : r instanceof ie.Notebook && (n = null === (t = r.activeCell) || void 0 === t ? void 0 : t.editor), n instanceof oe.CodeMirrorEditor ? n : void 0
             }
-            class ie {
+            class de {
                 constructor(e) {
-                    if (this._mainAreaWidget = null, this._selection = null, this._selectionChanged = new oe.Signal(this), !(e instanceof r.LabShell)) throw "Shell is not an instance of LabShell. Jupyter AI does not currently support custom shells.";
+                    if (this._mainAreaWidget = null, this._selection = null, this._selectionChanged = new se.Signal(this), !(e instanceof r.LabShell)) throw "Shell is not an instance of LabShell. Jupyter AI does not currently support custom shells.";
                     this._shell = e, this._shell.currentChanged.connect(((e, t) => {
                         this._mainAreaWidget = t.newValue
                     })), setInterval(this._poll.bind(this), 200)
                 }
                 get selectionChanged() {
                     return this._selectionChanged
                 }
                 replaceSelection(e) {
-                    const t = (0, re.find)(this._shell.widgets(), (t => t.id === e.widgetId));
-                    if (!(t instanceof X.DocumentWidget)) return;
-                    if (this._shell.activateById(e.widgetId), t.content instanceof ne.Notebook && e.cellId) {
+                    const t = (0, ae.find)(this._shell.widgets(), (t => t.id === e.widgetId));
+                    if (!(t instanceof re.DocumentWidget)) return;
+                    if (this._shell.activateById(e.widgetId), t.content instanceof ie.Notebook && e.cellId) {
                         const n = function(e, t) {
                             var n;
                             const r = null === (n = e.model) || void 0 === n ? void 0 : n.sharedModel.cells.findIndex((e => e.getId() === t));
                             return void 0 === r ? -1 : r
                         }(t.content, e.cellId); - 1 !== n && (t.content.activeCellIndex = n)
                     }
-                    const n = le(t);
+                    const n = ce(t);
                     if (!n) return;
                     n.model.sharedModel.updateSource(n.getOffsetAt(e.start), n.getOffsetAt(e.end), e.text);
                     const r = n.getPositionAt(n.getOffsetAt(e.start) + e.text.length);
                     n.setSelection({
                         start: r,
                         end: r
                     })
                 }
                 _poll() {
                     const e = this._selection,
                         t = function(e) {
                             var t;
-                            const n = le(e);
-                            if (!(n && e instanceof X.DocumentWidget)) return null;
+                            const n = ce(e);
+                            if (!(n && e instanceof re.DocumentWidget)) return null;
                             let r;
-                            e.content instanceof ne.Notebook && (r = null === (t = e.content.activeCell) || void 0 === t ? void 0 : t.model.id);
+                            e.content instanceof ie.Notebook && (r = null === (t = e.content.activeCell) || void 0 === t ? void 0 : t.model.id);
                             let {
                                 start: o,
                                 end: l,
                                 ...i
                             } = n.getSelection();
                             const a = n.getOffsetAt(o),
                                 s = n.getOffsetAt(l),
@@ -892,33 +990,21 @@
                                     cellId: r
                                 }
                             }
                         }(this._mainAreaWidget);
                     (null == e ? void 0 : e.text) !== (null == t ? void 0 : t.text) && (this._selection = t, this._selectionChanged.emit(t))
                 }
             }
-            class ae {
+            class ue {
                 constructor(e = {}) {
                     var t;
-                    this.id = "", this._sendResolverQueue = [], this._replyForResolverDict = {}, this._isDisposed = !1, this._socket = null, this._listeners = [], this.serverSettings = null !== (t = e.serverSettings) && void 0 !== t ? t : V.ServerConnection.makeSettings()
+                    this.id = "", this._sendResolverQueue = [], this._replyForResolverDict = {}, this._isDisposed = !1, this._socket = null, this._listeners = [], this.serverSettings = null !== (t = e.serverSettings) && void 0 !== t ? t : J.ServerConnection.makeSettings()
                 }
-                initialize() {
-                    return new Promise(((e, t) => {
-                        if (this.isDisposed) return;
-                        const {
-                            token: n,
-                            WebSocket: r,
-                            wsUrl: o
-                        } = this.serverSettings, l = O.URLExt.join(o, "api/ai/chats") + (n ? `?token=${encodeURIComponent(n)}` : ""), i = this._socket = new r(l);
-                        i.onerror = e => t(e), i.onmessage = e => e.data && this._onMessage(JSON.parse(e.data));
-                        const a = t => {
-                            "connection" === t.type && (this.id = t.client_id, e(), this.removeListener(a))
-                        };
-                        this.addListener(a)
-                    }))
+                async initialize() {
+                    await this._initialize()
                 }
                 sendMessage(e) {
                     return new Promise((t => {
                         var n;
                         null === (n = this._socket) || void 0 === n || n.send(JSON.stringify(e)), this._sendResolverQueue.push(t)
                     }))
                 }
@@ -935,15 +1021,15 @@
                     t > -1 && this._listeners.splice(t, 1)
                 }
                 async getHistory() {
                     let e = {
                         messages: []
                     };
                     try {
-                        e = await J("chats/history", {
+                        e = await V("chats/history", {
                             method: "GET"
                         })
                     } catch (e) {
                         return Promise.reject(e)
                     }
                     return e
                 }
@@ -956,31 +1042,53 @@
                     const e = this._socket;
                     e && (this._socket = null, e.onopen = () => {}, e.onerror = () => {}, e.onmessage = () => {}, e.onclose = () => {}, e.close())
                 }
                 _onMessage(e) {
                     var t;
                     "human" === e.type && e.client.id === this.id && (null === (t = this._sendResolverQueue.shift()) || void 0 === t || t(e.id)), "agent" === e.type && e.reply_to in this._replyForResolverDict && (this._replyForResolverDict[e.reply_to](e), delete this._replyForResolverDict[e.reply_to]), this._listeners.forEach((t => t(e)))
                 }
+                _onClose(e, t) {
+                    if (t(new Error("Chat UI websocket disconnected")), console.error("Chat UI websocket disconnected"), 1006 === e.code) {
+                        const e = 1;
+                        console.info(`Will try to reconnect in ${e} s.`), setTimeout((async () => await this._initialize()), 1e3 * e)
+                    }
+                }
+                _initialize() {
+                    return new Promise(((e, t) => {
+                        if (this.isDisposed) return;
+                        console.log("Creating a new websocket connection for chat...");
+                        const {
+                            token: n,
+                            WebSocket: r,
+                            wsUrl: o
+                        } = this.serverSettings, l = D.URLExt.join(o, "api/ai/chats") + (n ? `?token=${encodeURIComponent(n)}` : ""), i = this._socket = new r(l);
+                        i.onclose = e => this._onClose(e, t), i.onerror = e => t(e), i.onmessage = e => e.data && this._onMessage(JSON.parse(e.data));
+                        const a = t => {
+                            "connection" === t.type && (this.id = t.client_id, e(), this.removeListener(a))
+                        };
+                        this.addListener(a)
+                    }))
+                }
             }
-            const se = {
+            const me = {
                 id: "jupyter_ai:plugin",
                 autoStart: !0,
                 optional: [o.IGlobalAwareness, r.ILayoutRestorer],
                 activate: async (e, t, n) => {
-                    const r = new ie(e.shell),
-                        o = new ae;
+                    const r = new de(e.shell),
+                        o = new ue;
                     let l = null;
                     try {
                         await o.initialize(), l = function(e, t, n) {
-                            const r = a.ReactWidget.create(i().createElement(Y, {
+                            const r = a.ReactWidget.create(i().createElement(ne, {
                                 selectionWatcher: e,
                                 chatHandler: t,
                                 globalAwareness: n
                             }));
-                            return r.id = "jupyter-ai::chat", r.title.icon = R, r.title.caption = "Jupyter AI Chat", r
+                            return r.id = "jupyter-ai::chat", r.title.icon = N, r.title.caption = "Jupyter AI Chat", r
                         }(r, o, t)
                     } catch (e) {
                         l = function() {
                             const e = a.ReactWidget.create(i().createElement(g, null, i().createElement(c.Box, {
                                 sx: {
                                     width: "100%",
                                     height: "100%",
@@ -992,15 +1100,15 @@
                             }, i().createElement(c.Box, {
                                 sx: {
                                     padding: 4
                                 }
                             }, i().createElement(c.Alert, {
                                 severity: "error"
                             }, "There seems to be a problem with the Chat backend, please look at the JupyterLab server logs or contact your administrator to correct this problem.")))));
-                            return e.id = "jupyter-ai::chat", e.title.icon = R, e.title.caption = "Jupyter AI Chat", e
+                            return e.id = "jupyter-ai::chat", e.title.icon = N, e.title.caption = "Jupyter AI Chat", e
                         }()
                     }
                     e.shell.add(l, "left", {
                         rank: 2e3
                     }), n && n.add(l, "jupyter-ai-chat")
                 }
             }
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/643.d05f12a52798d8475b12.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/643.ca949b2ea9d252cbcc23.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,35 @@
 "use strict";
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
     [643], {
         61246: (e, n, t) => {
             t.d(n, {
-                Z: () => s
+                Z: () => l
             });
             var r = t(82609),
                 i = t.n(r),
                 o = t(83055),
                 a = t(98814),
+                s = t(22299),
                 c = i()((function(e) {
                     return e[1]
                 }));
-            c.i(o.Z), c.i(a.Z), c.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/", ""]);
-            const s = c
+            c.i(o.Z), c.i(a.Z), c.i(s.Z), c.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/", ""]);
+            const l = c
+        },
+        22299: (e, n, t) => {
+            t.d(n, {
+                Z: () => o
+            });
+            var r = t(82609),
+                i = t.n(r)()((function(e) {
+                    return e[1]
+                }));
+            i.push([e.id, ".jp-ai-ChatSettings-header {\n    font-size: var(--jp-ui-font-size3);\n    font-weight: 400;\n    color: var(--jp-ui-font-color1);\n}", ""]);
+            const o = i
         },
         83055: (e, n, t) => {
             t.d(n, {
                 Z: () => o
             });
             var r = t(82609),
                 i = t.n(r)()((function(e) {
@@ -51,17 +63,17 @@
                     ]);
                     var i = {};
                     if (r)
                         for (var o = 0; o < this.length; o++) {
                             var a = this[o][0];
                             null != a && (i[a] = !0)
                         }
-                    for (var c = 0; c < e.length; c++) {
-                        var s = [].concat(e[c]);
-                        r && i[s[0]] || (t && (s[2] ? s[2] = "".concat(t, " and ").concat(s[2]) : s[2] = t), n.push(s))
+                    for (var s = 0; s < e.length; s++) {
+                        var c = [].concat(e[s]);
+                        r && i[c[0]] || (t && (c[2] ? c[2] = "".concat(t, " and ").concat(c[2]) : c[2] = t), n.push(c))
                     }
                 }, n
             }
         },
         46062: (e, n, t) => {
             var r, i = function() {
                     var e = {};
@@ -84,36 +96,36 @@
                 for (var n = -1, t = 0; t < o.length; t++)
                     if (o[t].identifier === e) {
                         n = t;
                         break
                     } return n
             }
 
-            function c(e, n) {
+            function s(e, n) {
                 for (var t = {}, r = [], i = 0; i < e.length; i++) {
-                    var c = e[i],
-                        s = n.base ? c[0] + n.base : c[0],
-                        l = t[s] || 0,
-                        d = "".concat(s, " ").concat(l);
-                    t[s] = l + 1;
+                    var s = e[i],
+                        c = n.base ? s[0] + n.base : s[0],
+                        l = t[c] || 0,
+                        d = "".concat(c, " ").concat(l);
+                    t[c] = l + 1;
                     var u = a(d),
                         f = {
-                            css: c[1],
-                            media: c[2],
-                            sourceMap: c[3]
+                            css: s[1],
+                            media: s[2],
+                            sourceMap: s[3]
                         }; - 1 !== u ? (o[u].references++, o[u].updater(f)) : o.push({
                         identifier: d,
                         updater: h(f, n),
                         references: 1
                     }), r.push(d)
                 }
                 return r
             }
 
-            function s(e) {
+            function c(e) {
                 var n = document.createElement("style"),
                     r = e.attributes || {};
                 if (void 0 === r.nonce) {
                     var o = t.nc;
                     o && (r.nonce = o)
                 }
                 if (Object.keys(r).forEach((function(e) {
@@ -153,16 +165,16 @@
             var p = null,
                 v = 0;
 
             function h(e, n) {
                 var t, r, i;
                 if (n.singleton) {
                     var o = v++;
-                    t = p || (p = s(n)), r = u.bind(null, t, o, !1), i = u.bind(null, t, o, !0)
-                } else t = s(n), r = f.bind(null, t, n), i = function() {
+                    t = p || (p = c(n)), r = u.bind(null, t, o, !1), i = u.bind(null, t, o, !0)
+                } else t = c(n), r = f.bind(null, t, n), i = function() {
                     ! function(e) {
                         if (null === e.parentNode) return !1;
                         e.parentNode.removeChild(e)
                     }(t)
                 };
                 return r(e),
                     function(n) {
@@ -170,26 +182,26 @@
                             if (n.css === e.css && n.media === e.media && n.sourceMap === e.sourceMap) return;
                             r(e = n)
                         } else i()
                     }
             }
             e.exports = function(e, n) {
                 (n = n || {}).singleton || "boolean" == typeof n.singleton || (n.singleton = (void 0 === r && (r = Boolean(window && document && document.all && !window.atob)), r));
-                var t = c(e = e || [], n);
+                var t = s(e = e || [], n);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
                         for (var r = 0; r < t.length; r++) {
                             var i = a(t[r]);
                             o[i].references--
                         }
-                        for (var s = c(e, n), l = 0; l < t.length; l++) {
+                        for (var c = s(e, n), l = 0; l < t.length; l++) {
                             var d = a(t[l]);
                             0 === o[d].references && (o[d].updater(), o.splice(d, 1))
                         }
-                        t = s
+                        t = c
                     }
                 }
             }
         },
         76643: (e, n, t) => {
             t.r(n);
             var r = t(46062),
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
                 return ("" === n[n.length - 1] ? [...n, ""] : n).join((e.padRight ? " " : "") + "," + (!1 === e.padLeft ? "" : " ")).trim()
             }
             e.d(l, {
                 P: () => a,
                 Q: () => o
             })
         },
-        30253: (n, l, e) => {
+        67597: (n, l, e) => {
             e.d(l, {
                 dy: () => y,
                 YP: () => v
             });
             class o {
                 constructor(n, l, e) {
                     this.property = n, this.normal = l, e && (this.space = e)
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/861.f0852a9fe000bee67405.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 861.f0852a9fe000bee67405.js.LICENSE.txt */
+/*! For license information please see 861.c7c12ea31e8b5552473d.js.LICENSE.txt */
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
     [861], {
         49385: e => {
             "use strict";
             var t = Object.prototype.hasOwnProperty,
                 n = Object.prototype.toString,
                 r = Object.defineProperty,
@@ -3906,15 +3906,15 @@
                     }
                 }(e, t) : function(e) {
                     return t => Rt(t, e)
                 }(e || t)
             };
             var Mt = n(13980),
                 $t = n.n(Mt),
-                Vt = n(30253);
+                Vt = n(67597);
 
             function qt(e) {
                 if (e.allowedElements && e.disallowedElements) throw new TypeError("Only one of `allowedElements` and `disallowedElements` should be defined");
                 if (e.allowedElements || e.disallowedElements || e.allowElement) return t => {
                     (0, xt.Vn)(t, "element", ((t, n, r) => {
                         const i = r;
                         let o;
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/900.aad7c14c6d8f76011810.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9738,15 +9738,15 @@
                 html: "http://www.w3.org/1999/xhtml",
                 mathml: "http://www.w3.org/1998/Math/MathML",
                 svg: "http://www.w3.org/2000/svg",
                 xlink: "http://www.w3.org/1999/xlink",
                 xml: "http://www.w3.org/XML/1998/namespace",
                 xmlns: "http://www.w3.org/2000/xmlns/"
             };
-            var xn = r(30253),
+            var xn = r(67597),
                 wn = r(60204),
                 kn = r(4144);
             const Sn = /[#.]/g;
             var Mn = r(93113),
                 zn = r(97327);
             const An = new Set(["menu", "submit", "reset", "button"]),
                 Tn = {}.hasOwnProperty;
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/remoteEntry.df84a6245b68ae8abd9f.js` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/remoteEntry.e77e7c805bbe3d26eec6.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, f, l, c, d, u, s, p, h, b, m, v, y, g, j, P, w, k, _, O, S = {
+    var e, r, t, a, o, n, i, l, f, d, u, c, s, p, h, b, m, v, y, g, j, P, w, k, _, O, S = {
             22399: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(639)]).then((() => () => t(11639))),
-                        "./extension": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(639)]).then((() => () => t(11639))),
+                        "./index": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(253)]).then((() => () => t(30253))),
+                        "./extension": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(253)]).then((() => () => t(30253))),
                         "./style": () => t.e(643).then((() => () => t(76643)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -56,87 +56,87 @@
         return n.default = () => t, x.d(o, n), o
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
+        253: "0b5d158f3577d0bfbee5",
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
-        639: "b63fa10cbcf2eccddd7d",
-        643: "d05f12a52798d8475b12",
+        643: "ca949b2ea9d252cbcc23",
         675: "e2778aeb06575c94bca0",
-        693: "2c3da85cc10c904e2289",
+        693: "970d9a45469683adfff5",
         703: "3d0d8b7012529f0dd511",
         819: "5279f5daf1d1f505f15f",
         860: "03421bb262ea8bfa0af1",
-        861: "f0852a9fe000bee67405",
-        900: "aad7c14c6d8f76011810",
+        861: "c7c12ea31e8b5552473d",
+        900: "899d3fbf00938382f665",
         963: "59c8f2feb6aaf0b34378"
     } [e] + ".js?v=" + {
+        253: "0b5d158f3577d0bfbee5",
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
-        639: "b63fa10cbcf2eccddd7d",
-        643: "d05f12a52798d8475b12",
+        643: "ca949b2ea9d252cbcc23",
         675: "e2778aeb06575c94bca0",
-        693: "2c3da85cc10c904e2289",
+        693: "970d9a45469683adfff5",
         703: "3d0d8b7012529f0dd511",
         819: "5279f5daf1d1f505f15f",
         860: "03421bb262ea8bfa0af1",
-        861: "f0852a9fe000bee67405",
-        900: "aad7c14c6d8f76011810",
+        861: "c7c12ea31e8b5552473d",
+        900: "899d3fbf00938382f665",
         963: "59c8f2feb6aaf0b34378"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupyter-ai/core:", x.l = (e, r, o, n) => {
         if (t[e]) t[e].push(r);
         else {
-            var i, f;
+            var i, l;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), c = 0; c < l.length; c++) {
-                    var d = l[c];
-                    if (d.getAttribute("src") == e || d.getAttribute("data-webpack") == a + o) {
-                        i = d;
+                for (var f = document.getElementsByTagName("script"), d = 0; d < f.length; d++) {
+                    var u = f[d];
+                    if (u.getAttribute("src") == e || u.getAttribute("data-webpack") == a + o) {
+                        i = u;
                         break
                     }
                 }
-            i || (f = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
-            var u = (r, a) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
+            var c = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var o = t[e];
                     if (delete t[e], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                s = setTimeout(u.bind(null, void 0, {
+                s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = u.bind(null, i.onerror), i.onload = u.bind(null, i.onload), f && document.head.appendChild(i)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
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
-                    f = (e, r, t, a) => {
+                    l = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            f = o[r];
-                        (!f || !f.loaded && (!a != !f.eager ? a : i > f.from)) && (o[r] = {
+                            l = o[r];
+                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    l = [];
-                return "default" === t && (f("@emotion/react", "11.11.0", (() => Promise.all([x.e(296), x.e(527), x.e(271), x.e(342)]).then((() => () => x(26527))))), f("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(271), x.e(564), x.e(407)]).then((() => () => x(52675))))), f("@jupyter-ai/core", "0.7.3", (() => Promise.all([x.e(341), x.e(380), x.e(271), x.e(963), x.e(639)]).then((() => () => x(11639))))), f("@mui/material", "5.13.1", (() => Promise.all([x.e(296), x.e(860), x.e(341), x.e(271), x.e(564), x.e(963), x.e(456)]).then((() => () => x(30860))))), f("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(271)]).then((() => () => x(81861))))), f("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(271)]).then((() => () => x(95598))))), f("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), f("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (l("@emotion/react", "11.11.0", (() => Promise.all([x.e(296), x.e(527), x.e(271), x.e(342)]).then((() => () => x(26527))))), l("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(271), x.e(564), x.e(407)]).then((() => () => x(52675))))), l("@jupyter-ai/core", "0.8.0", (() => Promise.all([x.e(341), x.e(380), x.e(271), x.e(963), x.e(253)]).then((() => () => x(30253))))), l("@mui/material", "5.13.1", (() => Promise.all([x.e(296), x.e(860), x.e(341), x.e(271), x.e(564), x.e(963), x.e(456)]).then((() => () => x(30860))))), l("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(271)]).then((() => () => x(81861))))), l("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(271)]).then((() => () => x(95598))))), l("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), l("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,132 +185,132 @@
         e = o(e), r = o(r);
         for (var t = 0;;) {
             if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
             var a = e[t],
                 n = (typeof a)[0];
             if (t >= r.length) return "u" == n;
             var i = r[t],
-                f = (typeof i)[0];
-            if (n != f) return "o" == n && "n" == f || "s" == f || "u" == n;
+                l = (typeof i)[0];
+            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
             if ("o" != n && "u" != n && a != i) return a < i;
             t++
         }
     }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(f = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, f);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
         var n = [];
         for (o = 1; o < e.length; o++) {
-            var f = e[o];
-            n.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? n.pop() + " " + n.pop() : i(f))
+            var l = e[o];
+            n.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? n.pop() + " " + n.pop() : i(l))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return n.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, f = (e, r) => {
+    }, l = (e, r) => {
         if (0 in e) {
             r = o(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
-            for (var n = 0, i = 1, l = !0;; i++, n++) {
-                var c, d, u = i < e.length ? (typeof e[i])[0] : "";
-                if (n >= r.length || "o" == (d = (typeof(c = r[n]))[0])) return !l || ("u" == u ? i > t && !a : "" == u != a);
-                if ("u" == d) {
-                    if (!l || "u" != u) return !1
-                } else if (l)
-                    if (u == d)
+            for (var n = 0, i = 1, f = !0;; i++, n++) {
+                var d, u, c = i < e.length ? (typeof e[i])[0] : "";
+                if (n >= r.length || "o" == (u = (typeof(d = r[n]))[0])) return !f || ("u" == c ? i > t && !a : "" == c != a);
+                if ("u" == u) {
+                    if (!f || "u" != c) return !1
+                } else if (f)
+                    if (c == u)
                         if (i <= t) {
-                            if (c != e[i]) return !1
+                            if (d != e[i]) return !1
                         } else {
-                            if (a ? c > e[i] : c < e[i]) return !1;
-                            c != e[i] && (l = !1)
+                            if (a ? d > e[i] : d < e[i]) return !1;
+                            d != e[i] && (f = !1)
                         }
-                else if ("s" != u && "n" != u) {
+                else if ("s" != c && "n" != c) {
                     if (a || i <= t) return !1;
-                    l = !1, i--
+                    f = !1, i--
                 } else {
-                    if (i <= t || d < u != a) return !1;
-                    l = !1
-                } else "s" != u && "n" != u && (l = !1, i--)
+                    if (i <= t || u < c != a) return !1;
+                    f = !1
+                } else "s" != c && "n" != c && (f = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (n = 1; n < e.length; n++) {
             var h = e[n];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? f(h, r) : !p())
+            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? l(h, r) : !p())
         }
         return !!p()
-    }, l = (e, r) => {
+    }, f = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, c = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
-    }, d = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(a) + ")", s = (e, r, t, a) => {
-        var o = d(e, t);
-        return f(a, o) || b(u(e, t, o, a)), v(e[t][o])
+    }, c = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(a) + ")", s = (e, r, t, a) => {
+        var o = u(e, t);
+        return l(a, o) || b(c(e, t, o, a)), v(e[t][o])
     }, p = (e, r, t) => {
         var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !f(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+        return (r = Object.keys(a).reduce(((e, r) => !l(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
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
-    })(((e, r, t, a) => r && x.o(r, t) ? v(c(r, t)) : a())), j = y(((e, r, t, a) => (l(e, t), v(p(r, t, a) || m(r, e, t, a) || c(r, t))))), P = y(((e, r, t, a) => (l(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
+    })(((e, r, t, a) => r && x.o(r, t) ? v(d(r, t)) : a())), j = y(((e, r, t, a) => (f(e, t), v(p(r, t, a) || m(r, e, t, a) || d(r, t))))), P = y(((e, r, t, a) => (f(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
         var n = r && x.o(r, t) && p(r, t, a);
         return n ? v(n) : o()
     })), k = {}, _ = {
         56271: () => P("default", "react", [1, 17, 0, 1]),
         79510: () => w("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([x.e(296), x.e(527), x.e(365)]).then((() => () => x(26527))))),
         92764: () => w("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([x.e(675), x.e(564), x.e(407)]).then((() => () => x(52675))))),
-        22502: () => P("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
-        26413: () => P("default", "@jupyterlab/codemirror", [1, 3, 6, 3]),
-        28142: () => P("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        11872: () => P("default", "@jupyterlab/services", [1, 6, 6, 4]),
+        26676: () => j("default", "@jupyterlab/docregistry", [1, 3, 6, 4]),
         30535: () => w("default", "react-markdown", [1, 8, 0, 6], (() => Promise.all([x.e(693), x.e(861)]).then((() => () => x(81861))))),
         35048: () => w("default", "@mui/material", [1, 5, 11, 0], (() => Promise.all([x.e(296), x.e(860), x.e(564), x.e(456)]).then((() => () => x(30860))))),
-        35059: () => P("default", "@jupyterlab/collaboration", [1, 3, 6, 3]),
+        36705: () => P("default", "@jupyterlab/codemirror", [1, 3, 6, 4]),
         40532: () => w("default", "rehype-katex", [1, 6, 0, 2], (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))),
-        41123: () => P("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        45687: () => P("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        48820: () => P("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        51473: () => P("default", "@jupyterlab/fileeditor", [1, 3, 6, 3]),
+        49764: () => P("default", "@jupyterlab/apputils", [1, 3, 6, 4]),
         55351: () => w("default", "react-syntax-highlighter", [1, 15, 5, 0], (() => x.e(598).then((() => () => x(95598))))),
         71840: () => P("default", "@lumino/signaling", [1, 1, 10, 0]),
-        73033: () => P("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        75884: () => P("default", "@jupyterlab/collaboration", [1, 3, 6, 4]),
+        76779: () => P("default", "@jupyterlab/notebook", [1, 3, 6, 4]),
+        78667: () => P("default", "@jupyterlab/ui-components", [1, 3, 6, 4]),
         78918: () => P("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        80819: () => j("default", "@jupyterlab/docregistry", [1, 3, 6, 3]),
+        82883: () => P("default", "@jupyterlab/fileeditor", [1, 3, 6, 4]),
+        83058: () => P("default", "@jupyterlab/coreutils", [1, 5, 6, 4]),
+        96175: () => P("default", "@jupyterlab/application", [1, 3, 6, 4]),
         96707: () => w("default", "remark-math", [1, 5, 1, 1], (() => x.e(703).then((() => () => x(7703))))),
         17564: () => g("default", "@emotion/react", (() => Promise.all([x.e(296), x.e(527), x.e(819)]).then((() => () => x(26527))))),
         24407: () => w("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([x.e(296), x.e(527)]).then((() => () => x(26527))))),
         14456: () => P("default", "react-dom", [1, 17, 0, 1])
     }, O = {
+        253: [11872, 26676, 30535, 35048, 36705, 40532, 49764, 55351, 71840, 75884, 76779, 78667, 78918, 82883, 83058, 96175, 96707],
         271: [56271],
         407: [24407],
         456: [14456],
         564: [17564],
-        639: [22502, 26413, 28142, 30535, 35048, 35059, 40532, 41123, 45687, 48820, 51473, 55351, 71840, 73033, 78918, 80819, 96707],
         963: [79510, 92764]
     }, x.f.consumes = (e, r) => {
         x.o(O, e) && O[e].forEach((e => {
             if (x.o(k, e)) return r.push(k[e]);
             var t = r => {
                     k[e] = 0, x.m[e] = t => {
                         delete x.c[e], t.exports = r()
@@ -348,21 +348,21 @@
                             n = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, i, f] = t,
-                    l = 0;
+                var a, o, [n, i, l] = t,
+                    f = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in i) x.o(i, a) && (x.m[a] = i[a]);
-                    f && f(x)
+                    l && l(x)
                 }
-                for (r && r(t); l < n.length; l++) o = n[l], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < n.length; f++) o = n[f], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), x.nc = void 0;
     var T = x(22399);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter-ai/core"] = T
 })();
```

### Comparing `jupyter_ai-0.7.3/jupyter_ai/labextension/static/third-party-licenses.json` & `jupyter_ai-0.8.0/jupyter_ai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/schema/plugin.json` & `jupyter_ai-0.8.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/chat_handler.ts` & `jupyter_ai-0.8.0/src/chat_handler.ts`

 * *Files 6% similar despite different names*

```diff
@@ -25,42 +25,19 @@
   }
 
   /**
    * Initializes the WebSocket connection to the Chat backend. Promise is
    * resolved when server acknowledges connection and sends the client ID. This
    * must be awaited before calling any other method.
    */
-  public initialize(): Promise<void> {
-    return new Promise<void>((resolve, reject) => {
-      if (this.isDisposed) {
-        return;
-      }
-      const { token, WebSocket, wsUrl } = this.serverSettings;
-      const url =
-        URLExt.join(wsUrl, CHAT_SERVICE_URL) +
-        (token ? `?token=${encodeURIComponent(token)}` : '');
-
-      const socket = (this._socket = new WebSocket(url));
-      socket.onerror = (e) => reject(e);
-      socket.onmessage = msg =>
-        msg.data && this._onMessage(JSON.parse(msg.data));
-
-      const listenForConnection = (message: AiService.Message) => {
-        if (message.type !== 'connection') {
-          return;
-        }
-        this.id = message.client_id;
-        resolve();
-        this.removeListener(listenForConnection);
-      };
-
-      this.addListener(listenForConnection);
-    });
+  public async initialize() {
+    await this._initialize();
   }
 
+
   /**
    * Sends a message across the WebSocket. Promise resolves to the message ID
    * when the server sends the same message back, acknowledging receipt.
    */
   public sendMessage(message: AiService.ChatRequest): Promise<string> {
     return new Promise(resolve => {
       this._socket?.send(JSON.stringify(message));
@@ -112,15 +89,14 @@
    * Dispose the chat handler.
    */
   dispose(): void {
     if (this.isDisposed) {
       return;
     }
     this._isDisposed = true;
-
     this._listeners = [];
 
     // Clean up socket.
     const socket = this._socket;
     if (socket) {
       this._socket = null;
       socket.onopen = () => undefined;
@@ -160,11 +136,53 @@
    * `replyFor()`.
    */
   private _replyForResolverDict: Record<
     string,
     (value: AiService.AgentChatMessage) => void
   > = {};
 
+  private _onClose(e: CloseEvent, reject: any) {
+    reject(new Error("Chat UI websocket disconnected"))
+    console.error("Chat UI websocket disconnected")
+    // only attempt re-connect if there was an abnormal closure
+    // WebSocket status codes defined in RFC 6455: https://www.rfc-editor.org/rfc/rfc6455.html#section-7.4.1
+    if (e.code === 1006) {
+      const delaySeconds = 1
+      console.info(`Will try to reconnect in ${delaySeconds} s.`)
+      setTimeout(async () => await this._initialize(), delaySeconds * 1000);
+    }
+  }
+
+  private _initialize(): Promise<void> {
+    return new Promise<void>((resolve, reject) => {
+      if (this.isDisposed) {
+        return;
+      }
+      console.log("Creating a new websocket connection for chat...");
+      const { token, WebSocket, wsUrl } = this.serverSettings;
+      const url =
+        URLExt.join(wsUrl, CHAT_SERVICE_URL) +
+        (token ? `?token=${encodeURIComponent(token)}` : '');
+      
+        const socket = (this._socket = new WebSocket(url));
+        socket.onclose = (e) => this._onClose(e, reject);
+        socket.onerror = (e) => reject(e);
+        socket.onmessage = msg =>
+          msg.data && this._onMessage(JSON.parse(msg.data));
+        
+        const listenForConnection = (message: AiService.Message) => {
+          if (message.type !== 'connection') {
+            return;
+          }
+          this.id = message.client_id;
+          resolve();
+          this.removeListener(listenForConnection);
+        };
+  
+        this.addListener(listenForConnection);
+    });
+  }
+
   private _isDisposed = false;
   private _socket: WebSocket | null = null;
   private _listeners: ((msg: any) => void)[] = [];
 }
```

### Comparing `jupyter_ai-0.7.3/src/handler.ts` & `jupyter_ai-0.8.0/src/handler.ts`

 * *Files 5% similar despite different names*

```diff
@@ -166,14 +166,15 @@
   }
 
   export type Config = {
     model_provider_id: string | null;
     embeddings_provider_id: string | null;
     api_keys: Record<string, string>;
     send_with_shift_enter: boolean | null;
+    fields: Record<string, Record<string, any>>;
   };
 
   export type GetConfigResponse = Config;
 
   export type UpdateConfigRequest = Config;
 
   export async function getConfig(): Promise<GetConfigResponse> {
@@ -187,19 +188,35 @@
 
   export type AwsAuthStrategy = {
     type: 'aws';
   };
 
   export type AuthStrategy = EnvAuthStrategy | AwsAuthStrategy | null;
 
+  export type TextField = {
+    type: 'text';
+    key: string;
+    label: string;
+  };
+
+  export type MultilineTextField = {
+    type: 'text-multiline';
+    key: string;
+    label: string;
+  };
+
+  export type Field = TextField | MultilineTextField;
+
   export type ListProvidersEntry = {
     id: string;
     name: string;
     models: string[];
     auth_strategy: AuthStrategy;
+    registry: boolean;
+    fields: Field[];
   };
 
   export type ListProvidersResponse = {
     providers: ListProvidersEntry[];
   };
 
   export async function listLmProviders(): Promise<ListProvidersResponse> {
```

### Comparing `jupyter_ai-0.7.3/src/icons.ts` & `jupyter_ai-0.8.0/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/index.ts` & `jupyter_ai-0.8.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/inserter.ts` & `jupyter_ai-0.8.0/src/inserter.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/selection-watcher.ts` & `jupyter_ai-0.8.0/src/selection-watcher.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/theme-provider.ts` & `jupyter_ai-0.8.0/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/utils.ts` & `jupyter_ai-0.8.0/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/__tests__/widgets/closable-dialog.spec.tsx` & `jupyter_ai-0.8.0/src/__tests__/widgets/closable-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/chat-code-view.tsx` & `jupyter_ai-0.8.0/src/components/chat-code-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/chat-input.tsx` & `jupyter_ai-0.8.0/src/components/chat-input.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/chat-messages.tsx` & `jupyter_ai-0.8.0/src/components/chat-messages.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/chat.tsx` & `jupyter_ai-0.8.0/src/components/chat.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/expandable-text-field.tsx` & `jupyter_ai-0.8.0/src/components/expandable-text-field.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/jl-theme-provider.tsx` & `jupyter_ai-0.8.0/src/components/jl-theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/open-task-dialog.tsx` & `jupyter_ai-0.8.0/src/components/open-task-dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/scroll-container.tsx` & `jupyter_ai-0.8.0/src/components/scroll-container.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/components/select.tsx` & `jupyter_ai-0.8.0/src/components/select.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/contexts/collaborators-context.tsx` & `jupyter_ai-0.8.0/src/contexts/collaborators-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/contexts/selection-context.tsx` & `jupyter_ai-0.8.0/src/contexts/selection-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/widgets/chat-error.tsx` & `jupyter_ai-0.8.0/src/widgets/chat-error.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/widgets/chat-sidebar.tsx` & `jupyter_ai-0.8.0/src/widgets/chat-sidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/src/widgets/closable-dialog.tsx` & `jupyter_ai-0.8.0/src/widgets/closable-dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/style/icons/jupyternaut.svg` & `jupyter_ai-0.8.0/style/icons/jupyternaut.svg`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/ui-tests/README.md` & `jupyter_ai-0.8.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/ui-tests/jupyter_server_test_config.py` & `jupyter_ai-0.8.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/ui-tests/tests/jupyter_ai.spec.ts` & `jupyter_ai-0.8.0/ui-tests/tests/jupyter_ai.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/.gitignore` & `jupyter_ai-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/LICENSE` & `jupyter_ai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/README.md` & `jupyter_ai-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/pyproject.toml` & `jupyter_ai-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.7.3/PKG-INFO` & `jupyter_ai-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai
-Version: 0.7.3
+Version: 0.8.0
 Summary: A generative AI extension for JupyterLab
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

