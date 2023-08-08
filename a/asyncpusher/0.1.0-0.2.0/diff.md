# Comparing `tmp/asyncpusher-0.1.0.tar.gz` & `tmp/asyncpusher-0.2.0.tar.gz`

## Comparing `asyncpusher-0.1.0.tar` & `asyncpusher-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/Pipfile
--rw-r--r--   0        0        0    52210 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/asyncpusher/__init__.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/asyncpusher/channel.py
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/asyncpusher/connection.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/asyncpusher/pusher.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/LICENSE
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/README.md
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 asyncpusher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/.env.example
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/Pipfile
+-rw-r--r--   0        0        0    71208 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/Pipfile.lock
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/asyncpusher/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/asyncpusher/channel.py
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/asyncpusher/connection.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/asyncpusher/pusher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/tests/simple_api.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/tests/test_pusher.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/README.md
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 asyncpusher-0.2.0/PKG-INFO
```

### Comparing `asyncpusher-0.1.0/Pipfile.lock` & `asyncpusher-0.2.0/Pipfile.lock`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9503676470588235%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'8e0f42893a47d7deaf86b43a34884cb06b614827ff8100cd0b73c711fab604d1'}}",*

 * * "'develop'": "{'cffi': OrderedDict([('hashes', "*

 * *              "['sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5', "*

 * *              "'sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef', "*

 * *              "'sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104', "*

 * *              "'sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8be […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "302e78767d76b694ff264eea545d9733960880ce1b1ece133b303b2553e012bb"
+            "sha256": "8e0f42893a47d7deaf86b43a34884cb06b614827ff8100cd0b73c711fab604d1"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.11"
         },
         "sources": [
             {
@@ -491,22 +491,201 @@
             "hashes": [
                 "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
                 "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2023.7.22"
         },
+        "cffi": {
+            "hashes": [
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+            ],
+            "version": "==1.15.1"
+        },
+        "charset-normalizer": {
+            "hashes": [
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
+            ],
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.2.0"
+        },
         "click": {
             "hashes": [
                 "sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd",
                 "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.1.6"
         },
+        "cryptography": {
+            "hashes": [
+                "sha256:0d09fb5356f975974dbcb595ad2d178305e5050656affb7890a1583f5e02a306",
+                "sha256:23c2d778cf829f7d0ae180600b17e9fceea3c2ef8b31a99e3c694cbbf3a24b84",
+                "sha256:3fb248989b6363906827284cd20cca63bb1a757e0a2864d4c1682a985e3dca47",
+                "sha256:41d7aa7cdfded09b3d73a47f429c298e80796c8e825ddfadc84c8a7f12df212d",
+                "sha256:42cb413e01a5d36da9929baa9d70ca90d90b969269e5a12d39c1e0d475010116",
+                "sha256:4c2f0d35703d61002a2bbdcf15548ebb701cfdd83cdc12471d2bae80878a4207",
+                "sha256:4fd871184321100fb400d759ad0cddddf284c4b696568204d281c902fc7b0d81",
+                "sha256:5259cb659aa43005eb55a0e4ff2c825ca111a0da1814202c64d28a985d33b087",
+                "sha256:57a51b89f954f216a81c9d057bf1a24e2f36e764a1ca9a501a6964eb4a6800dd",
+                "sha256:652627a055cb52a84f8c448185922241dd5217443ca194d5739b44612c5e6507",
+                "sha256:67e120e9a577c64fe1f611e53b30b3e69744e5910ff3b6e97e935aeb96005858",
+                "sha256:6af1c6387c531cd364b72c28daa29232162010d952ceb7e5ca8e2827526aceae",
+                "sha256:6d192741113ef5e30d89dcb5b956ef4e1578f304708701b8b73d38e3e1461f34",
+                "sha256:7efe8041897fe7a50863e51b77789b657a133c75c3b094e51b5e4b5cec7bf906",
+                "sha256:84537453d57f55a50a5b6835622ee405816999a7113267739a1b4581f83535bd",
+                "sha256:8f09daa483aedea50d249ef98ed500569841d6498aa9c9f4b0531b9964658922",
+                "sha256:95dd7f261bb76948b52a5330ba5202b91a26fbac13ad0e9fc8a3ac04752058c7",
+                "sha256:a74fbcdb2a0d46fe00504f571a2a540532f4c188e6ccf26f1f178480117b33c4",
+                "sha256:a983e441a00a9d57a4d7c91b3116a37ae602907a7618b882c8013b5762e80574",
+                "sha256:ab8de0d091acbf778f74286f4989cf3d1528336af1b59f3e5d2ebca8b5fe49e1",
+                "sha256:aeb57c421b34af8f9fe830e1955bf493a86a7996cc1338fe41b30047d16e962c",
+                "sha256:ce785cf81a7bdade534297ef9e490ddff800d956625020ab2ec2780a556c313e",
+                "sha256:d0d651aa754ef58d75cec6edfbd21259d93810b73f6ec246436a21b7841908de"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.3"
+        },
         "distlib": {
             "hashes": [
                 "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
                 "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
             "version": "==0.3.7"
         },
@@ -633,14 +812,22 @@
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
+        "ndg-httpsclient": {
+            "hashes": [
+                "sha256:d2c7225f6a1c6cf698af4ebc962da70178a99bcde24ee6d1961c4f3338130d57",
+                "sha256:d72faed0376ab039736c2ba12e30695e2788c4aa569c9c3e3d72131de2592210",
+                "sha256:dd174c11d971b6244a891f7be2b32ca9853d3797a72edb34fa5d7b07d8fff7d4"
+            ],
+            "version": "==0.5.1"
+        },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
@@ -679,28 +866,83 @@
         "ptyprocess": {
             "hashes": [
                 "sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35",
                 "sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220"
             ],
             "version": "==0.7.0"
         },
+        "pusher": {
+            "hashes": [
+                "sha256:14f412c8e26562aaf663a114951792fefae01f0d220dac84971f926404620760",
+                "sha256:4ae2d2dc77eb28043da042796992b8b41454f458c4d8c8e151f7498f2c4374c7"
+            ],
+            "index": "pypi",
+            "version": "==3.3.2"
+        },
+        "pyasn1": {
+            "hashes": [
+                "sha256:87a2121042a1ac9358cabcaf1d07680ff97ee6404333bacca15f76aa8ad01a57",
+                "sha256:97b7290ca68e62a832558ec3976f15cbf911bf5d7c7039d8b861c2a0ece69fde"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
+            "version": "==0.5.0"
+        },
+        "pycparser": {
+            "hashes": [
+                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
+                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+            ],
+            "version": "==2.21"
+        },
         "pygments": {
             "hashes": [
                 "sha256:13fc09fa63bc8d8671a6d247e1eb303c4b343eaee81d861f3404db2935653692",
                 "sha256:1daff0494820c69bc8941e407aa20f577374ee88364ee10a98fdbe0aece96e29"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.16.1"
         },
+        "pynacl": {
+            "hashes": [
+                "sha256:06b8f6fa7f5de8d5d2f7573fe8c863c051225a27b61e6860fd047b1775807858",
+                "sha256:0c84947a22519e013607c9be43706dd42513f9e6ae5d39d3613ca1e142fba44d",
+                "sha256:20f42270d27e1b6a29f54032090b972d97f0a1b0948cc52392041ef7831fee93",
+                "sha256:401002a4aaa07c9414132aaed7f6836ff98f59277a234704ff66878c2ee4a0d1",
+                "sha256:52cb72a79269189d4e0dc537556f4740f7f0a9ec41c1322598799b0bdad4ef92",
+                "sha256:61f642bf2378713e2c2e1de73444a3778e5f0a38be6fee0fe532fe30060282ff",
+                "sha256:8ac7448f09ab85811607bdd21ec2464495ac8b7c66d146bf545b0f08fb9220ba",
+                "sha256:a36d4a9dda1f19ce6e03c9a784a2921a4b726b02e1c736600ca9c22029474394",
+                "sha256:a422368fc821589c228f4c49438a368831cb5bbc0eab5ebe1d7fac9dded6567b",
+                "sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==1.5.0"
+        },
+        "pyopenssl": {
+            "hashes": [
+                "sha256:24f0dc5227396b3e831f4c7f602b950a5e9833d292c8e4a2e06b709292806ae2",
+                "sha256:276f931f55a452e7dea69c7173e984eb2a4407ce413c918aa34b55f82f9b8bac"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==23.2.0"
+        },
         "pyperclip": {
             "hashes": [
                 "sha256:105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57"
             ],
             "version": "==1.8.2"
         },
+        "requests": {
+            "hashes": [
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
+        },
         "rich": {
             "hashes": [
                 "sha256:146a90b3b6b47cac4a73c12866a499e9817426423f57c5a66949c086191a8808",
                 "sha256:fb9d6c0a0f643c99eed3875b5377a184132ba9be4d61516a55273d3554d75a39"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.5.2"
@@ -732,14 +974,22 @@
             "hashes": [
                 "sha256:368bf8c00754fd4f55afb7bbb86e272df77e4dc76ac29dbcbb81a59e9fc15744",
                 "sha256:823bc5fb5c34d60f285b624e7264f4dda254bc803a3774a147bf99c0e3004a28"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.5.0.post1"
         },
+        "six": {
+            "hashes": [
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
+        },
         "sniffio": {
             "hashes": [
                 "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101",
                 "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.3.0"
@@ -763,14 +1013,22 @@
         "trove-classifiers": {
             "hashes": [
                 "sha256:8a8e168b51d20fed607043831d37632bb50919d1c80a64e0f1393744691a8b22",
                 "sha256:b420d5aa048ee7c456233a49203f7d58d1736af4a6cde637657d78c13ab7969b"
             ],
             "version": "==2023.7.6"
         },
+        "urllib3": {
+            "hashes": [
+                "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
+                "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.4"
+        },
         "userpath": {
             "hashes": [
                 "sha256:8069f754d31edfbdb2c3b2e9abada057ce7518290838dac35d1c8cee1b4cc7b0",
                 "sha256:85e3274543174477c62d5701ed43a3ef1051824a9dd776968adc411e58640dd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.9.0"
```

