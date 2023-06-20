# Comparing `tmp/mpyl-1.0.4-py3-none-any.whl.zip` & `tmp/mpyl-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,87 +1,89 @@
-Zip file size: 129181 bytes, number of entries: 85
--rw-r--r--  2.0 unx      766 b- defN 23-Jun-13 14:26 mpyl/__init__.py
--rw-r--r--  2.0 unx      215 b- defN 23-Jun-13 14:26 mpyl/__main__.py
--rw-r--r--  2.0 unx      162 b- defN 23-Jun-13 14:26 mpyl/constants.py
--rw-r--r--  2.0 unx    12845 b- defN 23-Jun-13 14:26 mpyl/project.py
--rw-r--r--  2.0 unx     1708 b- defN 23-Jun-13 14:26 mpyl/validation.py
--rw-r--r--  2.0 unx     2163 b- defN 23-Jun-13 14:26 mpyl/cli/__init__.py
--rw-r--r--  2.0 unx    10555 b- defN 23-Jun-13 14:26 mpyl/cli/build.py
--rw-r--r--  2.0 unx      341 b- defN 23-Jun-13 14:26 mpyl/cli/health.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Jun-13 14:26 mpyl/cli/meta_info.py
--rw-r--r--  2.0 unx     3915 b- defN 23-Jun-13 14:26 mpyl/cli/projects.py
--rw-r--r--  2.0 unx       34 b- defN 23-Jun-13 14:26 mpyl/cli/commands/__init__.py
--rw-r--r--  2.0 unx      439 b- defN 23-Jun-13 14:26 mpyl/cli/commands/build/__init__.py
--rw-r--r--  2.0 unx     3822 b- defN 23-Jun-13 14:26 mpyl/cli/commands/build/jenkins.py
--rw-r--r--  2.0 unx     5644 b- defN 23-Jun-13 14:26 mpyl/cli/commands/build/mpyl.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-13 14:26 mpyl/cli/commands/health/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 23-Jun-13 14:26 mpyl/cli/commands/health/checks.py
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-13 14:26 mpyl/cli/commands/projects/__init__.py
--rw-r--r--  2.0 unx     1039 b- defN 23-Jun-13 14:26 mpyl/cli/commands/projects/formatting.py
--rw-r--r--  2.0 unx      620 b- defN 23-Jun-13 14:26 mpyl/projects/__init__.py
--rw-r--r--  2.0 unx     1993 b- defN 23-Jun-13 14:26 mpyl/projects/find.py
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:26 mpyl/reporting/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-13 14:26 mpyl/reporting/formatting/__init__.py
--rw-r--r--  2.0 unx     3664 b- defN 23-Jun-13 14:26 mpyl/reporting/formatting/markdown.py
--rw-r--r--  2.0 unx     1413 b- defN 23-Jun-13 14:26 mpyl/reporting/formatting/text.py
--rw-r--r--  2.0 unx     1096 b- defN 23-Jun-13 14:26 mpyl/reporting/targets/__init__.py
--rw-r--r--  2.0 unx     7939 b- defN 23-Jun-13 14:26 mpyl/reporting/targets/github.py
--rw-r--r--  2.0 unx     8965 b- defN 23-Jun-13 14:26 mpyl/reporting/targets/jira.py
--rw-r--r--  2.0 unx     7106 b- defN 23-Jun-13 14:26 mpyl/reporting/targets/slack.py
--rw-r--r--  2.0 unx     8208 b- defN 23-Jun-13 14:26 mpyl/schema/mpyl_config.schema.yml
--rw-r--r--  2.0 unx    25500 b- defN 23-Jun-13 14:26 mpyl/schema/project.schema.yml
--rw-r--r--  2.0 unx     2787 b- defN 23-Jun-13 14:26 mpyl/schema/run_properties.schema.yml
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 14:26 mpyl/stages/__init__.py
--rw-r--r--  2.0 unx     3439 b- defN 23-Jun-13 14:26 mpyl/stages/discovery.py
--rw-r--r--  2.0 unx     6135 b- defN 23-Jun-13 14:26 mpyl/steps/__init__.py
--rw-r--r--  2.0 unx     5977 b- defN 23-Jun-13 14:26 mpyl/steps/models.py
--rw-r--r--  2.0 unx     3429 b- defN 23-Jun-13 14:26 mpyl/steps/run.py
--rw-r--r--  2.0 unx     8850 b- defN 23-Jun-13 14:26 mpyl/steps/steps.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jun-13 14:26 mpyl/steps/build/__init__.py
--rw-r--r--  2.0 unx     2093 b- defN 23-Jun-13 14:26 mpyl/steps/build/docker_after_build.py
--rw-r--r--  2.0 unx     2865 b- defN 23-Jun-13 14:26 mpyl/steps/build/dockerbuild.py
--rw-r--r--  2.0 unx      765 b- defN 23-Jun-13 14:26 mpyl/steps/build/echo.py
--rw-r--r--  2.0 unx     2402 b- defN 23-Jun-13 14:26 mpyl/steps/build/sbt.py
--rw-r--r--  2.0 unx       60 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/__init__.py
--rw-r--r--  2.0 unx     1001 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/echo.py
--rw-r--r--  2.0 unx     1310 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/ephemeral_docker_deploy.py
--rw-r--r--  2.0 unx     2432 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/kubernetes.py
--rw-r--r--  2.0 unx     1111 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/kubernetes_job.py
--rw-r--r--  2.0 unx     1118 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/kubernetes_spark_job.py
--rw-r--r--  2.0 unx     3341 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/__init__.py
--rw-r--r--  2.0 unx    18819 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/chart.py
--rw-r--r--  2.0 unx     2856 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/helm.py
--rw-r--r--  2.0 unx     1579 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/rancher.py
--rw-r--r--  2.0 unx     4467 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/resources/__init__.py
--rw-r--r--  2.0 unx      591 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/resources/sealed_secret.py
--rw-r--r--  2.0 unx     6143 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/resources/spark.py
--rw-r--r--  2.0 unx     1948 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/resources/traefik.py
--rw-r--r--  2.0 unx   168371 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
--rw-r--r--  2.0 unx   151469 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
--rw-r--r--  2.0 unx    11703 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
--rw-r--r--  2.0 unx    42950 b- defN 23-Jun-13 14:26 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
--rw-r--r--  2.0 unx       64 b- defN 23-Jun-13 14:26 mpyl/steps/postdeploy/__init__.py
--rw-r--r--  2.0 unx     5924 b- defN 23-Jun-13 14:26 mpyl/steps/postdeploy/cypress_test.py
--rw-r--r--  2.0 unx       58 b- defN 23-Jun-13 14:26 mpyl/steps/test/__init__.py
--rw-r--r--  2.0 unx     1428 b- defN 23-Jun-13 14:26 mpyl/steps/test/after_test.py
--rw-r--r--  2.0 unx     2453 b- defN 23-Jun-13 14:26 mpyl/steps/test/before_test.py
--rw-r--r--  2.0 unx     3994 b- defN 23-Jun-13 14:26 mpyl/steps/test/dockertest.py
--rw-r--r--  2.0 unx     1657 b- defN 23-Jun-13 14:26 mpyl/steps/test/echo.py
--rw-r--r--  2.0 unx     4885 b- defN 23-Jun-13 14:26 mpyl/steps/test/sbt.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 14:26 mpyl/utilities/__init__.py
--rw-r--r--  2.0 unx      749 b- defN 23-Jun-13 14:26 mpyl/utilities/cypress/__init__.py
--rw-r--r--  2.0 unx     4382 b- defN 23-Jun-13 14:26 mpyl/utilities/docker/__init__.py
--rw-r--r--  2.0 unx     1739 b- defN 23-Jun-13 14:26 mpyl/utilities/github/__init__.py
--rw-r--r--  2.0 unx     1533 b- defN 23-Jun-13 14:26 mpyl/utilities/jenkins/__init__.py
--rw-r--r--  2.0 unx     7617 b- defN 23-Jun-13 14:26 mpyl/utilities/jenkins/runner.py
--rw-r--r--  2.0 unx     1288 b- defN 23-Jun-13 14:26 mpyl/utilities/junit/__init__.py
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-13 14:26 mpyl/utilities/pyaml_env/__init__.py
--rw-r--r--  2.0 unx     6037 b- defN 23-Jun-13 14:26 mpyl/utilities/repo/__init__.py
--rw-r--r--  2.0 unx     1551 b- defN 23-Jun-13 14:26 mpyl/utilities/sbt/__init__.py
--rw-r--r--  2.0 unx     2110 b- defN 23-Jun-13 14:26 mpyl/utilities/subprocess/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-13 14:26 mpyl-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     5911 b- defN 23-Jun-13 14:26 mpyl-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:26 mpyl-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 23-Jun-13 14:26 mpyl-1.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 14:26 mpyl-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7481 b- defN 23-Jun-13 14:26 mpyl-1.0.4.dist-info/RECORD
-85 files, 650931 bytes uncompressed, 117259 bytes compressed:  82.0%
+Zip file size: 132278 bytes, number of entries: 87
+-rw-r--r--  2.0 unx      766 b- defN 23-Jun-20 14:38 mpyl/__init__.py
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-20 14:38 mpyl/__main__.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-20 14:38 mpyl/constants.py
+-rw-r--r--  2.0 unx    13469 b- defN 23-Jun-20 14:38 mpyl/project.py
+-rw-r--r--  2.0 unx     1708 b- defN 23-Jun-20 14:38 mpyl/validation.py
+-rw-r--r--  2.0 unx     2163 b- defN 23-Jun-20 14:38 mpyl/cli/__init__.py
+-rw-r--r--  2.0 unx    10555 b- defN 23-Jun-20 14:38 mpyl/cli/build.py
+-rw-r--r--  2.0 unx      341 b- defN 23-Jun-20 14:38 mpyl/cli/health.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jun-20 14:38 mpyl/cli/meta_info.py
+-rw-r--r--  2.0 unx     3915 b- defN 23-Jun-20 14:38 mpyl/cli/projects.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-20 14:38 mpyl/cli/commands/__init__.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Jun-20 14:38 mpyl/cli/commands/build/__init__.py
+-rw-r--r--  2.0 unx     3822 b- defN 23-Jun-20 14:38 mpyl/cli/commands/build/jenkins.py
+-rw-r--r--  2.0 unx     5802 b- defN 23-Jun-20 14:38 mpyl/cli/commands/build/mpyl.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-20 14:38 mpyl/cli/commands/health/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 23-Jun-20 14:38 mpyl/cli/commands/health/checks.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-20 14:38 mpyl/cli/commands/projects/__init__.py
+-rw-r--r--  2.0 unx     1039 b- defN 23-Jun-20 14:38 mpyl/cli/commands/projects/formatting.py
+-rw-r--r--  2.0 unx      620 b- defN 23-Jun-20 14:38 mpyl/projects/__init__.py
+-rw-r--r--  2.0 unx     1993 b- defN 23-Jun-20 14:38 mpyl/projects/find.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 14:38 mpyl/reporting/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-20 14:38 mpyl/reporting/formatting/__init__.py
+-rw-r--r--  2.0 unx     3664 b- defN 23-Jun-20 14:38 mpyl/reporting/formatting/markdown.py
+-rw-r--r--  2.0 unx     1413 b- defN 23-Jun-20 14:38 mpyl/reporting/formatting/text.py
+-rw-r--r--  2.0 unx     1096 b- defN 23-Jun-20 14:38 mpyl/reporting/targets/__init__.py
+-rw-r--r--  2.0 unx     7939 b- defN 23-Jun-20 14:38 mpyl/reporting/targets/github.py
+-rw-r--r--  2.0 unx     8965 b- defN 23-Jun-20 14:38 mpyl/reporting/targets/jira.py
+-rw-r--r--  2.0 unx     7106 b- defN 23-Jun-20 14:38 mpyl/reporting/targets/slack.py
+-rw-r--r--  2.0 unx     8433 b- defN 23-Jun-20 14:38 mpyl/schema/mpyl_config.schema.yml
+-rw-r--r--  2.0 unx    25500 b- defN 23-Jun-20 14:38 mpyl/schema/project.schema.yml
+-rw-r--r--  2.0 unx     2787 b- defN 23-Jun-20 14:38 mpyl/schema/run_properties.schema.yml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 14:38 mpyl/stages/__init__.py
+-rw-r--r--  2.0 unx     3439 b- defN 23-Jun-20 14:38 mpyl/stages/discovery.py
+-rw-r--r--  2.0 unx     6135 b- defN 23-Jun-20 14:38 mpyl/steps/__init__.py
+-rw-r--r--  2.0 unx     5977 b- defN 23-Jun-20 14:38 mpyl/steps/models.py
+-rw-r--r--  2.0 unx     3429 b- defN 23-Jun-20 14:38 mpyl/steps/run.py
+-rw-r--r--  2.0 unx     8978 b- defN 23-Jun-20 14:38 mpyl/steps/steps.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-20 14:38 mpyl/steps/build/__init__.py
+-rw-r--r--  2.0 unx     2093 b- defN 23-Jun-20 14:38 mpyl/steps/build/docker_after_build.py
+-rw-r--r--  2.0 unx     2865 b- defN 23-Jun-20 14:38 mpyl/steps/build/dockerbuild.py
+-rw-r--r--  2.0 unx      765 b- defN 23-Jun-20 14:38 mpyl/steps/build/echo.py
+-rw-r--r--  2.0 unx     2402 b- defN 23-Jun-20 14:38 mpyl/steps/build/sbt.py
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/__init__.py
+-rw-r--r--  2.0 unx     2444 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/cloudfront_kubernetes_deploy.py
+-rw-r--r--  2.0 unx     1001 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/echo.py
+-rw-r--r--  2.0 unx     1310 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/ephemeral_docker_deploy.py
+-rw-r--r--  2.0 unx     2432 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/kubernetes.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/kubernetes_job.py
+-rw-r--r--  2.0 unx     1118 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/kubernetes_spark_job.py
+-rw-r--r--  2.0 unx     3341 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/__init__.py
+-rw-r--r--  2.0 unx    18819 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/chart.py
+-rw-r--r--  2.0 unx     2856 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/helm.py
+-rw-r--r--  2.0 unx     1579 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/rancher.py
+-rw-r--r--  2.0 unx     4467 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/__init__.py
+-rw-r--r--  2.0 unx      591 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/sealed_secret.py
+-rw-r--r--  2.0 unx     6143 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/spark.py
+-rw-r--r--  2.0 unx     1948 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/traefik.py
+-rw-r--r--  2.0 unx   168371 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
+-rw-r--r--  2.0 unx   151469 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
+-rw-r--r--  2.0 unx    11703 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
+-rw-r--r--  2.0 unx    42950 b- defN 23-Jun-20 14:38 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-20 14:38 mpyl/steps/postdeploy/__init__.py
+-rw-r--r--  2.0 unx     5924 b- defN 23-Jun-20 14:38 mpyl/steps/postdeploy/cypress_test.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-20 14:38 mpyl/steps/test/__init__.py
+-rw-r--r--  2.0 unx     1428 b- defN 23-Jun-20 14:38 mpyl/steps/test/after_test.py
+-rw-r--r--  2.0 unx     2453 b- defN 23-Jun-20 14:38 mpyl/steps/test/before_test.py
+-rw-r--r--  2.0 unx     3218 b- defN 23-Jun-20 14:38 mpyl/steps/test/dockertest.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-Jun-20 14:38 mpyl/steps/test/echo.py
+-rw-r--r--  2.0 unx     4885 b- defN 23-Jun-20 14:38 mpyl/steps/test/sbt.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 14:38 mpyl/utilities/__init__.py
+-rw-r--r--  2.0 unx      749 b- defN 23-Jun-20 14:38 mpyl/utilities/cypress/__init__.py
+-rw-r--r--  2.0 unx     5583 b- defN 23-Jun-20 14:38 mpyl/utilities/docker/__init__.py
+-rw-r--r--  2.0 unx     1739 b- defN 23-Jun-20 14:38 mpyl/utilities/github/__init__.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-Jun-20 14:38 mpyl/utilities/jenkins/__init__.py
+-rw-r--r--  2.0 unx     7617 b- defN 23-Jun-20 14:38 mpyl/utilities/jenkins/runner.py
+-rw-r--r--  2.0 unx     1288 b- defN 23-Jun-20 14:38 mpyl/utilities/junit/__init__.py
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-20 14:38 mpyl/utilities/pyaml_env/__init__.py
+-rw-r--r--  2.0 unx     6037 b- defN 23-Jun-20 14:38 mpyl/utilities/repo/__init__.py
+-rw-r--r--  2.0 unx     4622 b- defN 23-Jun-20 14:38 mpyl/utilities/s3/__init__.py
+-rw-r--r--  2.0 unx     1551 b- defN 23-Jun-20 14:38 mpyl/utilities/sbt/__init__.py
+-rw-r--r--  2.0 unx     2110 b- defN 23-Jun-20 14:38 mpyl/utilities/subprocess/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5945 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       35 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7673 b- defN 23-Jun-20 14:39 mpyl-1.0.5.dist-info/RECORD
+87 files, 659783 bytes uncompressed, 120048 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -123,14 +123,17 @@
 
 Filename: mpyl/steps/build/sbt.py
 Comment: 
 
 Filename: mpyl/steps/deploy/__init__.py
 Comment: 
 
