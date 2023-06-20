# Comparing `tmp/litie-0.2.0.tar.gz` & `tmp/litie-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litie-0.2.0.tar", last modified: Tue Jun 20 14:28:59 2023, max compression
+gzip compressed data, was "litie-0.2.1.tar", last modified: Tue Jun 20 16:23:59 2023, max compression
```

## Comparing `litie-0.2.0.tar` & `litie-0.2.1.tar`

### file list

```diff
@@ -1,159 +1,162 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.565978 litie-0.2.0/
--rw-rw-rw-   0        0        0    10854 2023-06-12 13:46:58.000000 litie-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    25797 2023-06-20 14:28:59.564983 litie-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    25488 2023-06-19 14:20:42.000000 litie-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.412553 litie-0.2.0/litie/
--rw-rw-rw-   0        0        0       23 2023-06-13 13:33:13.000000 litie-0.2.0/litie/__about__.py
--rw-rw-rw-   0        0        0        0 2023-06-13 13:33:13.000000 litie-0.2.0/litie/__init__.py
--rw-rw-rw-   0        0        0     8729 2023-06-15 12:21:27.000000 litie-0.2.0/litie/arguments.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.420531 litie-0.2.0/litie/callbacks/
--rw-rw-rw-   0        0        0       82 2023-06-15 12:21:27.000000 litie-0.2.0/litie/callbacks/__init__.py
--rw-rw-rw-   0        0        0     2926 2023-06-15 12:21:27.000000 litie-0.2.0/litie/callbacks/adversarial.py
--rw-rw-rw-   0        0        0     1085 2023-06-15 11:34:55.000000 litie-0.2.0/litie/callbacks/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.424520 litie-0.2.0/litie/datasets/
--rw-rw-rw-   0        0        0      149 2023-06-16 14:35:08.000000 litie-0.2.0/litie/datasets/__init__.py
--rw-rw-rw-   0        0        0     8016 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/base.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.428511 litie-0.2.0/litie/datasets/ee/
--rw-rw-rw-   0        0        0      271 2023-06-16 11:00:22.000000 litie-0.2.0/litie/datasets/ee/__init__.py
--rw-rw-rw-   0        0        0     8441 2023-06-19 11:11:12.000000 litie-0.2.0/litie/datasets/ee/base.py
--rw-rw-rw-   0        0        0     3057 2023-06-18 05:00:47.000000 litie-0.2.0/litie/datasets/ee/gplinker.py
--rw-rw-rw-   0        0        0      566 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/iterable.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.439480 litie-0.2.0/litie/datasets/ner/
--rw-rw-rw-   0        0        0     1400 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/__init__.py
--rw-rw-rw-   0        0        0     7503 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/base.py
--rw-rw-rw-   0        0        0     4975 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/cnn.py
--rw-rw-rw-   0        0        0     4637 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/crf.py
--rw-rw-rw-   0        0        0     2913 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/global_pointer.py
--rw-rw-rw-   0        0        0     3189 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/lear.py
--rw-rw-rw-   0        0        0     6845 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/mrc.py
--rw-rw-rw-   0        0        0     1998 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/span.py
--rw-rw-rw-   0        0        0     2165 2023-06-13 13:33:13.000000 litie-0.2.0/litie/datasets/ner/tplinker.py
--rw-rw-rw-   0        0        0     9539 2023-06-20 11:50:41.000000 litie-0.2.0/litie/datasets/ner/w2ner.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.453442 litie-0.2.0/litie/datasets/re/
--rw-rw-rw-   0        0        0     1206 2023-06-15 14:25:21.000000 litie-0.2.0/litie/datasets/re/__init__.py
--rw-rw-rw-   0        0        0     8646 2023-06-13 13:33:14.000000 litie-0.2.0/litie/datasets/re/base.py
--rw-rw-rw-   0        0        0     2976 2023-06-13 13:33:14.000000 litie-0.2.0/litie/datasets/re/casrel.py
--rw-rw-rw-   0        0        0     2661 2023-06-13 13:33:14.000000 litie-0.2.0/litie/datasets/re/gplinker.py
--rw-rw-rw-   0        0        0     3215 2023-06-13 13:33:14.000000 litie-0.2.0/litie/datasets/re/grte.py
--rw-rw-rw-   0        0        0     2240 2023-06-15 14:24:51.000000 litie-0.2.0/litie/datasets/re/onerel.py
--rw-rw-rw-   0        0        0     2482 2023-06-13 13:33:14.000000 litie-0.2.0/litie/datasets/re/pfn.py
--rw-rw-rw-   0        0        0     4476 2023-06-20 14:27:43.000000 litie-0.2.0/litie/datasets/re/prgc.py
--rw-rw-rw-   0        0        0     2332 2023-06-13 13:33:14.000000 litie-0.2.0/litie/datasets/re/spn.py
--rw-rw-rw-   0        0        0     2690 2023-06-13 13:33:14.000000 litie-0.2.0/litie/datasets/re/tplinker.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.456434 litie-0.2.0/litie/datasets/tc/
--rw-rw-rw-   0        0        0        0 2023-06-20 11:54:53.000000 litie-0.2.0/litie/datasets/tc/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-20 11:55:22.000000 litie-0.2.0/litie/datasets/tc/base.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.460423 litie-0.2.0/litie/datasets/uie/
--rw-rw-rw-   0        0        0       92 2023-06-13 16:27:09.000000 litie-0.2.0/litie/datasets/uie/__init__.py
--rw-rw-rw-   0        0        0     3281 2023-06-13 16:26:56.000000 litie-0.2.0/litie/datasets/uie/data.py
--rw-rw-rw-   0        0        0     7871 2023-06-13 16:21:18.000000 litie-0.2.0/litie/datasets/uie/doccano.py
--rw-rw-rw-   0        0        0    21781 2023-06-13 16:23:51.000000 litie-0.2.0/litie/datasets/uie/utils.py
--rw-rw-rw-   0        0        0     7580 2023-06-18 16:02:48.000000 litie-0.2.0/litie/datasets/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.468405 litie-0.2.0/litie/engines/
--rw-rw-rw-   0        0        0      151 2023-06-16 14:33:25.000000 litie-0.2.0/litie/engines/__init__.py
--rw-rw-rw-   0        0        0    14877 2023-06-17 12:04:10.000000 litie-0.2.0/litie/engines/base.py
--rw-rw-rw-   0        0        0     4351 2023-06-16 14:32:54.000000 litie-0.2.0/litie/engines/ee.py
--rw-rw-rw-   0        0        0     4084 2023-06-15 12:21:27.000000 litie-0.2.0/litie/engines/ner.py
--rw-rw-rw-   0        0        0     4108 2023-06-15 12:21:27.000000 litie-0.2.0/litie/engines/re.py
--rw-rw-rw-   0        0        0     1837 2023-06-15 12:21:27.000000 litie-0.2.0/litie/engines/uie.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.484360 litie-0.2.0/litie/layers/
--rw-rw-rw-   0        0        0      771 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/__init__.py
--rw-rw-rw-   0        0        0     2930 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/conv.py
--rw-rw-rw-   0        0        0    20163 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/crf.py
--rw-rw-rw-   0        0        0     1719 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/dropouts.py
--rw-rw-rw-   0        0        0    13250 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/global_pointer.py
--rw-rw-rw-   0        0        0     3605 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/layer_norm.py
--rw-rw-rw-   0        0        0     2462 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/lear.py
--rw-rw-rw-   0        0        0     6918 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/pfn.py
--rw-rw-rw-   0        0        0     6790 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/pooling.py
--rw-rw-rw-   0        0        0     7142 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/position.py
--rw-rw-rw-   0        0        0     4364 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/set_decoder.py
--rw-rw-rw-   0        0        0     3209 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/transformer.py
--rw-rw-rw-   0        0        0      146 2023-06-13 13:33:14.000000 litie-0.2.0/litie/layers/utils.py
--rw-rw-rw-   0        0        0    23626 2023-06-13 14:50:53.000000 litie-0.2.0/litie/losses.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.486356 litie-0.2.0/litie/metrics/
--rw-rw-rw-   0        0        0       95 2023-06-16 14:28:24.000000 litie-0.2.0/litie/metrics/__init__.py
--rw-rw-rw-   0        0        0      319 2023-06-13 13:33:14.000000 litie-0.2.0/litie/metrics/base.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.492342 litie-0.2.0/litie/metrics/extraction/
--rw-rw-rw-   0        0        0       33 2023-06-13 13:33:14.000000 litie-0.2.0/litie/metrics/extraction/__init__.py
--rw-rw-rw-   0        0        0     2138 2023-06-18 04:21:44.000000 litie-0.2.0/litie/metrics/extraction/precision_recall_fscore.py
--rw-rw-rw-   0        0        0     1865 2023-06-16 13:04:36.000000 litie-0.2.0/litie/metrics/extraction/score.py
--rw-rw-rw-   0        0        0     6352 2023-06-13 13:33:14.000000 litie-0.2.0/litie/metrics/extraction/span.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.501316 litie-0.2.0/litie/models/
--rw-rw-rw-   0        0        0      151 2023-06-16 14:38:13.000000 litie-0.2.0/litie/models/__init__.py
--rw-rw-rw-   0        0        0     4580 2023-06-18 11:38:24.000000 litie-0.2.0/litie/models/base.py
--rw-rw-rw-   0        0        0     2224 2023-06-17 05:41:59.000000 litie-0.2.0/litie/models/ee.py
--rw-rw-rw-   0        0        0     2172 2023-06-15 12:21:27.000000 litie-0.2.0/litie/models/ner.py
--rw-rw-rw-   0        0        0     2178 2023-06-15 12:21:27.000000 litie-0.2.0/litie/models/re.py
--rw-rw-rw-   0        0        0     1868 2023-06-13 16:45:34.000000 litie-0.2.0/litie/models/uie.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.507298 litie-0.2.0/litie/nn/
--rw-rw-rw-   0        0        0      224 2023-06-15 15:46:07.000000 litie-0.2.0/litie/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.512285 litie-0.2.0/litie/nn/chinese_bert/
--rw-rw-rw-   0        0        0      342 2023-06-13 13:33:14.000000 litie-0.2.0/litie/nn/chinese_bert/__init__.py
--rw-rw-rw-   0        0        0     5399 2023-06-13 13:33:14.000000 litie-0.2.0/litie/nn/chinese_bert/configuration_chinese_bert.py
--rw-rw-rw-   0        0        0    29685 2023-06-13 13:33:14.000000 litie-0.2.0/litie/nn/chinese_bert/modeling_chinese_bert.py
--rw-rw-rw-   0        0        0     1710 2023-06-13 13:33:14.000000 litie-0.2.0/litie/nn/chinese_bert/tokenization_chinesebert_fast.py
--rw-rw-rw-   0        0        0     3155 2023-06-13 13:33:14.000000 litie-0.2.0/litie/nn/decode_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.515279 litie-0.2.0/litie/nn/ee/
--rw-rw-rw-   0        0        0      729 2023-06-15 15:46:07.000000 litie-0.2.0/litie/nn/ee/__init__.py
--rw-rw-rw-   0        0        0     8891 2023-06-19 11:11:12.000000 litie-0.2.0/litie/nn/ee/gplinker.py
--rw-rw-rw-   0        0        0     4328 2023-06-20 11:25:12.000000 litie-0.2.0/litie/nn/model_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.525087 litie-0.2.0/litie/nn/ner/
--rw-rw-rw-   0        0        0     2703 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/ner/__init__.py
--rw-rw-rw-   0        0        0    12856 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/ner/cnn.py
--rw-rw-rw-   0        0        0    15930 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/ner/crf.py
--rw-rw-rw-   0        0        0     7318 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/ner/global_pointer.py
--rw-rw-rw-   0        0        0     9715 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/ner/lear.py
--rw-rw-rw-   0        0        0     7262 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/ner/mrc.py
--rw-rw-rw-   0        0        0     5643 2023-06-20 11:25:12.000000 litie-0.2.0/litie/nn/ner/span.py
--rw-rw-rw-   0        0        0     6612 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/ner/tplinker.py
--rw-rw-rw-   0        0        0    11773 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/ner/w2ner.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.536058 litie-0.2.0/litie/nn/re/
--rw-rw-rw-   0        0        0     2161 2023-06-15 13:57:04.000000 litie-0.2.0/litie/nn/re/__init__.py
--rw-rw-rw-   0        0        0    11034 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/re/casrel.py
--rw-rw-rw-   0        0        0     7837 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/re/gplinker.py
--rw-rw-rw-   0        0        0     9001 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/re/grte.py
--rw-rw-rw-   0        0        0     6994 2023-06-15 13:54:49.000000 litie-0.2.0/litie/nn/re/onerel.py
--rw-rw-rw-   0        0        0     7342 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/re/pfn.py
--rw-rw-rw-   0        0        0    14301 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/re/prgc.py
--rw-rw-rw-   0        0        0     9936 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/re/spn.py
--rw-rw-rw-   0        0        0     9637 2023-06-15 12:21:27.000000 litie-0.2.0/litie/nn/re/tplinker.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.539050 litie-0.2.0/litie/nn/roformer/
--rw-rw-rw-   0        0        0      434 2023-06-13 13:33:14.000000 litie-0.2.0/litie/nn/roformer/__init__.py
--rw-rw-rw-   0        0        0     8143 2023-06-13 13:33:14.000000 litie-0.2.0/litie/nn/roformer/configuration_roformer.py
--rw-rw-rw-   0        0        0    79700 2023-06-13 13:33:14.000000 litie-0.2.0/litie/nn/roformer/modeling_roformer.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.544036 litie-0.2.0/litie/nn/uie/
--rw-rw-rw-   0        0        0       74 2023-06-13 16:31:51.000000 litie-0.2.0/litie/nn/uie/__init__.py
--rw-rw-rw-   0        0        0    15989 2023-06-13 16:31:51.000000 litie-0.2.0/litie/nn/uie/convert.py
--rw-rw-rw-   0        0        0     7217 2023-06-20 11:25:12.000000 litie-0.2.0/litie/nn/uie/model.py
--rw-rw-rw-   0        0        0     6167 2023-06-20 11:25:12.000000 litie-0.2.0/litie/nn/uie/siamese_uie.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.551017 litie-0.2.0/litie/pipelines/
--rw-rw-rw-   0        0        0      145 2023-06-16 14:29:12.000000 litie-0.2.0/litie/pipelines/__init__.py
--rw-rw-rw-   0        0        0     3234 2023-06-13 13:33:14.000000 litie-0.2.0/litie/pipelines/base.py
--rw-rw-rw-   0        0        0     5163 2023-06-18 15:44:54.000000 litie-0.2.0/litie/pipelines/ee.py
--rw-rw-rw-   0        0        0    16323 2023-06-13 13:33:14.000000 litie-0.2.0/litie/pipelines/ner.py
--rw-rw-rw-   0        0        0     6362 2023-06-19 11:11:12.000000 litie-0.2.0/litie/pipelines/re.py
--rw-rw-rw-   0        0        0    19411 2023-06-14 14:13:28.000000 litie-0.2.0/litie/pipelines/uie.py
--rw-rw-rw-   0        0        0     2862 2023-06-13 13:33:14.000000 litie-0.2.0/litie/pipelines/utils.py
--rw-rw-rw-   0        0        0      659 2023-06-13 13:33:14.000000 litie-0.2.0/litie/registry.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.557999 litie-0.2.0/litie/ui/
--rw-rw-rw-   0        0        0      121 2023-06-19 13:47:15.000000 litie-0.2.0/litie/ui/__init__.py
--rw-rw-rw-   0        0        0     2458 2023-06-19 14:41:32.000000 litie-0.2.0/litie/ui/ee.py
--rw-rw-rw-   0        0        0     3334 2023-06-14 14:13:28.000000 litie-0.2.0/litie/ui/ner.py
--rw-rw-rw-   0        0        0     3246 2023-06-13 13:33:14.000000 litie-0.2.0/litie/ui/re.py
--rw-rw-rw-   0        0        0     1294 2023-06-13 13:33:14.000000 litie-0.2.0/litie/ui/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.563984 litie-0.2.0/litie/utils/
--rw-rw-rw-   0        0        0        0 2023-06-13 13:33:14.000000 litie-0.2.0/litie/utils/__init__.py
--rw-rw-rw-   0        0        0     4654 2023-06-13 13:33:14.000000 litie-0.2.0/litie/utils/common.py
--rw-rw-rw-   0        0        0      609 2023-06-13 13:33:14.000000 litie-0.2.0/litie/utils/deepspeed.py
--rw-rw-rw-   0        0        0     7558 2023-06-13 13:33:14.000000 litie-0.2.0/litie/utils/download.py
--rw-rw-rw-   0        0        0      476 2023-06-13 13:33:14.000000 litie-0.2.0/litie/utils/imports.py
--rw-rw-rw-   0        0        0     3899 2023-06-13 13:33:14.000000 litie-0.2.0/litie/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:28:59.417538 litie-0.2.0/litie.egg-info/
--rw-rw-rw-   0        0        0    25797 2023-06-20 14:28:59.000000 litie-0.2.0/litie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2023-06-20 14:28:59.000000 litie-0.2.0/litie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:28:59.000000 litie-0.2.0/litie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      151 2023-06-20 14:28:59.000000 litie-0.2.0/litie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 14:28:59.000000 litie-0.2.0/litie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 14:28:59.565978 litie-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-06-20 14:28:10.000000 litie-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.818001 litie-0.2.1/
+-rw-rw-rw-   0        0        0    10854 2023-06-12 13:46:58.000000 litie-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    25797 2023-06-20 16:23:59.817005 litie-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    25488 2023-06-19 14:20:42.000000 litie-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.641471 litie-0.2.1/litie/
+-rw-rw-rw-   0        0        0       23 2023-06-13 13:33:13.000000 litie-0.2.1/litie/__about__.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:33:13.000000 litie-0.2.1/litie/__init__.py
+-rw-rw-rw-   0        0        0     8729 2023-06-15 12:21:27.000000 litie-0.2.1/litie/arguments.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.652442 litie-0.2.1/litie/callbacks/
+-rw-rw-rw-   0        0        0       82 2023-06-15 12:21:27.000000 litie-0.2.1/litie/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     2926 2023-06-15 12:21:27.000000 litie-0.2.1/litie/callbacks/adversarial.py
+-rw-rw-rw-   0        0        0     1085 2023-06-15 11:34:55.000000 litie-0.2.1/litie/callbacks/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.657429 litie-0.2.1/litie/datasets/
+-rw-rw-rw-   0        0        0      199 2023-06-20 15:59:01.000000 litie-0.2.1/litie/datasets/__init__.py
+-rw-rw-rw-   0        0        0     8016 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/base.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.660422 litie-0.2.1/litie/datasets/ee/
+-rw-rw-rw-   0        0        0      271 2023-06-16 11:00:22.000000 litie-0.2.1/litie/datasets/ee/__init__.py
+-rw-rw-rw-   0        0        0     8441 2023-06-19 11:11:12.000000 litie-0.2.1/litie/datasets/ee/base.py
+-rw-rw-rw-   0        0        0     3057 2023-06-18 05:00:47.000000 litie-0.2.1/litie/datasets/ee/gplinker.py
+-rw-rw-rw-   0        0        0      566 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/iterable.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.673386 litie-0.2.1/litie/datasets/ner/
+-rw-rw-rw-   0        0        0     1400 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/__init__.py
+-rw-rw-rw-   0        0        0     7503 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/base.py
+-rw-rw-rw-   0        0        0     4975 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/cnn.py
+-rw-rw-rw-   0        0        0     4637 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/crf.py
+-rw-rw-rw-   0        0        0     2913 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/global_pointer.py
+-rw-rw-rw-   0        0        0     3189 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/lear.py
+-rw-rw-rw-   0        0        0     6845 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/mrc.py
+-rw-rw-rw-   0        0        0     1998 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/span.py
+-rw-rw-rw-   0        0        0     2165 2023-06-13 13:33:13.000000 litie-0.2.1/litie/datasets/ner/tplinker.py
+-rw-rw-rw-   0        0        0     9539 2023-06-20 11:50:41.000000 litie-0.2.1/litie/datasets/ner/w2ner.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.689352 litie-0.2.1/litie/datasets/re/
+-rw-rw-rw-   0        0        0     1206 2023-06-15 14:25:21.000000 litie-0.2.1/litie/datasets/re/__init__.py
+-rw-rw-rw-   0        0        0     8646 2023-06-13 13:33:14.000000 litie-0.2.1/litie/datasets/re/base.py
+-rw-rw-rw-   0        0        0     2976 2023-06-13 13:33:14.000000 litie-0.2.1/litie/datasets/re/casrel.py
+-rw-rw-rw-   0        0        0     2661 2023-06-13 13:33:14.000000 litie-0.2.1/litie/datasets/re/gplinker.py
+-rw-rw-rw-   0        0        0     3215 2023-06-13 13:33:14.000000 litie-0.2.1/litie/datasets/re/grte.py
+-rw-rw-rw-   0        0        0     2240 2023-06-15 14:24:51.000000 litie-0.2.1/litie/datasets/re/onerel.py
+-rw-rw-rw-   0        0        0     2482 2023-06-13 13:33:14.000000 litie-0.2.1/litie/datasets/re/pfn.py
+-rw-rw-rw-   0        0        0     4476 2023-06-20 14:27:43.000000 litie-0.2.1/litie/datasets/re/prgc.py
+-rw-rw-rw-   0        0        0     2332 2023-06-13 13:33:14.000000 litie-0.2.1/litie/datasets/re/spn.py
+-rw-rw-rw-   0        0        0     2690 2023-06-13 13:33:14.000000 litie-0.2.1/litie/datasets/re/tplinker.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.693333 litie-0.2.1/litie/datasets/tc/
+-rw-rw-rw-   0        0        0      252 2023-06-20 15:58:36.000000 litie-0.2.1/litie/datasets/tc/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-06-20 15:51:20.000000 litie-0.2.1/litie/datasets/tc/base.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.702309 litie-0.2.1/litie/datasets/uie/
+-rw-rw-rw-   0        0        0       92 2023-06-13 16:27:09.000000 litie-0.2.1/litie/datasets/uie/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-13 16:26:56.000000 litie-0.2.1/litie/datasets/uie/data.py
+-rw-rw-rw-   0        0        0     7871 2023-06-13 16:21:18.000000 litie-0.2.1/litie/datasets/uie/doccano.py
+-rw-rw-rw-   0        0        0    21781 2023-06-13 16:23:51.000000 litie-0.2.1/litie/datasets/uie/utils.py
+-rw-rw-rw-   0        0        0     7580 2023-06-18 16:02:48.000000 litie-0.2.1/litie/datasets/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.710290 litie-0.2.1/litie/engines/
+-rw-rw-rw-   0        0        0      151 2023-06-16 14:33:25.000000 litie-0.2.1/litie/engines/__init__.py
+-rw-rw-rw-   0        0        0    14877 2023-06-17 12:04:10.000000 litie-0.2.1/litie/engines/base.py
+-rw-rw-rw-   0        0        0     4351 2023-06-16 14:32:54.000000 litie-0.2.1/litie/engines/ee.py
+-rw-rw-rw-   0        0        0     4084 2023-06-15 12:21:27.000000 litie-0.2.1/litie/engines/ner.py
+-rw-rw-rw-   0        0        0     4108 2023-06-15 12:21:27.000000 litie-0.2.1/litie/engines/re.py
+-rw-rw-rw-   0        0        0     1837 2023-06-15 12:21:27.000000 litie-0.2.1/litie/engines/uie.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.725247 litie-0.2.1/litie/layers/
+-rw-rw-rw-   0        0        0      771 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/__init__.py
+-rw-rw-rw-   0        0        0     2930 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/conv.py
+-rw-rw-rw-   0        0        0    20163 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/crf.py
+-rw-rw-rw-   0        0        0     1719 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/dropouts.py
+-rw-rw-rw-   0        0        0    15185 2023-06-20 16:20:33.000000 litie-0.2.1/litie/layers/global_pointer.py
+-rw-rw-rw-   0        0        0     3605 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/layer_norm.py
+-rw-rw-rw-   0        0        0     2462 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/lear.py
+-rw-rw-rw-   0        0        0     6918 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/pfn.py
+-rw-rw-rw-   0        0        0     6790 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/pooling.py
+-rw-rw-rw-   0        0        0     7142 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/position.py
+-rw-rw-rw-   0        0        0     4364 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/set_decoder.py
+-rw-rw-rw-   0        0        0     3209 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/transformer.py
+-rw-rw-rw-   0        0        0      146 2023-06-13 13:33:14.000000 litie-0.2.1/litie/layers/utils.py
+-rw-rw-rw-   0        0        0    23626 2023-06-13 14:50:53.000000 litie-0.2.1/litie/losses.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.727243 litie-0.2.1/litie/metrics/
+-rw-rw-rw-   0        0        0       95 2023-06-16 14:28:24.000000 litie-0.2.1/litie/metrics/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-06-13 13:33:14.000000 litie-0.2.1/litie/metrics/base.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.732229 litie-0.2.1/litie/metrics/extraction/
+-rw-rw-rw-   0        0        0       33 2023-06-13 13:33:14.000000 litie-0.2.1/litie/metrics/extraction/__init__.py
+-rw-rw-rw-   0        0        0     2138 2023-06-18 04:21:44.000000 litie-0.2.1/litie/metrics/extraction/precision_recall_fscore.py
+-rw-rw-rw-   0        0        0     1865 2023-06-16 13:04:36.000000 litie-0.2.1/litie/metrics/extraction/score.py
+-rw-rw-rw-   0        0        0     6352 2023-06-13 13:33:14.000000 litie-0.2.1/litie/metrics/extraction/span.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.739211 litie-0.2.1/litie/models/
+-rw-rw-rw-   0        0        0      151 2023-06-16 14:38:13.000000 litie-0.2.1/litie/models/__init__.py
+-rw-rw-rw-   0        0        0     4580 2023-06-18 11:38:24.000000 litie-0.2.1/litie/models/base.py
+-rw-rw-rw-   0        0        0     2224 2023-06-17 05:41:59.000000 litie-0.2.1/litie/models/ee.py
+-rw-rw-rw-   0        0        0     2172 2023-06-15 12:21:27.000000 litie-0.2.1/litie/models/ner.py
+-rw-rw-rw-   0        0        0     2178 2023-06-15 12:21:27.000000 litie-0.2.1/litie/models/re.py
+-rw-rw-rw-   0        0        0     1868 2023-06-13 16:45:34.000000 litie-0.2.1/litie/models/uie.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.743199 litie-0.2.1/litie/nn/
+-rw-rw-rw-   0        0        0      224 2023-06-15 15:46:07.000000 litie-0.2.1/litie/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.748187 litie-0.2.1/litie/nn/chinese_bert/
+-rw-rw-rw-   0        0        0      342 2023-06-13 13:33:14.000000 litie-0.2.1/litie/nn/chinese_bert/__init__.py
+-rw-rw-rw-   0        0        0     5399 2023-06-13 13:33:14.000000 litie-0.2.1/litie/nn/chinese_bert/configuration_chinese_bert.py
+-rw-rw-rw-   0        0        0    29685 2023-06-13 13:33:14.000000 litie-0.2.1/litie/nn/chinese_bert/modeling_chinese_bert.py
+-rw-rw-rw-   0        0        0     1710 2023-06-13 13:33:14.000000 litie-0.2.1/litie/nn/chinese_bert/tokenization_chinesebert_fast.py
+-rw-rw-rw-   0        0        0     3155 2023-06-13 13:33:14.000000 litie-0.2.1/litie/nn/decode_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.750185 litie-0.2.1/litie/nn/ee/
+-rw-rw-rw-   0        0        0      729 2023-06-15 15:46:07.000000 litie-0.2.1/litie/nn/ee/__init__.py
+-rw-rw-rw-   0        0        0     8891 2023-06-19 11:11:12.000000 litie-0.2.1/litie/nn/ee/gplinker.py
+-rw-rw-rw-   0        0        0     4328 2023-06-20 11:25:12.000000 litie-0.2.1/litie/nn/model_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.761151 litie-0.2.1/litie/nn/ner/
+-rw-rw-rw-   0        0        0     2703 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/ner/__init__.py
+-rw-rw-rw-   0        0        0    12856 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/ner/cnn.py
+-rw-rw-rw-   0        0        0    15930 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/ner/crf.py
+-rw-rw-rw-   0        0        0     7318 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/ner/global_pointer.py
+-rw-rw-rw-   0        0        0     9715 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/ner/lear.py
+-rw-rw-rw-   0        0        0     7262 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/ner/mrc.py
+-rw-rw-rw-   0        0        0     5643 2023-06-20 11:25:12.000000 litie-0.2.1/litie/nn/ner/span.py
+-rw-rw-rw-   0        0        0     6617 2023-06-20 16:21:22.000000 litie-0.2.1/litie/nn/ner/tplinker.py
+-rw-rw-rw-   0        0        0    11773 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/ner/w2ner.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.771136 litie-0.2.1/litie/nn/re/
+-rw-rw-rw-   0        0        0     2161 2023-06-15 13:57:04.000000 litie-0.2.1/litie/nn/re/__init__.py
+-rw-rw-rw-   0        0        0    11034 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/re/casrel.py
+-rw-rw-rw-   0        0        0     7837 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/re/gplinker.py
+-rw-rw-rw-   0        0        0     9001 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/re/grte.py
+-rw-rw-rw-   0        0        0     6994 2023-06-15 13:54:49.000000 litie-0.2.1/litie/nn/re/onerel.py
+-rw-rw-rw-   0        0        0     7342 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/re/pfn.py
+-rw-rw-rw-   0        0        0    14301 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/re/prgc.py
+-rw-rw-rw-   0        0        0     9936 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/re/spn.py
+-rw-rw-rw-   0        0        0     9637 2023-06-15 12:21:27.000000 litie-0.2.1/litie/nn/re/tplinker.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.776114 litie-0.2.1/litie/nn/roformer/
+-rw-rw-rw-   0        0        0      434 2023-06-13 13:33:14.000000 litie-0.2.1/litie/nn/roformer/__init__.py
+-rw-rw-rw-   0        0        0     8143 2023-06-13 13:33:14.000000 litie-0.2.1/litie/nn/roformer/configuration_roformer.py
+-rw-rw-rw-   0        0        0    79700 2023-06-13 13:33:14.000000 litie-0.2.1/litie/nn/roformer/modeling_roformer.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.778108 litie-0.2.1/litie/nn/tc/
+-rw-rw-rw-   0        0        0        0 2023-06-20 15:59:28.000000 litie-0.2.1/litie/nn/tc/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 16:02:49.000000 litie-0.2.1/litie/nn/tc/fc.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.782096 litie-0.2.1/litie/nn/uie/
+-rw-rw-rw-   0        0        0       74 2023-06-13 16:31:51.000000 litie-0.2.1/litie/nn/uie/__init__.py
+-rw-rw-rw-   0        0        0    15989 2023-06-13 16:31:51.000000 litie-0.2.1/litie/nn/uie/convert.py
+-rw-rw-rw-   0        0        0     7217 2023-06-20 11:25:12.000000 litie-0.2.1/litie/nn/uie/model.py
+-rw-rw-rw-   0        0        0     6167 2023-06-20 11:25:12.000000 litie-0.2.1/litie/nn/uie/siamese_uie.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.794065 litie-0.2.1/litie/pipelines/
+-rw-rw-rw-   0        0        0      145 2023-06-16 14:29:12.000000 litie-0.2.1/litie/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     3234 2023-06-13 13:33:14.000000 litie-0.2.1/litie/pipelines/base.py
+-rw-rw-rw-   0        0        0     5163 2023-06-18 15:44:54.000000 litie-0.2.1/litie/pipelines/ee.py
+-rw-rw-rw-   0        0        0    16323 2023-06-13 13:33:14.000000 litie-0.2.1/litie/pipelines/ner.py
+-rw-rw-rw-   0        0        0     6362 2023-06-19 11:11:12.000000 litie-0.2.1/litie/pipelines/re.py
+-rw-rw-rw-   0        0        0    19411 2023-06-14 14:13:28.000000 litie-0.2.1/litie/pipelines/uie.py
+-rw-rw-rw-   0        0        0     2862 2023-06-13 13:33:14.000000 litie-0.2.1/litie/pipelines/utils.py
+-rw-rw-rw-   0        0        0      659 2023-06-13 13:33:14.000000 litie-0.2.1/litie/registry.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.801050 litie-0.2.1/litie/ui/
+-rw-rw-rw-   0        0        0      121 2023-06-19 13:47:15.000000 litie-0.2.1/litie/ui/__init__.py
+-rw-rw-rw-   0        0        0     2458 2023-06-19 14:41:32.000000 litie-0.2.1/litie/ui/ee.py
+-rw-rw-rw-   0        0        0     3334 2023-06-14 14:13:28.000000 litie-0.2.1/litie/ui/ner.py
+-rw-rw-rw-   0        0        0     3246 2023-06-13 13:33:14.000000 litie-0.2.1/litie/ui/re.py
+-rw-rw-rw-   0        0        0     1294 2023-06-13 13:33:14.000000 litie-0.2.1/litie/ui/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.813017 litie-0.2.1/litie/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:33:14.000000 litie-0.2.1/litie/utils/__init__.py
+-rw-rw-rw-   0        0        0     4654 2023-06-13 13:33:14.000000 litie-0.2.1/litie/utils/common.py
+-rw-rw-rw-   0        0        0      609 2023-06-13 13:33:14.000000 litie-0.2.1/litie/utils/deepspeed.py
+-rw-rw-rw-   0        0        0     7558 2023-06-13 13:33:14.000000 litie-0.2.1/litie/utils/download.py
+-rw-rw-rw-   0        0        0      476 2023-06-13 13:33:14.000000 litie-0.2.1/litie/utils/imports.py
+-rw-rw-rw-   0        0        0     3899 2023-06-13 13:33:14.000000 litie-0.2.1/litie/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:23:59.648454 litie-0.2.1/litie.egg-info/
+-rw-rw-rw-   0        0        0    25797 2023-06-20 16:23:59.000000 litie-0.2.1/litie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3390 2023-06-20 16:23:59.000000 litie-0.2.1/litie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:23:59.000000 litie-0.2.1/litie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      151 2023-06-20 16:23:59.000000 litie-0.2.1/litie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 16:23:59.000000 litie-0.2.1/litie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 16:23:59.818001 litie-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-06-20 16:23:14.000000 litie-0.2.1/setup.py
```

### Comparing `litie-0.2.0/LICENSE` & `litie-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/PKG-INFO` & `litie-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litie
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pytorch-lightning Code Blocks for Information Extraction
 Home-page: https://github.com/xusenlinzy/lit-ie
 Author: xusenlin
 Author-email: 1659821119@qq.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: litie Version: 0.2.0 Summary: Pytorch-lightning