### Comparing `asyncpusher-0.1.0/asyncpusher/channel.py` & `asyncpusher-0.2.0/asyncpusher/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,19 @@
     class State(Enum):
         UNSUBSCRIBED = 1
         SUBSCRIBED = 2
         FAILED = 3
 
     def __init__(
         self,
-        channel_name,
-        auth,
+        name,
         connection: Connection,
         log: logging.Logger,
     ):
-        self.name = channel_name
-        self.auth = auth
+        self._name = name
         self._connection = connection
         self._log = log
 
         self._event_callbacks = defaultdict(dict)
         self.state = self.State.UNSUBSCRIBED
 
         self.bind("pusher_internal:subscription_succeeded", self._handle_success)
@@ -32,33 +30,34 @@
         self._event_callbacks[event_name][callback] = (args, kwargs)
 
     def unbind(self, event_name, callback):
         del self._event_callbacks[event_name][callback]
 
     async def handle_event(self, event_name, data):
         if event_name not in self._event_callbacks:
-            self._log.warning(f"Unhandled event, channel: {self.name}, event: {event_name}, data: {data}")
+            self._log.warning(f"Unhandled event, channel: {self._name}, event: {event_name}, data: {data}")
             return
 
         for callback, (args, kwargs) in self._event_callbacks[event_name].items():
             try:
                 await callback(data, *args, **kwargs)
             except Exception:
                 self._log.exception(f"Exception in callback: {data}")
 
     async def trigger(self, event):
         if not event["event"].startswith("client-"):
             raise ValueError("Client event has to start with client-")