+Filename: mpyl/steps/deploy/cloudfront_kubernetes_deploy.py
+Comment: 
+
 Filename: mpyl/steps/deploy/echo.py
 Comment: 
 
 Filename: mpyl/steps/deploy/ephemeral_docker_deploy.py
 Comment: 
 
 Filename: mpyl/steps/deploy/kubernetes.py
@@ -225,32 +228,35 @@
 
 Filename: mpyl/utilities/pyaml_env/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/repo/__init__.py
 Comment: 
 
+Filename: mpyl/utilities/s3/__init__.py
+Comment: 
+
 Filename: mpyl/utilities/sbt/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/subprocess/__init__.py
 Comment: 
 
-Filename: mpyl-1.0.4.dist-info/LICENSE
+Filename: mpyl-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: mpyl-1.0.4.dist-info/METADATA
+Filename: mpyl-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: mpyl-1.0.4.dist-info/WHEEL
+Filename: mpyl-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: mpyl-1.0.4.dist-info/entry_points.txt
+Filename: mpyl-1.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: mpyl-1.0.4.dist-info/top_level.txt
+Filename: mpyl-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mpyl-1.0.4.dist-info/RECORD
+Filename: mpyl-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mpyl/project.py

```diff
@@ -254,32 +254,42 @@
     hosts: list[Host]
 
     @staticmethod
     def from_config(values: dict):
         hosts = values.get('hosts')
         return Traefik(hosts=(list(map(Host.from_config, hosts) if hosts else [])))
 
+@dataclass(frozen=True)
+class S3Bucket:
+    bucket: TargetProperty[str]
+
+    @staticmethod
+    def from_config(values: dict):
+        return S3Bucket(bucket=TargetProperty.from_config(values.get('bucket', {})))
 
 @dataclass(frozen=True)
 class Deployment:
     namespace: Optional[str]
     properties: Properties
     kubernetes: Optional[Kubernetes]
     traefik: Optional[Traefik]
+    s3_bucket: Optional[S3Bucket]
 
     @staticmethod
     def from_config(values: dict):
         props = values.get('properties')
         kubernetes = values.get('kubernetes')
         traefik = values.get('traefik')
+        s3_bucket = values.get('s3')
 
         return Deployment(namespace=values.get('namespace'),
                           properties=Properties.from_config(props) if props else None,
                           kubernetes=Kubernetes.from_config(kubernetes) if kubernetes else None,
-                          traefik=Traefik.from_config(traefik) if traefik else None)
+                          traefik=Traefik.from_config(traefik) if traefik else None,
+                          s3_bucket=S3Bucket.from_config(s3_bucket) if s3_bucket else None)
 
 
 @dataclass(frozen=True)
 class ProjectName:
     name: str
     namespace: Optional[str]
 
@@ -313,14 +323,20 @@
     @property
     def kubernetes(self) -> Kubernetes:
         if self.deployment is None or self.deployment.kubernetes is None:
             raise KeyError(f"Project '{self.name}' does not have kubernetes configuration")
         return self.deployment.kubernetes
 
     @property
+    def s3_bucket(self) -> S3Bucket:
+        if self.deployment is None or self.deployment.s3_bucket is None:
+            raise KeyError(f"Project '{self.name}' does not have s3 configuration")
+        return self.deployment.s3_bucket
+
+    @property
     def resources(self) -> Resources:
         return self.kubernetes.resources
 
     @property
     def job(self) -> Job:
         if self.kubernetes.job is None:
             raise KeyError(f"Project '{self.name}' does not have kubernetes.job configuration")
```