+Metadata-Version: 2.1 Name: litie Version: 0.2.1 Summary: Pytorch-lightning
 Code Blocks for Information Extraction Home-page: https://github.com/
 xusenlinzy/lit-ie Author: xusenlin Author-email: 1659821119@qq.com Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE #
 Lit-IE
      [https://img.shields.io/github/license/xusenlinzy/lit-ner] [https://
    img.shields.io/badge/python-3.8+-aff.svg] [https://img.shields.io/badge/
 pytorch-%3E=1.12-red?logo=pytorch] [https://img.shields.io/github/last-commit/
```

### Comparing `litie-0.2.0/README.md` & `litie-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/arguments.py` & `litie-0.2.1/litie/arguments.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/callbacks/adversarial.py` & `litie-0.2.1/litie/callbacks/adversarial.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/callbacks/logger.py` & `litie-0.2.1/litie/callbacks/logger.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/base.py` & `litie-0.2.1/litie/datasets/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ee/base.py` & `litie-0.2.1/litie/datasets/ee/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ee/gplinker.py` & `litie-0.2.1/litie/datasets/ee/gplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/iterable.py` & `litie-0.2.1/litie/datasets/iterable.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/__init__.py` & `litie-0.2.1/litie/datasets/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/base.py` & `litie-0.2.1/litie/datasets/ner/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/cnn.py` & `litie-0.2.1/litie/datasets/ner/cnn.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/crf.py` & `litie-0.2.1/litie/datasets/ner/crf.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/global_pointer.py` & `litie-0.2.1/litie/datasets/ner/global_pointer.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/lear.py` & `litie-0.2.1/litie/datasets/ner/lear.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/mrc.py` & `litie-0.2.1/litie/datasets/ner/mrc.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/span.py` & `litie-0.2.1/litie/datasets/ner/span.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/tplinker.py` & `litie-0.2.1/litie/datasets/ner/tplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/ner/w2ner.py` & `litie-0.2.1/litie/datasets/ner/w2ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/__init__.py` & `litie-0.2.1/litie/datasets/re/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/base.py` & `litie-0.2.1/litie/datasets/re/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/casrel.py` & `litie-0.2.1/litie/datasets/re/casrel.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/gplinker.py` & `litie-0.2.1/litie/datasets/re/gplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/grte.py` & `litie-0.2.1/litie/datasets/re/grte.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/onerel.py` & `litie-0.2.1/litie/datasets/re/onerel.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/pfn.py` & `litie-0.2.1/litie/datasets/re/pfn.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/prgc.py` & `litie-0.2.1/litie/datasets/re/prgc.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/spn.py` & `litie-0.2.1/litie/datasets/re/spn.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/re/tplinker.py` & `litie-0.2.1/litie/datasets/re/tplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/uie/data.py` & `litie-0.2.1/litie/datasets/uie/data.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/uie/doccano.py` & `litie-0.2.1/litie/datasets/uie/doccano.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/uie/utils.py` & `litie-0.2.1/litie/datasets/uie/utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/datasets/utils.py` & `litie-0.2.1/litie/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/engines/base.py` & `litie-0.2.1/litie/engines/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/engines/ee.py` & `litie-0.2.1/litie/engines/ee.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/engines/ner.py` & `litie-0.2.1/litie/engines/ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/engines/re.py` & `litie-0.2.1/litie/engines/re.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/engines/uie.py` & `litie-0.2.1/litie/engines/uie.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/__init__.py` & `litie-0.2.1/litie/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/conv.py` & `litie-0.2.1/litie/layers/conv.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/crf.py` & `litie-0.2.1/litie/layers/crf.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/dropouts.py` & `litie-0.2.1/litie/layers/dropouts.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/global_pointer.py` & `litie-0.2.1/litie/layers/global_pointer.py`

 * *Files 19% similar despite different names*

```diff
@@ -267,52 +267,82 @@
         if self.tri_mask:
             logits = logits - torch.tril(torch.ones_like(logits), -1) * 1e12
 
         return logits
 
 
 class HandshakingKernel(nn.Module):
-    def __init__(self, hidden_size, shaking_type="cln"):
+    def __init__(self, hidden_size, shaking_type, inner_enc_type="lstm"):
         super().__init__()
         self.shaking_type = shaking_type
-
         if shaking_type == "cat":
-            self.cat_fc = nn.Linear(hidden_size * 2, hidden_size)
-        if shaking_type == "cln":
+            self.combine_fc = nn.Linear(hidden_size * 2, hidden_size)
+        elif shaking_type == "cat_plus":
+            self.combine_fc = nn.Linear(hidden_size * 3, hidden_size)
+        elif shaking_type == "cln":
+            self.tp_cln = LayerNorm(hidden_size, conditional_size=hidden_size)
+        elif shaking_type == "cln_plus":
             self.tp_cln = LayerNorm(hidden_size, conditional_size=hidden_size)
+            self.inner_context_cln = LayerNorm(hidden_size, conditional_size=hidden_size)
 
-    def upper_reg2seq(self, tensor):
-        """
-        drop lower region and flat upper region to sequence
-        :param tensor: (batch_size, matrix_size, matrix_size, hidden_size)
-        :return: (batch_size, matrix_size + ... + 1, hidden_size)
-        """
-        bs, matrix_size, matrix_size, hidden_size = tensor.shape
-        mask = torch.ones(matrix_size, matrix_size, device=tensor.device).triu().bool()[None, :, :, None]
-        return tensor.masked_select(mask).reshape(bs, -1, hidden_size)
+        self.inner_enc_type = inner_enc_type
+        if inner_enc_type == "mix_pooling":
+            self.lamtha = nn.Parameter(torch.rand(hidden_size))
+        elif inner_enc_type == "lstm":
+            self.inner_context_lstm = nn.LSTM(
+                hidden_size,
+                hidden_size,
+                num_layers=1,
+                bidirectional=False,
+                batch_first=True,
+            )
+
+    def enc_inner_hiddens(self, seq_hiddens, inner_enc_type="lstm"):
+        # seq_hiddens: (batch_size, seq_len, hidden_size)
+        def pool(seqence, pooling_type):
+            if pooling_type == "mean_pooling":
+                pooling = torch.mean(seqence, dim=-2)
+            elif pooling_type == "max_pooling":
+                pooling, _ = torch.max(seqence, dim=-2)
+            elif pooling_type == "mix_pooling":
+                pooling = self.lamtha * torch.mean(seqence, dim=-2) + (1 - self.lamtha) * torch.max(seqence, dim=-2)[0]
+            return pooling
+
+        if "pooling" in inner_enc_type:
+            inner_context = torch.stack(
+                [pool(seq_hiddens[:, :i + 1, :], inner_enc_type) for i in range(seq_hiddens.size()[1])],
+                dim=1
+            )
+        elif inner_enc_type == "lstm":
+            inner_context, _ = self.inner_context_lstm(seq_hiddens)
+
+        return inner_context
 
     def forward(self, seq_hiddens):
         """
-        seq_hiddens: (batch_size, seq_len, hidden_size_x)
-        return:
-            if only look after:
-                shaking_hiddenss: (batch_size, (1 + seq_len) * seq_len / 2, hidden_size); e.g. (32, 5+4+3+2+1, 5)
-            else:
-                shaking_hiddenss: (batch_size, seq_len * seq_len, hidden_size)
+        :param seq_hiddens: (batch_size, seq_len, hidden_size)
+        :return: shaking_hiddenss: (batch_size, (1 + seq_len) * seq_len / 2, hidden_size) (32, 5+4+3+2+1, 5)
         """
-        seq_len = seq_hiddens.size(1)
-
-        guide = seq_hiddens[:, :, None, :].repeat(1, 1, seq_len, 1)
-        visible = guide.permute(0, 2, 1, 3)
-
-        # guide, visible: (batch_size, shaking_seq_len, hidden_size)
-        guide = self.upper_reg2seq(guide)
-        visible = self.upper_reg2seq(visible)
-
-        if self.shaking_type == "cat":
-            tp_cat_pre = torch.cat([guide, visible], dim=-1)
-            shaking_pre = torch.relu(self.cat_fc(tp_cat_pre))
-
-        if self.shaking_type == "cln":
-            shaking_pre = self.tp_cln([visible, guide])
-
-        return shaking_pre
+        seq_len = seq_hiddens.size()[-2]
+        shaking_hiddens_list = []
+        for ind in range(seq_len):
+            hidden_each_step = seq_hiddens[:, ind, :]
+            visible_hiddens = seq_hiddens[:, ind:, :]  # ind: only look back
+            repeat_hiddens = hidden_each_step[:, None, :].repeat(1, seq_len - ind, 1)
+
+            if self.shaking_type == "cat":
+                shaking_hiddens = torch.cat([repeat_hiddens, visible_hiddens], dim=-1)
+                shaking_hiddens = torch.tanh(self.combine_fc(shaking_hiddens))
+            elif self.shaking_type == "cat_plus":
+                inner_context = self.enc_inner_hiddens(visible_hiddens, self.inner_enc_type)
+                shaking_hiddens = torch.cat([repeat_hiddens, visible_hiddens, inner_context], dim=-1)
+                shaking_hiddens = torch.tanh(self.combine_fc(shaking_hiddens))
+            elif self.shaking_type == "cln":
+                shaking_hiddens = self.tp_cln([visible_hiddens, repeat_hiddens])
+            elif self.shaking_type == "cln_plus":
+                inner_context = self.enc_inner_hiddens(visible_hiddens, self.inner_enc_type)
+                shaking_hiddens = self.tp_cln([visible_hiddens, repeat_hiddens])
+                shaking_hiddens = self.inner_context_cln([shaking_hiddens, inner_context])
+
+            shaking_hiddens_list.append(shaking_hiddens)
+        long_shaking_hiddens = torch.cat(shaking_hiddens_list, dim=1)
+        return long_shaking_hiddens
```

### Comparing `litie-0.2.0/litie/layers/layer_norm.py` & `litie-0.2.1/litie/layers/layer_norm.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/lear.py` & `litie-0.2.1/litie/layers/lear.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/pfn.py` & `litie-0.2.1/litie/layers/pfn.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/pooling.py` & `litie-0.2.1/litie/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/position.py` & `litie-0.2.1/litie/layers/position.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/set_decoder.py` & `litie-0.2.1/litie/layers/set_decoder.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/layers/transformer.py` & `litie-0.2.1/litie/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/losses.py` & `litie-0.2.1/litie/losses.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/metrics/extraction/precision_recall_fscore.py` & `litie-0.2.1/litie/metrics/extraction/precision_recall_fscore.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/metrics/extraction/score.py` & `litie-0.2.1/litie/metrics/extraction/score.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/metrics/extraction/span.py` & `litie-0.2.1/litie/metrics/extraction/span.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/models/base.py` & `litie-0.2.1/litie/models/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/models/ee.py` & `litie-0.2.1/litie/models/ee.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/models/ner.py` & `litie-0.2.1/litie/models/ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/models/re.py` & `litie-0.2.1/litie/models/re.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/models/uie.py` & `litie-0.2.1/litie/models/uie.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/chinese_bert/configuration_chinese_bert.py` & `litie-0.2.1/litie/nn/chinese_bert/configuration_chinese_bert.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/chinese_bert/modeling_chinese_bert.py` & `litie-0.2.1/litie/nn/chinese_bert/modeling_chinese_bert.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/chinese_bert/tokenization_chinesebert_fast.py` & `litie-0.2.1/litie/nn/chinese_bert/tokenization_chinesebert_fast.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/decode_utils.py` & `litie-0.2.1/litie/nn/decode_utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ee/__init__.py` & `litie-0.2.1/litie/nn/ee/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ee/gplinker.py` & `litie-0.2.1/litie/nn/ee/gplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/model_utils.py` & `litie-0.2.1/litie/nn/model_utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ner/__init__.py` & `litie-0.2.1/litie/nn/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ner/cnn.py` & `litie-0.2.1/litie/nn/ner/cnn.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ner/crf.py` & `litie-0.2.1/litie/nn/ner/crf.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ner/global_pointer.py` & `litie-0.2.1/litie/nn/ner/global_pointer.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ner/lear.py` & `litie-0.2.1/litie/nn/ner/lear.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ner/mrc.py` & `litie-0.2.1/litie/nn/ner/mrc.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ner/span.py` & `litie-0.2.1/litie/nn/ner/span.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/ner/tplinker.py` & `litie-0.2.1/litie/nn/ner/tplinker.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,12 +147,12 @@
 
 def get_tplinker_ner_model_config(labels: list, **kwargs):
     labels = sorted(labels)
     label2id = {v: i for i, v in enumerate(labels)}
     model_config = {
         "num_labels": len(labels),
         "tplinker_label2id": label2id,
-        "shaking_type": "cln",
+        "shaking_type": "cln_plus",
         "decode_thresh": 0.,
     }
     model_config.update(kwargs)
     return model_config
```

### Comparing `litie-0.2.0/litie/nn/ner/w2ner.py` & `litie-0.2.1/litie/nn/ner/w2ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/__init__.py` & `litie-0.2.1/litie/nn/re/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/casrel.py` & `litie-0.2.1/litie/nn/re/casrel.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/gplinker.py` & `litie-0.2.1/litie/nn/re/gplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/grte.py` & `litie-0.2.1/litie/nn/re/grte.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/onerel.py` & `litie-0.2.1/litie/nn/re/onerel.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/pfn.py` & `litie-0.2.1/litie/nn/re/pfn.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/prgc.py` & `litie-0.2.1/litie/nn/re/prgc.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/spn.py` & `litie-0.2.1/litie/nn/re/spn.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/re/tplinker.py` & `litie-0.2.1/litie/nn/re/tplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/roformer/configuration_roformer.py` & `litie-0.2.1/litie/nn/roformer/configuration_roformer.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/roformer/modeling_roformer.py` & `litie-0.2.1/litie/nn/roformer/modeling_roformer.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/uie/convert.py` & `litie-0.2.1/litie/nn/uie/convert.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/uie/model.py` & `litie-0.2.1/litie/nn/uie/model.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/nn/uie/siamese_uie.py` & `litie-0.2.1/litie/nn/uie/siamese_uie.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/pipelines/base.py` & `litie-0.2.1/litie/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/pipelines/ee.py` & `litie-0.2.1/litie/pipelines/ee.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/pipelines/ner.py` & `litie-0.2.1/litie/pipelines/ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/pipelines/re.py` & `litie-0.2.1/litie/pipelines/re.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/pipelines/uie.py` & `litie-0.2.1/litie/pipelines/uie.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/pipelines/utils.py` & `litie-0.2.1/litie/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/registry.py` & `litie-0.2.1/litie/registry.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/ui/ee.py` & `litie-0.2.1/litie/ui/ee.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/ui/ner.py` & `litie-0.2.1/litie/ui/ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/ui/re.py` & `litie-0.2.1/litie/ui/re.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/ui/utils.py` & `litie-0.2.1/litie/ui/utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/utils/common.py` & `litie-0.2.1/litie/utils/common.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/utils/deepspeed.py` & `litie-0.2.1/litie/utils/deepspeed.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/utils/download.py` & `litie-0.2.1/litie/utils/download.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie/utils/logger.py` & `litie-0.2.1/litie/utils/logger.py`

 * *Files identical despite different names*

### Comparing `litie-0.2.0/litie.egg-info/PKG-INFO` & `litie-0.2.1/litie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litie
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pytorch-lightning Code Blocks for Information Extraction
 Home-page: https://github.com/xusenlinzy/lit-ie
 Author: xusenlin
 Author-email: 1659821119@qq.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: litie Version: 0.2.0 Summary: Pytorch-lightning
+Metadata-Version: 2.1 Name: litie Version: 0.2.1 Summary: Pytorch-lightning
 Code Blocks for Information Extraction Home-page: https://github.com/
 xusenlinzy/lit-ie Author: xusenlin Author-email: 1659821119@qq.com Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE #
 Lit-IE
      [https://img.shields.io/github/license/xusenlinzy/lit-ner] [https://
    img.shields.io/badge/python-3.8+-aff.svg] [https://img.shields.io/badge/
 pytorch-%3E=1.12-red?logo=pytorch] [https://img.shields.io/github/last-commit/
```

### Comparing `litie-0.2.0/litie.egg-info/SOURCES.txt` & `litie-0.2.1/litie.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 litie/nn/re/pfn.py
 litie/nn/re/prgc.py
 litie/nn/re/spn.py
 litie/nn/re/tplinker.py
 litie/nn/roformer/__init__.py
 litie/nn/roformer/configuration_roformer.py
 litie/nn/roformer/modeling_roformer.py
+litie/nn/tc/__init__.py
+litie/nn/tc/fc.py
 litie/nn/uie/__init__.py
 litie/nn/uie/convert.py
 litie/nn/uie/model.py
 litie/nn/uie/siamese_uie.py
 litie/pipelines/__init__.py
 litie/pipelines/base.py
 litie/pipelines/ee.py
```

### Comparing `litie-0.2.0/setup.py` & `litie-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "torchmetrics",
     "transformers",
 ]
 
 
 setup(
     name="litie",
-    version="0.2.0",
+    version="0.2.1",
     description="Pytorch-lightning Code Blocks for Information Extraction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xusenlinzy/lit-ie",
     author="xusenlin",
     author_email="1659821119@qq.com",
     ikeywords=["deep learning", "pytorch", "AI"],
```