+
         if not self.is_private() and not self.is_presence():
             raise ValueError("Client event can only be sent on private or presence channels")
 
-        event["channel"] = self.name
+        event["channel"] = self._name
         await self._connection.send_event(event)
 
     def is_private(self):
-        return self.name.startswith("private-")
+        return self._name.startswith("private-")
 
     def is_presence(self):
-        return self.name.startswith("presence-")
+        return self._name.startswith("presence-")
 
     async def _handle_success(self, _):
         self.state = self.State.SUBSCRIBED
```

### Comparing `asyncpusher-0.1.0/asyncpusher/connection.py` & `asyncpusher-0.2.0/asyncpusher/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         # https://pusher.com/docs/channels/library_auth_reference/pusher-websockets-protocol/#recommendations-for-client-libraries
         self._activity_timeout = 120
         self._pong_timeout = 30
         self.state = self.State.IDLE
 
         self.bind("pusher:connection_established", self._handle_connection)
         self.bind("pusher:connection_failed", self._handle_failure)
+        self.bind("pusher:error", self._handle_error)
 
     async def open(self):
         self._loop.create_task(self._run_forever())
 
         while self.state != self.State.CONNECTED:
             await asyncio.sleep(1)
 
@@ -62,15 +63,15 @@
             await self._ws.close()
 
     async def _run_forever(self):
         async with aiohttp.ClientSession() as session:
             while not self._stop:
                 try:
                     await self._connect(session)