## mpyl/cli/commands/build/mpyl.py

```diff
@@ -128,11 +128,15 @@
     for stage, projects in accumulator.run_plan.items():
         for proj in projects:
             result = executor.execute(stage, proj, dry_run)
             accumulator.append(result)
             if reporter:
                 reporter.send_report(accumulator)
 
-            if not result.output.success:
-                logging.warning(f'Build failed at {stage} for {proj.name}')
+            if not result.output.success and stage == Stage.DEPLOY:
+                logging.warning(f'Deployment failed for {proj.name}')
                 return accumulator
+
+        if accumulator.failed_result:
+            logging.warning(f'One of the builds failed at {stage}')
+            return accumulator
     return accumulator
```

## mpyl/schema/mpyl_config.schema.yml

```diff
@@ -21,14 +21,16 @@
         "$ref": "#/definitions/Jenkins"
       sbt:
         "$ref": "#/definitions/Sbt"
       slack:
         "$ref": "#/definitions/Slack"
       jira:
         "$ref": "#/definitions/Jira"
+      s3:
+        "$ref": "#/definitions/s3"
     required:
       - cvs
       - docker
     title: MPyL global configuration
   Whitelists:
     type: object
     required:
@@ -323,7 +325,17 @@
         type: string
       ticketPattern:
         type: [ string, null ]
         default: '[A-Za-z]{2,}-\d+'
         description: 'A pattern that extracts a ticket number from the branch name'
     required:
       - site
+  s3:
+    type: object
+    properties:
+      accessKeyId:
+        type: string
+      secretAccessKey:
+        type: string
+    required:
+      - accessKeyId
+      - secretAccessKey
```

## mpyl/steps/steps.py

```diff
@@ -11,14 +11,15 @@
 
 from ruamel.yaml import YAML  # type: ignore
 
 from . import Step
 from .build.dockerbuild import BuildDocker
 from .build.echo import BuildEcho
 from .build.sbt import BuildSbt
+from .deploy.cloudfront_kubernetes_deploy import CloudFrontKubernetesDeploy
 from .deploy.echo import DeployEcho
 from .deploy.ephemeral_docker_deploy import EphemeralDockerDeploy
 from .deploy.kubernetes import DeployKubernetes
 from .deploy.kubernetes_job import DeployKubernetesJob
 from .deploy.kubernetes_spark_job import DeployKubernetesSparkJob
 from .models import Output, Input, RunProperties, ArtifactType, Artifact
 from .postdeploy.cypress_test import CypressTest
@@ -86,14 +87,15 @@
             },
             Stage.TEST: {
                 TestEcho(logger),
                 TestSbt(logger),
                 TestDocker(logger)
             },
             Stage.DEPLOY: {
+                CloudFrontKubernetesDeploy(logger),
                 DeployEcho(logger),
                 DeployKubernetes(logger),
                 DeployKubernetesJob(logger),
                 DeployKubernetesSparkJob(logger),
                 EphemeralDockerDeploy(logger)
             },
             Stage.POST_DEPLOY: {
```