-                except BaseException:
+                except aiohttp.ClientError:
                     self._log.exception("Exception while connecting to web socket")
                     self._connection_attempts += 1
         self._log.info("End of forever")
 
     async def _connect(self, session: aiohttp.ClientSession):
         self._log.info("Pusher connecting...")
 
@@ -88,15 +89,15 @@
         while True:
             msg = await ws.receive()
             self._log.debug(f"Websocket message: {msg}")
             if msg.type == aiohttp.WSMsgType.TEXT:
                 event = json.loads(msg.data)
                 await self._handle_event(event)
             else:
-                self._state = self.State.CLOSED
+                self.state = self.State.CLOSED
                 self._log.info(f"Exiting dispatch with message: {msg}")
                 if msg.type == aiohttp.WSMsgType.CLOSE:
                     if isinstance(msg.data, int):
                         code = msg.data
                         # 4000-4099: The connection SHOULD NOT be re-established unchanged.
                         if code >= 4000 and code < 4100:
                             self._stop = True
@@ -119,15 +120,19 @@
 
     async def _handle_event(self, event):
         if "event" not in event:
             self._log.warning(f"Unexpected event: {event}")
             return
 
         event_name = event["event"]
-        event_data = json.loads(event.get("data", "{}"))
+        event_data = event.get("data")
+        try:
+            event_data = json.loads(event_data)
+        except TypeError:
+            pass
 
         if "channel" in event:
             await self._callback(event["channel"], event_name, event_data)
             return
 
         if event_name in self._event_callbacks:
             for callback, (args, kwargs) in self._event_callbacks[event_name].items():
@@ -154,14 +159,17 @@
         self.state = self.State.CONNECTED
         self._log.info(f"Connection established: {data}")
 
     async def _handle_failure(self, data):
         self.state = self.State.FAILED
         self._log.error(f"Connection failed: {data}")
 
+    async def _handle_error(self, data):
+        self._log.error(f"Pusher error: {data}")
+
     def bind(self, event_name, callback, *args, **kwargs):
         self._event_callbacks[event_name][callback] = (args, kwargs)
 
     def unbind(self, event_name, callback):
         del self._event_callbacks[event_name][callback]
 
     def is_connected(self):
```

### Comparing `asyncpusher-0.1.0/asyncpusher/pusher.py` & `asyncpusher-0.2.0/asyncpusher/pusher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 import asyncio
-import hashlib
-import hmac
-import json
 import logging
 
 from asyncpusher.channel import Channel
 from asyncpusher.connection import Connection
 
-VERSION = "0.1.0"
+VERSION = "0.2.0"
 PROTOCOL = 7
 DEFAULT_CLIENT = "asyncpusher"
 
 
 class Pusher:
     def __init__(
         self,
         key: str,
         cluster: str | None = None,
         secure=True,
         custom_host: str | None = None,
         custom_port: int | None = None,
         custom_client: str | None = None,
-        secret: str | None = None,
-        signer=None,
-        user_data=None,
+        channel_authenticator=None,
+        user_authenticator=None,
         auto_sub=False,
         log: logging.Logger | None = None,
         loop: asyncio.AbstractEventLoop | None = None,
         **kwargs,
     ):
         self._key = key
 