## mpyl/steps/test/dockertest.py

```diff
@@ -8,27 +8,22 @@
 Otherwise, building of the container would stop and the test results would not be committed to a layer.
 
 The test results need to be writted  written to a folder named `$WORKDIR/target/test-reports/` for
 `TestDocker.extract_test_results` to find and extract them.
 
 
 """
-import shutil
 from logging import Logger
-from pathlib import Path
-
-from python_on_whales import docker
-from python_on_whales.exceptions import NoSuchContainer
 
 from .after_test import IntegrationTestAfter
 from .before_test import IntegrationTestBefore
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact, Artifact
 from ...project import Stage, Project
-from ...utilities.docker import DockerConfig, build, docker_image_tag, docker_file_path
+from ...utilities.docker import DockerConfig, build, docker_image_tag, docker_file_path, docker_copy
 from ...utilities.junit import to_test_suites, sum_suites, TEST_OUTPUT_PATH_KEY
 
 
 class TestDocker(Step):
     def __init__(self, logger: Logger) -> None:
         meta = Meta(name='Docker Test', description='Test docker image', version='0.0.1', stage=Stage.TEST)
         super().__init__(
@@ -63,29 +58,13 @@
 
         return Output(success=False,
                       message=f"Tests failed to run for {project.name}. No test results have been recorded.",
                       produced_artifact=None)
 
     @staticmethod
     def extract_test_results(logger: Logger, project: Project, tag: str, step_input: Input) -> Artifact:
-        test_result_path = Path(project.target_path, "test_results")
-        shutil.rmtree(test_result_path, ignore_errors=True)
-        Path(test_result_path).mkdir(parents=True, exist_ok=True)
-
-        container_id = docker.create(tag).id
-
-        if not docker.container.exists(container_id):
-            raise ValueError(f'Container {container_id} with test results does not exist')
-
+        test_result_path = f'{project.target_path}/test_results'
         path_in_container = f'/{project.test_report_path}/'
-        logger.info(
-            f"Copying test results from container {container_id} at "
-            f"path {path_in_container} to host at {test_result_path}"
-        )
-        try:
-            docker.copy(f'{container_id}:{path_in_container}.', test_result_path)
-        except NoSuchContainer as exc:
-            logger.warning(f'Could not find test results in container {tag} at expected location {path_in_container}')
-            raise exc
+        docker_copy(logger=logger, container_path=path_in_container, dst_path=test_result_path, image_name=tag)
 
         return input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
                                  spec={TEST_OUTPUT_PATH_KEY: f'{test_result_path}'})
```

## mpyl/utilities/docker/__init__.py

```diff
@@ -2,16 +2,18 @@
 import logging
 import shlex
 
 from dataclasses import dataclass
 from itertools import tee
 from logging import Logger
 from typing import Dict, Optional, Iterator, cast, Union
-
+import shutil
+from pathlib import Path
 from python_on_whales import docker, Image, Container
+from python_on_whales.exceptions import NoSuchContainer
 from rich.text import Text
 
 from ...project import Project
 from ...steps.models import Input
 
 
 @dataclass(frozen=True)
@@ -88,14 +90,42 @@
     return f"{step_input.project.name.lower()}:{tag}".replace('/', '_')
 
 
 def docker_file_path(project: Project, docker_config: DockerConfig):
     return f'{project.deployment_path}/{docker_config.docker_file_name}'
 
 
+def docker_copy(logger: Logger, container_path: str, dst_path: str, image_name: str):
+    """
+    Copies the contents of the specified path within the container to a locally created destination
+
+    :param logger: the logger
+    :param container_path: the path of the directory in the container to copy
+    :param dst_path: the path to copy the container content to
+    :param image_name: the name of the docker image which a container is created from
+    """
+    shutil.rmtree(dst_path, ignore_errors=True)
+    Path(dst_path).mkdir(parents=True, exist_ok=True)
+
+    container = docker.create(image_name)
+
+    if not docker.container.exists(container.id):
+        raise ValueError(f'Container {container.id} does not exist')
+
+    logger.info(
+        f"Copying contents from container {container.id} at "
+        f"path {container_path} to host at {dst_path}"
+    )
+    try:
+        docker.copy(f'{container.id}:{container_path}', dst_path)
+    except NoSuchContainer as exc:
+        logger.warning(f'Could not find data in container {image_name} at expected location {container_path}')
+        raise exc
+
+
 def build(logger: Logger, root_path: str, file_path: str, image_tag: str, target: str) -> bool:
     """
     :param logger: the logger
     :param root_path: the root path to which `docker_file_path` is relative
     :param file_path: path to the docker file to be built
     :param image_tag: the tag of the image
     :param target: the 'target' within the multi-stage docker image
```

## Comparing `mpyl-1.0.4.dist-info/LICENSE` & `mpyl-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mpyl-1.0.4.dist-info/METADATA` & `mpyl-1.0.5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpyl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Modular Pipeline Library
 Home-page: https://vandebron.github.io/mpyl
 Author: Vandebron Energie BV
 Project-URL: Documentation, https://vandebron.github.io/mpyl
 Project-URL: Source, https://github.com/Vandebron/mpyl
 Project-URL: Tracker, https://github.com/Vandebron/mpyl/issues
 Classifier: Topic :: Software Development :: Build Tools
@@ -33,14 +33,15 @@
 Requires-Dist: rich (==13.3.5)
 Requires-Dist: jenkinsapi (==0.3.13)
 Requires-Dist: pyaml-env (==1.2.1)
 Requires-Dist: aiohttp (==3.8.4)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: questionary (==1.10.0)
 Requires-Dist: toml (==0.10.2)
+Requires-Dist: boto3 (==1.26.140)
 
 # Modular Pypeline Library
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 ![build-and-test-module](https://github.com/Vandebron/pympl/actions/workflows/build-package.yml/badge.svg?branch=main)
 ![coverage](https://camo.githubusercontent.com/2cbb43d8fa7aae526e37e2528d7b084de2af1162440c1aec91e57dd399d65b45/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6465253230436f7665726167652d37382532352d79656c6c6f773f7374796c653d666c6174)
 [![publish-documentation](https://github.com/Vandebron/mpyl/actions/workflows/docs.yml/badge.svg?branch=main)](https://vandebron.github.io/mpyl)
 [![version](https://img.shields.io/github/v/tag/Vandebron/pympl.svg?color=blue&include_prereleases=&sort=semver)](https://pypi.org/project/mpyl/)
```

## Comparing `mpyl-1.0.4.dist-info/RECORD` & `mpyl-1.0.5.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 mpyl/__init__.py,sha256=sLR4OPN49X7SpQiYro_GrizAvJo_CI7nXiZh662D7OE,766
 mpyl/__main__.py,sha256=S7WS_61OT3kRc5RJq3vz4AI6N4YRU5h2KG1kBeQKK6I,215
 mpyl/constants.py,sha256=mr9QfGfl56MCHthSyWkFQfDTHrxMuxLW-1xy6TtHKKQ,162
-mpyl/project.py,sha256=K4c1sVoqZcSfF4Vw26iwYm8zxLLcXyH8N_0PuvXB9ts,12845
+mpyl/project.py,sha256=VHpyOsWYbi0nQ9EcJ7A8CZ84gr0jlyG1JGnQVTYJo9o,13469
 mpyl/validation.py,sha256=EMbkceP3w805916gdoKqGeD1SPONu3FEb2cJld5V05E,1708
 mpyl/cli/__init__.py,sha256=3sN-_zD8pS3JdHh49qC77aFdwIGTXEV2nGxZbc5Ijx8,2163
 mpyl/cli/build.py,sha256=GKLgpW9-dM7Yh1Fzqyr3SYxf0J4YUmjYp8XaC4vRGfg,10555
 mpyl/cli/health.py,sha256=ny37_DVoqXp8IxGQt9KeBZdrbvtd2WGxXtANXPDiENo,341
 mpyl/cli/meta_info.py,sha256=MJhWR8GxSL1Anx7Cs_6c0QU6_tYP_pNxaazGV8JoO60,2170
 mpyl/cli/projects.py,sha256=m6AYs8cn-TGTgobktzKd2MW7xj9D8Sm5GEkMXYVj1vA,3915
 mpyl/cli/commands/__init__.py,sha256=DaL5q4ibFJT7EMlgcQBSpAaaQNiBqnSJZ2WIKtPzLJk,34
 mpyl/cli/commands/build/__init__.py,sha256=Ox0F68re6bNGLBC4KEBLmXXSRf5OIJZ8N2Vens3rgEk,439
 mpyl/cli/commands/build/jenkins.py,sha256=ao1oRp-Hi26roh1EmHLOuqTuvrRncI0H5MT590wKlTg,3822
-mpyl/cli/commands/build/mpyl.py,sha256=tKH8JGPRMaILQuKJWyLruHsw57KgGXmNjb9wKUyTMnM,5644
+mpyl/cli/commands/build/mpyl.py,sha256=6D2d-MrhH2cjP9lTEGESoSnbzJejDd0mYktBvKat82U,5802
 mpyl/cli/commands/health/__init__.py,sha256=Bx6QcWIN-EadbpSe1XAXs1aYCD7Ad8_t3lWRlGDsIr0,38
 mpyl/cli/commands/health/checks.py,sha256=XEBcsrey-UsQBZJtPWn9wxOvJsEGZdVJalxYnczn3Mg,5090
 mpyl/cli/commands/projects/__init__.py,sha256=YoVobAUCYwqc23p-iAuQnpJQYpdri5ljtj8l_XKYOr0,46
 mpyl/cli/commands/projects/formatting.py,sha256=bhoLOUunClIPmSM6eZzJqHgTsdy6fidtz455IlV4xEU,1039
 mpyl/projects/__init__.py,sha256=31HPF5jDZK5UkQT8Zw0V0QSJLqzp8f2zFiWd-QkDjRE,620
 mpyl/projects/find.py,sha256=iUA1_8Tz3tZs-GvEQyvru3g9o3erSt5yxCHXLm96h4k,1993
 mpyl/reporting/__init__.py,sha256=vRvt_67opWXCfe_zYZChT-YhjoPOahAjLagoaVzOcFM,92
 mpyl/reporting/formatting/__init__.py,sha256=GAvYJpHT2SMQxjiLCSqFy57PNWsGI_Ow2bFnA8cX08k,76
 mpyl/reporting/formatting/markdown.py,sha256=n1KesnX2SzNan2L_tN0wPuaxOWDAaXceVeXDAbPsmHI,3664
 mpyl/reporting/formatting/text.py,sha256=zgRnXSvnwi69mCbAsmcJgiU0PITe9uD8cBgPat4l6t8,1413
 mpyl/reporting/targets/__init__.py,sha256=ePSvaZMALkukb0ovhKRGkyIcwavI_VZi7GUeRuLMeEo,1096
 mpyl/reporting/targets/github.py,sha256=en1ph8y_cVh4jaDeoZLsTPngZW6oxWu4DM6v2Md3p3g,7939
 mpyl/reporting/targets/jira.py,sha256=XLHi99E2liSnHSxu1mk_DUJ8fsWH92WZupFqphl7WH4,8965
 mpyl/reporting/targets/slack.py,sha256=mfyHI447djo6hHxUoVniETjPlHCe3B8SHWbmGiKiy2U,7106
-mpyl/schema/mpyl_config.schema.yml,sha256=8_3yx37MtNKVIvfg8HXzAPBM77mrVC4fMPYzSHsfytg,8208
+mpyl/schema/mpyl_config.schema.yml,sha256=f7j-04KI0Im1CoOZZ-Dale-Sw4RSnX0fdzsJ72FGKU8,8433
 mpyl/schema/project.schema.yml,sha256=Pn31oWBvupNXOVuUwykJv-P7C28eoELz5YwCJcKnntI,25500
 mpyl/schema/run_properties.schema.yml,sha256=A5T0m0_6JQ2D6yPHA6GyNNOggID9iWSnwWcfWCG6Fwk,2787
 mpyl/stages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mpyl/stages/discovery.py,sha256=Kv7zsV73jCPOelPiwXYNnMuomt2HDWh12xuzfvEpdfM,3439
 mpyl/steps/__init__.py,sha256=jpcKUPNLQm_8LngC7mbwYUzaoiisgyJy4R8u0qOkmAU,6135
 mpyl/steps/models.py,sha256=_TwBqCuMmQv4VBSuDVVpjXdk63-wTZ8KTcHyEx5hQKY,5977
 mpyl/steps/run.py,sha256=ZzyljvUxkD6Qrwd9QXAFqXLxVFwyf7ZKUcZECkvbB6U,3429
-mpyl/steps/steps.py,sha256=sQgS295KXncnH6laSjTy8LJRlweeKdWiFdft2rBzmbc,8850
+mpyl/steps/steps.py,sha256=4oIt_ePY9hY6oJEaoaYqer8ujJsf0dsX6IrjQb8bH_E,8978
 mpyl/steps/build/__init__.py,sha256=EyPUNNDMQfJK-RVjYM9WvPhEDITbu2n4fx9mxhGLlDs,59
 mpyl/steps/build/docker_after_build.py,sha256=nok2HRrH66e9FBvfwEKnalJhX3io__PQZaq_fR0S8BI,2093
 mpyl/steps/build/dockerbuild.py,sha256=6lqVqiuGYk8ISuzTterTFdcIWqUkvSOUCOCDmjHkM2s,2865
 mpyl/steps/build/echo.py,sha256=on6n-zYs55z6_CouMrSTRIV_JDSTVdQ53raTt3im1qU,765
 mpyl/steps/build/sbt.py,sha256=rvJzIVgsx6KrX5HW_jqEhu6yV2QAttEXQRJ3A7XJJ-k,2402
 mpyl/steps/deploy/__init__.py,sha256=14PYgOvt7YEO2Zw4kEeZxWUNBR7Lz91nSoJZpvJHqzE,60
+mpyl/steps/deploy/cloudfront_kubernetes_deploy.py,sha256=fPbV0TGVO8pReO9EunVpnGC-IZ6jAM22wWfD0q8vj3o,2444
 mpyl/steps/deploy/echo.py,sha256=f43TQmiY96Da_OLZcjkQx-RjCvlo09Dclpezv9RoMlo,1001
 mpyl/steps/deploy/ephemeral_docker_deploy.py,sha256=NySUtyGl7xOjsgDK48AxorVik_iljcifWcRhJZADFs8,1310
 mpyl/steps/deploy/kubernetes.py,sha256=snsHFF04Ns_5kJ8utwXEGmY2sJN4k_Dvw70pmEN1tOE,2432
 mpyl/steps/deploy/kubernetes_job.py,sha256=8b2F-ew51ld1L1Az7Gr4_qYSQ2OngZBrQdVuoitMa_E,1111
 mpyl/steps/deploy/kubernetes_spark_job.py,sha256=bM4vKv7HylmcztAhuUpX5Vsnq-Hul3L8B0B0c37KzPE,1118
 mpyl/steps/deploy/k8s/__init__.py,sha256=OhApd2MdkCm0P7MAvs35qRBdSIbyPKOQBZMr3tivE88,3341
 mpyl/steps/deploy/k8s/chart.py,sha256=uTklf6xJRS1NCSlF_Z6uq2csw3fLlWWSCND07fKpV0Y,18819
@@ -59,27 +60,28 @@
 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml,sha256=3Oc1awM23acMS36kqpbfqwx6D8Sft4FnL8abNLgcwBI,11703
 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml,sha256=6QCi1F9LJ3cgmwaPBV8dWFvbXb2B5huKvfp4Pa1hoBw,42950
 mpyl/steps/postdeploy/__init__.py,sha256=cUDlHPzcW5zGGPxr9T77pATS5lwKnP9Ge8JroAGSvBg,64
 mpyl/steps/postdeploy/cypress_test.py,sha256=NyltDXfYkOLZ8QVH_di2pEqrREJZowhdhCN0VcCriCw,5924
 mpyl/steps/test/__init__.py,sha256=XL1gSbIMJYSFcy4Vf8YRbZM9yAs3Fzvq2tfX9xTDZX8,58
 mpyl/steps/test/after_test.py,sha256=bKTBVFm88s4Kzr6JypxLAbKTlbRsha7gff3RjSr3ip0,1428
 mpyl/steps/test/before_test.py,sha256=IOUvAa3lKox8IKS28aGmmWJMNWcQWv9yGnTydVBvM14,2453
-mpyl/steps/test/dockertest.py,sha256=QZIXXI-xkslL8FPjtNJnOh0-QrNC0U60hBt3Ps90SxY,3994
+mpyl/steps/test/dockertest.py,sha256=EhSZzjWti2wlKtx2xZiOZkBzjlmZZULsdkbOJAgtLMY,3218
 mpyl/steps/test/echo.py,sha256=Jm4oKYhauVbfBZ4D3m6hRY9FM5CikBNP07qcg6NhxmM,1657
 mpyl/steps/test/sbt.py,sha256=3igitohnF_B2qujC1XN1rbUaPxCOBiDMt0ypS8ngM7g,4885
 mpyl/utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mpyl/utilities/cypress/__init__.py,sha256=cKSYzS1CfQgIClUX7Sj8EF5YlJ-34uck6rjyMJsBkFc,749
-mpyl/utilities/docker/__init__.py,sha256=hrFX6YfY66_JWrDa6OiAMMSSxWxIyvSidv58gz57-M8,4382
+mpyl/utilities/docker/__init__.py,sha256=ti4tDTEiuXT8MiiuhA06GafSR-N9Ye7RFXbORaVNobY,5583
 mpyl/utilities/github/__init__.py,sha256=EnkcxQ5UQ08ZZOfShr3LFodu4pmzED9wMoHakIRbYO4,1739
 mpyl/utilities/jenkins/__init__.py,sha256=sX-ZO6NnG0i0LOo_0AMdVMmOluG1zUFxwuHip31TDLE,1533
 mpyl/utilities/jenkins/runner.py,sha256=QNW71misEkmYcPKUB0RTLor-teaHZvo-5J2LWEmuy44,7617
 mpyl/utilities/junit/__init__.py,sha256=kdNbSYHvm5BaFcES_Cked-J5SlqZ_4GByzpg5pVVueY,1288
 mpyl/utilities/pyaml_env/__init__.py,sha256=vrWacRoipXG4SEVOG6ECvp1JwaukhHJhL3xKxVc1mKg,847
 mpyl/utilities/repo/__init__.py,sha256=OVM3es2dvOM-JH9fyet_04J9EMAoq7G1QazK22kUrjo,6037
+mpyl/utilities/s3/__init__.py,sha256=u7NBYcHgXBeSSsqGSFVQs3FLvK-3M4wPC2-Vsc0AQz8,4622
 mpyl/utilities/sbt/__init__.py,sha256=FQOMPPgmiU7HMgMoioM5T0fSk0LwGti-k8l3f75Cuqw,1551
 mpyl/utilities/subprocess/__init__.py,sha256=_NehZ65pzu_qxsQQ_Q9t_-zX-FBGeiiaNsjuuPJsgVc,2110
-mpyl-1.0.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mpyl-1.0.4.dist-info/METADATA,sha256=eYfKjjq4TssV-2WFpdrxVeszcL-Rp2iS2VnaVoc0BeY,5911
-mpyl-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mpyl-1.0.4.dist-info/entry_points.txt,sha256=Jf4zjGLsiokFbaQ2dfX9AC5Bu3kp7zxrBOAzErmAYs8,35
-mpyl-1.0.4.dist-info/top_level.txt,sha256=xVSrrk0ECDxKYaW8mAyGy02yY8KhKlUSyzHaq9UDVNs,5
-mpyl-1.0.4.dist-info/RECORD,,
+mpyl-1.0.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mpyl-1.0.5.dist-info/METADATA,sha256=OLmFQ9ruW2IbA2B5kKfnmoM81zmoYLf1Iit3RoccT1c,5945
+mpyl-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mpyl-1.0.5.dist-info/entry_points.txt,sha256=Jf4zjGLsiokFbaQ2dfX9AC5Bu3kp7zxrBOAzErmAYs8,35
+mpyl-1.0.5.dist-info/top_level.txt,sha256=xVSrrk0ECDxKYaW8mAyGy02yY8KhKlUSyzHaq9UDVNs,5
+mpyl-1.0.5.dist-info/RECORD,,
```