-        self._secret = secret
-        self._signer = signer
-        self._user_data = user_data if user_data is not None else {}
+        self._channel_authenticator = channel_authenticator
+        self._user_authenticator = user_authenticator
 
         self._log = log if log is not None else logging.getLogger(__name__)
         self._loop = loop if loop is not None else asyncio.get_running_loop()
 
         self.channels: dict[Channel] = {}
 
         if custom_host is not None and cluster is not None:
@@ -57,36 +52,32 @@
 
     async def _handle_event(self, channel_name, event_name, data):
         if channel_name not in self.channels:
             self._log.warning(f"Unsubscribed event, channel: {channel_name}, event: {event_name}, data: {data}")
             return
         await self.channels[channel_name].handle_event(event_name, data)
 
-    async def subscribe(self, channel_name, auth=None):
+    async def subscribe(self, channel_name):
         if channel_name in self.channels:
             return self.channels[channel_name]
 
-        await self._subscribe(channel_name, auth)
+        channel = Channel(channel_name, self.connection, self._log)
+        await self._subscribe(channel)
 
-        channel = Channel(channel_name, auth, self.connection, self._log)
         self.channels[channel_name] = channel
 
         return channel
 
-    async def _subscribe(self, channel_name, auth=None):
-        data = {"channel": channel_name}
-        if auth is None:
-            if channel_name.startswith("presence-"):
-                data["auth"] = await self._generate_auth_token(channel_name, is_presence=True)
-                data["channel_data"] = json.dumps(self.user_data)
-            elif channel_name.startswith("private-"):
-                data["auth"] = await self._generate_auth_token(channel_name)
-        else:
-            data["auth"] = auth
-
+    async def _subscribe(self, channel: Channel):
+        data = {"channel": channel._name}
+        if channel.is_private() or channel.is_presence():
+            auth = await self._authenticate_channel(channel)
+            data["auth"] = auth["auth"]
+            if channel.is_presence():
+                data["channel_data"] = auth["channel_data"]
         event = {"event": "pusher:subscribe", "data": data}
         await self.connection.send_event(event)
 
     async def unsubscribe(self, channel_name):
         if channel_name in self.channels:
             data = {"channel": channel_name}
             event = {"event": "pusher:unsubscribe", "data": data}
@@ -94,35 +85,25 @@
 
             del self.channels[channel_name]
 
     async def _resubscribe(self, _):
         if len(self.channels) > 0:
             self._log.info("Resubscribing channels...")
             for channel in self.channels.values():
-                await self._subscribe(channel.name, channel.auth)
+                await self._subscribe(channel)
 
-    async def _generate_auth_token(self, channel_name: str, is_presence=False):
-        if self._secret is None and self._signer is None:
-            raise ValueError("One of them has to be provided")
-
-        if self._secret is not None:
-            subject = f"{self.connection.socket_id}:{channel_name}"
-            if is_presence:
-                subject = f"{subject}:{json.dumps(self._user_data)}"
-            hasher = hmac.new(self._as_bytes(self._secret), subject.encode(), hashlib.sha256)
-            auth = f"{self._key}:{hasher.hexdigest()}"
-        else:
-            data = {
-                "socket_id": self.connection.socket_id,
-                "channel_name": channel_name,
-            }
-            if is_presence:
-                data["user_data"] = self._user_data
-            auth = await self._signer(data)
-        return auth
+    async def _authenticate_channel(self, channel: Channel):
+        if self._channel_authenticator is None:
+            raise ValueError("channel_authenticator has to be provided")
+
+        data = {
+            "socket_id": self.connection.socket_id,
+            "channel_name": channel._name,
+        }
+        return await self._channel_authenticator(data)
 
     def _build_url(self, custom_host, custom_client, custom_port, cluster, secure):
         self._protocol = "wss" if secure else "ws"
 
         if custom_host is not None:
             self._host = custom_host
         elif cluster is not None:
```

### Comparing `asyncpusher-0.1.0/.gitignore` & `asyncpusher-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `asyncpusher-0.1.0/LICENSE` & `asyncpusher-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncpusher-0.1.0/README.md` & `asyncpusher-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# asyncpusher
-
 asyncpusher is an asynchronous python client library for [Pusher](https://pusher.com/channels/)
 
 ## Features
 
-- uses well-maintained [aiohttp](https://github.com/aio-libs/aiohttp)'s websocket library
-- auto handles reconnection
-- asynchronous
-- supports Pusher Channels [protocol 7](https://pusher.com/docs/channels/library_auth_reference/pusher-websockets-protocol/)
+- Uses well-maintained [aiohttp](https://github.com/aio-libs/aiohttp)'s websocket library
+- Reliable connection
+- Auto handles reconnection
+- Asynchronous
+- Fast
+- Supports Pusher Channels [protocol 7](https://pusher.com/docs/channels/library_auth_reference/pusher-websockets-protocol/)
+- Support presence and private channels
 
 ## Install
 
 ```
 $ python3 -m pip install asyncpusher
 ```
 
@@ -36,16 +37,16 @@
     loop = asyncio.get_running_loop()
 
     pusher = Pusher("<PUSHER_APP_KEY>", loop=loop)
     pusher.channels[channel_name] = channel
     await pusher.connect()
     channel_name = "<CHANNEL_NAME>"
     channel = await pusher.subscribe(channel_name)
-    channel.bind("diff", handle_event, "usdt_tl")
+    channel.bind("diff", handle_event)
     await asyncio.sleep(5)
     await pusher.unsubscribe(channel_name)
-    await asyncio.sleep(5)
+    await asyncio.sleep(1)
     await pusher.disconnect()
 
 
 asyncio.run(main())
 ```
```

### Comparing `asyncpusher-0.1.0/pyproject.toml` & `asyncpusher-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asyncpusher-0.1.0/PKG-INFO` & `asyncpusher-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpusher
-Version: 0.1.0
+Version: 0.2.0
 Summary: An asynchronous Pusher client library
 Project-URL: Documentation, https://github.com/byildiz/asyncpusher#readme
 Project-URL: Issues, https://github.com/byildiz/asyncpusher/issues
 Project-URL: Source, https://github.com/byildiz/asyncpusher
 Author-email: Burak Yildiz <0byldz@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -18,24 +18,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Requires-Dist: aiohttp>=3.8
 Description-Content-Type: text/markdown
 
-# asyncpusher
-
 asyncpusher is an asynchronous python client library for [Pusher](https://pusher.com/channels/)
 
 ## Features
 
-- uses well-maintained [aiohttp](https://github.com/aio-libs/aiohttp)'s websocket library
-- auto handles reconnection
-- asynchronous
-- supports Pusher Channels [protocol 7](https://pusher.com/docs/channels/library_auth_reference/pusher-websockets-protocol/)
+- Uses well-maintained [aiohttp](https://github.com/aio-libs/aiohttp)'s websocket library
+- Reliable connection
+- Auto handles reconnection
+- Asynchronous
+- Fast
+- Supports Pusher Channels [protocol 7](https://pusher.com/docs/channels/library_auth_reference/pusher-websockets-protocol/)
+- Support presence and private channels
 
 ## Install
 
 ```
 $ python3 -m pip install asyncpusher
 ```
 
@@ -60,16 +61,16 @@
     loop = asyncio.get_running_loop()
 
     pusher = Pusher("<PUSHER_APP_KEY>", loop=loop)
     pusher.channels[channel_name] = channel
     await pusher.connect()
     channel_name = "<CHANNEL_NAME>"
     channel = await pusher.subscribe(channel_name)
-    channel.bind("diff", handle_event, "usdt_tl")
+    channel.bind("diff", handle_event)
     await asyncio.sleep(5)
     await pusher.unsubscribe(channel_name)
-    await asyncio.sleep(5)
+    await asyncio.sleep(1)
     await pusher.disconnect()
 
 
 asyncio.run(main())
 ```
```
